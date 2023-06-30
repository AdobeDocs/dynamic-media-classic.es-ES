---
title: Prueba de la integración de mediante un informe de Adobe Analytics
description: Obtenga información sobre cómo probar la integración en Adobe Dynamic Media Classic consultando un informe de Adobe Analytics.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 15%

---

# Prueba de la integración de mediante un informe de Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Después de crear las variables necesarias en Adobe Analytics, vincularlas a eventos de Adobe Dynamic Media Classic y completar los pasos de implementación necesarios, puede probar la configuración. Puede probar y verificar que se están capturando datos desde Adobe Analytics. Si la configuración funciona en SiteCatalyst, no serán necesarios más pasos. Suponiendo que ha seguido los pasos anteriores y ha vinculado los datos de evento de Adobe Dynamic Media Classic a una o más variables de tráfico personalizadas, siga este flujo de trabajo para probar los datos dentro de Adobe Analytics.

**Para probar la integración mediante la visualización de un informe de Adobe Analytics:**

1. Inicie un visualizador de Adobe Dynamic Media Classic desde su cuenta, especialmente uno que difunda la métrica que desea obtener e interactúe con él para crear algunos datos de evento.

   Por ejemplo, si desea medir vistas alternativas populares en un conjunto de imágenes, previsualice un conjunto de imágenes y haga clic en las distintas miniaturas de imágenes.

1. Dentro de Adobe Analytics, vaya a **[!UICONTROL Tráfico personalizado]** > **[!UICONTROL Tráfico personalizado 1-10]** > [Nombre de prop], seleccionando el nombre de la prop de tráfico en las opciones del menú.

   Por ejemplo, para acceder a **[!UICONTROL LoadAsset]** prop en la cuenta de ejemplo, la opción de menú adecuada es **[!UICONTROL Tráfico personalizado]** > **[!UICONTROL Tráfico personalizado 1-10]** > **[!UICONTROL LoadAsset]**. Si tiene más de diez propiedades personalizadas, también verá otras opciones de menú.

1. Consulte la tabla generada por Adobe Analytics. Este gráfico suele ser solo los datos de una única métrica. Si también desea saber con qué recurso están asociados estos datos, obtenga los datos de recursos de este evento. Por ejemplo, a menudo resulta útil saber qué vídeo se ve solo en el 50 % o qué imagen de un conjunto es popular.

>[!NOTE]
>
>Todos los datos del visualizador de Adobe Dynamic Media Classic se muestran y se comunican en los informes Tráfico personalizado o Conversión personalizada de Adobe Analytics.

Para obtener más información, consulte [Tutorials de Analytics](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).