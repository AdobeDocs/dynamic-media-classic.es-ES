---
title: Instrumentación de visores con el kit de instrumentación de Adobe Analytics
seo-title: Instrumentación de visores con el kit de instrumentación de Adobe Analytics
description: nulo
seo-description: Aprenda a instrumentar un visor con el kit de instrumentación de Adobe Analytics.
uuid: cf 9 a 4002-966 d -4641-9 cd 0-2 ee 8 b 5454 f 60
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: a 2824244-1755-42 de-a 167-42 af 117 cf 038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Instrumentación de visores con el kit de instrumentación de Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puede utilizar el kit de instrumentación de Adobe Analytics para integrar un visor HTML 5 con Adobe Analytics.

Si utiliza cualquiera de los ajustes preestablecidos de visor HTML 5 clásico predefinidos, tenga en cuenta que ya contienen todo el código de implementación necesario para enviar datos a Adobe Analytics—no se requiere ninguna otra instrumentación.

## Configuración del seguimiento de Adobe Analytics desde Scene7 Publishing System {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos los visores HTML 5, agregue el siguiente código JavaScript al contenedor HTML, normalmente en el elemento &lt; head &gt;:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company` se define en el nombre de la empresa de SPS. `&preset` es opcional a menos que el nombre de ajuste preestablecido de empresa `companypreset`no lo sea. In such cases, it could be `companypreset-1, companypreset-2`, and so on. El número más alto es una instancia más reciente del ajuste preestablecido. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

A continuación, añadirá una función que transmite el evento de visor al código de seguimiento de Adobe Analytics.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

En el nombre de la función se distingue entre mayúsculas y minúsculas. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` se define en s_ code. jsp arriba. `s7track` gestiona todos los seguimientos por cada evento. (Para personalizar aún más los datos transmitidos a Adobe Analytics, se hace en esta área.)

## Activación de eventos HREF e ITEM {#enabling-href-and-item-events}

Los eventos HREF (rollover) e ITEM (toques/clics de ratón) se pueden activar en los visores mediante la edición del mapa de imagen. Defina los identificadores de HREF e ITEM dentro del mapa de imagen asociado al contenido del visor. Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
