---
title: Descripción general de la plataforma Adobe Dynamic Media Classic
seo-title: Descripción general de la plataforma Adobe Dynamic Media Classic
description: nulo
seo-description: Información general sobre el proceso de flujo de trabajo y plataforma de Dynamic Media Classic.
uuid: e 7 d 3 bfb 3-1 cfe -43 ea-b 862-aae 3 b 3928 c 71
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/getting_ started
discoiquuid: 2 b 134 cfa -7 f 46-4 f 5 f -959 e-b 30 aae 610 bb 9
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Descripción general de la plataforma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic es un entorno de servicio, publicación y gestión de medios enriquecidos integrado. Los medios enriquecidos se pueden distribuir a través de todo tipo de canales de marketing y ventas: la Web, material impreso, campañas por correo electrónico, portales web, ordenadores de sobremesa y dispositivos.

## Flujo de trabajo {#workflow-process}

Los pasos clave del flujo de trabajo de Dynamic Media Classic son:

**Cargar y gestionar sus recursos** cargue los recursos de medios en SPS. Puede organizar, examinar y buscar recursos en el sistema. También puede aplicar metadatos a recursos. Si instala la aplicación de escritorio de Adobe Scene7 Publishing System, podrá cargar archivos y carpetas arrastrándolos desde el escritorio a una carpeta de carga.

**Crear medios enriquecidos** Cree diferentes configuraciones de sus recursos, como catálogos electrónicos, conjuntos de imágenes, conjuntos de giros, conjuntos de muestras, conjuntos de medios mixtos, plantillas básicas y plantillas FXG. Para obtener más información, consulte Acerca de los medios enriquecidos.

**Publique y administre** recursos en la red de Dynamic Media Classic Saas, y supervise el estado de los recursos cuando se publiquen, administre derechos de usuario y mantenga la seguridad.

**Proporcionar** medios desde la red saas de Dynamic Media Classic a páginas web, aplicaciones y dispositivos móviles; los medios se optimizan y se envían con caché CDN. Dynamic Media Classic le proporciona una URL para cada recurso. La URL se activará una vez publique el recurso.

![Proceso de flujo de trabajo de Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imágenes principales únicas y llamadas mediante URL únicas {#single-master-images-and-single-url-calls}

Dynamic Media Classic es fundamentalmente diferente de otros sistemas porque puede utilizar Dynamic Media Classic para distribuir medios dinámicamente desde llamadas de URL y recursos principales únicos.

Las cadenas URL que se generan con Dynamic Media Classic incluyen instrucciones que indican al servidor cómo mostrar el recurso cuando se envía. Por ejemplo, la misma imagen principal se puede proporcionar en diferentes tamaños, formatos, grosores, colores y vistas de zoom. Como parte de la creación y publicación de recursos de medios con Dynamic Media Classic, puede configurar los efectos de forma visual. Así se crean las llamadas mediante URL que indican al servidor cómo debe presentar a las aplicaciones el recurso principal.

![Dynamic Media Classic puede proporcionar la misma imagen principal a diferentes medios en diferentes tamaños y formatos.](/help/assets/gs_dynamic_publishing.png)

## Caché de contenido {#content-caching}

Las imágenes que Dynamic Media Classic genera dinámicamente son prácticas para la caché; En la mayoría de los casos, son imágenes JPEG con llamadas mediante URL exclusivas que las identifican. Las imágenes se envían a la red de entrega de contenido (CDN), un sistema de servidores conectados entre sí a través de Internet con el fin de agilizar las entregas. Las imágenes se distribuyen a los ordenadores desde servidores globales. Cuando implemente un mecanismo de caché con cualquier proveedor de CDN, simplemente cambie el nombre del servidor para que apunte al servidor de imágenes Dynamic Media habilitado para CDN. Todas las ediciones de Dynamic Media Classic incluyen la caché CDN compilada.
