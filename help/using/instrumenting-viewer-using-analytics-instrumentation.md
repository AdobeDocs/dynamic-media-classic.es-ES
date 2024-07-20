---
title: Instrumentación de un visor mediante el kit de instrumentación de Adobe Analytics
description: Aprenda a instrumentar un visor mediante el Kit de instrumentación de Adobe Analytics en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 15%

---

# Instrumentación de un visor mediante el kit de instrumentación de Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puede utilizar el kit de instrumentación de Adobe Analytics para integrar un visor HTML5 con Adobe Analytics.

Si utiliza cualquiera de los ajustes predefinidos del visualizador HTML 5 de Adobe Dynamic Media Classic, ya contienen todo el código de implementación para enviar datos a Adobe Analytics. No es necesario añadir más instrumentación.

## Configurar el seguimiento de Adobe Analytics desde Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos los visualizadores de HTML 5, añada la siguiente JavaScript al contenedor de HTML, normalmente en el elemento &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Donde `Adobe Dynamic Media Classic Company ID` se establece en el nombre de empresa de Adobe Dynamic Media Classic. Y `&preset` es opcional. Si el nombre del ajuste preestablecido de la empresa no es `companypreset`, no es opcional. En estos casos, podría ser `companypreset-1, companypreset-2`, etc. El número más alto es una instancia más reciente del ajuste preestablecido. Para determinar el nombre correcto del valor preestablecido de la empresa, seleccione **[!UICONTROL Copiar URL]** y, a continuación, observe el parámetro `preset=`para encontrar el nombre del ajuste preestablecido de la empresa.

A continuación, agregue una función que transmita el evento del visor al código de seguimiento de Adobe Analytics.

Agregue la función `s7ComponentEvent()` al HTML contenedor (o JSP, o ASPX u otro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

El nombre de la función distingue entre mayúsculas y minúsculas. El único parámetro pasado a `s7componentEvent` que es necesario es el último: `eventData`. Donde `s7track()` se define en s_code.jsp incluido anteriormente. Y `s7track` administra todo el seguimiento por cada evento. (En esta área se pueden personalizar aún más los datos transmitidos a Adobe Analytics).

## Habilitar eventos HREF y ITEM {#enabling-href-and-item-events}

Los eventos HREF (rollover) e ITEM (toques/clics de ratón) se pueden activar en los visores mediante la edición del mapa de imagen. Defina los identificadores de HREF e ITEM dentro del mapa de imagen asociado al contenido del visor. Agregue un parámetro `&rolloverKey=` al valor HREF en el mapa de imágenes.
