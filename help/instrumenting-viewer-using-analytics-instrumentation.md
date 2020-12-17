---
title: Instrumentación de visores con el kit de instrumentación de Adobe Analytics
seo-title: Instrumentación de visores con el kit de instrumentación de Adobe Analytics
description: nulo
seo-description: Aprenda a instrumentar un visor con el kit de instrumentación de Adobe Analytics.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 38%

---


# Instrumentación de visores con el kit de instrumentación de Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puede utilizar el kit de instrumentación de Adobe Analytics para integrar un visor HTML5 con Adobe Analytics.

Si utiliza cualquiera de los ajustes preestablecidos de visor Dynamic Media Classic HTML5 predefinidos, tenga en cuenta que ya contienen todo el código de implementación necesario para enviar datos a Adobe Analytics, ya que no necesita más instrumentación.

## Configure el seguimiento de Adobe Analytics desde Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos los visores HTML5, agregue el siguiente JavaScript al contenedor HTML, normalmente en el elemento &lt;head>:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` se establece en el nombre de la compañía de Dynamic Media Classic. `&preset` es opcional a menos que el nombre del ajuste preestablecido de compañía no sea  `companypreset`. En esos casos, podría ser `companypreset-1, companypreset-2`, y así sucesivamente. El número más alto es una instancia más reciente del ajuste preestablecido. Para determinar el nombre correcto del valor preestablecido de compañía, haga clic en **Copiar URL** y, a continuación, consulte el parámetro `preset=`para encontrar el nombre del ajuste preestablecido de compañía.

A continuación, añadirá una función que transmite el evento de visor al código de seguimiento de Adobe Analytics.

Añada la función `s7ComponentEvent()` en el HTML de contenedor (o JSP, ASPX u otro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

En el nombre de la función se distingue entre mayúsculas y minúsculas. El único parámetro que se pasa a `s7componentEvent`que es obligatorio es el último: `eventData`. `s7track()` se define en s_code.jsp, incluido arriba. `s7track` controla todos los seguimientos por cada evento. (Para personalizar aún más los datos transmitidos a Adobe Analytics, se hace en esta área.)

## Activación de eventos HREF e ITEM  {#enabling-href-and-item-events}

Los eventos HREF (rollover) e ITEM (toques/clics de ratón) se pueden activar en los visores mediante la edición del mapa de imagen. Defina los identificadores de HREF e ITEM dentro del mapa de imagen asociado al contenido del visor. Añada un parámetro `&rolloverKey=` al valor HREF dentro del mapa de imagen.
