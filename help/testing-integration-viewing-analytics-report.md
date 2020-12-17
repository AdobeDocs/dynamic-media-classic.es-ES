---
title: Prueba de integración mediante la visualización de un informe de Adobe Analytics
seo-title: Prueba de integración mediante la visualización de un informe de Adobe Analytics
description: nulo
seo-description: Aprender a probar la integración mediante la visualización de un informe de Adobe Analytics.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 42%

---


# Prueba de integración mediante la visualización de un informe de Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Después de crear las variables necesarias en Adobe Analytics, vincularlas a los eventos de Dynamic Media Classic y completar los pasos de implementación necesarios, debe probar la configuración. Puede probar y verificar que se están capturando datos desde Adobe Analytics. Si la configuración funciona en SiteCatalyst, no serán necesarios más pasos. Si ha seguido los pasos anteriores y ha vinculado los datos de evento de Dynamic Media Classic a una o varias variables de tráfico personalizadas, siga este flujo de trabajo para probar los datos dentro de Adobe Analytics.

**Prueba de la integración de mediante la visualización de un informe de Adobe Analytics**

1. Inicie un visor de Dynamic Media Classic desde su cuenta, en particular uno que difunda la métrica que desee capturar e interactúe con él para crear datos de evento.

   Por ejemplo, si desea medir las vistas alternativas más populares de un conjunto de imágenes, previsualice un conjunto de imágenes y haga clic en las distintas imágenes de miniaturas.

1. Dentro de Adobe Analytics, vaya a Tráfico personalizado > Tráfico personalizado 1-10 > [Nombre de prop] y seleccione el nombre de la propiedad de tráfico en las opciones de menú.

   Por ejemplo, para acceder a la propiedad LoadAsset de la cuenta de muestra, la opción de menú correcta sería Tráfico personalizado > Tráfico personalizado 1-10 > LoadAsset. Si tiene más de diez propiedades personalizadas, verá opciones adicionales del menú .

1. Consulte la tabla generada por Adobe Analytics. Tenga en cuenta que suelen ser solo los datos de una métrica. Si también desea saber con qué recurso están asociados estos datos (por ejemplo, qué vídeo se está viendo solo al 50 % o qué imagen de un conjunto es la más popular), asegúrese de capturar también los datos de recursos de este evento.

>[!NOTE]
>
>Todos los datos del visor de Dynamic Media Classic se muestran e incluyen en los informes de tráfico personalizado o de conversión personalizada de Adobe Analytics.

Para obtener más información, consulte [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
