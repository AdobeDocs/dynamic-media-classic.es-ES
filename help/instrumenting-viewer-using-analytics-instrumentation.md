---
title: Instrumentación de un visor con el kit de instrumentación de Adobe Analytics
description: Aprenda a instrumentar un visor con el kit de instrumentación de Adobe Analytics en Adobe Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Instrumentación de un visor con el kit de instrumentación de Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puede utilizar el kit de instrumentación de Adobe Analytics para integrar un visor HTML5 con Adobe Analytics.

Si utiliza cualquiera de los ajustes preestablecidos de visor HTML5 de Adobe Dynamic Media Classic predefinidos, ya contendrán todo el código de implementación para enviar datos a Adobe Analytics; usted no necesita más instrumentación.

## Configuración del seguimiento de Adobe Analytics desde Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos los visores HTML5, agregue el siguiente JavaScript al contenedor HTML, normalmente en el elemento &lt;head> :

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Donde `Adobe Dynamic Media Classic Company ID` está configurado con el nombre de empresa de Dynamic Media Classic de Adobe. Y `&preset` es opcional a menos que el nombre de ajuste preestablecido de la empresa no sea `companypreset`. En estos casos, podría ser `companypreset-1, companypreset-2`, etc. El número más alto es una instancia más reciente del ajuste preestablecido. Para determinar el nombre de valor preestablecido correcto de la empresa, seleccione **[!UICONTROL Copiar URL]** y, a continuación, observe el parámetro `preset=`para encontrar el nombre de ajuste preestablecido de la empresa.

A continuación, agregue una función que transmita el evento del visor al código de seguimiento de Adobe Analytics.

Agregue la función `s7ComponentEvent()` al HTML contenedor (o JSP, o ASPX u otro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

El nombre de la función distingue entre mayúsculas y minúsculas. El único parámetro pasado a `s7componentEvent`que es obligatorio es el último: `eventData`. Donde `s7track()` se define en s_code.jsp incluido arriba. Y `s7track` gestiona todo el seguimiento por cada evento. (Para personalizar aún más los datos transmitidos a Adobe Analytics, se hace en esta área.)

## Habilitar eventos HREF e ITEM {#enabling-href-and-item-events}

Los eventos HREF (rollover) e ITEM (toques/clics de ratón) se pueden activar en los visores mediante la edición del mapa de imagen. Defina los identificadores de HREF e ITEM dentro del mapa de imagen asociado al contenido del visor. Agregue un parámetro `&rolloverKey=` al valor HREF dentro del mapa de imagen.
