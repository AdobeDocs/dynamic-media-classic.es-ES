---
title: '"Inicio rápido: Integración de Target Standard/Premium"'
seo-title: '"Inicio rápido: Integración de Target Standard/Premium"'
description: nulo
seo-description: Introducción y Inicio rápido a Adobe Target Standard/Premium para ayudarle en el uso inicial de las técnicas de integración de Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 19%

---


# Inicio rápido: Integración con Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium pone el control directamente en manos de los especialistas en mercadotecnia para ejecutar rápida y continuamente varias pruebas A/B y multivariadas, medir la eficacia y aumentar la relevancia del contenido en línea mediante la segmentación, la determinación de objetivos y la personalización automatizada.

Dynamic Media Classic le permite crear ofertas y conjuntos de ofertas para campañas de Target Standard/Premium. Por ejemplo, puede crear un conjunto de ofertas con tres variaciones del mismo recurso de medios enriquecidos. A continuación, puede hacer que Target Standard/Premium determine qué recurso proporciona un mejor alza de conversión. Puede crear ofertas y ofrecer conjuntos de ofertas a partir de una plantilla básica o de imágenes individuales. Una vez insertado o guardado el conjunto de ofertas en Adobe Target Standard/Premium, donde las ofertas están asociadas con mboxes y experiencias, Target Standard/Premium puede ejecutar campañas para determinar qué variación de un sitio web puede funcionar mejor para las pulsaciones y la conversión.

Para una buena personalización del contenido de Dynamic Media Classic, utilice ofertas HTML de Target Standard/Premium. Consulte la documentación del producto Target Standard/Premium para obtener más información.

>[!NOTE]
>
>Se requiere una cuenta válida de Adobe Target Standard/Premium para usar Target Standard/Premium con Dynamic Media Classic.

**Inicio rápido**

Este Inicio rápido está diseñado para ayudarle en el uso inicial de los conjuntos de ofertas HTML de Target Standard/Premium. Siga los pasos del 1 al 3. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

**1. Enter your Adobe Target Standard/Premium URL in the Application General Settings screen.**

Dynamic Media Classic necesita que la URL de Target Standard/Premium se integre con Target Standard/Premium. Copy the portion of your Target Standard/Premium URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. Consulte [Integración de Dynamic Media Classic con Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

**2. Creación del conjunto de ofertas**

Utilice una plantilla parametrizada o imágenes para crear un conjunto de ofertas. Los conjuntos de ofertas HTML se crean en la pantalla Conjuntos de ofertas de Test&amp;Target. To open this screen, select your template or images, and click **Build** > **Test&amp;Target Offer Set**.

Para crear una oferta con una plantilla, haga clic en **Añadir y Previsualización**. En la pantalla Añadir y Previsualización, cambie los valores de los parámetros.

Para crear una oferta con imágenes, arrástrelas a la pantalla Conjuntos de ofertas de Test&amp;Target. Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

Guarde el conjunto de ofertas una vez creado.

Consulte [Creación de un conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

**3. Inserte el conjunto de ofertas en Adobe Target Standard/Premium**

In the Test&amp;Target Offer Set screen, click **Push Offers**, and enter your login credentials in the Test&amp;Target Login dialog box. Consulte [Inserción de conjuntos de ofertas en Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
