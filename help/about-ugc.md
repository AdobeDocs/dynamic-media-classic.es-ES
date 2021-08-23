---
title: Acerca del contenido generado por el usuario en Dynamic Media Classic
description: Introducción al contenido generado por el usuario.
uuid: ba867a6a-84a4-4968-9a77-712f3ce5dad5
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: c1594abf-8cc2-46dd-88bf-af93db7db607
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 53%

---

# Acerca del contenido generado por el usuario en Dynamic Media Classic {#about-user-generated-content}

El uso de UGC (contenido generado por el usuario) consiste en cargar recursos en un repositorio de almacenamiento de Dynamic Media Classic dedicado y realizar operaciones relacionadas.

El contenido generado por usuarios admite los siguientes formatos de archivo:

* Rasterizado: JPG, PNG, TIFF
* Vector: AI, EPS (no se admiten los archivos EPS de Adobe Illustrator 2018), PDF (solo cuando el archivo PDF se ha abierto y guardado previamente en Adobe Illustrator CS6)

Antes de cargar los recursos, es preciso obtener una clave secreta compartida. Esta clave permite recuperar un distintivo de carga. El distintivo de carga se envía al cargar recursos y al realizar otras tareas con el contenido generado por usuarios.

Tras recuperar una clave secreta compartida y un distintivo de carga, se pueden realizar las operaciones siguientes con el contenido generado por usuarios:

* Cargar un recurso.
* Obtenga los metadatos de un recurso de imagen.
* Eliminar un recurso cargado.
* Obtener información sobre el uso de espacio en disco de una empresa.
