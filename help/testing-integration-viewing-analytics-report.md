---
title: Prueba de integración mediante la visualización de un informe de Adobe Analytics
seo-title: Prueba de integración mediante la visualización de un informe de Adobe Analytics
description: nulo
seo-description: Aprenda a probar la integración mediante la visualización de un informe de Adobe Analytics.
uuid: 937375 e 0-6 dea -4 baa-a 2 b 0-4 f 3 e 461 c 9 ee 2
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 1 ddc 89 ff-d 2 e 9-42 eb-a 442-aa 6 b 9871 c 991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Prueba de integración mediante la visualización de un informe de Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Después de crear las variables necesarias en Adobe Analytics, vincularlas a eventos de Dynamic Media Classic y completar los pasos de implementación necesarios, debe probar la configuración. Puede probar y verificar que se están capturando datos desde Adobe Analytics. Si la configuración funciona en SiteCatalyst, no serán necesarios más pasos. Si ha seguido los pasos anteriores y ha vinculado los datos de eventos de Dynamic Media Classic a una o más variables de tráfico personalizadas, siga este flujo de trabajo para probar los datos dentro de Adobe Analytics.

**Prueba de la integración de mediante la visualización de un informe de Adobe Analytics**

1. Inicie un visor de Dynamic Media Classic de su cuenta, especialmente uno que difunda la métrica que desee capturar, e interactúe con él para crear algunos datos de eventos.

   Por ejemplo, si desea medir las vistas alternativas más populares de un conjunto de imágenes, previsualice un conjunto de imágenes y haga clic en las distintas imágenes de miniaturas.

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   Por ejemplo, para acceder a la propiedad LoadAsset de la cuenta de muestra, la opción de menú correcta sería Tráfico personalizado &gt; Tráfico personalizado 1-10 &gt; LoadAsset. Si tiene más de diez propiedades personalizadas, verá opciones adicionales del menú .

1. Consulte la tabla generada por Adobe Analytics. Tenga en cuenta que suelen ser solo los datos de una métrica. Si también desea saber con qué recurso están asociados estos datos (por ejemplo, qué vídeo solo se mira hasta el 50% o qué imagen de un conjunto es más popular), asegúrese de capturar también los datos de recursos de este evento.

>[!NOTE]
>
>Todos los datos de visores de Dynamic Media Classic se muestran e incluyen en informes de tráfico personalizado o en informes de conversión personalizada de Adobe Analytics.

Para obtener más información, consulte [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
