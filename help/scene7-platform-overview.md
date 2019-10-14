---
title: Descripción general de la plataforma Adobe Dynamic Media Classic
seo-title: Descripción general de la plataforma Adobe Dynamic Media Classic
description: nulo
seo-description: Información general sobre la plataforma y el proceso de flujo de trabajo de Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: referencia
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Descripción general de la plataforma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic es un entorno integrado de administración, publicación y servicio de medios enriquecidos. Los medios enriquecidos se pueden distribuir a través de todo tipo de canales de marketing y ventas: la Web, material impreso, campañas por correo electrónico, portales web, ordenadores de sobremesa y dispositivos.

## Flujo de trabajo {#workflow-process}

Los pasos clave del flujo de trabajo de Dynamic Media Classic son:

* **Cargue y gestione sus recursos** Cargue sus recursos de medios en SPS. Puede organizar, examinar y buscar recursos en el sistema. También puede aplicar metadatos a recursos. Si instala la aplicación de escritorio de Adobe Scene7 Publishing System, podrá cargar archivos y carpetas arrastrándolos desde el escritorio a una carpeta de carga.

* **Crear medios** enriquecidos Cree diferentes configuraciones de los recursos, como catálogos electrónicos, conjuntos de imágenes, conjuntos de giros, conjuntos de muestras, conjuntos de medios mixtos, plantillas básicas y plantillas FXG. Para obtener más información, consulte Acerca de los medios enriquecidos.

* **Publique y administre** recursos en la red Saas de Dynamic Media Classic, supervise el estado de los recursos cuando se publiquen, administre derechos de usuario y mantenga la seguridad.

* **Proporcionar** medios desde la red SaaS de Dynamic Media Classic a páginas web, aplicaciones y dispositivos móviles; los medios están optimizados para el rendimiento y se entregan con almacenamiento en caché CDN. Dynamic Media Classic le proporciona una URL para cada recurso. La URL se activará una vez publique el recurso.

![Proceso de flujo de trabajo de Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imágenes principales únicas y llamadas mediante URL únicas {#single-master-images-and-single-url-calls}

Dynamic Media Classic es fundamentalmente diferente de otros sistemas porque puede utilizar Dynamic Media Classic para distribuir medios dinámicamente desde recursos maestros únicos y llamadas mediante URL.

Las cadenas URL que se generan con Dynamic Media Classic incluyen instrucciones que indican al servidor cómo mostrar el recurso cuando se entrega. Por ejemplo, la misma imagen principal se puede proporcionar en diferentes tamaños, formatos, grosores, colores y vistas de zoom. Como parte de la creación y publicación de recursos de medios con Dynamic Media Classic, puede configurar los efectos visualmente. Así se crean las llamadas mediante URL que indican al servidor cómo debe presentar a las aplicaciones el recurso principal.

![Dynamic Media Classic puede distribuir la misma imagen principal a distintos medios en diferentes tamaños y formatos.](/help/assets/gs_dynamic_publishing.png)

## Caché de contenido {#content-caching}

Las imágenes que genera dinámicamente Dynamic Media Classic son compatibles con la caché; en la mayoría de los casos, son imágenes JPEG con llamadas de URL únicas que las identifican. Las imágenes se envían a la red de entrega de contenido (CDN), un sistema de servidores conectados entre sí a través de Internet con el fin de agilizar las entregas. Las imágenes se distribuyen a los ordenadores desde servidores globales. Al implementar un mecanismo de almacenamiento en caché con cualquier proveedor de CDN, simplemente debe cambiar el nombre del servidor para que apunte al servidor de imágenes de Dynamic Media habilitado para CDN. Todas las ediciones de Dynamic Media Classic incluyen almacenamiento en caché CDN integrado.
