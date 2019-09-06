---
title: Optimización para motores de búsqueda de vídeos
seo-title: Optimización para motores de búsqueda de vídeos
description: nulo
seo-description: Descubra cómo configurar la configuración de la optimización para motores de búsqueda de vídeos.
uuid: bac 2 c 6 a 9-8466-4 b 8 f-b 835-6 cb 0 b 4168513
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/setup
discoiquuid: 34 ecd 868-775 f -452 b-b 26 e-d 139 f 0 e 280 ae
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# Optimización para motores de búsqueda de vídeos{#video-seo-search-engine-optimization}

La optimización para motores de búsqueda de vídeos es el proceso que consiste en mejorar el volumen del tráfico a un sitio web desde motores de búsqueda. Aunque los motores de búsqueda destacan por reunir información sobre el contenido basado en texto, no consiguen adquirir de forma adecuada información sobre vídeos a menos que se les proporcione.

Con la optimización para motores de búsqueda de vídeos de Dynamic Media Classic, puede aprovechar los metadatos de vídeo para proporcionar a los motores de búsqueda descripciones de sus vídeos. Dynamic Media Classic permite crear mapas de vídeos y recursos mrss. que son archivos XML estándar para enviar información sobre los vídeos a los motores de búsqueda:

**Mapa de vídeos** informa a Google exactamente donde y qué contenido del vídeo está en un sitio. Por consiguiente, es posible buscar los vídeos en Google. Por ejemplo, un mapa de vídeos puede especificar el tiempo de reproducción y las categorías de los vídeos. Para obtener más información sobre los mapas de vídeos, consulte https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**La fuente mrss (Media Really Simple Synation)** usada por los editores de contenido para suministrar archivos de medios a Yahoo! búsqueda de vídeos de Yahoo!. Para obtener más información sobre los recursos mrss, consulte https://www.rssboard.org/media-rss.

>[!NOTE]
>
>Google admite los protocolos tanto de mapas de vídeos como de recursos mRSS para enviar información a los motores de búsqueda.

Dynamic Media Classic puede generar mapas de vídeos y recursos mrss a partir de metadatos almacenados con cada vídeo. Al crear los mapas de vídeos y los recursos mRSS, se decide qué campos de metadatos de los archivos de vídeo se incluyen. Así, describe los vídeos a los motores de búsqueda de modo que dirijan el tráfico a los vídeos de su sitio web con más precisión.

>[!NOTE]
>
>antes de crear un mapa de vídeos o un recurso mRSS, averigüe qué campos necesita el motor de búsqueda en el archivo XML y cómo se deben estructurar. Para crear un mapa de vídeos o un recurso mRSS correcto, debe cumplir los requisitos del motor de búsqueda.

Dynamic Media Classic crea informes sobre mapas de vídeos y recursos mrss después de generarlos. Estos informes se encuentran disponibles en la pantalla Informe de la optimización para motores de búsqueda de vídeos.

>[!NOTE]
>
>Para los mapas de vídeos y los recursos mrss, Dynamic Media Classic captura los metadatos únicamente de los vídeos marcados para publicación. Marque los vídeos para su publicación si desea incluir sus metadatos en los mapas de vídeos y los recursos mRSS.

## Choosing video SEO settings {#choosing-video-seo-settings}

Seleccione la configuración de la optimización para los mapas de vídeos y los recursos mRSS en la pantalla Ajustes de la optimización para motores de búsqueda de vídeos. Para abrir esta pantalla, seleccione Ajustes &gt; Ajustes de aplicación &gt; Optimización para motores de búsqueda de vídeos &gt; Configuración.

En el área Configuración general, elija si se deben generar mapas de vídeos, recursos mRSS o ambos. En el área Configuración de creación, asigne los campos de metadatos a los campos de entrada.

Una vez seleccionada la configuración, haga clic en Generar (o en Guardar y crear) para crear los mapas de vídeos, los recursos mRSS o ambos.

### Selección de la configuración general {#choosing-general-settings}

