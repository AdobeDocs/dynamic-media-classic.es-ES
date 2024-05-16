---
title: Optimización para motores de búsqueda de vídeos
description: Aprenda a configurar los ajustes de optimización para motores de búsqueda de vídeos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 27%

---

# Optimización para motores de búsqueda de vídeos{#video-seo-search-engine-optimization}

La optimización para motores de búsqueda de vídeos es el proceso que consiste en mejorar el volumen del tráfico a un sitio web desde motores de búsqueda. Aunque los motores de búsqueda se destacan en recopilar información sobre contenido basado en texto, no pueden adquirir adecuadamente información sobre vídeo. Esa información debe proporcionárseles.

Con Adobe Dynamic Media Classic Video SEO, puede aplicar metadatos de vídeo para proporcionar a los motores de búsqueda descripciones de sus vídeos. Adobe Dynamic Media Classic le permite crear mapas del sitio de vídeo y fuentes mRSS. Estos archivos XML estándar se utilizan para enviar información de vídeo a los motores de búsqueda:

* **Mapa de vídeos**: informa a Google exactamente dónde y qué contenido de vídeo hay en un sitio. Por lo tanto, los vídeos se pueden buscar completamente en Google. Por ejemplo, un mapa de vídeos puede especificar el tiempo de reproducción y las categorías de los vídeos. Para obtener información sobre los mapas del sitio de vídeo, consulte [Mapas del sitio de vídeo y alternativas de mapas del sitio de vídeo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Fuente mRSS (Media Really Simple Syndication)**: Utilizado por los editores de contenido para alimentar archivos multimedia en Yahoo! búsqueda de vídeos de Yahoo!. Para obtener información acerca de las fuentes mRSS, consulte [Mapas del sitio de vídeo y alternativas de mapas del sitio de vídeo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google admite los protocolos tanto de mapas de vídeos como de recursos mRSS para enviar información a los motores de búsqueda.

Adobe Dynamic Media Classic puede generar mapas del sitio de vídeos y fuentes mRSS a partir de los metadatos almacenados con cada vídeo. Al crear los mapas de vídeos y los recursos mRSS, se decide qué campos de metadatos de los archivos de vídeo se incluyen. De este modo, se describen los vídeos a los motores de búsqueda para que los motores de búsqueda puedan dirigir con mayor precisión el tráfico a los vídeos del sitio web.

>[!NOTE]
>
>antes de crear un mapa de vídeos o un recurso mRSS, averigüe qué campos necesita el motor de búsqueda en el archivo XML y cómo se deben estructurar. Para crear un mapa de vídeos o un recurso mRSS correcto, debe cumplir los requisitos del motor de búsqueda.

Adobe Dynamic Media Classic crea informes sobre los mapas del sitio de vídeo y las fuentes mRSS después de generarlos. Estos informes están disponibles en la página Informe de optimización para motores de búsqueda de vídeos.

>[!NOTE]
>
>Para los mapas del sitio de vídeos y las fuentes mRSS, Adobe Dynamic Media Classic captura metadatos solo de los vídeos marcados para publicación. Marque los vídeos para su publicación a fin de incluir sus metadatos en los mapas de vídeos y las fuentes mRSS.

## Elija la configuración de SEO de vídeo

Seleccione la configuración de optimización para motores de búsqueda (SEO) de vídeo para mapas de sitio de vídeo y fuentes mRSS en **[!UICONTROL Configuración de optimización del motor de búsqueda de vídeo]** página. Para abrir esta página, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Vídeo SEO]** > **[!UICONTROL Configuración]**.

En el **[!UICONTROL Configuración general]** , elija si desea generar mapas del sitio de vídeo, fuentes mRSS o ambos. En el **[!UICONTROL Configuración de generación]** , asigne campos de metadatos a campos de entrada.

Después de elegir la configuración, seleccione **[!UICONTROL Guardar]** (o **[!UICONTROL Guardar y generar]**) para crear el mapa de vídeos, fuentes mRSS o ambos.

### Configurar la configuración general {#choosing-general-settings}

En el **[!UICONTROL Modo de generación]** , elija un modo de informe:

* **Mapa de vídeos**: Cree un mapa de vídeos.

* **Fuente mRSS**: cree una fuente RSS de medios (mRSS).

* **Ambos**: cree ambos tipos de archivos XML.

* **Desactivado**: para dejar de generar mapas del sitio de vídeo y fuentes RSS de medios (mRSS), elija esta opción.

En el **[!UICONTROL Modo automático/manual]** , elija si desea generar de forma automática o manual:

* **Modo automático**: Adobe Dynamic Media Classic genera automáticamente un mapa de vídeos, una fuente RSS de medios (mRSS) o ambas cada día. Seleccione el **[!UICONTROL Marcar para publicación]** opción para que pueda marcar automáticamente para publicar el archivo XML que genera Adobe Dynamic Media Classic.

   * **Marcar para publicación** Marcas para publicar el archivo XML generado.

* **Modo manual**: Adobe Dynamic Media Classic genera el mapa de vídeos, la fuente RSS de medios (mRSS) o ambos al seleccionar **[!UICONTROL Generar]** o **[!UICONTROL Guardar y generar]** en la pantalla Configuración de optimización de búsqueda de vídeo. Elija también estas opciones:

   * **No hay más configuraciones**: No marca para publicar el archivo XML generado.

   * **Marcar para publicación**: Marcas para publicar el archivo XML generado.

   * **Permitir generación parcial**: los motores de búsqueda pueden rechazar un archivo XML si no contiene información de metadatos completa para todos los vídeos. Esta opción genera el archivo XML incluso si los metadatos no están disponibles para algunos vídeos. Se registra un aviso en la pantalla del informe. Elija esta opción si pretende exportar el archivo XML y procesar la información que falta manualmente.

### Selección de la configuración de creación {#choosing-generation-settings}

El área Configuración de generación muestra los campos de entrada para el mapa de vídeos, la fuente mRSS o ambos. En el panel Metadatos, se muestran los nombres de los campos de metadatos. Use el área Configuración general para asignar los campos de entrada a los campos de metadatos. Al hacerlo, le indica a Adobe Dynamic Media Classic dónde obtener metadatos para el mapa de vídeos y/o la fuente mRSS.

1. En el menú Vistas de metadatos, elija una vista de metadatos. Después de elegir una vista, los nombres de los campos de metadatos aparecen en el panel Metadatos.
Consulte [Vistas de metadatos](application-setup.md#metadata_views).
1. Arrastre los nombres de los campos de metadatos del panel Metadatos a los campos de entrada Página de aterrizaje, Título, Descripción, Etiquetas y Categoría. Los campos Página de aterrizaje, Título y Descripción son obligatorios.

   >[!NOTE]
   >
   >Si lo prefiere, introduzca manualmente los campos de entrada.

1. Realice una de las siguientes acciones:

   * Para guardar la configuración sin generar el archivo XML, seleccione **[!UICONTROL Guardar]**.
   * Para guardar y generar el archivo, seleccione **[!UICONTROL Guardar y generar]**.

     El archivo XML se crea y se registra en el registro de trabajo. Los archivos de mapas de vídeos (video-sitemap) y de recursos mRSS (mrss-feed) se almacenan en la carpeta raíz de la empresa.

>[!NOTE]
>
>Publique el mapa de vídeos o la fuente mRSS antes de enviarla a los motores de búsqueda. Los archivos de mapas de vídeos y de recursos mRSS se almacenan en la carpeta raíz de la empresa. Si es necesario, marque estos archivos XML para la publicación y seleccione **[!UICONTROL Publish]**.

## Envíe archivos de mapa de vídeos y de fuente mRSS a un motor de búsqueda {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Los archivos de mapas de vídeos y de recursos mRSS se almacenan en la carpeta raíz de la empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie una de estas URL en las herramientas de webmaster del motor de búsqueda para enviar el archivo de fuente Video Sitemap o Media RSS (mRSS) a los motores de búsqueda.

## Ver informes de optimización para motores de búsqueda {#viewing-video-seo-reports}

Vea los informes de Video SEO en la página Informe de optimización del motor de búsqueda de vídeo. Para abrir esta página, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Vídeo SEO]** > **[!UICONTROL Informes]**.

Si se produjeron errores cuando se generó un informe, aparecen en la página Informe.
