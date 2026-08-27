---
title: Cargar imágenes principales
description: Obtenga información sobre cómo cargar imágenes principales en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:17:09.649Z'
TQID: 'https://experienceleague.adobe.com/xi8ZvTLYacPSL7P2uqo142VpXY6SOOU7cZvA7tT0zOQ'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 53821984bf36bb648ed236d3c547a390cd7de836
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 2%

---

# Cargar imágenes principales{#uploading-master-images}

Antes de cargar imágenes en Adobe Dynamic Media Classic, asegúrese de que tengan el tamaño y el formato de mayor calidad. Adobe Dynamic Media Classic recomienda cargar imágenes de alta calidad con un recuento de píxeles suficiente (de 1500 a 2000 píxeles en la dimensión larga). Este tamaño permite cualquier Dynamic Imaging que sea necesario.

Para obtener más información sobre cómo cargar imágenes, consulte [Cargar archivos](uploading-files.md#uploading_files).

**Prepare sus imágenes principales para la carga:**

Prepare los archivos de imagen principales antes de cargarlos en Adobe Dynamic Media Classic:

* **Tamaño de imagen**: cree las imágenes de mayor tamaño que espera usar. Los tamaños de imagen habituales varían de 1500 a 2500 píxeles en el tamaño más largo. Si tiene intención de utilizar la función Zoom, Adobe Dynamic Media Classic recomienda utilizar imágenes que tengan al menos 2000 píxeles del tamaño más largo para obtener un detalle de zoom óptimo. Adobe Dynamic Media Classic puede procesar imágenes de hasta 25 megapíxeles cada una. Por ejemplo, puede utilizar una imagen de 5000 × 5000 MP o cualquier otra combinación de tamaño de hasta 25 MP.

* **Formatos de archivo**: Adobe Dynamic Media Classic admite todos los formatos de archivo de imagen estándar. Estos formatos incluyen TIFF, BMP, JPEG, PSD, GIF y EPS. Se recomiendan los formatos de imagen sin pérdida (TIFF y PNG). Si utiliza una imagen de JPEG, utilice la configuración de máxima calidad.

* **Espacio de color**: RGB es el espacio de color para presentaciones de imágenes Web. Las imágenes CMYK que se utilizan normalmente para imprimir se convierten a RGB cuando se cargan. Se recomienda cargar imágenes CMYK con un perfil de color ICC (International Color Consortium) incorporado para convertirlas a RGB. Vea también [perfiles ICC (International Color Consortium)](/help/using/icc-profiles.md).
