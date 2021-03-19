---
title: '"Inicio rápido: Integración de Target Standard/Premium"'
description: Introducción y inicio rápido a Adobe Target Standard/Premium para ayudarle a poner en marcha rápidamente las técnicas de integración de Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Ingeniero de datos, administrador, profesional empresarial
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 19%

---


# Inicio rápido: Integración de Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium pone el control directamente en manos de los especialistas en marketing para ejecutar rápida y continuamente varias pruebas A/B y multivariable, medir la eficacia y aumentar la relevancia del contenido en línea mediante la segmentación, el direccionamiento y la personalización automatizada.

Dynamic Media Classic permite crear ofertas y conjuntos de ofertas para campañas de Target Standard/Premium. Por ejemplo, puede crear un conjunto de ofertas con tres variaciones del mismo recurso de medios enriquecidos. A continuación, puede hacer que Target Standard/Premium determine qué recurso ofrece un mejor alza de conversión. Puede crear ofertas y ofrecer conjuntos de ofertas a partir de una plantilla básica o de imágenes individuales. Una vez que el conjunto de ofertas se inserta o se guarda en Adobe Target Standard/Premium, donde las ofertas están asociadas con mboxes y experiencias, Target Standard/Premium puede ejecutar campañas para determinar qué variación de un sitio web tendrá un mejor rendimiento para las pulsaciones y la conversión.

Para una buena personalización del contenido dinámico de Dynamic Media Classic, utilice ofertas HTML de Target Standard/Premium. Consulte la documentación del producto Target Standard/Premium para obtener más información.

>[!NOTE]
>
>Se requiere una cuenta de Adobe Target Standard/Premium válida para usar Target Standard/Premium con Dynamic Media Classic.

**Inicio rápido**

Este inicio rápido está diseñado para ayudarle a empezar a utilizarlo rápidamente con los conjuntos de ofertas HTML de Target Standard/Premium. Siga los pasos del 1 al 3. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

**1. Introduzca la URL de Adobe Target Standard/Premium en la pantalla Configuración general de la aplicación.**

Dynamic Media Classic necesita la URL de Target Standard/Premium para integrarla con Target Standard/Premium. Copie la parte de la URL de Target Standard/Premium hasta *.com*, inclusive, e introdúzcala en la pantalla Configuración general de la aplicación de Dynamic Media Classic. Consulte [Integración de Dynamic Media Classic con Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

**2. Creación del conjunto de ofertas**

Utilice una plantilla parametrizada o imágenes para crear un conjunto de ofertas. Los conjuntos de ofertas HTML se crean en la pantalla Conjuntos de ofertas de Test&amp;Target. Para abrir esta pantalla, seleccione la plantilla o las imágenes y haga clic en **Generar** > **Conjunto de ofertas de Test&amp;Target**.

Para crear una oferta con una plantilla, haga clic en **Agregar y previsualizar**. En la pantalla Agregar y previsualizar, cambie los valores de parámetro.

Para crear una oferta con imágenes, arrástrelas a la pantalla Conjuntos de ofertas de Test&amp;Target. Haga clic en **Preview** para elegir un ajuste preestablecido de imagen para una imagen o todas las imágenes del conjunto de ofertas.

Guarde el conjunto de ofertas una vez creado.

Consulte [Creación de un conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

**3. Inserte el conjunto de ofertas en Adobe Target Standard/Premium**

En la pantalla Conjunto de ofertas de Test&amp;Target, haga clic en **Ofertas push** e introduzca sus credenciales de inicio de sesión en el cuadro de diálogo Inicio de sesión de Test&amp;Target. Consulte [Inserción de conjuntos de ofertas en Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
