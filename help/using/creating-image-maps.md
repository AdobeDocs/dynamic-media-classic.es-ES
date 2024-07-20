---
title: Crear mapas de imagen
description: Obtenga información sobre cómo crear mapas de imagen en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '2444'
ht-degree: 31%

---

# Crear mapas de imagen {#creating-image-maps}

Un mapa de imagen es una región de una imagen, una página de catálogo electrónico o una imagen de un conjunto de giros que muestra un panel de rollover con texto. Cuando el usuario selecciona un mapa de imagen, se activa un tipo de acción. Por ejemplo, se inicia una página web para que el usuario pueda obtener más información sobre un producto. Aparece un contorno alrededor de un mapa de imagen cuando el usuario mueve el puntero sobre él.

Además de la capacidad de crear mapas de imágenes en Adobe Dynamic Media Classic, también puede crear mapas de imágenes al diseñar un catálogo en Adobe Acrobat o Adobe InDesign.

Al crear mapas de imagen, puede realizar una de las siguientes acciones:

* Introducir texto de rollover.
* Introduzca JavaScript y direcciones URL para iniciar páginas web.
* Crear plantillas URL para mapas de imagen.
* Copiar mapas de imagen en otras imágenes, páginas de catálogo electrónico o conjuntos de giro.
* Exportar mapas de imagen a CSV o XML.
* Importe metadatos de imagen desde un archivo delimitado por tabuladores o desde un archivo XML.
* Defina Otras acciones según lo determinado por el World Wide Web Consortium.
* Obtener una vista previa de mapas de imagen.

## Dibujo y ajuste de un mapa de imagen {#drawing-and-adjusting-an-image-map}

1. Realice una de las siguientes acciones:

   * Si está trabajando con una imagen en la vista de cuadrícula o en la vista de lista, en la lista desplegable Editar seleccione **[!UICONTROL Mapa de imágenes]**. O bien, ábralo en Vista de detalles y, a continuación, seleccione **[!UICONTROL Mapa de imagen]** encima de la imagen.
   * Si está trabajando con un conjunto de giros en la vista de cuadrícula o vista de lista, seleccione **[!UICONTROL Editar]**. O bien, ábralo en Vista de detalles y, a continuación, seleccione **[!UICONTROL Editar]**. Seleccione un recurso de imagen y, a continuación, seleccione **[!UICONTROL Mapa de imagen]**.
   * Si está trabajando con un catálogo electrónico, en las vistas Cuadrícula, Lista, Detalle, seleccione **[!UICONTROL Editar]**. Seleccione la ficha **[!UICONTROL Asignar páginas]**.

   ![Ilustración de mapa de imagen](assets/ma_image_map.png)

1. Dibuje un mapa de imagen rectangular o poligonal (de varios lados):

   * **Mapa rectangular**: Seleccione la herramienta Mapa de imagen rectangular y arrastre en la página para crear el rectángulo. Para añadir un punto a un mapa rectangular (convirtiéndolo así en un mapa poligonal), pulse Ctrl, coloque la herramienta de inserción en la ubicación deseada y seleccione.

   * **Mapa poligonal**: seleccione la herramienta Mapa de imagen poligonal y seleccione puntos en el perímetro del área de la imagen que desea incluir. Use el control deslizante de densidad del polígono para modificar la densidad de punto del polígono. Se recuerda la densidad original al seleccionar otros mapas. Si se añade, elimina o mueve algún punto en el polígono, se pierde la densidad original. El control deslizante se restablece a su valor máximo.

1. Si lo desea, asigne un nombre al mapa de imagen en la lista de mapas de imagen. Después de dibujar un mapa de imagen, Adobe Dynamic Media Classic le asigna un nombre.

   Para crear el nombre, Adobe Dynamic Media Classic añade un número secuencial al nombre de la imagen o página de catálogo electrónico con la que está trabajando. Puede introducir el nombre que desee.

