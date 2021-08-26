---
title: '"Inicio rápido: Catálogos electrónicos"'
description: Introducción y inicio rápido a los catálogos electrónicos para ayudarle a poner en marcha rápidamente las técnicas del catálogo electrónico.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 48%

---

# Inicio rápido: Catálogos electrónicos{#quick-start-ecatalogs}

Un catálogo electrónico es una versión web digital de material impreso: por ejemplo, un catálogo, un folleto, un manual de un producto o una circular publicitaria. Los catálogos electrónicos se muestran en un visor de catálogos electrónicos contenido en un sitio web. Este visor simula la lectura de material impreso. Según la configuración que elija para el catálogo electrónico, el visor puede permitirle hacer lo siguiente:

* Busque en el catálogo una palabra clave o palabras clave. Los resultados de la búsqueda se muestran como una lista de miniaturas en un panel de búsqueda situado en la parte izquierda del catálogo. Cada miniatura en la que se puede hacer clic representa una extensión de catálogo en la que se encontró el término de búsqueda resaltado.

* Compartir el catálogo a través de los medios sociales; descargar el catálogo para verlo sin conexión; active Favoritos para marcar los elementos a los que desee regresar rápidamente o imprimir el catálogo.
* Navegar por el catálogo utilizando la tabla de contenido o la vista de cuadrícula de página; hacia delante o hacia atrás haciendo clic en el borde medio de una página.
* Acercar o alejar la página, y desplazarse por ella para examinar sus elementos.
* Mueva el puntero sobre una región de la página (denominada mapa de imagen) para que pueda ver una ventana emergente con información sobre un elemento.
* Haga clic en una región de página para abrir una nueva página web con más información sobre un elemento.
* Escribir una nota adhesiva y adjuntarla a una página del catálogo electrónico.
* Pulse los iconos de mapa de imagen si desea iniciar páginas web relacionadas o paneles de información en contexto.
* Usar interacciones de gestos como pellizcar para ampliar y reducir la imagen o arrastrar para pasar de página.
* Buscar elementos por palabras clave.

![Catálogo electrónico tal como aparece para los usuarios. A) página de apertura del catálogo electrónico. B)Catálogo electrónico convertido a la página 2.](/help/assets/ec_cat_viewer_popup.png)

Para crear un catálogo electrónico, suelen utilizarse archivos PDF de alta resolución creados en Adobe® Acrobat® o en otro programa de impresión, aunque también pueden crearse catálogos electrónicos a partir de archivos de imagen.

Al crear el catálogo electrónico, tiene la posibilidad de ordenar como desee páginas o conjuntos de páginas. También puede decidir si desea ver páginas individuales, dobles o múltiples. Puede crear mapas de imagen en algunas regiones de las páginas para que los usuarios puedan, por ejemplo, hacer clic en una zona de la página y abrir una nueva página dentro de su sitio web. Puede gestionar el texto de rollover que aparece mediante la configuración del panel de información en la pantalla del catálogo electrónico. También puede configurar el visor de catálogos electrónicos, para lo cual puede elegir entre más de 100 opciones de configuración diferentes. Puede adaptar las funciones, el aspecto y el diseño del visor según sus destinatarios.

>[!NOTE]
>
>Si es usuario del modo Dynamic Media - Scene7 y desea utilizar catálogos electrónicos, debe editar el valor `pdfbrochure` en CRXDE Lite. Para ello, en Adobe Experience Manager, haga clic en **[!UICONTROL Tools]** > **[!UICONTROL General]** > **[!UICONTROL CRXDE Lite]**. En el árbol de navegación del panel izquierdo, vaya a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>En el panel inferior derecho, en la pestaña **[!UICONTROL Properties]**, seleccione la fila `jobParam`. Establezca el valor para `pdfbrochure` de `false` a `true`. Como en `pdfbrochure=true`
>
>En la esquina superior izquierda de la página CRXDE Lite, haga clic en **[!UICONTROL Guardar todo]**.
>
>Ahora puede crear catálogos electrónicos en Adobe Dynamic Media Classic.

Este inicio rápido de catálogos electrónicos se ha diseñado para ayudarle en el uso inicial de catálogos electrónicos. Siga los pasos del 1 al 7. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

## 1. Carga de los archivos PDF

Los catálogos electrónicos suelen crearse a partir de archivos PDF. Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. Adobe Dynamic Media Classic detecta estas imágenes y las convierte utilizando un perfil de color CMYK estándar. Sin embargo, debe cargar y usar un perfil de color personalizado.

En la barra de navegación global, haga clic en **[!UICONTROL Cargar]** para iniciar la carga de archivos PDF o imágenes para su catálogo electrónico. Puede cargar archivos desde el escritorio o por medio de FTP; se recomienda usar FTP si va a cargar muchos archivos o archivos cuyo tamaño es superior a 100 MB.

En la pantalla de carga, Opciones de PDF le ofrece las opciones necesarias para cargar los archivos PDF con la resolución adecuada y el espacio de color correcto. Se recomienda utilizar una resolución de 150 píxeles por pulgada. Puede seleccionar la opción Generar catálogo electrónico automáticamente y crear un catálogo electrónico al cargar un archivo PDF. 

