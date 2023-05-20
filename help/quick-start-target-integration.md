---
title: "Inicio rápido: Integración de Adobe Target Standard/Premium"
description: Introducción y inicio rápido de Adobe Target Standard/Premium para ayudarle a ponerse en marcha rápidamente con las técnicas de integración de Adobe Target Standard/Premium en Adobe Dynamic Media Classic.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# Inicio rápido: Integración de Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium pone el control directamente en manos de los especialistas en marketing para ejecutar de forma rápida y continua varias pruebas A/B y multivariable, medir la eficacia y aumentar la relevancia del contenido en línea mediante la segmentación, el direccionamiento y Automated Personalization.

Adobe Dynamic Media Classic permite crear ofertas y conjuntos de ofertas para campañas de Adobe Target Standard/Premium. Por ejemplo, puede crear un conjunto de ofertas con tres variaciones del mismo recurso de medios enriquecidos. A continuación, puede hacer que Adobe Target Standard/Premium determine qué recurso proporciona un mejor alza de conversión. Puede crear ofertas y ofrecer conjuntos de ofertas a partir de una plantilla básica o de imágenes individuales. Una vez que el conjunto de ofertas se inserta o se guarda en Adobe Target Standard/Premium, donde las ofertas están asociadas a mboxes y experiencias, Adobe Target Standard/Premium puede ejecutar campañas. Estas campañas determinan qué variación de un sitio web probablemente funcione mejor para las pulsaciones y la conversión.

Para la buena personalización del contenido dinámico de Adobe Dynamic Media Classic, utilice ofertas de HTML de Adobe Target Standard/Premium. Consulte la [Documentación del producto de Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) para obtener más información.

>[!NOTE]
>
>Se necesita una cuenta válida de Adobe Target Standard/Premium para utilizar Adobe Target Standard/Premium con Adobe Dynamic Media Classic.

Este inicio rápido está diseñado para ayudarle a empezar rápidamente con los conjuntos de ofertas de HTML Adobe Target Standard/Premium. Siga los pasos del 1 al 3. Después de cada paso, se hace una referencia cruzada a un encabezado de tema donde puede encontrar más información.

## 1. Introduzca la URL de Adobe Target Standard/Premium en la página Configuración general de la aplicación

Adobe Dynamic Media Classic necesita su URL de Adobe Target Standard/Premium para integrarse con Adobe Target Standard/Premium. Copie la parte de la URL de Adobe Target Standard/Premium hasta el `.com`y escríbalo en el Adobe Dynamic Media Classic **[!UICONTROL Configuración general de la aplicación]** , en la **[!UICONTROL Servidores]** grupo, **[!UICONTROL Nombre del servidor de Test&amp;Target]** campo de texto. Consulte [Integración de Adobe Dynamic Media Classic con Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Creación del conjunto de ofertas

Utilice una plantilla parametrizada o imágenes para crear un conjunto de ofertas. Puede crear conjuntos de ofertas de HTML en la página Conjunto de ofertas de Test&amp;Target. Para abrir esta página, seleccione la plantilla o las imágenes y, en la barra de navegación global, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjunto de ofertas de Test&amp;Target]**.

Para crear una oferta con una plantilla, seleccione **[!UICONTROL Agregar y previsualizar]**. En la página Agregar y previsualizar, cambie los valores de los parámetros.

Para crear una oferta con imágenes, arrastre imágenes a la página Conjunto de ofertas de Test&amp;Target. Seleccionar **[!UICONTROL Previsualizar]** y seleccione un ajuste preestablecido de imagen para una imagen o para todas las imágenes del conjunto de ofertas.

Guarde el conjunto de ofertas una vez creado.

Consulte [Creación de un conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

## 3. Insertar el conjunto de ofertas en Adobe Target Standard/Premium

En la página Conjunto de ofertas de Test&amp;Target, seleccione **[!UICONTROL Transferir ofertas]** e introduzca sus credenciales de inicio de sesión en el cuadro de diálogo Inicio de sesión de Test&amp;Target. Consulte [Insertar conjuntos de ofertas en Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
