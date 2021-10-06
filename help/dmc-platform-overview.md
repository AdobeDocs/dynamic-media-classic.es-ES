---
title: Información general del programa de Adobe Dynamic Media Classic
description: Información general sobre el programa Adobe Dynamic Media Classic y todo el proceso de flujo de trabajo.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 25%

---

# Información general del programa de Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic es un entorno de administración, publicación y servicio de medios enriquecido e integrado. Los medios enriquecidos se pueden distribuir a través de todo tipo de canales de marketing y ventas: la Web, material impreso, campañas por correo electrónico, portales web, ordenadores de sobremesa y dispositivos.

Consulte también el vídeo de capacitación [Información general de la plataforma](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS).

## Flujo de trabajo {#workflow-process}

Los pasos clave del flujo de trabajo de Adobe Dynamic Media Classic son:

* **Cargue y administre sus recursos** : Cargue sus recursos de medios en Adobe Dynamic Media Classic. Puede organizar, examinar y buscar recursos en el sistema. También puede aplicar metadatos a recursos.

* **Crear medios enriquecidos** : cree distintas configuraciones de los recursos, como catálogos electrónicos, conjuntos de imágenes, conjuntos de giros, conjuntos de muestras, conjuntos de medios mixtos, plantillas básicas y plantillas FXG.

* **Publicar y administrar** : publique recursos en la red SaaS de Adobe Dynamic Media Classic, supervise el estado de los recursos cuando se publiquen, administre derechos de usuario y mantenga la seguridad.

* **Servir** : Entregar medios de la red SaaS de Adobe Dynamic Media Classic a páginas web, aplicaciones y dispositivos móviles; los medios están optimizados para el rendimiento y se entregan con el almacenamiento en caché de CDN. Adobe Dynamic Media Classic le proporciona una dirección URL para cada recurso. La URL se activará una vez publique el recurso.

![El proceso de flujo de trabajo de Adobe Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imágenes principales únicas y llamadas mediante URL únicas {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic es fundamentalmente diferente de otros sistemas, ya que puede utilizar Adobe Dynamic Media Classic para distribuir medios de forma dinámica desde recursos maestros únicos y llamadas URL.

Las cadenas URL que genera con Adobe Dynamic Media Classic incluyen instrucciones que indican al servidor cómo mostrar el recurso cuando se entrega. Por ejemplo, la misma imagen principal se puede proporcionar en diferentes tamaños, formatos, grosores, colores y vistas de zoom. Como parte de la creación y publicación de recursos de medios con Adobe Dynamic Media Classic, puede configurar visualmente los efectos. Así se crean las llamadas mediante URL que indican al servidor cómo debe presentar a las aplicaciones el recurso principal.

![Adobe Dynamic Media Classic puede entregar la misma imagen maestra a distintos medios en diferentes tamaños y formatos.](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic garantiza que las experiencias coherentes y de calidad se entreguen a cualquier pantalla, independientemente del tamaño o el ancho de banda.*

## Caché de contenido {#content-caching}

Las imágenes que Adobe Dynamic Media Classic genera dinámicamente son fáciles de almacenar en caché; normalmente, son imágenes JPEG con llamadas URL únicas que las identifican. Las imágenes se envían a la red de entrega de contenido (CDN), un sistema de servidores conectados entre sí a través de Internet con el fin de agilizar las entregas. Las imágenes se distribuyen a los ordenadores desde servidores globales. Al implementar un mecanismo de almacenamiento en caché utilizando cualquier proveedor de CDN, simplemente cambie el nombre del servidor para que apunte al servidor de imagen de Dynamic Media habilitado para CDN. Todas las ediciones de Adobe Dynamic Media Classic incluyen el almacenamiento en caché de CDN empaquetado.
