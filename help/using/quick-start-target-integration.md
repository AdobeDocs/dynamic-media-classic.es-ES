---
title: "Inicio rápido: Integración de Adobe Target Standard/Premium"
description: Introducción y inicio rápido de Adobe Target Standard/Premium para ayudarle a ponerse en marcha rápidamente con las técnicas de integración de Adobe Target Standard/Premium en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Inicio rápido: Integración de Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium pone el control directamente en manos de los especialistas en marketing. Al hacerlo, puede ejecutar de forma rápida y continua varias pruebas A/B y multivariable, así como medir la eficacia. Además, puede aumentar la relevancia del contenido en línea mediante la segmentación, el direccionamiento y Automated Personalization.

Adobe Dynamic Media Classic permite crear ofertas y conjuntos de ofertas para campañas de Adobe Target Standard/Premium. Por ejemplo, puede crear un conjunto de ofertas con tres variaciones del mismo recurso de medios enriquecidos. A continuación, puede tener Adobe Target Standard o Premium para determinar qué recurso proporciona un mejor aumento de conversión. Puede crear ofertas y conjuntos de ofertas a partir de una plantilla básica o de imágenes individuales. Una vez que el conjunto de ofertas se haya insertado o guardado en Adobe Target Standard/Premium, donde las ofertas están asociadas a mboxes y experiencias, Adobe Target Standard/Premium podrá ejecutar campañas. Estas campañas determinan qué variación de un sitio web probablemente funcione mejor para las pulsaciones y la conversión.

Para una mayor personalización del contenido dinámico de Adobe Dynamic Media Classic, utilice las ofertas de HTML de Adobe Target Standard/Premium. Consulte la [documentación del producto de Adobe Target Standard/Premium](https://experienceleague.adobe.com/es/docs/target) para obtener más información.

>[!NOTE]
>
>Se necesita una cuenta válida de Adobe Target Standard/Premium para utilizar Adobe Target Standard/Premium con Adobe Dynamic Media Classic.

Este inicio rápido está diseñado para ayudarle a empezar rápidamente con los conjuntos de ofertas de HTML de Adobe Target Standard/Premium. Siga los pasos del 1 al 3. Después de cada paso, se hace una referencia cruzada a un encabezado de tema donde puede encontrar más información.

## 1. Introduzca la URL de Adobe Target Standard/Premium en la página Configuración general de la aplicación

Adobe Dynamic Media Classic necesita su URL de Adobe Target Standard/Premium para integrarse con Adobe Target Standard/Premium. Copie la parte de la dirección URL de Adobe Target Standard/Premium hasta `.com`, inclusive, y escríbala en la página de **[!UICONTROL Configuración general de la aplicación]** de Adobe Dynamic Media Classic, en el campo de texto **[!UICONTROL Servidores]**, **[!UICONTROL Nombre del servidor de Test&amp;Target]**. Consulte [Integrar Adobe Dynamic Media Classic con Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Crear el conjunto de ofertas

Utilice una plantilla o imágenes parametrizadas para crear un conjunto de ofertas. Puede crear conjuntos de ofertas de HTML en la página Conjunto de ofertas de Test&amp;Target. Para abrir esta página, selecciona tu plantilla o imágenes y, en la barra de navegación global, ve a **[!UICONTROL Generar]** > **[!UICONTROL Conjunto de ofertas de Test&amp;Target]**.

Para crear una oferta con una plantilla, seleccione **[!UICONTROL Agregar y previsualizar]**. En la página Agregar y previsualizar, cambie los valores de los parámetros.

Para crear una oferta con imágenes, arrastre las imágenes a la página Conjunto de ofertas de Test&amp;Target. Seleccione **[!UICONTROL Vista previa]** y elija un ajuste preestablecido de imagen para una imagen o para todas las imágenes del conjunto de ofertas.

Guarde el conjunto de ofertas después de crearlo.

Ver [Crear un conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

## 3. Insertar el conjunto de ofertas en Adobe Target Standard/Premium

En la página Conjunto de ofertas de Test&amp;Target, seleccione **[!UICONTROL Ofertas push]** e introduzca sus credenciales de inicio de sesión en el cuadro de diálogo Inicio de sesión de Test&amp;Target. Consulte [Conjuntos de ofertas push en Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
