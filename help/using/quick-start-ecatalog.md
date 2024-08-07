---
title: "Inicio rápido: Catálogos electrónicos"
description: Introducción y Inicio rápido a los catálogos electrónicos para ayudarle a ponerse en marcha rápidamente con las técnicas de catálogo electrónico en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# Inicio rápido: Catálogos electrónicos{#quick-start-ecatalogs}

Un catálogo electrónico es una versión digital en la Web del material impreso: un catálogo, un folleto, un folleto, un manual de producto o una circular publicitaria, por ejemplo. Se muestra un catálogo electrónico en un visor de catálogos electrónicos de un sitio Web. Este visor simula la experiencia de lectura de material impreso.

Consulte también los siguientes vídeos de formación:

* [Inicio rápido 1: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Inicio rápido 2: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Según la configuración que elija para el catálogo electrónico, el visor puede permitirle hacer lo siguiente:

* Busque en el catálogo una palabra clave o palabras clave. Los resultados de la búsqueda se muestran como una lista de miniaturas en un panel de búsqueda a la izquierda del catálogo. Cada miniatura en la que se puede hacer clic representa un pliego de catálogo en el que se encontró el término de búsqueda resaltado.

* Comparta el catálogo a través de las redes sociales; descargue el catálogo para verlo sin conexión; habilite Favoritos para marcar los elementos a los que desee volver rápidamente o imprima el catálogo.
* Navegue por el catálogo utilizando la tabla de contenido o la vista de cuadrícula de la página; página hacia delante o hacia atrás seleccionando el borde central de una página.
* Acercar o alejar la página, y desplazarse por ella para examinar sus elementos.
* Mueva el puntero sobre una región de la página (denominada mapa de imagen) para que pueda ver una ventana emergente con información sobre un elemento.
* Seleccione una región de página para que abra una nueva página Web con más información sobre un elemento.
* Escribir una nota adhesiva y adjuntarla a una página del catálogo electrónico.
* Pulse los iconos de mapa de imagen si desea iniciar páginas web relacionadas o paneles de información en contexto.
* Usar interacciones de gestos como pellizcar para ampliar y reducir la imagen o arrastrar para pasar de página.
* Buscar elementos por palabras clave.

![Catálogo electrónico tal como lo ven los usuarios. A) Página de apertura del catálogo electrónico. B)Catálogo electrónico convertido a página 2.](/help/using/assets/ec_cat_viewer_popup.png)

Para crear un catálogo electrónico, normalmente se utilizan archivos de PDF de alta resolución creados en Adobe Acrobat u otro programa de impresión, pero también se puede crear un catálogo electrónico a partir de archivos de imagen.

Al crear el catálogo electrónico, tiene la posibilidad de ordenar como desee páginas o conjuntos de páginas. También puede decidir si desea ver páginas individuales, dobles o múltiples. Puede crear mapas de imágenes para regiones de página, de modo que los visualizadores puedan, por ejemplo, seleccionar un área de la página y abrir una nueva página en el sitio web. Puede gestionar el texto de rollover que aparece mediante la configuración del panel de información en la pantalla del catálogo electrónico. También puede configurar el visor de catálogos electrónicos, para lo cual puede elegir entre más de 100 opciones de configuración diferentes. Puede adaptar las funciones, el aspecto y el diseño del visor según sus destinatarios.

