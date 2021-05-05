---
title: Optimización para motores de búsqueda de vídeos
description: Aprenda a configurar las opciones de SEO de vídeo.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Administrator
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 40%

---

# Optimización para motores de búsqueda de vídeos{#video-seo-search-engine-optimization}

La optimización para motores de búsqueda de vídeos es el proceso que consiste en mejorar el volumen del tráfico a un sitio web desde motores de búsqueda. Aunque los motores de búsqueda destacan por reunir información sobre el contenido basado en texto, no consiguen adquirir de forma adecuada información sobre vídeos a menos que se les proporcione.

Con Dynamic Media Classic Video SEO, puede aplicar metadatos de vídeo para proporcionar a los motores de búsqueda descripciones de los vídeos. Dynamic Media Classic le permite crear mapas del sitio de vídeo y fuentes mRSS. Estos archivos XML estándar se utilizan para enviar información de vídeo a los motores de búsqueda:

* **Mapa del sitio del vídeo** : informa a Google exactamente dónde y qué contenido del vídeo está en un sitio. Por lo tanto, los vídeos se pueden buscar completamente en Google. Por ejemplo, un mapa de vídeos puede especificar el tiempo de reproducción y las categorías de los vídeos. Para obtener información sobre los mapas del sitio de vídeo, consulte [Mapas del sitio de vídeo y alternativas de mapa del sitio de vídeo](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Fuente mRSS (Media Realmente Simple Syndication)** : la utilizan los editores de contenido para enviar archivos multimedia a Yahoo! búsqueda de vídeos de Yahoo!. Para obtener información sobre las fuentes mRSS, consulte [Mapas del sitio de vídeo y alternativas de mapa del sitio de vídeo](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google admite los protocolos tanto de mapas de vídeos como de recursos mRSS para enviar información a los motores de búsqueda.

Dynamic Media Classic puede generar mapas del sitio de vídeo y fuentes mRSS a partir de metadatos almacenados con cada vídeo. Al crear los mapas de vídeos y los recursos mRSS, se decide qué campos de metadatos de los archivos de vídeo se incluyen. Así, describe los vídeos a los motores de búsqueda de modo que dirijan el tráfico a los vídeos de su sitio web con más precisión.

>[!NOTE]
>
>antes de crear un mapa de vídeos o un recurso mRSS, averigüe qué campos necesita el motor de búsqueda en el archivo XML y cómo se deben estructurar. Para crear un mapa de vídeos o un recurso mRSS correcto, debe cumplir los requisitos del motor de búsqueda.

Dynamic Media Classic crea informes sobre los mapas del sitio de vídeo y las fuentes mRSS después de generarlos. Estos informes están disponibles en la página Informe de SEO de vídeo .

>[!NOTE]
>
>Para los mapas del sitio de vídeo y las fuentes mRSS, Dynamic Media Classic captura los metadatos solo de los vídeos marcados para su publicación. Marque los vídeos para su publicación si desea incluir sus metadatos en los mapas de vídeos y los recursos mRSS.

## Selección de la configuración de SEO de vídeo {#choosing-video-seo-settings}

Haga clic en Configuración de la optimización para motores de búsqueda de vídeo para mapas de sitios de vídeo y fuentes mRSS en la página **[!UICONTROL Configuración de la optimización del motor de búsqueda de vídeo]**. Para abrir esta página, en la barra de navegación global, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Configuración]**.

En el área **[!UICONTROL Configuración general]**, elija si generar mapas de sitios de vídeo, fuentes mRSS o ambos. En el área **[!UICONTROL Generation Settings]**, asigne campos de metadatos a los campos de entrada.

Después de elegir la configuración, haga clic en **[!UICONTROL Guardar]** (o **[!UICONTROL Guardar y generar]**) para crear el mapa del sitio del vídeo, las fuentes mRSS o ambas.

### Selección de la configuración general {#choosing-general-settings}

En la lista desplegable **[!UICONTROL Generation Mode]**, elija un modo de informe:

* **Mapa del sitio del vídeo** : cree un mapa del sitio del vídeo.

* **Fuente mRSS** : cree una fuente RSS de medios (mRSS).

* **Ambos** : cree ambos tipos de archivos XML.

* **Desactivado** : para dejar de generar mapas de sitios de vídeo y fuentes RSS de medios (mRSS), elija esta opción.

En la lista desplegable **[!UICONTROL Automatic/Manual Mode]**, elija si generar automáticamente o manualmente:

* **Modo automático** : Dynamic Media Classic genera automáticamente un mapa del sitio de vídeo, una fuente RSS de medios (mRSS) o ambas, cada día. Elija la opción Marcar para publicación para marcar automáticamente para publicar el archivo XML que Dynamic Media Classic genera.

   * **Marcar para** PublishMarks para publicar el archivo XML generado.

* **Modo manual** : Dynamic Media Classic genera el mapa del sitio del vídeo, la fuente RSS de medios (mRSS) o ambos al hacer clic en Generar o Guardar y generar en la pantalla Configuración de optimización de búsqueda de vídeo. Elija también estas opciones:

   * **Sin configuración adicional** : no marca para publicar el archivo XML generado.

   * **Marcar para publicación** : marca para publicar el archivo XML generado.

   * **Permitir generación parcial** : los motores de búsqueda pueden rechazar un archivo XML si no contiene información de metadatos completa para todos los vídeos. Con esta opción, se crea el archivo XML aunque no haya metadatos disponibles para algunos vídeos. Se registra un aviso en la pantalla del informe. Elija esta opción si pretende exportar el archivo XML y procesar la información que falta manualmente.

### Selección de la configuración de creación  {#choosing-generation-settings}

El área Configuración de generación enumera los campos de entrada para el mapa del sitio de vídeo, la fuente mRSS o ambos, y en el panel Metadatos, los nombres de los campos de metadatos. Use el área Configuración general para asignar los campos de entrada a los campos de metadatos. Al hacerlo, indica a Dynamic Media Classic dónde obtener metadatos para el mapa del sitio del vídeo y/o la fuente mRSS.

1. En el menú Vistas de metadatos, elija una vista de metadatos. Una vez seleccionada la vista, los nombres de los campos de metadatos aparecen en el panel Metadatos.
Consulte [Vistas de metadatos](application-setup.md#metadata_views).
1. Arrastre los nombres de los campos de metadatos del panel Metadatos a los campos de entrada Página de aterrizaje, Título, Descripción, Etiquetas y Categoría. Los campos Página de aterrizaje, Título y Descripción son obligatorios.

   >[!NOTE]
   >
   >Si lo prefiere, introduzca manualmente los campos de entrada.

1. Realice una de las siguientes acciones:

   * Para guardar la configuración sin generar el archivo XML, haga clic en **[!UICONTROL Guardar]**.
   * Para guardar y generar el archivo, haga clic en **[!UICONTROL Guardar y generar]**.

      El archivo XML se crea y se registra en el registro de trabajo. Los archivos de mapas de vídeos (video-sitemap) y de recursos mRSS (mrss-feed) se almacenan en la carpeta raíz de la empresa.

>[!NOTE]
>
>Publique el mapa del sitio del vídeo o la fuente mRSS para poder enviarlo a los motores de búsqueda. Los archivos de mapas de vídeos y de recursos mRSS se almacenan en la carpeta raíz de la empresa. Marque estos archivos XML para publicarlos, si es necesario, y haga clic en **[!UICONTROL Publicar]**.

## Envío de archivos de mapas de vídeos y recursos mRSS a los motores de búsqueda {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Los archivos de mapas de vídeos y de recursos mRSS se almacenan en la carpeta raíz de la empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie una de estas URL en las herramientas del webmaster del motor de búsqueda para enviar el archivo de mapa de vídeos o de recurso mRSS a los motores de búsqueda.

## Visualización de informes de la optimización para motores de búsqueda de vídeos  {#viewing-video-seo-reports}

Vea los informes de SEO de vídeo en la página Informe de optimización del motor de búsqueda de vídeo . Para abrir esta página, en la barra de navegación global, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Informes]**.

Si se produjeron errores al generar un informe, estos se enumeran en la página Informe.
