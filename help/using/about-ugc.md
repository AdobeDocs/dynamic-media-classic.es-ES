---
title: Acerca del contenido generado por el usuario en Adobe Dynamic Media Classic
description: Introducción al contenido generado por el usuario.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:34:44.287Z'
TQID: 'https://experienceleague.adobe.com/SwNEO6U33qx45AECK79nff9f9kABWuOdq91d4X8SHd0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 857a52d41b870d41aa1ae64787d03c08dd457eea
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 29%

---

# Acerca del contenido generado por el usuario en Adobe Dynamic Media Classic {#about-user-generated-content}

UGC (contenido generado por el usuario) consiste en cargar recursos a un repositorio de almacenamiento de [!DNL Adobe Dynamic Media Classic] dedicado y realizar operaciones relacionadas.

UGC admite los formatos de archivo de imagen rasterizada BMP, GIF, JPG, PNG, PSD y TIFF.

>[!IMPORTANT]
>
>A partir del 1 de mayo de 2023, los recursos UGC en Dynamic Media seguirán estando disponibles para su uso hasta 60 días después de la fecha de carga. Después de 60 días, los recursos se eliminan.

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>La compatibilidad con recursos de imagen vectorial UGC nuevos o existentes en Adobe Dynamic Media Classic finalizó el 30 de septiembre de 2021.

Antes de cargar recursos, debe obtener una clave de secreto compartido. Esta clave permite recuperar un distintivo de carga. El distintivo de carga se envía al cargar recursos y al realizar otras tareas con el contenido generado por usuarios.

Tras recuperar una clave secreta compartida y un distintivo de carga, se pueden realizar las operaciones siguientes con el contenido generado por usuarios:

* Cargue un recurso.
* Obtenga los metadatos de un recurso de imagen.
* Eliminar un recurso cargado.
* Obtener información acerca del uso del espacio en disco de una empresa.
