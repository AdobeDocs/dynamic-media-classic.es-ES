---
title: Creación de mapas de imagen
seo-title: Creación de mapas de imagen
description: nulo
seo-description: Aprenda a crear mapas de imagen.
uuid: 0 dcc 4956-006 e -4 a 74-9 d 6 a -6 d 4 bb 23790 ce
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 4 eddf 983-38 cb -4 f 00-b 3 be -85 c 20 bdd 6 f 69
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Creación de mapas de imagen{#creating-image-maps}

Un mapa de imagen es una zona de una imagen, una página del catálogo electrónico o una imagen del Conjunto de giros, que muestra un panel de rollover con texto. Cuando el usuario hace clic en un mapa de imagen, se activa una acción de cierto tipo. Por ejemplo, se abre una página web para que el usuario pueda obtener más información sobre un producto. Para llamar la atención sobre un mapa de imagen, aparece un contorno alrededor de este cuando el usuario coloca el puntero sobre él.

Además de crear un mapa de imagen en Dynamic Media Classic, también puede crear mapas de imagen al diseñar un catálogo en Adobe Acrobat o Adobe indesign.

Al crear mapas de imagen, puede realizar cualquiera de las siguientes acciones:

* Introducir texto de rollover.
* Introducir JavaScript y URL para abrir páginas web.
* Crear plantillas URL para mapas de imagen.
* Copiar mapas de imagen en otras imágenes, páginas de catálogo electrónico o conjuntos de giro.
* Exportar mapas de imagen a CSV o XML.
* Importar metadatos de imagen desde un archivo delimitado por tabuladores o desde un archivo XML.
* Definir otras acciones determinadas por el consorcio World Wide Web.
* Obtener una vista previa de mapas de imagen.

## Dibujo y ajuste de mapas de imagen {#drawing-and-adjusting-an-image-map}

1. Realice una de las siguientes acciones:

   * If you are working with an image in the Grid View or List View, in the Edit drop-down list click **Image Map**. Or, open it in Detail View, and then click **Image Map** above the image.
   * If you are working with a SpinSet in the Grid View or List View, click **Edit**. Or, open it in Detail View, and then click **Edit**. Select an image asset, and then click **Image Map**.
   * If you are working with an eCatalog, in the Grid View, List View, Detail View, click **Edit**. Click the **Map Pages** tab.
   ![](assets/ma_image_map.png)

1. Dibuje un mapa de imagen rectangular o poligonal (de varios lados):

   **Mapa rectangular** Seleccione la herramienta de asignación de imagen rectangular y arrastre en la página para crear el rectángulo. Para añadir un punto a un mapa rectangular (y, por lo tanto, cambiarlo a un mapa poligonal), pulse Ctrl y, a continuación, coloque la herramienta de inserción en el lugar deseado y haga clic.

   **Mapa poligonal** Seleccione la herramienta de mapa de imagen poligonal y haga clic en puntos del perímetro del área de la imagen que desee encerrar. Use el control deslizante de densidad del polígono para modificar la densidad de punto del polígono. Se recuerda la densidad original al seleccionar otros mapas. Si se añade, elimina o mueve cualquier punto del polígono, se pierde la densidad original y se restablece el valor máximo del control deslizante.

1. Si lo desea, asigne un nombre al mapa de imagen en la lista de mapas de imagen. Después de dibujar un mapa de imagen, Dynamic Media Classic le asigna un nombre.

   Para crear el nombre, Dynamic Media Classic anexa un número secuencial al nombre de la imagen o página del catálogo electrónico con la que está trabajando. Puede introducir el nombre que desee.

1. Si desea que se abra una nueva página web cuando los usuarios hagan clic en el mapa de imagen, introduzca la URL en la lista de mapas de imagen. 

   Consulte [Uso de plantillas para introducir elementos de JavaScript y direcciones URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Para mostrar texto de rollover cuando los usuarios muevan el puntero sobre el mapa de imagen, introduzca el texto en la lista Mapa de imagen. En la lista de mapas de imagen, seleccione el menú Mostrar y elija Texto de rollover. Introduzca el texto que desee que vean en pantalla los usuarios. Puede escribir el texto en un procesador de textos y copiarlo en el campo Texto de rollover.
1. Si desea que se produzca otra acción cuando los usuarios muevan el ratón sobre un mapa de imagen, defina la acción. En la lista desplegable Mostrar, haga clic en Otras acciones. Introduzca los atributos de la acción. (Haga clic en Mostrar &gt; Ambos para crear texto de rollover y una acción para un mapa de imagen).

   Consulte [Definición de otras acciones para los mapas de imagen](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Opcional) Lleve a cabo uno de los procedimientos siguientes:

   * Haga clic en Vista previa para realizar una vista previa de los mapas de imagen.
   * Para eliminar un mapa de imagen o vértice de polígono, seleccione una forma de la imagen y, a continuación, haga clic en Eliminar. O bien, en un catálogo electrónico, en la ficha Ordenar páginas, haga clic en Borrar mapas para eliminar los mapas de imagen de todas las páginas.
   * Para quitar temporalmente un mapa de imagen de una imagen, una imagen de un conjunto de giros o una página del catálogo electrónico sin eliminarla, anule la selección de la opción Activado correspondiente en la lista Mapa de imagen.

1. Haga clic en Guardar.

### Ajuste de la posición, la forma y el tamaño de los mapas de imagen {#adjusting-the-position-shape-and-size-of-image-maps}

Para cambiar la posición, la forma y el tamaño de un mapa de imagen, seleccione el botón Mapa de imagen . A continuación, seleccione la herramienta de desplazamiento y siga estas instrucciones:

**Cambio de posición** Mueva el puntero cerca del borde del mapa de imagen, pero no por encima del mismo. Cuando vea el icono de flecha con cuatro puntas, arrastre el mapa a una nueva ubicación.

**Cambiar el tamaño y la forma** de cambio de forma y tamaño de un mapa de imagen depende de si está trabajando con un mapa de imagen rectangular o poligonal:

***Sugerencia**: Puede arrastrar el control deslizante Tamaño en la parte inferior de la pantalla para cambiar las vistas y ver mejor el mapa de imagen.*

**Mapa de imagen rectangular** Mueva el puntero sobre un lado o una esquina del mapa de imagen. Al ver el icono de flecha con dos puntas, comience a arrastrar. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño pero manteniendo la proporción de aspecto (la forma).

**Mapa de imagen poligonal** Arrastre un tirador de selección cuadrada. Para crear un tirador de selección, haga clic en el borde del mapa de imagen y arrastre el ratón.

### Control de superposición de mapas de imagen {#handling-overlapping-image-maps}

Si la imagen o página de catálogo electrónico incluye más de un mapa de imagen y estos se superponen, puede determinar cómo lo hacen. Para ello, cambie el orden de los mapas en la lista de mapas de imagen. Arrastre sus nombres hacia la parte superior o inferior de la lista. La posición de un nombre en la lista determina si su mapa de imagen se superpone sobre otros.

### Importación de datos de mapa de imagen {#importing-image-map-data}

En lugar de introducir datos de mapa de imagen en cada página, puede importar los datos de su conjunto de giros o catálogo electrónico desde la pantalla Resumen de mapas. Los datos de mapa de imagen se importan como un archivo delimitado por tabuladores o DTD de XML. Los campos del archivo deben tener el orden que se muestra en la pantalla Resumen de mapas: Nombre, Etiquetas de tabla de contenido, Mapas, Direcciones URL, Texto de rollover, Otras acciones y Cadenas de búsqueda. Si importa los datos de mapa de imagen, no tendrá que introducir los datos en la lista de mapas de imagen cada vez que crea un mapa de imagen.

**Para importar los datos de mapa de imagen**

1. Vaya a la página del editor Mapa de imagen (para las imágenes o imágenes de los conjuntos de giros) o a la ficha Páginas de mapa de la pantalla de edición del catálogo electrónico.
1. Haga clic en Importar metadatos.
1. En el cuadro de diálogo Cargar metadatos, haga clic en la imagen o mapa de imagen para cargar los metadatos del tipo de propiedad de recurso que desee.
1. En la lista desplegable Generar archivo, seleccione el tipo de archivo que desea crear.
1. (Opcional) Haga clic en Generar para obtener una vista previa de los datos resultantes en función del tipo de archivo que desea crear. Haga clic en Cerrar para regresar al cuadro de diálogo Cargar metadatos.
1. Busque el archivo que desea cargar. En el campo de texto Nombre del archivo, especifique el nombre del archivo generado.
1. (Opcional) En el campo Nombre del trabajo, especifique un nombre para el trabajo de carga de metadatos.
1. Haga clic en Cargar.

### Copia de mapas de imagen {#copying-image-maps}

Puede copiar mapas de imagen de una imagen o página de catálogo electrónico a otra. Utilice la copia de mapas de imagen para avanzar en su creación. También puede copiar mapas de imagen para volver a crearlos en imágenes o páginas que compartan el mismo diseño o la misma estructura de mapas. 

Por ejemplo, copiar mapas de imagen en un catálogo electrónico es una forma cómoda de copiar todos los mapas de imagen entre las versiones en distintos idiomas del mismo catálogo electrónico. Para obtener los mejores resultados, la copia es más eficaz si se realiza entre catálogos electrónicos que tengan el mismo número de páginas y las mismas imágenes. Si el catálogo electrónico al que copia ya contiene mapas de imagen, dichos mapas se eliminarán cuando se realice la copia.

**Para copiar mapas de imagen**

1. Vaya a la página del editor Mapa de imagen (para las imágenes o imágenes de los conjuntos de giros) o a la ficha Páginas de mapa de la pantalla de edición del catálogo electrónico.
1. Haga clic en Copiar mapas a.
1. Realice una de las acciones siguientes, dependiendo de si está copiando los mapas de imagen desde imágenes o desde un catálogo electrónico:

   * (Imágenes) En la pantalla Seleccionar imágenes, seleccione las imágenes a las que desea copiar los mapas de imagen.
   * (Catálogo electrónico) En la pantalla Seleccionar recurso, seleccione las imágenes o las páginas del catálogo electrónico a las que desea copiar los mapas de imagen.

1. Haga clic en Seleccionar.

## Uso de plantillas para introducir elementos de JavaScript y direcciones URL {#using-a-template-to-enter-javascript-and-urls}

Puede definir una plantilla URL (conocida también como plantilla Href) para introducir direcciones URL de mapa de imagen con mayor facilidad y eficiencia. Defina una plantilla URL si la mayoría de las URL de mapa de imagen comparten un formato común, fijo. Al introducir la parte de la URL que es fija como plantilla de URL, no tiene que introducir esta parte de la URL cada vez que cree un mapa de imagen. La plantilla URL también puede contener comandos JavaScript, nombres de ruta y parámetros. By default, the URL template contains a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens the image in a new window.

>[!NOTE]
>
>Tenga en cuenta que al añadir el código JavaScript al atributo HREF del mapa de imagen, el código se ejecutará en el equipo del cliente. Por lo tanto, compruebe que el código JavaScript sea seguro.

### Acerca de las plantillas URL {#about-url-templates}

La plantilla URL sustituye el contenido de la columna URL en la lista de mapas de imagen con dos signos de dólar (‘$$’) en la plantilla:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Deberá colocar todos los valores que no cambian entre los mapas de imagen en la plantilla URL. Agregue solo los valores que no cambien en la columna URL en la lista de mapas de imagen. Por ejemplo:

* Plantilla URL: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valor de URL: `product.htm`
* URL real generada: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

By default, the URL template includes a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens a new window with the URL destination. Sin embargo, puede utilizar cualquier código JavaScript para reemplazar este controlador JavaScript o utilizar uno de los siguientes controladores de Dynamic Media Classic:

* `loadProductCW`

   muestra el destino URL especificado en la columna URL en la ventana activa. Este controlador es fundamentalmente para catálogos electrónicos que se integran en una página dentro de un sitio Web.

* `loadProductPW`

   muestra el destino URL especificado en la columna URL en la ventana principal (la página que abrió la activa). La ventana activa permanece abierta, pero la principal cambia para mostrar el destino URL.

   ***nota**: El controlador`loadProductPW`no admite visores DHTML ni HTML 5.*

### Creación de una plantilla URL {#creating-a-url-template}

Para crear una plantilla de URL:

1. En la pantalla Editor de mapas (imágenes o conjuntos de giros) o la ficha Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos), seleccione Editar, junto a la opción Plantilla URL. Se abrirá el cuadro de diálogo Editar la plantilla del mapa.
1. Introduzca el código JavaScript y la URL completa (con la parte variable sustituida por signo de dólar [$$]). Puede pegar el código si hace clic con el botón derecho y elige Pegar.
1. Seleccione el botón Guardar.

### Trabajo con plantillas URL {#handling-url-templates}

La página Editor de mapas (imágenes y conjuntos de giros) y la ficha Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos) ofrecen los siguientes comandos para el trabajo con plantillas URL:

