---
title: Crear y habilitar ajustes preestablecidos de imagen
description: Obtenga información sobre cómo crear y habilitar ajustes preestablecidos de imagen en Adobe Dynamic Media Classic.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 60%

---

# Crear y habilitar ajustes preestablecidos de imagen{#creating-and-enabling-image-presets}

Cuando los usuarios exportan recursos de imagen con Media Portal, pueden elegir un ajuste preestablecido de imagen en el cuadro de diálogo Exportar recursos seleccionados. Un ajuste preestablecido de imagen es una recopilación de ajustes predefinidos para cambiar el tamaño, la calidad de la imagen, el formato, la resolución y otros aspectos visuales de una imagen al exportarse.

Los administradores de Media Portal pueden crear ajustes preestablecidos de imagen para controlar la forma en la que se cambia el formato de las imágenes al exportarse. Los ajustes preestablecidos de imagen reformatean las imágenes según las especificaciones de su empresa cuando los usuarios exportan imágenes desde Adobe Dynamic Media Classic. En lugar de cambiar el formato de las imágenes ellos mismos, los usuarios las exportan a las especificaciones concretas de un ajuste preestablecido de imagen.

Las siguientes restricciones se aplican al exportar recursos de imagen:

* La anchura × altura deben ser inferiores o iguales a 100 MB por imagen. Por ejemplo, la imagen no puede superar los 10 K × 10 K ni ninguna variación de aspecto inferior, como 8 K × 12 K.
* El tamaño total de archivo por trabajo de exportación es de 1 GB como máximo.
* Puede tener un máximo de 500 recursos en total por trabajo de exportación.

>[!NOTE]
>
>Estas restricciones se aplican únicamente a la exportación de recursos de imagen derivados, no a la exportación de archivos principales.

Para crear ajustes preestablecidos de imagen, consulte [Ajustes preestablecidos de imagen](application-setup.md#image_presets).

Para permitir que los usuarios puedan elegir Ajustes preestablecidos de imagen al exportar archivos, consulte [Especificación de opciones de exportación disponibles para los usuarios de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Para elegir los ajustes preestablecidos de imagen que podrán utilizar los miembros de un grupo, consulte [Elección de permisos de acceso a ajustes preestablecidos de imagen para un grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
