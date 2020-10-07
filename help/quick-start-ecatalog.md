---
title: '"Inicio rápido: Catálogos electrónicos"'
seo-title: '"Inicio rápido: Catálogos electrónicos"'
description: nulo
seo-description: Introducción y Inicio rápido a los catálogos electrónicos para ayudarle en el uso inicial de las técnicas de catálogos electrónicos.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: 83b88623b898fdadd1b334b1c12901830c831c5c
workflow-type: tm+mt
source-wordcount: '1450'
ht-degree: 63%

---


# Inicio rápido: Catálogos electrónicos{#quick-start-ecatalogs}

Un catálogo electrónico es una versión web digital de material impreso: por ejemplo, un catálogo, un folleto, un manual de un producto o una circular publicitaria. Los catálogos electrónicos se muestran en un visor de catálogos electrónicos contenido en un sitio web. Este visor simula la lectura de material impreso. Según la configuración que elija para el catálogo electrónico, el visor puede permitirle hacer lo siguiente:

* Busque en el catálogo una palabra clave o palabras clave. Los resultados de la búsqueda se muestran como una lista de miniaturas en un panel de búsqueda a la izquierda del catálogo. Cada miniatura en la que se puede hacer clic representa un pliego de catálogo en el que se encontró el término de búsqueda resaltado.

* Compartir el catálogo a través de los medios sociales; descargar el catálogo para vista sin conexión; active Favoritos para marcar los elementos a los que desee volver rápidamente o imprimir el catálogo.
* Navegue por el catálogo utilizando la tabla de contenido o la vista de cuadrícula de página; para avanzar o retroceder, haga clic en el borde medio de una página.
* Acercar o alejar la página, y desplazarse por ella para examinar sus elementos.
* Pasar el puntero por encima de una región de la página (denominada mapa de imagen) para ver una ventana emergente con información sobre un producto.
* Hacer clic en una región de la página para abrir una nueva página web con más información sobre un determinado producto.
* Escribir una nota adhesiva y adjuntarla a una página del catálogo electrónico.
* Tocar los iconos del mapa de imagen para iniciar las páginas web relacionadas o los paneles de información en contexto.
* Usar interacciones de gestos como pellizcar para ampliar y reducir la imagen o arrastrar para pasar de página.
* Buscar elementos por palabras clave.

![Catálogo electrónico que ven los usuarios. A) Página de inicio del catálogo electrónico. B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

Para crear un catálogo electrónico, suelen utilizarse archivos PDF de alta resolución creados en Adobe® Acrobat® o en otro programa de impresión, aunque también pueden crearse catálogos electrónicos a partir de archivos de imagen.

Al crear el catálogo electrónico, tiene la posibilidad de ordenar como desee páginas o conjuntos de páginas. También puede decidir si desea ver páginas individuales, dobles o múltiples. Puede crear mapas de imagen en algunas regiones de las páginas para que los usuarios puedan, por ejemplo, hacer clic en una zona de la página y abrir una nueva página dentro de su sitio web. Puede gestionar el texto de rollover que aparece mediante la configuración del panel de información en la pantalla del catálogo electrónico. También puede configurar el visor de catálogos electrónicos, para lo cual puede elegir entre más de 100 opciones de configuración diferentes. Puede adaptar las funciones, el aspecto y el diseño del visor según sus destinatarios.

>[!NOTE]
>
>Si es un usuario del modo Medios dinámicos AEM - Scene7 y desea utilizar catálogos electrónicos, deberá editar el `pdfbrochure` valor en CRXDE Lite. Para ello, en AEM, haga clic en **[!UICONTROL Herramientas > General > CRXDE Lite]**. En el árbol de navegación del panel izquierdo, vaya a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>En el panel inferior derecho, en la ficha **[!UICONTROL Propiedades]** , seleccione la `jobParam` fila. Establezca el valor de `pdfbrochure` de `false` a `true`. Como en `pdfbrochure=true`
>
>En la esquina superior izquierda de la página CRXDE Lite, haga clic en **[!UICONTROL Guardar todo]**.
>
>Ahora podrá crear catálogos electrónicos en Dynamic Media Classic.

**Inicio rápido**

Este inicio rápido de catálogos electrónicos se ha diseñado para ayudarle en el uso inicial de catálogos electrónicos. Siga los pasos del 1 al 7. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

**1. Carga de archivos PDF**

Los catálogos electrónicos suelen crearse a partir de archivos PDF. Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. Dynamic Media Classic detecta estas imágenes y las convierte con un perfil de color CMYK estándar. Sin embargo, quizás debe cargar y usar un perfil de color personalizado.

Haga clic en Cargar en la barra de navegación global para cargar inicios de archivos PDF o imágenes para el catálogo electrónico. Puede cargar archivos desde el escritorio o por medio de FTP; se recomienda usar FTP si va a cargar muchos archivos o archivos cuyo tamaño es superior a 100 MB.

En la pantalla de carga, Opciones de PDF le ofrece las opciones necesarias para cargar los archivos PDF con la resolución adecuada y el espacio de color correcto. Se recomienda utilizar una resolución de 150 píxeles por pulgada. Puede seleccionar la opción Generar catálogo electrónico automáticamente y crear un catálogo electrónico al cargar un archivo PDF. 