**Opción Plantilla URL** Seleccione la opción Plantilla URL para aplicar la plantilla URL a todos los mapas de imagen en una imagen o página de catálogo electrónico.

**Opción Plantilla** Anule la selección de una opción Plantilla en la lista de mapas de imagen URL si no desea que un mapa de imagen individual use la plantilla URL.

## Definición de otras acciones para los mapas de imagen {#defining-other-actions-for-image-maps}

Puede seleccionar el menú Mostrar y elegir Otras acciones para activar acciones que no sean las de texto de rollover e inicio de página web. Cuando el usuario mueve el puntero sobre un mapa de imagen, se puede iniciar una acción. Estas acciones son atributos definidos para mapas de imagen de la parte del cliente acorde con las especificaciones del lenguaje HTML del consorcio World Wide Web. Incluyen:

**accesskey** Desencadena una acción cuando el usuario pulsa una tecla designada en el teclado.

**onfocus** Desencadena un evento cuando el mapa de imagen recibe atención, por el cursor, por el tabulador o por una tecla de acceso. Por ejemplo, puede abrir una página web cuando el mapa de imagen recibe atención y cerrarla cuando pierde dicha atención.

**onblur** Desencadena un evento cuando el mapa de imagen pierde atención, ya sea por el cursor o por tabulación.

