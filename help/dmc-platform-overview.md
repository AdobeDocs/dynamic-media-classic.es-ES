---
title: Descripción general del programa de Adobe Dynamic Media Classic
description: Información general sobre el programa y el proceso de flujo de trabajo de Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 30%

---

# Descripción general del programa de Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic es un entorno integrado y rico de administración de medios, publicación y servicio. Los medios enriquecidos se pueden distribuir a través de todo tipo de canales de marketing y ventas: la Web, material impreso, campañas por correo electrónico, portales web, ordenadores de sobremesa y dispositivos.

## Flujo de trabajo {#workflow-process}

Los pasos clave del flujo de trabajo de Dynamic Media Classic son:

* **Cargue y administre sus recursos** : Cargue sus recursos de medios en Dynamic Media Classic. Puede organizar, examinar y buscar recursos en el sistema. También puede aplicar metadatos a recursos.

* **Crear medios enriquecidos** : cree distintas configuraciones de los recursos, como catálogos electrónicos, conjuntos de imágenes, conjuntos de giros, conjuntos de muestras, conjuntos de medios mixtos, plantillas básicas y plantillas FXG.

* **Publicar y administrar** : publique recursos en la red SaaS de Dynamic Media Classic, supervise el estado de los recursos cuando se publiquen, administre derechos de usuario y mantenga la seguridad.

* **Servir** : Entregar medios de la red SaaS de Dynamic Media Classic a páginas web, aplicaciones y dispositivos móviles; los medios están optimizados para el rendimiento y se entregan con el almacenamiento en caché de CDN. Dynamic Media Classic proporciona una URL para cada recurso. La URL se activará una vez publique el recurso.

![El proceso de flujo de trabajo de Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imágenes principales únicas y llamadas mediante URL únicas {#single-master-images-and-single-url-calls}

Dynamic Media Classic es fundamentalmente diferente de otros sistemas, ya que puede utilizar Dynamic Media Classic para distribuir medios dinámicamente desde recursos maestros únicos y llamadas URL.

Las cadenas URL que genera con Dynamic Media Classic incluyen instrucciones que indican al servidor cómo mostrar el recurso cuando se entrega. Por ejemplo, la misma imagen principal se puede proporcionar en diferentes tamaños, formatos, grosores, colores y vistas de zoom. Como parte de la creación y publicación de recursos de medios con Dynamic Media Classic, puede configurar visualmente los efectos. Así se crean las llamadas mediante URL que indican al servidor cómo debe presentar a las aplicaciones el recurso principal.

![Dynamic Media Classic puede entregar la misma imagen maestra a distintos medios en diferentes tamaños y formatos.](/help/assets/gs_dynamic_publishing.png)
*Dynamic Media Classic garantiza que las experiencias coherentes y de calidad se entreguen a cualquier pantalla, independientemente del tamaño o el ancho de banda.*

## Caché de contenido {#content-caching}

Las imágenes que Dynamic Media Classic genera dinámicamente son fáciles de almacenar en caché; normalmente, son imágenes JPEG con llamadas URL únicas que las identifican. Las imágenes se envían a la red de entrega de contenido (CDN), un sistema de servidores conectados entre sí a través de Internet con el fin de agilizar las entregas. Las imágenes se distribuyen a los ordenadores desde servidores globales. Al implementar un mecanismo de almacenamiento en caché utilizando cualquier proveedor de CDN, simplemente cambie el nombre del servidor para que apunte al servidor de imagen de Dynamic Media habilitado para CDN. Todas las ediciones de Dynamic Media Classic incluyen almacenamiento en caché de CDN empaquetado.