Consulte [Carga de archivos PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Creación de un catálogo electrónico

Cree su catálogo electrónico seleccionando archivos PDF o de imagen en el panel Examinar. Haga clic en **[!UICONTROL Generar]** y, a continuación, elija **[!UICONTROL Catálogos electrónicos]**.

En la página Catálogo electrónico, en la ficha **[!UICONTROL Ordenar páginas]**, seleccione una opción Diseño: **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** o **[!UICONTROL Custom]**. Puede reorganizar las páginas o los conjuntos de páginas arrastrándolos o, en el caso de los catálogos electrónicos de mayor tamaño, eligiendo un nombre de página en el menú Mover a.

Para agregar páginas, seleccione una carpeta en la biblioteca de recursos y arrastre los archivos PDF o de imagen a la pantalla Ordenar páginas. En lugar de los números de página predeterminados, puede proporcionar nombres de página personalizados o importar muchos nombres de página.

Haga clic en **[!UICONTROL Guardar]**, introduzca un nombre para el catálogo electrónico, elija una carpeta de Dynamic Media Classic de Adobe para almacenarla y haga clic en **[!UICONTROL Guardar]**. Cada vez que cambie el orden de la página o edite el catálogo electrónico, guarde los cambios haciendo clic en **[!UICONTROL Guardar]**.

Consulte [Creación de un catálogo electrónico](creating-ecatalog.md).

## 3. Creación de mapas de imagen

Los mapas de imagen añaden otro aspecto a las páginas del catálogo electrónico. Un mapa de imagen es una región de la página que ofrece más información sobre un elemento determinado. Al pasar el puntero sobre el mapa de imagen, los usuarios verán una descripción del elemento. Al hacer clic en el mapa de imagen se activa una referencia externa, que abre una nueva página web donde hay más información sobre el elemento seleccionado.

Para crear un mapa de imagen, abra la pantalla Catálogo electrónico. A continuación, vaya a la pestaña **[!UICONTROL Páginas de mapa]** de la pantalla del catálogo electrónico y enmarque el mapa con la herramienta Rectángulo de mapa de imagen o la herramienta Polígono de mapa de imagen. Si desea ajustar la posición y el tamaño de los mapas de imagen, arrastre los bordes del mapa con la Herramienta de desplazamiento .

Después de enmarcar el mapa de imagen, introduzca la dirección URL a la que desea dirigirse cuando haga clic en el mapa de imagen. También puede escribir el texto de rollover que aparecerá al mover el puntero sobre el mapa de imagen. 

Consulte [Creación de mapas de imagen de catálogos electrónicos](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulte [Uso de mapas de imagen para incrustar medios enriquecidos en catálogos electrónicos](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Puede configurar y gestionar el texto del mapa de imagen mediante la configuración del panel de información en la pantalla del catálogo electrónico.

Consulte [Administrar contenido del panel de información en catálogos electrónicos](/help/info-panel-content-ecatalog.md).

## 4. Configuración de ajustes preestablecidos del visor de catálogos electrónicos

Los usuarios finales ven el catálogo electrónico en el visor de catálogos electrónicos. Si es un administrador, puede configurar el visor de catálogos electrónicos. Puede cambiar el color del contorno y seleccionar una nueva “apariencia” para personalizar el catálogo electrónico. Adobe Dynamic Media Classic incluye varios ajustes preestablecidos de visor de catálogos electrónicos &quot;recomendados&quot;. Puede elegir uno de estos ajustes preestablecidos para mostrar los catálogos electrónicos. También puede crear un ajuste preestablecido de visor de catálogos electrónicos propio si es administrador.

Para crear un ajuste preestablecido de visualizador de catálogos electrónicos, en la barra de navegación global, haga clic en **[!UICONTROL Configuración]** y seleccione **[!UICONTROL Ajustes preestablecidos de visualizador]**. A continuación, haga clic en **[!UICONTROL Add]**, elija una plataforma y haga clic en **[!UICONTROL eCatalog > Viewer]**.

Consulte [Configuración de ajustes preestablecidos del visor de catálogos electrónicos](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Vista previa de catálogos electrónicos en el visor de catálogos electrónicos

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo y comportamiento de los visores de catálogos electrónicos.

Para saber cómo se muestran los ajustes preestablecidos del visor de catálogos electrónicos en el catálogo electrónico, seleccione el catálogo electrónico en el panel Examinar y haga clic en **[!UICONTROL Vista previa]**. Se abrirá la pantalla Vista previa en el visor predeterminado.

Fíjese en la orientación, la combinación de colores, el aspecto de los controles con los que se cambia de página y la apariencia de las páginas al pasar de página.

Consulte [Vista previa de catálogos electrónicos en el visor de catálogos electrónicos](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publicación de catálogos electrónicos y archivos PDF asociados

Al publicar el catálogo electrónico y el PDF asociado, se coloca en los servidores de imágenes de Dynamic Media para que se pueda enviar al sitio web y a la aplicación. Como parte del proceso de publicación, Adobe Dynamic Media Classic activa la cadena URL del catálogo electrónico. Utilice esta URL para llamar al catálogo electrónico desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Después de marcar el catálogo electrónico y el PDF para su publicación en el panel Examinar, seleccione el botón Publicar en la barra de navegación global para iniciar una publicación. En la pantalla Publicar, haga clic en **[!UICONTROL Enviar publicación]**.

Consulte [Publicación de catálogos electrónicos y archivos PDF asociados](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Vinculación de un catálogo electrónico a una página web

Adobe Dynamic Media Classic activa la cadena de llamada de URL necesaria para mostrar el catálogo electrónico cuando se publica en los servidores de imágenes de Dynamic Media. Puede copiar esta cadena URL desde la pantalla Vista previa y el panel Examinar (en la Vista detallada) seleccionando direcciones URL en el panel. Cuando haya copiado la cadena URL, estará disponible para los sitios web y las aplicaciones.

Decida junto con su grupo de TI cuál es el lugar más apropiado de la página web para colocar el vínculo al catálogo electrónico. Al hacer clic en el vínculo, aparecerá el visor de catálogos electrónicos y los usuarios podrán examinar el catálogo electrónico.

Consulte [Vinculación de un catálogo electrónico a una página web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