**Para definir otras acciones para los mapas de imagen**

1. En la pantalla Editor de mapas (imágenes y conjuntos de giros) o la ficha Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos), seleccione el menú Mostrar y elija Otras acciones.
1. Mediante la sintaxis del lenguaje HTML del consorcio World Wide Web, agregue los atributos admitidos en la columna Otras acciones de la lista de mapas de imagen.
1. Haga clic en **Guardar**.

Seleccione el menú Mostrar y elija Ambos si desea que un mapa de imagen tenga texto de rollover además de una acción.

## Creación de mapas de imagen en Adobe Acrobat o en Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Puede crear mapas de imagen mientras diseña su catálogo electrónico en Adobe Acrobat o en Adobe InDesign.

En Acrobat o InDesign, cree referencias de hipervínculo donde desee que aparezcan los mapas de imagen y especifique ubicaciones de URL para el mapa de imagen. Al seleccionar la opción Extraer vínculos al cargar el archivo PDF en Dynamic Media Classic, se convierten automáticamente los vínculos a mapas de imagen.

Para obtener más información, consulte la Ayuda de InDesign o Acrobat.

### Para crear mapas de imagen en Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. En InDesign, haga clic en Ventana &gt; Interactiva &gt; Hipervínculos para abrir el panel Hipervínculos.
1. Seleccione el texto, fotograma o gráfico que desea que aparezca en el mapa de imagen.
1. En el panel de hipervínculos, haga clic en Nuevo hipervínculo en el menú del panel.
1. En el cuadro de diálogo Nuevo Hipervínculo, elija URL en el menú Vincular a.
1. Escriba o pegue la ID de producto en el cuadro URL y haga clic en Aceptar. (Dynamic Media Classic completa la URL utilizando la plantilla URL del mapa de imagen).

   >[!NOTE]
   >
   >No es necesario definir las opciones de apariencia en InDesign. Puede especificar la apariencia en Dynamic Media Classic.