1. Si desea que los usuarios abran una nueva página Web al seleccionar el mapa de imagen, escriba la dirección URL en la lista Mapa de imagen.

   Consulte [para ingresar JavaScript y direcciones URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Para mostrar texto de rollover cuando los usuarios muevan el puntero sobre el mapa de imagen, introduzca el texto en la lista Mapa de imagen. En la lista Mapa de imagen, seleccione el menú **[!UICONTROL Mostrar]** y seleccione **[!UICONTROL Texto de rollover]**. A continuación, escriba el texto que desea que los usuarios vean en pantalla. Puede escribir el texto en un procesador de textos y copiarlo en el campo Texto de rollover.

1. Si desea que se produzca otra acción cuando los usuarios muevan el ratón sobre un mapa de imagen, defina la acción. En la lista desplegable **[!UICONTROL Mostrar]**, seleccione **[!UICONTROL Otras acciones]**. Introduzca los atributos de la acción. (Vaya a **[!UICONTROL Mostrar]** > **[!UICONTROL Ambos]** para crear texto de rollover y una acción para un mapa de imagen).

   Ver [Definir otras acciones para los mapas de imágenes](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Opcional) Lleve a cabo uno de los procedimientos siguientes:

   * Para obtener una vista previa de los mapas de imágenes, seleccione **[!UICONTROL Vista previa]**.
   * Para eliminar un vértice de polígono o un mapa de imagen, seleccione una forma de la imagen y, a continuación, seleccione **[!UICONTROL Eliminar]**. O bien, para un catálogo electrónico, en la ficha Ordenar páginas, seleccione **[!UICONTROL Borrar mapas]** para quitar los mapas de imágenes de todas las páginas.
   * Para eliminar un:
      * Mapa de imagen de una imagen
      * Crear una imagen en un conjunto de giros
      * o una página de catálogo electrónico

     de forma temporal, sin eliminarla, anule la selección de la opción Activado correspondiente en la lista Mapa de imagen.

1. Seleccione **[!UICONTROL Guardar]**.

### Ajustar la posición, la forma y el tamaño de los mapas de imagen {#adjusting-the-position-shape-and-size-of-image-maps}

Para cambiar la posición, la forma y el tamaño de un mapa de imagen, seleccione el botón Mapa de imagen. A continuación, seleccione la herramienta **[!UICONTROL Panorámica]** y siga estas instrucciones:

* **Cambiar posición**: mueva el puntero cerca del borde del mapa de imagen, pero no sobre él. Cuando vea el icono de flecha con cuatro puntas, arrastre el mapa a una nueva ubicación.

* **Cambiar el tamaño y la forma**: El modo de cambiar la forma y el tamaño de un mapa de imagen depende de si está trabajando con un mapa de imagen rectangular o poligonal:

>[!TIP]
>
>Puede arrastrar el control deslizante Tamaño en la parte inferior de la pantalla para cambiar de vista y visualizar mejor el mapa de imagen.

* **Mapa de imagen rectangular**: mueva el puntero sobre un lado o esquina del Mapa de imagen. Al ver el icono de flecha con dos puntas, comience a arrastrar. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño pero mantener la relación de aspecto (la forma).

* **Mapa de imagen poligonal**: arrastre un controlador de selección cuadrado. Para crear un controlador de selección, seleccione el borde del mapa de imagen y comience a arrastrar.

### Gestión de mapas de imagen superpuestos {#handling-overlapping-image-maps}

Si la imagen o la página de catálogo electrónico incluye más de un mapa de imagen y los mapas se superponen, puede determinar cómo se superponen los mapas. Para ello, cambie el orden de los mapas en la lista de mapas de imagen. Arrastre sus nombres hacia la parte superior o inferior de la lista. La posición de un nombre en la lista determina si su mapa de imagen se superpone sobre otros.

### Importación de datos de mapa de imagen {#importing-image-map-data}

En lugar de introducir datos de mapa de imagen en cada página, puede importar los datos de su conjunto de giros o catálogo electrónico desde la pantalla Resumen de mapas. Los datos de mapa de imagen se importan como un archivo delimitado por tabuladores o DTD de XML. Los campos del archivo deben tener el orden que se muestra en la pantalla Resumen de mapas: Nombre, Etiquetas de tabla de contenido, Mapas, Direcciones URL, Texto de rollover, Otras acciones y Cadenas de búsqueda. La importación de datos de mapa de imagen evita tener que introducir los datos en la lista de mapa de imagen a medida que se crea cada mapa de imagen.

**Para importar datos de mapa de imagen:**

1. Vaya a la página del editor Mapa de imagen (para las imágenes o imágenes de los conjuntos de giros) o a la ficha Páginas de mapa de la pantalla de edición del catálogo electrónico.
1. Seleccione **[!UICONTROL Importar metadatos]**.
1. En el cuadro de diálogo Cargar metadatos, seleccione Imagen o Mapa de imagen para cargar los metadatos desde el tipo de propiedad de recurso deseado.
1. En la lista desplegable `Generate File`, seleccione el tipo de archivo que desea crear.
1. (Opcional) Seleccione **[!UICONTROL Generar]** para obtener una vista previa de los datos resultantes en función del tipo de archivo que desee crear. Seleccione **[!UICONTROL Cerrar]** para volver al cuadro de diálogo Cargar metadatos.
1. Busque el archivo que desea cargar. En el campo de texto Nombre del archivo, especifique el nombre del archivo generado.
1. (Opcional) En el campo Nombre del trabajo, especifique un nombre para el trabajo de carga de metadatos.
1. Seleccione **[!UICONTROL Cargar]**.

### Copiar mapas de imagen {#copying-image-maps}

Puede copiar mapas de imagen de una imagen o página de catálogo electrónico a otra. Use **[!UICONTROL Copiar mapa de imagen]** para empezar a crearlos. También puede copiar mapas de imagen para volver a crearlos en imágenes o páginas que compartan diseño o estructura de asignación.

Por ejemplo, copiar los mapas de imágenes en un catálogo electrónico es una forma cómoda de copiar todos los mapas de imágenes entre versiones en idiomas extranjeros del mismo catálogo electrónico. Para obtener mejores resultados, la copia es más exitosa si copia entre catálogos electrónicos con el mismo número de páginas y las mismas imágenes. Si el catálogo electrónico al que copia ya contiene mapas de imágenes, estos se eliminan cuando se realiza la copia.

**Para copiar los mapas de imagen:**

1. Vaya a la página del editor Mapa de imagen (para las imágenes o imágenes de los conjuntos de giros) o a la ficha Páginas de mapa de la pantalla de edición del catálogo electrónico.
1. Seleccionar **[!UICONTROL Copiar asignaciones en]**.
1. Realice una de las acciones siguientes, dependiendo de si está copiando los mapas de imagen desde imágenes o desde un catálogo electrónico:

   * (Imágenes) En la pantalla Seleccionar imágenes, seleccione las imágenes a las que desea copiar los mapas de imagen.
   * (Catálogo electrónico) En la pantalla Seleccionar recurso, seleccione las imágenes o las páginas del catálogo electrónico a las que desea copiar los mapas de imagen.

1. Elija **[!UICONTROL Seleccionar]**.

## Utilice una plantilla para introducir JavaScript y direcciones URL {#using-a-template-to-enter-javascript-and-urls}

Puede definir una plantilla URL (conocida también como plantilla Href) para introducir direcciones URL de mapa de imagen con mayor facilidad y eficiencia. Defina una plantilla URL si la mayoría de las URL de mapa de imagen comparten un formato común, fijo. Al introducir la parte de la URL que es fija como plantilla de URL, no tiene que introducir esta parte de la URL cada vez que cree un mapa de imagen. La plantilla URL también puede contener comandos, nombres de ruta y parámetros de JavaScript. De manera predeterminada, la plantilla de dirección URL contiene un controlador JavaScript de Adobe Dynamic Media Classic propiedad denominado `loadProduct` que abre la imagen en una nueva ventana.

>[!NOTE]
>
>Cuando agrega el código JavaScript al atributo HREF del mapa de imágenes, el código se ejecuta en el equipo cliente. Por lo tanto, asegúrese de que el código de JavaScript sea seguro.

### Acerca de las plantillas URL {#about-url-templates}

La plantilla URL funciona sustituyendo el contenido de la columna URL en la lista Mapa de imágenes. Lo sustituye por los signos de dólar dobles (&#39;$$&#39;) en la plantilla:

```as3
Javascript:loadProduct('$$');void(0);
```

En la plantilla URL se colocan todos los valores que no cambian entre Mapas de imagen. Agregue solo los valores que no cambien en la columna URL en la lista de mapas de imagen. Por ejemplo:

* Plantilla de URL: `javascript:loadProduct('https://www.examplesitehere.com/$$');void(0);`
* Valor de URL: `product.htm`
* Dirección URL real generada: `javascript:loadProduct('https://www.examplesitehere.com/product.html);void(0);`

De manera predeterminada, la plantilla de dirección URL incluye un controlador JavaScript de Adobe Dynamic Media Classic propiedad denominado `loadProduct` que abre una nueva ventana con el destino de la dirección URL. Sin embargo, puede utilizar cualquier código de JavaScript para reemplazar este controlador de JavaScript o utilizar uno de los siguientes controladores de Adobe Dynamic Media Classic:

* `loadProductCW`: muestra el destino de URL especificado en la columna URL de la ventana actual. Este controlador es fundamentalmente para catálogos electrónicos que se integran en una página dentro de un sitio Web.

* `loadProductPW`: muestra el destino de dirección URL especificado en la columna URL de la ventana principal (la página que abrió la actual). La ventana activa permanece abierta, pero la principal cambia para mostrar el destino URL.

  >[!NOTE]
  >
  >El controlador `loadProductPW` no admite visores DHTML y HTML 5.

### Creación de una plantilla de URL {#creating-a-url-template}

1. En la pantalla Editor de mapas (imágenes o conjuntos de giros) o en la pestaña Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos), seleccione Editar junto a la opción Plantilla URL. Se abrirá el cuadro de diálogo Editar la plantilla del mapa.
1. Introduzca el código JavaScript y la dirección URL completa (con la parte de variable reemplazada por signos de dólar [$]). Puede pegar el código haciendo clic con el botón derecho y eligiendo **[!UICONTROL Pegar]**.
1. Seleccione **[!UICONTROL Guardar]**.

### Administrar plantillas de URL {#handling-url-templates}

La página Editor de mapas (imágenes y conjuntos de giros) y la ficha Páginas de mapa de la pantalla Catálogo electrónico (catálogos electrónicos) ofrecen los siguientes comandos para el trabajo con plantillas URL:

* **Opción de plantilla URL**: seleccione la opción de plantilla URL para aplicar la plantilla URL a todos los mapas de imágenes de una imagen o página de catálogo electrónico.

* **Opción de plantilla**: anule la selección de una opción de plantilla en la lista Mapa de imágenes de URL si no desea que un mapa de imágenes individual utilice la plantilla URL.

## Definir otras acciones para los mapas de imagen {#defining-other-actions-for-image-maps}

Puede seleccionar el menú **[!UICONTROL Mostrar]** y elegir **[!UICONTROL Otras acciones]** para almacenar en déclencheur acciones que no sean texto de rollover y lanzamientos de páginas web. Cuando el usuario mueve el puntero sobre un mapa de imagen, se puede iniciar una acción. Estas acciones son atributos definidos para mapas de imagen de la parte del cliente acorde con las especificaciones del lenguaje HTML del consorcio World Wide Web. Incluyen:

* **`accesskey`**: Déclencheur una acción cuando el usuario presiona una tecla designada en el teclado.

* **`onfocus`**: almacena en Déclencheur un evento cuando el mapa de imagen recibe el enfoque mediante el cursor, tabulando o presionando una tecla de acceso. Por ejemplo, puede iniciar una página web cuando el mapa de imagen recibe el enfoque y cerrarla cuando el mapa de imagen pierde el enfoque.

* **`onblur`**: almacena en Déclencheur un evento cuando el mapa de imagen pierde el enfoque, ya sea por el cursor o por tabulación.

**Para definir otras acciones para los mapas de imágenes:**

1. En la pantalla Editor de mapas (imágenes y conjuntos de giros) o en la pestaña Páginas de mapas de la pantalla Catálogo electrónico (eCatálogos), seleccione el menú **[!UICONTROL Mostrar]** y seleccione **[!UICONTROL Otras acciones]**.
1. Mediante la sintaxis del lenguaje HTML del consorcio World Wide Web, agregue los atributos admitidos en la columna Otras acciones de la lista de mapas de imagen.
1. Seleccione **[!UICONTROL Guardar]**.

Seleccione el menú **[!UICONTROL Mostrar]** y seleccione **[!UICONTROL Ambos]** si desea que un mapa de imagen tenga texto de rollover y una acción.

## Creación de mapas de imagen en Adobe Acrobat o Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Puede crear mapas de imagen mientras diseña su catálogo electrónico en Adobe Acrobat o en Adobe InDesign.

En Adobe Acrobat o Adobe InDesign, cree referencias de hipervínculo donde desee que aparezcan los mapas de imagen y especifique las ubicaciones URL para el mapa de imagen. Al seleccionar la opción Extraer vínculos al cargar el archivo del PDF en Adobe Dynamic Media Classic, se convierten automáticamente los vínculos a mapas de imágenes.

Para obtener más información, consulte Ayuda de Adobe InDesign o Ayuda de Adobe Acrobat.

### Para crear mapas de imagen en Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. En Adobe InDesign, vaya a **[!UICONTROL Windows®]** > **[!UICONTROL Interactivo]** > **[!UICONTROL Hipervínculos]**.
1. En el panel Hipervínculos, seleccione el texto, el marco o el gráfico que desea convertir en un mapa de imagen.
1. Seleccione **[!UICONTROL Nuevo hipervínculo]** en el menú del panel.
1. En el cuadro de diálogo Nuevo hipervínculo, en el menú **[!UICONTROL Vincular a]**, elija la **[!UICONTROL URL]**.
1. Escriba o pegue el ID de producto en el cuadro URL.
1. Seleccione **[!UICONTROL Aceptar]**. (Adobe Dynamic Media Classic completa la dirección URL con la plantilla URL del mapa de imagen).

   >[!NOTE]
   >
   >No es necesario establecer las opciones de apariencia en Adobe InDesign. Puede especificar el aspecto en Adobe Dynamic Media Classic.

1. Repita los pasos 2 a 6 para todos los mapas de imágenes que desee crear.
1. Exporte el archivo como PDF.
1. Cargue el PDF en Adobe Dynamic Media Classic.
1. En **[!UICONTROL Opciones de PDF]**, seleccione **[!UICONTROL Extraer vínculos]**.

### Para crear mapas de imagen en Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. En Adobe Acrobat, vaya a **[!UICONTROL Herramientas]** > **[!UICONTROL Edición avanzada]** > **[!UICONTROL Herramienta de vinculación]**.
1. Arrastre para crear el mapa de imagen.
1. En el cuadro Crear vínculo, seleccione **[!UICONTROL Vínculo personalizado]** y seleccione **[!UICONTROL Siguiente]**.

>[!NOTE]
>
>No es necesario establecer las opciones de apariencia en Adobe Acrobat. Puede especificar el aspecto en Adobe Dynamic Media Classic.

1. En el cuadro Propiedades del vínculo, seleccione **[!UICONTROL Acciones]**.
1. Seleccione **[!UICONTROL Abrir un vínculo web]** en el menú Seleccionar acción y, a continuación, seleccione **[!UICONTROL Agregar]**.
1. Escriba el id. de producto para el mapa de imagen en el cuadro Editar URL y seleccione **[!UICONTROL Aceptar]**. (Adobe Dynamic Media Classic completa la dirección URL con la plantilla URL del mapa de imagen).
1. Repita los pasos 1 a 7 para todos los mapas de imágenes que desee crear.
1. Guarde el archivo.
1. Cargue el PDF en Adobe Dynamic Media Classic y seleccione Extraer vínculos en las opciones del PDF.
