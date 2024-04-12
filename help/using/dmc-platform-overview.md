---
title: Información general del programa Adobe Dynamic Media Classic
description: Una visión general del programa Adobe Dynamic Media Classic y todo su proceso de flujo de trabajo.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 17%

---

# Información general del programa Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic es un entorno integrado, completo, de administración, publicación y servicio de medios. Los medios enriquecidos se pueden distribuir a través de todo tipo de canales de marketing y ventas: la Web, material impreso, campañas por correo electrónico, portales web, ordenadores de sobremesa y dispositivos.

Consulte también [Información general de plataforma](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) vídeo de formación.

## Flujo de trabajo {#workflow-process}

Los pasos clave del flujo de trabajo de Adobe Dynamic Media Classic son:

* **Carga y administración de recursos** : Cargue sus recursos de medios en Adobe Dynamic Media Classic. Puede organizar, examinar y buscar recursos en el sistema. También puede aplicar metadatos a los recursos.

* **Crear medios enriquecidos** : cree diferentes configuraciones de los recursos, como catálogos electrónicos, conjuntos de imágenes, conjuntos de giros, conjuntos de muestras, conjuntos de medios mixtos, plantillas básicas y plantillas FXG.

* **Publicar y administrar** : publique recursos en la red SaaS de Adobe Dynamic Media Classic. Monitorice el estado de los recursos cuando se publiquen. Administrar los derechos de usuario y mantener la seguridad.

* **Servir** : Ofrezca medios de la red SaaS de Adobe Dynamic Media Classic a páginas web, aplicaciones y dispositivos móviles; los medios están optimizados para el rendimiento y se entregan con almacenamiento en caché de CDN. Adobe Dynamic Media Classic proporciona una URL para cada recurso. La URL se activará una vez publique el recurso.

![Proceso de flujo de trabajo de Adobe Dynamic Media Classic](/help/using/assets/gs_workflow.png)

## Imágenes principales únicas y llamadas de URL únicas {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic es fundamentalmente diferente a otros sistemas, ya que puede utilizar Adobe Dynamic Media Classic para entregar medios de forma dinámica desde recursos principales únicos y llamadas de URL.

Las cadenas URL que ha generado con Adobe Dynamic Media Classic incluyen instrucciones que indican al servidor cómo mostrar el recurso cuando se envía. Por ejemplo, la misma imagen principal se puede entregar en diferentes tamaños, formatos, pesos, colores y vistas de zoom. Como parte de la creación y publicación de recursos multimedia con Adobe Dynamic Media Classic, puede configurar visualmente los efectos. Al hacerlo, crea las llamadas URL que indican correctamente al servidor cómo presentar el recurso principal a las aplicaciones.

![Adobe Dynamic Media Classic puede entregar la misma imagen principal a diferentes medios en diferentes tamaños y formatos.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic garantiza que las experiencias coherentes y de calidad se entreguen a cualquier pantalla, independientemente del tamaño o el ancho de banda.*

## Caché de contenido {#content-caching}

Las imágenes que Adobe Dynamic Media Classic genera dinámicamente son favorables para la caché; normalmente, son imágenes de JPEG con llamadas URL únicas que las identifican. Las imágenes se envían a la red de entrega de contenido (CDN), un sistema de servidores conectados entre sí a través de Internet con el fin de agilizar las entregas. Las imágenes se distribuyen a los ordenadores desde servidores globales. Al implementar un mecanismo de almacenamiento en caché utilizando cualquier proveedor de CDN, solo tiene que cambiar el nombre del servidor para que apunte al servidor de imágenes de Dynamic Media habilitado para CDN. Todas las ediciones de Adobe Dynamic Media Classic incluyen almacenamiento en caché de CDN agrupado.
