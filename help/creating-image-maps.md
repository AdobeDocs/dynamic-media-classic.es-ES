---
title: Creación de mapas de imagen
description: Aprenda a crear mapas de imágenes.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Administración de recursos
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '2427'
ht-degree: 62%

---

# Creación de mapas de imagen{#creating-image-maps}

Un mapa de imagen es una zona de una imagen, una página del catálogo electrónico o una imagen del Conjunto de giros, que muestra un panel de rollover con texto. Cuando el usuario hace clic en un mapa de imagen, se activa una acción de cierto tipo. Por ejemplo, se abre una página web para que el usuario pueda obtener más información sobre un producto. Un contorno aparece alrededor de un mapa de imagen cuando el usuario mueve el puntero sobre él.

Además de la capacidad de crear mapas de imágenes en Dynamic Media Classic, también puede crear mapas de imágenes al diseñar un catálogo en Adobe Acrobat o Adobe InDesign.

Al crear mapas de imagen, puede realizar cualquiera de las siguientes acciones:

* Introducir texto de rollover.
* Introduzca JavaScript™ y direcciones URL para iniciar páginas web.
* Crear plantillas URL para mapas de imagen.
* Copiar mapas de imagen en otras imágenes, páginas de catálogo electrónico o conjuntos de giro.
* Exportar mapas de imagen a CSV o XML.
* Importe metadatos de imagen desde un archivo delimitado por tabuladores o desde un archivo XML.
* Definir otras acciones determinadas por el consorcio World Wide Web.
* Obtener una vista previa de mapas de imagen.

## Dibujo y ajuste de mapas de imagen {#drawing-and-adjusting-an-image-map}

1. Realice una de las siguientes acciones:

   * Si está trabajando con una imagen en la vista de cuadrícula o de lista, en la lista desplegable Editar haga clic en **Mapa de imagen**. O bien, ábrala en la Vista de detalles y, a continuación, haga clic en **Mapa de imágenes** encima de la imagen.
   * Si está trabajando con un conjunto de giros en la vista de cuadrícula o de lista, haga clic en **Editar**. O bien, ábrala en la Vista de detalles y haga clic en **Editar**. Seleccione un recurso de imagen y haga clic en **Mapa de imagen**.
   * Si está trabajando con un catálogo electrónico, en la vista de cuadrícula, de lista o de detalles, haga clic en **Editar**. Haga clic en la pestaña **Map Pages**.

   ![](assets/ma_image_map.png)

1. Dibuje un mapa de imagen rectangular o poligonal (de varios lados):

   **Mapa** rectangularSeleccione la herramienta Mapa de imagen rectangular y arrastre la página para crear el rectángulo. Para añadir un punto a un mapa rectangular (y, por lo tanto, cambiarlo a un mapa poligonal), pulse Ctrl y, a continuación, coloque la herramienta de inserción en el lugar deseado y haga clic.

   **Mapa poligonal** Seleccione la herramienta Mapa de imagen poligonal y haga clic en los puntos del perímetro del área de la imagen que desea incluir. Use el control deslizante de densidad del polígono para modificar la densidad de punto del polígono. Se recuerda la densidad original al seleccionar otros mapas. Si se añade, elimina o mueve cualquier punto del polígono, se pierde la densidad original y se restablece el valor máximo del control deslizante.

1. Si lo desea, asigne un nombre al mapa de imagen en la lista de mapas de imagen. Después de dibujar un mapa de imagen, Dynamic Media Classic le asigna un nombre.

   Para crear el nombre, Dynamic Media Classic añade un número secuencial al nombre de la imagen o página de catálogo electrónico con la que está trabajando. Puede introducir el nombre que desee.

