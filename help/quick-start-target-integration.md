---
title: '"Inicio rápido: Integración con Adobe Target Standard/Premium"'
description: Introducción y inicio rápido a Adobe Target Standard/Premium para ayudarle a poner en marcha rápidamente las técnicas de integración de Adobe Target Standard/Premium en Adobe Dynamic Media Classic.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 11%

---

# Inicio rápido: Integración con Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium pone el control directamente en las manos de los especialistas en marketing para ejecutar rápida y continuamente varias pruebas A/B y multivariable, medir la eficacia y aumentar la relevancia del contenido en línea mediante la segmentación, el direccionamiento y Automated Personalization.

Adobe Dynamic Media Classic permite crear ofertas y conjuntos de ofertas para campañas de Adobe Target Standard/Premium. Por ejemplo, puede crear un conjunto de ofertas con tres variaciones del mismo recurso de medios enriquecidos. A continuación, puede hacer que Adobe Target Standard/Premium determine qué recurso ofrece un mejor alza de conversión. Puede crear ofertas y ofrecer conjuntos de ofertas a partir de una plantilla básica o de imágenes individuales. Una vez que el conjunto de ofertas se inserta o se guarda en Adobe Target Standard/Premium, donde las ofertas están asociadas con mboxes y experiencias, Adobe Target Standard/Premium puede ejecutar campañas. Estas campañas determinan qué variación de un sitio web tiene más probabilidades de funcionar mejor para las pulsaciones y la conversión.

Para una buena personalización del contenido de Dynamic Media Classic de Adobe dinámico, utilice las ofertas HTML de Adobe Target Standard/Premium. Consulte la [documentación del producto de Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) para obtener más información.

>[!NOTE]
>
>Se requiere una cuenta de Adobe Target Standard/Premium válida para usar Adobe Target Standard/Premium con Adobe Dynamic Media Classic.

Este inicio rápido está diseñado para ayudarle a empezar a utilizarlo rápidamente con los conjuntos de ofertas HTML de Adobe Target Standard/Premium. Siga los pasos del 1 al 3. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

## 1. Introduzca la URL de Adobe Target Standard/Premium en la página Configuración general de la aplicación

Adobe Dynamic Media Classic necesita la URL de Adobe Target Standard/Premium para integrarla con Adobe Target Standard/Premium. Copie la parte de la URL de Adobe Target Standard/Premium hasta `.com` inclusive e ingréela en la página Adobe Dynamic Media Classic **[!UICONTROL Configuración general de la aplicación]**, en el grupo **[!UICONTROL Servidores]**, **[!UICONTROL Nombre del servidor de Test&amp;Target]** . Consulte [Integrar Adobe Dynamic Media Classic con Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Creación del conjunto de ofertas

Utilice una plantilla parametrizada o imágenes para crear un conjunto de ofertas. Los conjuntos de ofertas HTML se crean en la página Conjunto de ofertas de Test&amp;Target . Para abrir esta página, seleccione la plantilla o las imágenes y, a continuación, en la barra de navegación global, vaya a **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target Offer Set]**.

Para crear una oferta con una plantilla, seleccione **[!UICONTROL Agregar y previsualizar]**. En la página Agregar y previsualizar, cambie los valores de parámetro.

Para crear una oferta con imágenes, arrastre imágenes a la página Conjunto de ofertas de Test&amp;Target . Seleccione **[!UICONTROL Preview]** y elija un ajuste preestablecido de imagen para una imagen o todas las imágenes del conjunto de ofertas.

Guarde el conjunto de ofertas una vez creado.

Consulte [Creación de un conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

## 3. Inserte el conjunto de ofertas en Adobe Target Standard/Premium

En la página Conjunto de ofertas de Test&amp;Target , seleccione **[!UICONTROL Ofertas push]** e introduzca sus credenciales de inicio de sesión en el cuadro de diálogo Inicio de sesión de Test&amp;Target. Consulte [Inserción de conjuntos de ofertas en Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
