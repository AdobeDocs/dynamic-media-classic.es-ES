---
title: Crear y activar ajustes preestablecidos de imagen
description: Obtenga información sobre cómo crear y habilitar ajustes preestablecidos de imagen en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:41:19.856Z'
TQID: 'https://experienceleague.adobe.com/AlYkBI41GganXzy28kbNN9DXU1Pd4mVCwJKCdwmnN4M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: da232d1762d4bb21788ab094ea56d715a58c27d2
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 46%

---

# Crear y habilitar ajustes preestablecidos de imagen{#creating-and-enabling-image-presets}

Cuando los usuarios exportan recursos de imagen con Media Portal, pueden elegir un ajuste preestablecido de imagen en el cuadro de diálogo Exportar recursos seleccionados. Un ajuste preestablecido de imagen es un conjunto de ajustes predefinidos. Estos ajustes pueden cambiar el tamaño, la calidad de imagen, el formato, la resolución y otros aspectos de la apariencia de una imagen cuando se exporta.

Los administradores de Media Portal pueden crear ajustes preestablecidos de imagen para controlar la forma en la que se cambia el formato de las imágenes al exportarse. Los ajustes preestablecidos de imagen reformatean las imágenes según las especificaciones de su empresa cuando los usuarios exportan imágenes desde Adobe Dynamic Media Classic. En lugar de volver a dar formato a las imágenes manualmente, los usuarios las exportan a las especificaciones precisas de un ajuste preestablecido de imagen.

Las siguientes restricciones se aplican al exportar recursos de imagen:

* La anchura × altura deben ser inferiores o iguales a 100 MB por imagen. Por ejemplo, la imagen no puede superar los 10 K × 10 K ni ninguna variación de aspecto inferior, como 8 K × 12 K.
* El tamaño total del archivo no puede superar 1 GB por trabajo de exportación.
* Puede tener un máximo de 500 recursos en total por trabajo de exportación.

>[!NOTE]
>
>Estas restricciones se aplican únicamente a la exportación de recursos de imagen derivados, no a la exportación de archivos principales.

Para crear ajustes preestablecidos de imagen, consulte [Ajustes preestablecidos de imagen](application-setup.md#image_presets).

Para permitir que los usuarios puedan elegir Ajustes preestablecidos de imagen al exportar archivos, consulte [Especificación de opciones de exportación disponibles para los usuarios de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Para elegir los ajustes preestablecidos de imagen que podrán utilizar los miembros de un grupo, consulte [Elección de permisos de acceso a ajustes preestablecidos de imagen para un grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