En la lista desplegable Modo de creación, elija un modo de informe:

**Mapa de vídeos** Cree un mapa de vídeos.

**Fuente** mrss Cree un recurso mrss.

**Ambos** tipos de archivos XML.

**Desactive** esta opción para dejar de generar mapas de vídeos y recursos mrss.

En la lista desplegable Modo automático/manual, elija si la creación se realiza de manera automática o manual:

**El modo** Automático Media Media Classic genera automáticamente un mapa de vídeos, un recurso mrss o ambos, todos los días. Elija la opción Marcar para publicación para marcar automáticamente para publicación el archivo XML que genera Dynamic Media Classic.

**El modo** Manual Media Media Classic genera el mapa de vídeos, el recurso mrss o ambos, al hacer clic en Generar o Guardar y crear en la pantalla Ajustes de optimización de búsqueda de vídeo. Elija también estas opciones:

**No hay más opciones de configuración** que marquen para publicación el archivo XML que se genera.

**Marque** Marcas para publicación para publicar el archivo XML que se genera.

**Permitir que los motores** de búsqueda de generación parcial rechacen un archivo XML si no contiene información completa de los metadatos de todos los vídeos. Con esta opción, se crea el archivo XML aunque no haya metadatos disponibles para algunos vídeos. Se registra un aviso en la pantalla del informe. Elija esta opción si pretende exportar el archivo XML y procesar la información que falta manualmente.

### Selección de la configuración de creación {#choosing-generation-settings}

En el área Configuración de creación se muestran los campos de entrada del mapa de vídeos o del recurso mRSS y, en el panel Metadatos, los nombres de los campos de metadatos. Use el área Configuración general para asignar los campos de entrada a los campos de metadatos. Al hacerlo, se indica a Dynamic Media Classic que obtenga metadatos para el mapa de vídeos y/o el recurso mrss.

1. En el menú Vistas de metadatos, elija una vista de metadatos. Una vez seleccionada la vista, los nombres de los campos de metadatos aparecen en el panel Metadatos. (Para obtener más información acerca de las vistas de metadatos, consulte [Vistas de metadatos](application-setup.md#metadata_views)).
1. Arrastre los nombres de los campos de metadatos del panel Metadatos a los campos de entrada Página de aterrizaje, Título, Descripción, Etiquetas y Categoría. Los campos Página de aterrizaje, Título y Descripción son obligatorios.

   >[!NOTE]
   >
   >Si lo prefiere, introduzca manualmente los campos de entrada.

1. Haga clic en Guardar (para guardar la configuración sin crear el archivo XML), en Generar (para crear el archivo XML) o en Guardar y crear (para guardar y crear el archivo).

   El archivo XML se crea y se registra en el registro de trabajo. Los archivos de mapas de vídeos (video-sitemap) y de recursos mRSS (mrss-feed) se almacenan en la carpeta raíz de la empresa.

>[!NOTE]
>
>Es preciso publicar los mapas de vídeos o los recursos mRSS para poder enviarlos a los motores de búsqueda. Los archivos de mapas de vídeos y de recursos mRSS se almacenan en la carpeta raíz de la empresa. Si es necesario, marque estos archivos XML para su publicación y haga clic en Publicar.

## Envío de archivos de mapas de vídeos y recursos mRSS a los motores de búsqueda {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Los archivos de mapas de vídeos y de recursos mRSS se almacenan en la carpeta raíz de la empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie una de estas URL en las herramientas del webmaster del motor de búsqueda para enviar el archivo de mapa de vídeos o de recurso mRSS a los motores de búsqueda.

## Visualización de informes de la optimización para motores de búsqueda de vídeos {#viewing-video-seo-reports}

Consulte estos informes en la pantalla Informe de la optimización para motores de búsqueda de vídeos. Para abrir esta pantalla, haga clic en Ajustes &gt; Ajustes de aplicación &gt; Optimización para motores de búsqueda de vídeos &gt; Informes.

Si se ha producido algún error al crear un informe, se muestra en la pantalla del informe.
