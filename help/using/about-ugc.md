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
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 36%

---

# Acerca del contenido generado por el usuario en Adobe Dynamic Media Classic {#about-user-generated-content}

El uso de UGC (contenido generado por el usuario) consiste en cargar recursos a un repositorio de almacenamiento de Adobe Dynamic Media Classic dedicado y realizar operaciones relacionadas.

UGC admite formatos de archivo de imagen rasterizada BMP, GIF, JPG, PNG, PSD, TIFF.

>[!IMPORTANT]
>
>A partir del 1 de mayo de 2023, los recursos UGC de Dynamic Media estarán disponibles para su uso durante un máximo de 60 días a partir de la fecha de carga. Después de 60 días, los recursos se eliminarán.

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>La compatibilidad con recursos de imagen vectorial UGC nuevos o existentes en Adobe Dynamic Media Classic finalizó el 30 de septiembre de 2021.

Antes de cargar los recursos, es preciso obtener una clave secreta compartida. Esta clave permite recuperar un distintivo de carga. El distintivo de carga se envía al cargar recursos y al realizar otras tareas con el contenido generado por usuarios.

Tras recuperar una clave secreta compartida y un distintivo de carga, se pueden realizar las operaciones siguientes con el contenido generado por usuarios:

* Cargar un recurso.
* Obtenga los metadatos de un recurso de imagen.
* Eliminar un recurso cargado.
* Obtener información acerca del uso del espacio en disco de una empresa.
