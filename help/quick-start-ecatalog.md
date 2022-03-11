---
title: '"Inicio rápido: Catálogos electrónicos"'
description: Introducción y inicio rápido a los catálogos electrónicos para ayudarle a poner en marcha rápidamente las técnicas del catálogo electrónico en Adobe Dynamic Media Classic.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: ec1a981dd5cfa92ce4ae8e2676dd131d1509216f
workflow-type: tm+mt
source-wordcount: '1558'
ht-degree: 36%

---

# Inicio rápido: Catálogos electrónicos{#quick-start-ecatalogs}

Un catálogo electrónico es una versión web digital de material impreso: por ejemplo, un catálogo, un folleto, un manual de un producto o una circular publicitaria. Los catálogos electrónicos se muestran en un visor de catálogos electrónicos contenido en un sitio web. Este visor simula la lectura de material impreso.

Consulte también los siguientes vídeos de formación:

* [Inicio rápido 1: Catálogos electrónicos](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Inicio rápido 2: Catálogos electrónicos](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Según la configuración que elija para el catálogo electrónico, el visor puede permitirle hacer lo siguiente:

* Busque en el catálogo una palabra clave o palabras clave. Los resultados de la búsqueda se muestran como una lista de miniaturas en un panel de búsqueda situado en la parte izquierda del catálogo. Cada miniatura en la que se puede hacer clic representa una extensión de catálogo en la que se encontró el término de búsqueda resaltado.

* Compartir el catálogo a través de los medios sociales; descargar el catálogo para verlo sin conexión; active Favoritos para marcar los elementos a los que desee regresar rápidamente o imprimir el catálogo.
* Navegar por el catálogo utilizando la tabla de contenido o la vista de cuadrícula de página; hacia delante o hacia atrás haciendo clic en el borde medio de una página.
* Acercar o alejar la página, y desplazarse por ella para examinar sus elementos.
* Mueva el puntero sobre una región de la página (denominada mapa de imagen) para que pueda ver una ventana emergente con información sobre un elemento.
* Seleccione una región de página para que se abra una nueva página web con más información sobre un elemento.
* Escribir una nota adhesiva y adjuntarla a una página del catálogo electrónico.
* Pulse los iconos de mapa de imagen si desea iniciar páginas web relacionadas o paneles de información en contexto.
* Usar interacciones de gestos como pellizcar para ampliar y reducir la imagen o arrastrar para pasar de página.
* Buscar elementos por palabras clave.

![Catálogo electrónico tal como aparece para los usuarios. A) página de apertura del catálogo electrónico. B)Catálogo electrónico convertido a la página 2.](/help/assets/ec_cat_viewer_popup.png)

Para crear un catálogo electrónico, normalmente se utilizan archivos de PDF de alta resolución creados en Adobe Acrobat u otro programa de impresión, pero también se puede crear un catálogo electrónico a partir de archivos de imagen.

Al crear el catálogo electrónico, tiene la posibilidad de ordenar como desee páginas o conjuntos de páginas. También puede decidir si desea ver páginas individuales, dobles o múltiples. Puede crear mapas de imagen para las regiones de la página, de modo que los visitantes puedan, por ejemplo, seleccionar un área en la página y abrir una nueva página en el sitio web. Puede gestionar el texto de rollover que aparece mediante la configuración del panel de información en la pantalla del catálogo electrónico. También puede configurar el visor de catálogos electrónicos, para lo cual puede elegir entre más de 100 opciones de configuración diferentes. Puede adaptar las funciones, el aspecto y el diseño del visor según sus destinatarios.