Consulte [Carga de archivos PDF](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Creación de un catálogo electrónico**

Para crear un catálogo electrónico, seleccione los archivos PDF o archivos de imagen en el panel Examinar, haga clic en el botón Generar y elija Catálogos electrónicos. Se abre la pantalla Catálogo electrónico. 

En la ficha Ordenar páginas, seleccione uno de los botones de presentación (1 vertical, 2 verticales o personalizado) para elegir si desea que se muestre una página individual, una doble o si desea personalizar la presentación. Puede reorganizar las páginas o los conjuntos de páginas arrastrándolos o, en el caso de los catálogos electrónicos de mayor tamaño, eligiendo un nombre de página en el menú Mover a.

Para agregar páginas, seleccione una carpeta en la biblioteca de recursos y arrastre los archivos PDF o de imagen a la pantalla Ordenar páginas. Si no desea utilizar la numeración de páginas predeterminada, puede proporcionar nombres de página personalizados o importar varios nombres de página.

Haga clic en **[!UICONTROL Guardar]**, escriba un nombre para el catálogo electrónico, elija una carpeta de Dynamic Media Classic para almacenarla y haga clic en **[!UICONTROL Guardar]**. Each time you change the page order or edit your eCatalog, save your changes by clicking **[!UICONTROL Save]**.

Consulte [Creación de un catálogo electrónico](creating-ecatalog.md).

**3. Creación de mapas de imagen**

Los mapas de imagen agregan otra dimensión a las páginas del catálogo electrónico. Un mapa de imagen es una región de la página que ofrece más información sobre un elemento determinado. Al pasar el puntero sobre el mapa de imagen, los usuarios verán una descripción del elemento. Al hacer clic en el mapa de imagen se activa una referencia externa, que abre una nueva página web donde hay más información sobre el elemento seleccionado.

Para crear un mapa de imagen, abra la pantalla Catálogo electrónico. Then go to the **[!UICONTROL Map Pages]** tab of the eCatalog screen, and draw the map with the Rectangle Image Map tool or Polygon Image Map tool. Si desea ajustar la posición y el tamaño de los mapas de imagen, arrastre los bordes del mapa con la Herramienta de desplazamiento .

Tras dibujar el mapa de imagen, introduzca la dirección URL a la que desea ir al hacer clic en el mapa de imagen. También puede escribir el texto de rollover que aparecerá al mover el puntero sobre el mapa de imagen. 

Consulte [Creación de mapas de imagen de catálogos electrónicos](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulte [Uso de mapas de imagen para incrustar medios enriquecidos en catálogos electrónicos](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Puede configurar y gestionar el texto del mapa de imagen mediante la configuración del panel de información en la pantalla del catálogo electrónico.

Consulte [Gestión del contenido del panel de información](info-panel-content.md#managing-info-panel-content).

**4. Configuración de ajustes preestablecidos del visor de catálogos electrónicos**

Los usuarios finales ven el catálogo electrónico en el visor de catálogos electrónicos. Si es un administrador, puede configurar el visor de catálogos electrónicos. Puede cambiar el color del contorno y seleccionar una nueva “apariencia” para personalizar el catálogo electrónico. Dynamic Media Classic incluye varios ajustes preestablecidos de visor de catálogos electrónicos &quot;recomendados&quot;. Puede elegir uno de estos ajustes preestablecidos para mostrar los catálogos electrónicos. También puede crear un ajuste preestablecido de visor de catálogos electrónicos propio si es administrador.

Para crear un ajuste preestablecido de visor de catálogos electrónicos, en la barra de navegación global, haga clic en **[!UICONTROL Ajustes]** y elija Ajustes preestablecidos **[!UICONTROL de visor]**. Then click **[!UICONTROL Add]**, choose a platform, then click **[!UICONTROL eCatalog > Viewer]**.

Consulte [Configuración de ajustes preestablecidos del visor de catálogos electrónicos](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

**5. Vista previa de catálogos electrónicos en el visor de catálogos electrónicos**

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo y comportamiento de los visores de catálogos electrónicos.

To find out how eCatalog Viewer Presets display your eCatalog, select your eCatalog in the Browse Panel and click **[!UICONTROL Preview]**. Se abrirá la pantalla Vista previa en el visor predeterminado.

Fíjese en la orientación, la combinación de colores, el aspecto de los controles con los que se cambia de página y la apariencia de las páginas al pasar de página.

Consulte [Vista previa de catálogos electrónicos en el visor de catálogos electrónicos](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Publicación de catálogos electrónicos y archivos PDF asociados**

Al publicar el catálogo electrónico y el PDF asociado, éste se coloca en los servidores de imágenes de Dynamic Media para que se pueda entregar en el sitio web y la aplicación. Como parte del proceso de publicación, Dynamic Media Classic activa la cadena URL del catálogo electrónico. Utilice esta URL para llamar al catálogo electrónico desde los servidores de imágenes de Dynamic Media al sitio web o la aplicación.

Después de marcar el catálogo electrónico y el PDF para publicación en el panel Examinar, seleccione el botón Publicar en la barra de navegación global para iniciar una publicación. On the Publish screen, click **[!UICONTROL Start Publish]**.

Consulte [Publicación de catálogos electrónicos y archivos PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)asociados.

**7. Vinculación de un catálogo electrónico a una página web**

Dynamic Media Classic activa la cadena de llamada URL necesaria para mostrar el catálogo electrónico al publicarlo en los servidores de imágenes de Dynamic Media. Puede copiar esta cadena URL desde la pantalla Vista previa o desde la vista de detalles del panel Examinar si selecciona Direcciones URL en el panel. Cuando haya copiado la cadena URL, estará disponible para los sitios web y las aplicaciones.

Decida junto con su grupo de TI cuál es el lugar más apropiado de la página web para colocar el vínculo al catálogo electrónico. Al hacer clic en el vínculo, aparecerá el visor de catálogos electrónicos y los usuarios podrán examinar el catálogo electrónico.

Consulte [Vinculación de un catálogo electrónico a una página web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