1. Repita los pasos 2 a 5 para todos los mapas de imágenes que desee crear.
1. Exporte el archivo como PDF.
1. Cargue el PDF en Dynamic Media Classic y seleccione Extraer vínculos de las opciones de PDF.

### Para crear mapas de imagen en Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. En Acrobat, elija Herramientas &gt; Edición avanzada &gt; Herramienta Vínculos.
1. Arrastre para crear el mapa de imagen. Se abre el cuadro Crear vínculo.
1. Seleccione Vínculo personalizado y haga clic en Siguiente.

   ***nota**: No es necesario definir las opciones de apariencia en Acrobat. Puede especificar la apariencia en Dynamic Media Classic.*

1. En el cuadro Propiedades del Vínculo, haga clic en Acciones.
1. Seleccione Abrir un vínculo web en el menú Seleccionar acción y haga clic en Agregar.
1. Escriba la ID del producto para el mapa de imagen en el cuadro Editar URL y haga clic en Aceptar. (Dynamic Media Classic completa la URL utilizando la plantilla URL del mapa de imagen).
1. Repita los pasos 1 a 7 para todos los mapas de imágenes que desee crear.
1. Guarde el archivo.
1. Cargue el PDF en Dynamic Media Classic y seleccione Extraer vínculos de las opciones de PDF.