>[!NOTE]
>
>Si es usuario del modo Dynamic Media - Scene7 y desea utilizar catálogos electrónicos, edite la `pdfbrochure` en CRXDE Lite. Para ello, en Adobe Experience Manager, vaya a **[!UICONTROL Herramientas]** > **[!UICONTROL General]** > **[!UICONTROL CRXDE Lite]**. En el árbol de navegación del panel izquierdo, vaya a `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>En el panel inferior derecho, en la **[!UICONTROL Propiedades]** , seleccione `jobParam` fila. Establezca el valor de `pdfbrochure` from `false` a `true`. Como en `pdfbrochure=true`
>
>En la esquina superior izquierda de la página CRXDE Lite, seleccione **[!UICONTROL Guardar todo]**.
>
>Ahora puede crear catálogos electrónicos en Adobe Dynamic Media Classic.

Este inicio rápido de catálogos electrónicos se ha diseñado para ayudarle en el uso inicial de catálogos electrónicos. Siga los pasos del 1 al 7. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

## 1. Cargue los archivos del PDF

Los catálogos electrónicos suelen crearse a partir de archivos PDF. Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. Adobe Dynamic Media Classic detecta estas imágenes y las convierte utilizando un perfil de color CMYK estándar. Sin embargo, debe cargar y usar un perfil de color personalizado.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]** para empezar a cargar archivos PDF o imágenes para su catálogo electrónico. Puede cargar archivos desde el escritorio o por medio de FTP; se recomienda usar FTP si va a cargar muchos archivos o archivos cuyo tamaño es superior a 100 MB.

En la pantalla de carga, Opciones de PDF le ofrece las opciones necesarias para cargar los archivos PDF con la resolución adecuada y el espacio de color correcto. Se recomienda utilizar una resolución de 150 píxeles por pulgada. Puede seleccionar la opción Generar catálogo electrónico automáticamente y crear un catálogo electrónico al cargar un archivo PDF. 

Consulte [Carga de los archivos del PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Crear un catálogo electrónico

Cree su catálogo electrónico seleccionando archivos de imagen o PDF en el panel Examinar. Select **[!UICONTROL Generar]** y, a continuación, elija **[!UICONTROL Catálogos electrónicos]**.

En la página Catálogo electrónico, en la **[!UICONTROL Ordenar páginas]** , seleccione una opción Diseño: **[!UICONTROL 1 arriba]**, **[!UICONTROL 2 arriba]** o **[!UICONTROL Personalizado]**. Puede reorganizar las páginas o los conjuntos de páginas arrastrándolos o, en el caso de los catálogos electrónicos de mayor tamaño, eligiendo un nombre de página en el menú Mover a.

Para agregar páginas, seleccione una carpeta en la biblioteca de recursos y arrastre los archivos PDF o de imagen a la pantalla Ordenar páginas. En lugar de los números de página predeterminados, puede proporcionar nombres de página personalizados o importar muchos nombres de página.

Select **[!UICONTROL Guardar]**, introduzca un nombre para el catálogo electrónico, elija una carpeta de Adobe Dynamic Media Classic para almacenarla y seleccione **[!UICONTROL Guardar]**. Cada vez que cambie el orden de la página o edite el catálogo electrónico, guarde los cambios haciendo clic en **[!UICONTROL Guardar]**.

Consulte [Crear un catálogo electrónico](creating-ecatalog.md).

## 3. Crear mapas de imagen

Los mapas de imagen añaden otro aspecto a las páginas del catálogo electrónico. Un mapa de imagen es una región de la página que ofrece más información sobre un elemento determinado. Al pasar el puntero sobre el mapa de imagen, los usuarios verán una descripción del elemento. Al hacer clic en el mapa de imagen se activa una referencia externa, que abre una nueva página web donde hay más información sobre el elemento seleccionado.

Para crear un mapa de imagen, abra la pantalla Catálogo electrónico. A continuación, vaya a la **[!UICONTROL Asignar páginas]** de la pantalla Catálogo electrónico, y enmarque el mapa con la herramienta Mapa de imagen de rectángulo o la herramienta Mapa de imagen de polígono. Si desea ajustar la posición y el tamaño de los mapas de imagen, arrastre los bordes del mapa con la Herramienta de desplazamiento .

Después de enmarcar el mapa de imagen, introduzca la dirección URL a la que desea dirigirse cuando seleccione el mapa de imagen. También puede escribir el texto de rollover que aparecerá al mover el puntero sobre el mapa de imagen. 

Consulte [Creación de mapas de imagen de catálogos electrónicos](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulte [Usar mapas de imagen para incrustar medios enriquecidos en un catálogo electrónico](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Puede configurar y gestionar el texto del mapa de imagen mediante la configuración del panel de información en la pantalla del catálogo electrónico.

Consulte [Administrar contenido del panel de información en catálogos electrónicos](/help/info-panel-content-ecatalog.md).

## 4. Configurar ajustes preestablecidos del visualizador de catálogos electrónicos

Los usuarios finales ven el catálogo electrónico en el visor de catálogos electrónicos. Si es un administrador, puede configurar el visor de catálogos electrónicos. Puede cambiar el color del contorno y seleccionar una nueva “apariencia” para personalizar el catálogo electrónico. Adobe Dynamic Media Classic incluye varios ajustes preestablecidos de visor de catálogos electrónicos &quot;recomendados&quot;. Puede elegir uno de estos ajustes preestablecidos para mostrar los catálogos electrónicos. También puede crear un ajuste preestablecido de visor de catálogos electrónicos propio si es administrador.

Para crear un ajuste preestablecido de visualizador de catálogos electrónicos, en la barra de navegación global, seleccione **[!UICONTROL Configuración]** y, a continuación, elija **[!UICONTROL Ajustes preestablecidos de visor]**. Select **[!UICONTROL Agregar]**, elija una plataforma y, a continuación, seleccione **[!UICONTROL Catálogo electrónico]** > **[!UICONTROL Visualizador]**.

Consulte [Configuración de ajustes preestablecidos del visualizador de catálogos electrónicos](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Previsualizar catálogos electrónicos en el visor de catálogos electrónicos

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo y comportamiento de los visores de catálogos electrónicos.

Para saber cómo se muestran los ajustes preestablecidos del visor de catálogos electrónicos en el catálogo electrónico, seleccione el catálogo electrónico en el panel Examinar y, a continuación, seleccione **[!UICONTROL Vista previa]**. Se abrirá la pantalla Vista previa en el visor predeterminado.

Fíjese en la orientación, la combinación de colores, el aspecto de los controles con los que se cambia de página y la apariencia de las páginas al pasar de página.

Consulte [Vista previa de catálogos electrónicos en el visor de catálogos electrónicos](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publicar catálogo electrónico y PDF asociados

Al publicar el catálogo electrónico y el PDF asociado, se coloca en los servidores de imágenes de Dynamic Media para que se pueda enviar al sitio web y a la aplicación. Como parte del proceso de publicación, Adobe Dynamic Media Classic activa la cadena URL del catálogo electrónico. Utilice esta URL para llamar al catálogo electrónico desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Después de marcar el catálogo electrónico y el PDF para su publicación en el panel Examinar, seleccione el botón Publicar en la barra de navegación global para iniciar una publicación. En la pantalla Publicar , seleccione **[!UICONTROL Enviar publicación]**.

Consulte [Publicar catálogos electrónicos y PDF asociados](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Vincular un catálogo electrónico a una página web

Adobe Dynamic Media Classic activa la cadena de llamada URL necesaria para mostrar el catálogo electrónico cuando se publica en los servidores de imágenes de Dynamic Media. Puede copiar esta cadena URL desde la pantalla Vista previa y el panel Examinar (en la Vista detallada) seleccionando direcciones URL en el panel. Cuando haya copiado la cadena URL, estará disponible para los sitios web y las aplicaciones.

Decida junto con su grupo de TI cuál es el lugar más apropiado de la página web para colocar el vínculo al catálogo electrónico. Cuando los usuarios seleccionan el vínculo, aparece el visor de catálogos electrónicos y los usuarios pueden navegar por el catálogo electrónico.

Consulte [Vincular un catálogo electrónico a una página web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