1. Si desea que se abra una nueva página web cuando los usuarios hagan clic en el mapa de imagen, introduzca la URL en la lista de mapas de imagen. 

   Consulte [para introducir JavaScript™ y direcciones URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Para mostrar texto de rollover cuando los usuarios muevan el puntero sobre el mapa de imagen, introduzca el texto en la lista Mapa de imagen. En la lista de mapas de imagen, seleccione el menú Mostrar y elija Texto de rollover. Introduzca el texto que desee que vean en pantalla los usuarios. Puede escribir el texto en un procesador de textos y copiarlo en el campo Texto de rollover.
1. Si desea que se produzca otra acción cuando los usuarios muevan el ratón sobre un mapa de imagen, defina la acción. En la lista desplegable Mostrar, haga clic en Otras acciones. Introduzca los atributos de la acción. (Haga clic en Mostrar > Ambos para crear texto de rollover y una acción para un mapa de imagen).

   Consulte [Definición de otras acciones para los mapas de imagen](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Opcional) Lleve a cabo uno de los procedimientos siguientes:

   * Para obtener una vista previa de los mapas de imagen, haga clic en **[!UICONTROL Vista previa]**.
   * Para eliminar un mapa de imagen o vértice de polígono, seleccione una forma en la imagen y haga clic en **[!UICONTROL Eliminar]**. O bien, para un catálogo electrónico, en la ficha Ordenar páginas, haga clic en **[!UICONTROL Borrar mapas]** para eliminar los mapas de imagen de todas las páginas.
   * Para quitar temporalmente un mapa de imagen de una imagen, una imagen de un conjunto de giros o una página del catálogo electrónico sin eliminarla, anule la selección de la opción Activado correspondiente en la lista Mapa de imagen.

1. Haga clic en **[!UICONTROL Guardar]**.

### Ajuste de la posición, la forma y el tamaño de los mapas de imagen {#adjusting-the-position-shape-and-size-of-image-maps}

Para cambiar la posición, la forma y el tamaño de un mapa de imagen, seleccione el botón Mapa de imagen . A continuación, seleccione la herramienta **[!UICONTROL Panorámica]** y siga estas instrucciones:

**Cambio de posición** : mueva el puntero cerca del borde del mapa de imagen, pero no por encima de él. Cuando vea el icono de flecha con cuatro puntas, arrastre el mapa a una nueva ubicación.

**Cambiar el tamaño y la forma** : la forma y el tamaño de un mapa de imagen depende de si está trabajando con un mapa de imagen rectangular o poligonal:

>[!TIP]
>
>Puede arrastrar el control deslizante Tamaño en la parte inferior de la pantalla para cambiar de vista y visualizar mejor el mapa de imagen.

**Mapa de imagen rectangular** : mueva el puntero sobre un lado o una esquina del mapa de imagen. Al ver el icono de flecha con dos puntas, comience a arrastrar. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño pero manteniendo la proporción de aspecto (la forma).

**Mapa de imagen poligonal** : arrastre un control de selección cuadrado. Para crear un tirador de selección, haga clic en el borde del mapa de imagen y arrastre el ratón.

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

Puede copiar mapas de imagen de una imagen o página de catálogo electrónico a otra. Utilice **[!UICONTROL Copiar mapa de imagen]** para obtener una idea de cómo empezar a crearlos. También puede copiar mapas de imagen para volver a crearlos en imágenes o páginas que compartan el mismo diseño o la misma estructura de mapas. 

Por ejemplo, copiar mapas de imagen en un catálogo electrónico es una forma cómoda de copiar todos los mapas de imagen entre las versiones en distintos idiomas del mismo catálogo electrónico. Para obtener los mejores resultados, la copia es más eficaz si se realiza entre catálogos electrónicos que tengan el mismo número de páginas y las mismas imágenes. Si el catálogo electrónico al que copia ya contiene mapas de imagen, esos mapas de imagen se eliminan cuando se realiza la copia.

**Para copiar mapas de imagen**

1. Vaya a la página del editor Mapa de imagen (para las imágenes o imágenes de los conjuntos de giros) o a la ficha Páginas de mapa de la pantalla de edición del catálogo electrónico.
1. Haga clic en Copiar mapas a.
1. Realice una de las acciones siguientes, dependiendo de si está copiando los mapas de imagen desde imágenes o desde un catálogo electrónico:

   * (Imágenes) En la pantalla Seleccionar imágenes, seleccione las imágenes a las que desea copiar los mapas de imagen.
   * (Catálogo electrónico) En la pantalla Seleccionar recurso, seleccione las imágenes o las páginas del catálogo electrónico a las que desea copiar los mapas de imagen.

1. Haga clic en Seleccionar.

## Uso de una plantilla para introducir JavaScript™ y direcciones URL {#using-a-template-to-enter-javascript-and-urls}

Puede definir una plantilla URL (conocida también como plantilla Href) para introducir direcciones URL de mapa de imagen con mayor facilidad y eficiencia. Defina una plantilla URL si la mayoría de las URL de mapa de imagen comparten un formato común, fijo. Al introducir la parte de la URL que es fija como plantilla de URL, no tiene que introducir esta parte de la URL cada vez que cree un mapa de imagen. La plantilla URL también puede contener comandos, rutas de acceso y parámetros de JavaScript™. De forma predeterminada, la plantilla URL contiene un controlador propietario de Dynamic Media Classic JavaScript™ llamado `loadProduct` que abre la imagen en una nueva ventana.

>[!NOTE]
>
>Cuando agrega el código JavaScript™ al atributo HREF de su mapa de imagen, el código se ejecuta en el equipo del cliente. Por lo tanto, asegúrese de que el código JavaScript™ sea seguro.

### Acerca de las plantillas URL {#about-url-templates}

La plantilla URL sustituye el contenido de la columna URL en la lista de mapas de imagen con dos signos de dólar (‘$$’) en la plantilla:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Se colocan todos los valores que no cambian entre los mapas de imagen en la plantilla URL. Agregue solo los valores que no cambien en la columna URL en la lista de mapas de imagen. Por ejemplo:

* Plantilla URL: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valor de URL: `product.htm`
* URL real generada: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

De forma predeterminada, la plantilla URL incluye un controlador propietario de Dynamic Media Classic JavaScript™ llamado `loadProduct` que abre una nueva ventana con el destino URL. Sin embargo, puede utilizar cualquier código JavaScript™ para reemplazar este controlador JavaScript™ o utilizar uno de los siguientes controladores de Dynamic Media Classic:

* `loadProductCW`

   muestra el destino URL especificado en la columna URL en la ventana activa. Este controlador es fundamentalmente para catálogos electrónicos que se integran en una página dentro de un sitio Web.

* `loadProductPW`

   muestra el destino URL especificado en la columna URL en la ventana principal (la página que abrió la activa). La ventana activa permanece abierta, pero la principal cambia para mostrar el destino URL.

   >[!NOTE]
   >
   >El controlador `loadProductPW` no admite los visores de DHTML y HTML5.

### Creación de una plantilla URL {#creating-a-url-template}

Para crear una plantilla de URL:

1. En la pantalla Editor de mapas (imágenes o conjuntos de giros) o la ficha Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos), seleccione Editar, junto a la opción Plantilla URL. Se abrirá el cuadro de diálogo Editar la plantilla del mapa.
1. Introduzca el código JavaScript™ y la dirección URL completa (con la parte de variable reemplazada por los signos de dólar [$$]). Puede pegar el código si hace clic con el botón derecho y elige Pegar.
1. Seleccione el botón Guardar.