>[!NOTE]
>
>Si es un usuario de Dynamic Media: Scene7 mode y desea utilizar catálogos electrónicos, edite el valor `pdfbrochure` en el CRXDE Lite. Para ello, en Adobe Experience Manager, vaya a **[!UICONTROL Herramientas]** > **[!UICONTROL General]** > **[!UICONTROL CRXDE Lite]**. En el árbol de navegación del panel izquierdo, navegue hasta `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>En el panel inferior derecho, en la ficha **[!UICONTROL Propiedades]**, seleccione la fila `jobParam`. Establezca el valor de `pdfbrochure` de `false` a `true`. Como en `pdfbrochure=true`
>
>En la esquina superior izquierda de la página CRXDE Lite, seleccione **[!UICONTROL Guardar todo]**.
>
>Ahora puede crear catálogos electrónicos en Adobe Dynamic Media Classic.

Este inicio rápido de catálogos electrónicos se ha diseñado para ayudarle en el uso inicial de catálogos electrónicos. Siga los pasos del 1 al 7. Después de cada paso, se hace una referencia cruzada a un encabezado de tema donde puede encontrar más información.

## 1. Cargar los archivos del PDF

Los catálogos electrónicos suelen crearse a partir de archivos PDF. Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. Adobe Dynamic Media Classic detecta estas imágenes y las convierte con un perfil de color CMYK estándar. Sin embargo, debe cargar y utilizar un perfil de color personalizado.

En la barra de navegación global, selecciona **[!UICONTROL Cargar]** para empezar a cargar archivos o imágenes de PDF para tu catálogo electrónico. Puede cargar archivos desde su escritorio o mediante FTP; se recomienda usar FTP si carga muchos archivos o archivos con un tamaño superior a 100 MB.

En la pantalla de carga, Opciones de PDF le ofrece las opciones necesarias para cargar los archivos PDF con la resolución adecuada y el espacio de color correcto. Se recomienda utilizar una resolución de 150 píxeles por pulgada. Puede seleccionar la opción **[!UICONTROL Generar catálogo electrónico automáticamente]** para crear un catálogo electrónico cuando cargue un archivo de PDF.

Consulte [Cargar los archivos del PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Crear un catálogo electrónico

Cree su catálogo electrónico seleccionando PDF o archivos de imagen en el panel Examinar. Seleccione **[!UICONTROL Generar]** y, a continuación, elija **[!UICONTROL catálogos electrónicos]**.

En la página Catálogo electrónico, en la ficha **[!UICONTROL Ordenar páginas]**, seleccione una opción de diseño: **[!UICONTROL 1 arriba]**, **[!UICONTROL 2 arriba]** o **[!UICONTROL personalizado]**. Puede reorganizar las páginas o los conjuntos de páginas arrastrándolos o, en el caso de los catálogos electrónicos de mayor tamaño, eligiendo un nombre de página en el menú Mover a.

Para agregar páginas, seleccione una carpeta en la biblioteca de recursos y arrastre los archivos PDF o de imagen a la pantalla Ordenar páginas. En lugar de los números de página predeterminados, puede proporcionar nombres de página personalizados o importar muchos nombres de página.

Seleccione **[!UICONTROL Guardar]**, escriba un nombre para el catálogo electrónico, elija una carpeta de Adobe Dynamic Media Classic para almacenarla y seleccione **[!UICONTROL Guardar]**. Cada vez que cambie el orden de las páginas o edite el catálogo electrónico, guarde los cambios seleccionando **[!UICONTROL Guardar]**.

Consulte [Crear un catálogo electrónico](creating-ecatalog.md).

## 3. Crear mapas de imagen

Los mapas de imágenes añaden otro aspecto a las páginas del catálogo electrónico. Un mapa de imagen es una región de la página que ofrece más información sobre un elemento determinado. Al pasar el puntero sobre el mapa de imagen, los usuarios verán una descripción del elemento. Al hacer clic en un mapa de imagen, se activa una referencia externa que abre una nueva página Web donde puede obtener más información sobre un elemento.

Para crear un mapa de imagen, abra la pantalla Catálogo electrónico. A continuación, vaya a la ficha **[!UICONTROL Páginas de mapa]** de la pantalla Catálogo electrónico y enmarque el mapa con la herramienta Mapa de imagen rectangular o Mapa de imagen poligonal. Para ajustar la posición y el tamaño de los mapas de imagen, arrastre los bordes de los mapas con la herramienta Panorámica.

Después de enmarcar el mapa de imagen, escriba la dirección URL a la que desea ir al seleccionar el mapa de imagen. También puede escribir el texto de rollover que aparecerá al mover el puntero sobre el mapa de imagen. 

Consulte [Crear mapas de imágenes de catálogo electrónico](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Ver [Usar mapas de imagen para incrustar medios enriquecidos en un catálogo electrónico](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Puede configurar y administrar el texto del mapa de imagen mediante la configuración del panel de información de la pantalla Catálogo electrónico.

Ver [Administrar contenido del panel de información en catálogos electrónicos](/help/using/info-panel-content-ecatalog.md).

## 4. Configurar ajustes preestablecidos del visor de catálogos electrónicos

Los usuarios finales ven el catálogo electrónico en el visor de catálogos electrónicos. Si es un administrador, puede configurar el visor de catálogos electrónicos. Puede cambiar el color del contorno y seleccionar una nueva &quot;apariencia&quot; para personalizar el catálogo electrónico. Adobe Dynamic Media Classic incluye varios ajustes preestablecidos de visualizador de catálogos electrónicos de prácticas recomendadas. Puede elegir uno de estos ajustes preestablecidos para mostrar los catálogos electrónicos. También puede crear un ajuste preestablecido de visor de catálogos electrónicos propio si es administrador.

Para crear un ajuste preestablecido de visor de catálogo electrónico, en la barra de navegación global, seleccione **[!UICONTROL Configuración]** y, a continuación, elija **[!UICONTROL Ajustes preestablecidos de visor]**. Seleccione **[!UICONTROL Agregar]**, elija una plataforma y luego seleccione **[!UICONTROL Catálogo electrónico]** > **[!UICONTROL Visor]**.

Consulte [Configurar ajustes preestablecidos del visor de catálogos electrónicos](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Vista previa de catálogos electrónicos en el visor de catálogos electrónicos

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo y comportamiento de los visores de catálogos electrónicos.

Para saber cómo se muestran los ajustes preestablecidos del visor de catálogos electrónicos en el catálogo electrónico, selecciónelo en el panel Examinar y, a continuación, seleccione **[!UICONTROL Vista previa]**. Se abrirá la pantalla Vista previa en el visor predeterminado.

Fíjese en la orientación, la combinación de colores, el aspecto de los controles con los que se cambia de página y la apariencia de las páginas al pasar de página.

Consulte [Vista previa de catálogos electrónicos en el visor de catálogos electrónicos](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Catálogo electrónico de Publish y PDF asociados

La publicación del catálogo electrónico y del PDF asociado lo coloca en los servidores de imágenes de Dynamic Media para que se pueda enviar al sitio web y a la aplicación. Como parte del proceso de publicación, Adobe Dynamic Media Classic activa la cadena URL del catálogo electrónico. Utilice esta URL para llamar al catálogo electrónico desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Después de marcar el catálogo electrónico y el PDF para publicarlos en el panel Examinar, seleccione el botón Publish de la barra de navegación global para iniciar una publicación. En la página Publicación, seleccione **[!UICONTROL Enviar Publish]**.

Ver [catálogos electrónicos de Publish y PDF asociados](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Vinculación de un catálogo electrónico a una página web

Adobe Dynamic Media Classic activa la cadena de llamada de URL necesaria para mostrar el catálogo electrónico al publicarlo en Dynamic Media Image Servers. Puede copiar esta cadena de URL desde la pantalla Vista previa y el panel Examinar (en la Vista de detalles) seleccionando URL en el panel. Una vez copiada la cadena URL, estará disponible para los sitios Web y las aplicaciones.

Trabaje con su equipo de TI para colocar el vínculo al catálogo electrónico en el lugar adecuado de la página Web. Cuando los usuarios seleccionan el vínculo, aparece el Visor de catálogos electrónicos y los usuarios pueden examinar el catálogo electrónico.

Ver [Vincular un catálogo electrónico a una página web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
