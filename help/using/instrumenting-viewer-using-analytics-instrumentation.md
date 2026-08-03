---
title: Instrumentación de un visor mediante el kit de instrumentación de Adobe Analytics
description: Aprenda a instrumentar un visor mediante el Kit de instrumentación de Adobe Analytics en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:34.654Z'
TQID: 'https://experienceleague.adobe.com/veMzN35J6flKfCAFvdPfZPgxJ9oGy0LYYGhjr-hZLcY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 596e4337002ebd67dd9f915a5ae63ae2a6e18437
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 15%

---

# Instrumentación de un visor mediante el kit de instrumentación de Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Puede utilizar el kit de instrumentación de Adobe Analytics para integrar un visor de HTML5 con Adobe Analytics.

Si utiliza cualquiera de los ajustes predefinidos del visualizador HTML5 de Adobe Dynamic Media Classic, ya contienen todo el código de implementación para enviar datos a Adobe Analytics. No es necesario añadir más instrumentación.

## Configurar el seguimiento de Adobe Analytics desde Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos los visualizadores de HTML5, añada la siguiente JavaScript al contenedor de HTML, normalmente en el elemento &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Donde `Adobe Dynamic Media Classic Company ID` se establece en el nombre de empresa de Adobe Dynamic Media Classic. Y `&preset` es opcional. Si el nombre del ajuste preestablecido de la empresa no es `companypreset`, no es opcional. En estos casos, son `companypreset-1`, `companypreset-2` y versiones posteriores. El número más alto es una instancia más reciente del ajuste preestablecido. Para determinar el nombre de ajuste preestablecido de empresa correcto, seleccione **[!UICONTROL Copiar URL]** y, a continuación, observe el parámetro `preset=` para encontrar el nombre de ajuste preestablecido de empresa.

Añada una función que transmita el evento del visor al código de seguimiento de Adobe Analytics.

Agregue la función `s7ComponentEvent()` al contenedor HTML (o JSP, o ASPX, u otro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

El nombre de la función distingue entre mayúsculas y minúsculas. El único parámetro pasado a `s7ComponentEvent` que es necesario es el último, `eventData`. Donde `s7track()` se define en s_code.jsp incluido anteriormente. Y `s7track` procesa todo el seguimiento de cada evento. (Puede personalizar aún más los datos transmitidos a Adobe Analytics en esta área).

## Habilitar eventos HREF y ITEM {#enabling-href-and-item-events}

Los eventos HREF (rollover) e ITEM (toques/clics de ratón) se pueden activar en los visores mediante la edición del mapa de imagen. Defina los identificadores de HREF e ITEM dentro del mapa de imagen asociado al contenido del visor. Agregue un parámetro `&rolloverKey=` al valor HREF en el mapa de imágenes.
