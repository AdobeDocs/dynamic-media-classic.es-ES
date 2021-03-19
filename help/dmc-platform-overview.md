---
title: Información general sobre la plataforma de Adobe Dynamic Media Classic
description: Información general sobre la plataforma y el proceso de flujo de trabajo de Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administrador, profesional empresarial
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 32%

---


# Información general sobre la plataforma de Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic es un entorno integrado y rico de administración de medios, publicación y servicio. Los medios enriquecidos se pueden distribuir a través de todo tipo de canales de marketing y ventas: la Web, material impreso, campañas por correo electrónico, portales web, ordenadores de sobremesa y dispositivos.

## Flujo de trabajo  {#workflow-process}

Los pasos clave del flujo de trabajo de Dynamic Media Classic son:

* **Cargue y administre sus**
recursosCargue sus recursos de medios en Dynamic Media Classic. Puede organizar, examinar y buscar recursos en el sistema. También puede aplicar metadatos a recursos.

* **Crear**
medios enriquecidosCree distintas configuraciones de los recursos, como catálogos electrónicos, conjuntos de imágenes, conjuntos de giros, conjuntos de muestras, conjuntos de medios mixtos, plantillas básicas y plantillas FXG. Para obtener más información, consulte Acerca de los medios enriquecidos.

* **Publicar y**
administrarPublicar recursos en la red Saas de Dynamic Media Classic, así como supervisar el estado de los recursos cuando se publican, administrar derechos de usuario y mantener la seguridad.

* ****
Proporcionar medios de la red SaaS de Dynamic Media Classic a páginas web, aplicaciones y dispositivos móviles; los medios están optimizados para el rendimiento y se entregan con el almacenamiento en caché de CDN. Dynamic Media Classic proporciona una URL para cada recurso. La URL se activará una vez publique el recurso.

![El proceso de flujo de trabajo de Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imágenes principales únicas y llamadas mediante URL únicas {#single-master-images-and-single-url-calls}

Dynamic Media Classic es fundamentalmente diferente de otros sistemas, ya que puede utilizar Dynamic Media Classic para distribuir medios dinámicamente desde recursos maestros únicos y llamadas URL.

Las cadenas URL que genera con Dynamic Media Classic incluyen instrucciones que indican al servidor cómo mostrar el recurso cuando se entrega. Por ejemplo, la misma imagen principal se puede proporcionar en diferentes tamaños, formatos, grosores, colores y vistas de zoom. Como parte de la creación y publicación de recursos de medios con Dynamic Media Classic, puede configurar visualmente los efectos. Así se crean las llamadas mediante URL que indican al servidor cómo debe presentar a las aplicaciones el recurso principal.

![Dynamic Media Classic puede entregar la misma imagen maestra a distintos medios en diferentes tamaños y formatos.](/help/assets/gs_dynamic_publishing.png)

## Caché de contenido {#content-caching}

Las imágenes que Dynamic Media Classic genera dinámicamente son fáciles de almacenar en caché; en la mayoría de los casos, son imágenes JPEG con llamadas URL únicas que las identifican. Las imágenes se envían a la red de entrega de contenido (CDN), un sistema de servidores conectados entre sí a través de Internet con el fin de agilizar las entregas. Las imágenes se distribuyen a los ordenadores desde servidores globales. Al implementar un mecanismo de almacenamiento en caché utilizando cualquier proveedor de CDN, simplemente cambie el nombre del servidor para que apunte al servidor de imagen de Dynamic Media habilitado para CDN. Todas las ediciones de Dynamic Media Classic incluyen almacenamiento en caché de CDN empaquetado.
