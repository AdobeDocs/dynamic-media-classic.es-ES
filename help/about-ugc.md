---
title: Acerca del contenido generado por el usuario en Adobe Dynamic Media Classic
description: Introducción al contenido generado por el usuario.
uuid: ba867a6a-84a4-4968-9a77-712f3ce5dad5
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: c1594abf-8cc2-46dd-88bf-af93db7db607
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
source-git-commit: f92109182283f3bf046604b1b6910180f858d73e
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 48%

---

# Acerca del contenido generado por el usuario en Adobe Dynamic Media Classic {#about-user-generated-content}

El uso de UGC (contenido generado por el usuario) consiste en la carga de recursos en un repositorio de almacenamiento de Dynamic Media Classic de Adobe dedicado y la realización de operaciones relacionadas.

UGC admite formatos de archivo de imagen de trama BMP, GIF, JPG, PNG, PSD, TIFF.
<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!IMPORTANT]
>
>La compatibilidad con recursos de imagen vectoriales UGC nuevos o existentes en Adobe Dynamic Media Classic finalizó el 30 de septiembre de 2021.

Antes de cargar los recursos, es preciso obtener una clave secreta compartida. Esta clave permite recuperar un distintivo de carga. El distintivo de carga se envía al cargar recursos y al realizar otras tareas con el contenido generado por usuarios.

Tras recuperar una clave secreta compartida y un distintivo de carga, se pueden realizar las operaciones siguientes con el contenido generado por usuarios:

* Cargar un recurso.
* Obtenga los metadatos de un recurso de imagen.
* Eliminar un recurso cargado.
* Obtener información sobre el uso de espacio en disco de una empresa.