### Trabajo con plantillas URL {#handling-url-templates}

La página Editor de mapas (imágenes y conjuntos de giros) y la ficha Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos) ofrecen los siguientes comandos para el trabajo con plantillas URL:

* **Opción Plantilla URL** Seleccione la opción Plantilla URL para aplicar la plantilla URL a todos los mapas de imagen de una imagen o página de catálogo electrónico.

* **Plantilla** opciónAnule la selección de una opción Plantilla en la lista Mapa de imagen de URL si no desea que un Mapa de imagen individual utilice la plantilla URL.

## Definición de otras acciones para los mapas de imagen {#defining-other-actions-for-image-maps}

Puede seleccionar el menú Mostrar y elegir Otras acciones para activar acciones que no sean las de texto de rollover e inicio de página web. Cuando el usuario mueve el puntero sobre un mapa de imagen, se puede iniciar una acción. Estas acciones son atributos definidos para mapas de imagen de la parte del cliente acorde con las especificaciones del lenguaje HTML del consorcio World Wide Web. Incluyen:

* **acceskey** : Déclencheur una acción cuando el usuario pulsa una tecla designada en el teclado.

* **onfocus** : Déclencheur un evento cuando el mapa de imagen recibe el enfoque, por el cursor, por tabulación o presionando una clave de acceso. Por ejemplo, puede abrir una página web cuando el mapa de imagen recibe atención y cerrarla cuando pierde dicha atención.

