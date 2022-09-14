---
title: Instrumentación de un visor con el kit de instrumentación de Adobe Analytics
description: Aprenda a instrumentar un visor con el kit de instrumentación de Adobe Analytics en Adobe Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Instrumentación de un visor con el kit de instrumentación de Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puede utilizar el kit de instrumentación de Adobe Analytics para integrar un visor HTML5 con Adobe Analytics.

Si utiliza cualquiera de los ajustes preestablecidos de visor predefinidos de Adobe Dynamic Media Classic HTML5, ya contendrán todo el código de implementación para enviar datos a Adobe Analytics; usted no necesita más instrumentación.

## Configuración del seguimiento de Adobe Analytics desde Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos los visores de HTML5, agregue el siguiente JavaScript al contenedor de HTML, normalmente en la variable &lt;head> elemento:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Donde `Adobe Dynamic Media Classic Company ID` se establece en el nombre de empresa de Adobe Dynamic Media Classic. Y `&preset` es opcional a menos que el nombre preestablecido de la empresa no `companypreset`. En tales casos, podría ser `companypreset-1, companypreset-2`, etc. El número más alto es una instancia más reciente del ajuste preestablecido. Para determinar el nombre de valor preestablecido de la empresa correcto, seleccione **[!UICONTROL Copiar URL]** y, a continuación, consulte la `preset=`para encontrar el nombre del ajuste preestablecido de empresa.

A continuación, agregue una función que transmita el evento del visor al código de seguimiento de Adobe Analytics.

Agregue la variable `s7ComponentEvent()` al HTML del contenedor (o JSP, o ASPX u otro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

El nombre de la función distingue entre mayúsculas y minúsculas. El único parámetro pasado a `s7componentEvent`que es obligatorio es el último: `eventData`. Donde `s7track()` se define en s_code.jsp incluido anteriormente. Y `s7track` gestiona todo el seguimiento por cada evento. (Para personalizar aún más los datos transmitidos a Adobe Analytics, se hace en esta área.)

## Habilitar eventos HREF e ITEM {#enabling-href-and-item-events}

Los eventos HREF (rollover) e ITEM (toques/clics de ratón) se pueden activar en los visores mediante la edición del mapa de imagen. Defina los identificadores de HREF e ITEM dentro del mapa de imagen asociado al contenido del visor. Agregue un `&rolloverKey=` al valor HREF dentro del mapa de imagen.