* **onblur** : Déclencheur un evento en el que el mapa de imagen pierde el foco, ya sea por el cursor o mediante tabulación.

**Para definir otras acciones para los mapas de imagen:**

1. En la pantalla Editor de mapas (imágenes y conjuntos de giros) o la ficha Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos), seleccione el menú Mostrar y elija Otras acciones.
1. Mediante la sintaxis del lenguaje HTML del consorcio World Wide Web, agregue los atributos admitidos en la columna Otras acciones de la lista de mapas de imagen.
1. Haga clic en **[!UICONTROL Guardar]**.

Seleccione el menú **[!UICONTROL Mostrar]** y elija **[!UICONTROL Ambos]** si desea que un mapa de imagen tenga texto de sustitución y una acción.

## Creación de mapas de imagen en Adobe Acrobat o en Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Puede crear mapas de imagen mientras diseña su catálogo electrónico en Adobe Acrobat o en Adobe InDesign.

En Acrobat o InDesign, cree referencias de hipervínculo donde desee que aparezcan los mapas de imagen y especifique ubicaciones de URL para el mapa de imagen. Al seleccionar la opción Extraer vínculos al cargar el archivo PDF en Dynamic Media Classic, los vínculos se convierten automáticamente en mapas de imágenes.

Para obtener más información, consulte la Ayuda de Adobe InDesign o la Ayuda de Adobe Acrobat.

### Para crear mapas de imagen en Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. En el InDesign, haga clic en **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hipervínculos]** para abrir el panel Hipervínculos.
1. Seleccione el texto, fotograma o gráfico que desea que aparezca en el mapa de imagen.
1. En el panel Hipervínculos, haga clic en **[!UICONTROL Nuevo hipervínculo]** en el menú del panel.
1. En el cuadro de diálogo Nuevo hipervínculo, seleccione **[!UICONTROL URL]** en el menú Vincular a.
1. Escriba o pegue el ID del producto en el cuadro URL y haga clic en **[!UICONTROL Aceptar]**. (Dynamic Media Classic completa la dirección URL usando la plantilla de dirección URL del mapa de imagen ).

   >[!NOTE]
   >
   >No es necesario que configure las opciones de aspecto en Adobe InDesign. Puede especificar la apariencia en Dynamic Media Classic.

1. Repita los pasos 2 a 5 para todos los mapas de imágenes que desee crear.
1. Exporte el archivo como PDF.
1. Cargue el PDF a Dynamic Media Classic y seleccione Extraer vínculos en las Opciones de PDF.

### Para crear mapas de imagen en Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. En Acrobat, haga clic en **[!UICONTROL Herramientas]** > **[!UICONTROL Edición avanzada]** > **[!UICONTROL Herramienta de enlace]**.
1. Arrastre para crear el mapa de imagen. Se abre el cuadro Crear vínculo.
1. Seleccione **[!UICONTROL Vínculo personalizado]** y haga clic en **[!UICONTROL Siguiente]**.

>[!NOTE]
>
>No es necesario que configure las opciones de aspecto en Adobe Acrobat. Puede especificar la apariencia en Dynamic Media Classic.

1. En el cuadro Propiedades del vínculo, haga clic en **[!UICONTROL Acciones]**.
1. Seleccione **[!UICONTROL Abrir un vínculo web]** en el menú Seleccionar acción y, a continuación, haga clic en **[!UICONTROL Agregar]**.
1. Escriba el ID del producto para el mapa de imagen en el cuadro Editar URL y haga clic en **[!UICONTROL Aceptar]**. (Dynamic Media Classic completa la dirección URL usando la plantilla URL de mapa de imagen).
1. Repita los pasos 1 a 7 para todos los mapas de imágenes que desee crear.
1. Guarde el archivo.
1. Cargue el PDF a Dynamic Media Classic y seleccione Extraer vínculos en las Opciones de PDF.
