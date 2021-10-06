---
title: Creación de una plantilla
description: Obtenga información sobre cómo crear una plantilla en Adobe Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '3466'
ht-degree: 44%

---

# Creación de una plantilla {#creating-a-template}

Para crear una plantilla, vaya a **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Seleccione Diseñador o Desarrollador. En esta página puede añadir capas de imagen y de texto. También puede cambiar el orden de las capas, modificar el tamaño y la posición de éstas y aplicarles efectos de sombra y resplandor.

Consulte también el vídeo de capacitación [Conceptos básicos de plantilla](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

>[!NOTE]
>
>Si edita una plantilla creada en una versión anterior de Adobe Dynamic Media Classic, una solicitud le preguntará al guardar &quot;¿Desea añadir una capa de lienzo?&quot;. Seleccione **[!UICONTROL No]** para evitar añadir una capa base. Si selecciona **[!UICONTROL Yes]** accidentalmente, elimine los modificadores `&allowCanvasPrompt` y `&layer=0` en la dirección URL y pulse **[!UICONTROL Enter]** o **[!UICONTROL Return]**.

## Creación de la plantilla inicial {#creating-the-initial-template}

Al crear un conjunto de plantillas, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| **[!UICONTROL ¿Publicar después de]** guardar está seleccionada la opción antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

Puede crear una plantilla a partir de una existente. Abra la plantilla, seleccione **[!UICONTROL Guardar como]** e introduzca un nuevo nombre en el cuadro de diálogo Guardar como.

**Para crear la plantilla inicial:**

1. Para crear la plantilla inicial, utilice uno de los siguientes métodos:

   * **Seleccione el PSD o las imágenes primero** : en el panel Examinar, seleccione el archivo PSD o las imágenes que desee para la plantilla y vaya a  **[!UICONTROL Generar]**  > Conceptos básicos de  **[!UICONTROL plantilla]**.

   * **Comenzar desde la pantalla**  Plantilla: vaya a  **[!UICONTROL Generar]**  > Conceptos básicos  **[!UICONTROL de plantilla]**. Seleccione Diseñador o Desarrollador.

1. En el cuadro de diálogo Introducir tamaño de lienzo, introduzca los valores de anchura y altura de la plantilla.
1. Seleccione una carpeta en la biblioteca de recursos y arrastre el archivo PSD o las imágenes requeridas hasta la pantalla Plantilla.
1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccione **[!UICONTROL Guardar]**.
1. Seleccione una carpeta para almacenar la plantilla, introduzca un nombre para la plantilla y seleccione **[!UICONTROL Submit]**.

   Adobe Dynamic Media Classic reduce las imágenes si es necesario para ajustarlas al lienzo, el área de la pantalla Plantilla para definir la plantilla.

## Editar un conjunto de plantillas {#editing-a-template-set}

Tanto si edita un conjunto publicado como un conjunto de plantillas sin publicar, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL ¿Publicar después de]** guardar una opción seleccionada antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de plantillas:**

1. En la vista de cuadrícula, busque un conjunto de plantillas y, debajo de la imagen, seleccione **[!UICONTROL Editar]**.
1. Cambie la plantilla según sea necesario.
1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar una plantilla {#deleting-a-template}

Cuando se elimina un conjunto de plantillas, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar una plantilla:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione una o varias plantillas.
1. En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.

## Explicación de la pantalla Plantilla {#understanding-the-template-screen}

La pantalla Plantilla contiene herramientas de edición y parametrización de capas.

Utilice estas herramientas en la pantalla Plantilla para crear plantillas:

* **[!UICONTROL Panorámica]** : permite seleccionar capas, moverlas por el lienzo, cambiar su tamaño o girarlas.

* **[!UICONTROL Texto]** : crea una capa de texto. Arrastre el puntero sobre el lienzo para crear una capa de texto e introduzca el texto en la capa. Consulte [Creación de una capa de texto](#creating-a-text-layer).

* **[!UICONTROL Vista previa]** : abre la pantalla Vista previa y muestra la plantilla en un visor de zoom. La plantilla aparece tal y como la verán los usuarios que accedan al sitio web o utilicen la aplicación.

* **[!UICONTROL Resumen de]** parámetrosAbre la pantalla Resumen de parámetros. Puede ver el nombre de cada una de las capas de una plantilla y, en cada capa, los nombres de los parámetros que se han activado.

* **[!UICONTROL Editor de texto v4.3 y Editor de texto v4.2]** : puede elegir usar el editor de texto más reciente y con más funciones, Editor de texto v4.3, o el editor de texto anterior, Editor de texto v4.2. Al crear plantillas, el Editor de texto v4.3 está seleccionado de forma predeterminada. Al editar plantillas antiguas, se seleccionará por defecto el Editor de texto 4.2. El Editor de texto v4.3 no admite el ajuste de palabras, de modo que si desea editar plantillas antiguas que utilicen ajuste de palabras, deberá utilizar el Editor de texto v4.2 para mantener intacta la fidelidad de la plantilla. Si la plantilla anterior no utiliza ajuste de palabras, puede elegir Editor de texto v4.3 para aprovechar las muchas nuevas funciones que ofrece. Por ejemplo, Aumentar márgenes, Reducir márgenes, Establecer texto en mayúsculas y Copiar texto de ajuste.

   >[!NOTE]
   >
   >La eliminación del Editor de texto v4.2 está planificada como una opción en Adobe Dynamic Media Classic, por lo que se recomienda usar el Editor de texto 4.3 cuando sea posible. La opción **[!UICONTROL Ajuste de palabras]** se incorporará en una versión futura del Editor de texto.

* **[!UICONTROL Diseñador y desarrollador]** : seleccione la opción que mejor describe su función.

* **[!UICONTROL Lienzo]** : define el área total disponible, en píxeles, para definir la plantilla. El tamaño predeterminado es 300 x 300 píxeles. La capas se colocan en el lienzo.

* **[!UICONTROL Lista de capas]** : enumera el nombre de las capas de la plantilla. Para seleccionar una capa, seleccione su nombre en esta lista. La lista de capas ofrece herramientas para agregar efectos a capas, eliminar y parametrizar capas y modificar el orden de éstas. Consulte [Trabajo con capas](#working-with-layers).

* **[!UICONTROL Área Propiedades de capa]** : ofrece herramientas para cambiar el color de fondo, la opacidad, el tamaño y la posición de una capa, así como el color de fondo, la opacidad y el tamaño del lienzo. También es posible ajustar efectos de sombra y resplandor. Consulte [Trabajo con capas](#working-with-layers).

## Creación de capas de imagen {#creating-image-layers}

1. Arrastre la imagen desde la biblioteca de recursos al lienzo.

   El ID de la imagen aparece en la lista de capas.

   >[!NOTE]
   >
   >Si es necesario, Adobe Dynamic Media Classic reduce las imágenes para ajustarlas al lienzo al crear una capa de imagen.

## Creación de una capa de texto {#creating-a-text-layer}

1. Seleccione la herramienta **[!UICONTROL Texto]**.
1. Arrastre para crear un cuadro de texto en el lienzo o en una imagen.
1. En la pantalla Texto que aparece, agregue texto mediante uno de los siguientes procedimientos en la ficha Vista previa:

   * Escriba el texto en el cuadro de texto. Seleccione Copiar texto de ajuste para ajustar el texto al cuadro de texto.
   * Pegue el texto desde el portapapeles en el cuadro de texto. 

1. Seleccione **[!UICONTROL Aplicar]** y cierre la pantalla Texto.

### Formateo de texto {#format-text}

Para dar formato al texto de una capa de texto, haga lo siguiente:

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. En el cuadro de texto del Editor de texto, seleccione el texto al que desee dar formato. Puede seleccionar todo el texto, partes del texto o caracteres individuales.
1. Especifique cualquiera de las siguientes opciones de formato y, a continuación, seleccione **[!UICONTROL Aplicar]**.

   * **[!UICONTROL Fuente]** : elija una fuente en el menú Fuente. Si la fuente que desea no aparece en el menú, puede cargarla en Adobe Dynamic Media Classic. Consulte Fuentes.

   * **[!UICONTROL Tamaño de fuente]** : elija un tamaño de fuente en el menú, escriba un tamaño específico en el cuadro o seleccione las  **** flechas  **** inferiores para aumentar o reducir el tamaño en dos puntos.

   * **[!UICONTROL Color]** : seleccione para elegir un color para el texto.

   * **[!UICONTROL Negrita]**,  **[!UICONTROL cursiva]** o  **[!UICONTROL subrayado]** : seleccione el texto y, a continuación, seleccione el icono del tipo de formato que desee aplicar al texto.

   * **[!UICONTROL Todo en mayúsculas]**,  **[!UICONTROL Superíndice]** o  **[!UICONTROL Subíndice]** : seleccione el texto y, a continuación, seleccione el icono del tipo de formato que desee aplicar al texto.

   * **[!UICONTROL Alineación]** : elija un botón Alineación para alinear a la izquierda, al centro o a la derecha en la capa de texto.

   * **[!UICONTROL Seguimiento]** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre palabras.

   * **[!UICONTROL Interletraje]** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre caracteres.

   * **[!UICONTROL Interlineado]** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre líneas.

   * **[!UICONTROL Desplazamiento vertical]** : escriba o seleccione un valor numérico para mover un carácter seleccionado hacia arriba o hacia abajo en relación con la línea base del texto que lo rodea. Esta opción resulta especialmente útil al definir fracciones manualmente o al ajustar la posición de gráficos integrados.

>[!NOTE]
>
>Seleccione **[!UICONTROL Deshacer]** si desea revertir la última acción. Seleccione **[!UICONTROL Rehacer]** si cambia de opinión acerca de revertir una acción después de seleccionar **[!UICONTROL Deshacer]**.

### Formateo de párrafos {#format-paragraphs}

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. Seleccione el párrafo al que desea dar formato.
1. Especifique cualquiera de las siguientes opciones de formato y, a continuación, seleccione **[!UICONTROL Aplicar]**.

   * **[!UICONTROL Alineación]** : seleccione para especificar el tipo de alineación: alinee a la izquierda, alinee el centro, alinee a la derecha o justifique.

   * **[!UICONTROL Justificación del final del párrafo]** : seleccione esta opción para especificar el tipo de justificación de la última línea del párrafo: la última línea se alinea a la izquierda; la última línea alinea el centro; y la última línea se alinea a la derecha.

   * **[!UICONTROL Interlineado]** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre todas las líneas del párrafo.

   * **[!UICONTROL Sangrar todo]** : seleccione esta opción para aumentar la sangría del texto.

   * **[!UICONTROL Quitar sangría]** : seleccione esta opción para reducir la sangría del texto.

   * **[!UICONTROL Sangría en primera línea]** : especifique la cantidad en la que desea sangrar la primera línea de texto.

   * **[!UICONTROL Espacio antes del párrafo]** : especifique el espacio que desea que aparezca encima de la primera línea de texto del párrafo.

   * **[!UICONTROL Espacio después del párrafo]** : especifique el espacio que desea que aparezca debajo de la última línea de texto del párrafo.

   * **[!UICONTROL Alineación vertical]** : seleccione dónde desea que aparezca el texto verticalmente dentro del cuadro de texto: Arriba, Centro, Abajo.

   * **[!UICONTROL Dirección del texto]** : seleccione la dirección en la que desea que se muestre el texto: De derecha a izquierda o de izquierda a derecha.

### Ajuste de propiedades de capas de texto {#adjust-text-layer-properties}

1. En la pantalla Funciones básicas de plantilla, seleccione el cuadro de texto que desea ajustar.
1. En el panel Propiedades de la capa, seleccione cualquiera de los siguientes:

   * **[!UICONTROL Reducir texto (solo Editor de texto v4.2)]** : para ajustar dentro del cuadro de texto, seleccione reducir el texto.

   * **[!UICONTROL Ajuste de texto (solo Editor de texto v4.2)]** : para especificar si el texto se ajusta o cómo se ajusta, seleccione una opción de ajuste:

   * **[!UICONTROL Ajustar]** : ajusta el texto para que quepa en un cuadro de texto que sea demasiado pequeño horizontalmente.

   * **[!UICONTROL Sin ajuste]** : no ajusta el texto cuando el cuadro de texto es demasiado pequeño horizontalmente y, en su lugar, corta una parte del texto.

   * **[!UICONTROL Ajuste de no separación]** : ajusta el texto para que quepa en un cuadro de texto y no rompe las palabras.

   * **[!UICONTROL Posición]** : especifica la ubicación del cuadro de texto en el lienzo.

   * **[!UICONTROL Relleno]** : Añade márgenes o recorta el rectángulo de la capa. Especifique el número de píxeles que desea agregar o quitar para Izquierda, Arriba, Abajo y Derecha. Introduzca números positivos si desea agregar un margen o números negativos para recortar.

### Visualización y edición de texto del código fuente {#view-and-edit-text-source-code}

La información que se proporciona en la ficha Origen del Editor de texto es para su referencia. Modifique el texto únicamente si está familiarizado con la edición de código fuente.

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. En el Editor de texto, para mostrar el código fuente del texto, seleccione la pestaña **[!UICONTROL Source]** en el Editor de texto.
1. Vea o edite el texto según lo necesite.

   Los cambios se mantienen intactos al alternar entre la vista previa y la vista de código fuente.

1. Seleccione **[!UICONTROL Aplicar]** para procesar las ediciones.

## Trabajo con capas {#working-with-layers}

Use la lista de capas y el área Propiedades de la capa para trabajar con capas. Puede reordenar las capas, modificar su tamaño y posición, girarlas y determinar el color de fondo, color de primer plano, opacidad y modo de mezcla de una capa.

También es posible modificar el tamaño del lienzo y especificar su color de fondo y opacidad.

### Reordenar capas {#reordering-layers}

Cambiar el orden de las capas puede afectar al aspecto, especialmente cuando se trata de transparencia o sobreimpresión. Asegúrese de comprobar el resultado mediante una vista previa antes de confirmar los cambios.

1. Use una de estas técnicas para cambiar el orden de las capas de una plantilla:

   * Seleccione una capa en la lista de capas. A continuación, seleccione **[!UICONTROL Up]** o **[!UICONTROL Down]** tantas veces como sea necesario para colocarlo en la posición correcta de la lista.
   * Arrastre una capa a una posición superior o inferior en la lista.

### Cambiar el tamaño y la posición de las capas y el lienzo {#changing-the-size-and-position-of-layers-and-the-canvas}

El tamaño de las capas no debe superar las restricciones del lienzo. Puede modificar el tamaño de una capa o el del lienzo manualmente o introduciendo las medidas requeridas. Puede modificar la posición de una capa manualmente o introduciendo los valores de desfase requeridos. También puede rotar una capa.

>[!NOTE]
>
>Adobe Dynamic Media Classic recomienda crear un ajuste preestablecido de imagen que sea del tamaño exacto de la plantilla. De este modo se asegura una definición correcta de las opciones de enfoque y el tamaño de salida final de la plantilla. Después de crear este ajuste de imagen preestablecido, está disponible en el menú Ajustes preestablecidos, en la pantalla Vista previa de plantilla. La pantalla muestra el aspecto que tendrá la imagen procedente del servidor. Consulte [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

* **Cambio del tamaño de una capa** : para cambiar el tamaño de una capa o del lienzo, seleccione la capa o el lienzo en la lista Capas y utilice una de estas técnicas:

* **Cambio manual de tamaño** : seleccione y arrastre una esquina de la capa o del lienzo. Con las capas de texto, también puede arrastrar un lado de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño pero manteniendo la proporción de aspecto (la forma).

* **Introducción de medidas de tamaño de capa** : introduzca medidas de píxeles en los cuadros de texto W (ancho) y H (alto) del área Propiedades de capa.

Además de cambiar el tamaño, también es posible añadir un margen a la capa. Para ello, introduzca un valor de margen en los cuadros Izquierda, Derecha, Superior e Inferior del área Propiedades de la capa. Se insertará un margen entre la capa actual y el perímetro de la capa base. El margen es útil para hacer más visibles efectos de sombra paralela o resplandor exterior añadidos. El margen incrementa el tamaño de una capa y muestra su color de fondo en el área extendida. La posición de la capa base se ajusta con relación al nuevo tamaño de la capa. Por ejemplo, si la capa actual está centrada en la capa base, al extenderse el lado izquierdo de la capa ésta se desplaza hacia la derecha de la capa base.

* **Cambio de la posición de una capa** : para cambiar la posición de una capa en el lienzo, seleccione su nombre en la lista Capas y utilice una de estas técnicas:

* **Cambio manual de posición** : mueva el puntero cerca de un límite de capa pero no sobre él y, cuando vea el cursor de flecha de cuatro puntas, seleccione y comience a arrastrar.

* **Introducción de medidas de desvío de posición** : introduzca las medidas de desvío X e Y en los cuadros de texto X e Y. Esto valores representan el desfase x, y del punto de anclaje, medido en píxeles.

* **Rotación de una capa** : el cuadro Rotar muestra el ángulo al que giró la capa. Para rotar una capa, seleccione el nombre de ésta en la lista de capas y use una de estas técnicas:

* **Giro manual** : mueva el cursor cerca de una esquina de la capa, pero no sobre ella. Cuando aparezca el cursor de rotación, arrastre la esquina de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para rotar en incrementos de 15 grados.

* **Introducción de una medición de grado** : introduzca el número de grados para rotar la capa. Se aplica una rotación hacia la derecha; para rotar la capa hacia la izquierda, debe introducir un valor negativo.

**Ocultar una capa o un efecto de capa:**

Puede ocultar una capa o un efecto de capa seleccionando el icono de ojo junto al nombre de una capa o del efecto. Las capas ocultas no aparecen en las vistas previas o en el resultado final. La información de la capa no se elimina de la URL. En su lugar, se agrega `hide=1` a la dirección URL para tener en cuenta que la capa está oculta a la vista. Por ejemplo:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Determinar el color de fondo, la opacidad y el modo de mezcla {#determining-the-background-color-opacity-and-blend-mode}

Para definir el color de fondo, la opacidad y el modo de fusión de una capa o del lienzo, seleccione la capa o el lienzo y use una de esta técnicas:

* **Color frontal** : seleccione  **[!UICONTROL Color frontal y]** elija una muestra de color para cambiar el color de la sombra o el resplandor. También puede introducir un valor de color en el cuadro. El color de fondo solo se aplica a las capas con transparencia. Se puede utilizar, por ejemplo, en una capa con transparencia parcial de una etiqueta de precio o en el fondo de un campo de texto. Las capas que consisten en una imagen PSD, TIFF o PNG con transparencia activada pueden tener fondos transparentes.

* **Color de fondo** : seleccione  **[!UICONTROL Color de]** fondo y elija una muestra de color para cambiar el color de las áreas acolchadas.

* **Opacidad** : arrastre el control deslizante de Opacidad para que cualquier capa sea translúcida de modo que parte de la imagen subyacente se muestre. La configuración del 100% es opaca; 0 es transparente.

* **Modo de fusión** : para simular uno de los modos de mezcla disponibles en Photoshop, elija una opción. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla. Estas opciones están disponibles para capas únicamente, no son aplicables a lienzos.

## Utilizar efectos de sombra y resplandor en capas {#using-shadow-and-glow-effects-on-layers}

Puede aplicar una sombra o un resplandor a una capa. La sombra o el resplandor se aplican al perímetro de la capa y se extienden hacia dentro o hacia fuera, según la opción elegida. Si la plantilla se originó con un archivo PSD con efectos de sombra y resplandor, puede ajustar estos efectos en Adobe Dynamic Media Classic.

Después de aplicar un efecto de sombra o resplandor, puede ajustar su tamaño, color, opacidad y posición en el área Propiedades de la capa, en la pantalla Plantilla.

### Aplicar un efecto de sombra o resplandor a una capa {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Seleccione una capa en la lista de capas.
1. Seleccione el menú Agregar efecto y elija una opción:

   * **[!UICONTROL Sombra paralela]** : aplica una sombra a los lados inferior y derecho de la capa.

   * **[!UICONTROL Sombra interna]** : aplica un efecto de sombra dentro de todos los bordes de la capa.

   * **[!UICONTROL Resplandor exterior]** : aplica un efecto de resplandor alrededor de todos los bordes de la capa.

   * **[!UICONTROL Resplandor interior]** : aplica un efecto de resplandor dentro de todos los bordes de la capa.

Después de aplicar un efecto, el nombre del mismo aparece en la lista de capas. Para eliminar un efecto, seleccione su nombre en la lista Capas y, a continuación, seleccione **[!UICONTROL Eliminar]**.

>[!NOTE]
>
>A veces no se puede ver el efecto de una sombra paralela o un resplandor exterior si la capa subyacente no es lo suficientemente grande para mostrarla. Si no puede ver la sombra o el resplandor, considere añadir valores de relleno a la capa o reordenar la capa. Consulte [Cambio del tamaño y la posición de las capas y el lienzo](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) y [Reordenación de las capas](creating-template.md#reordering_layers).

### Ajustar un efecto de sombra o resplandor {#adjusting-a-shadow-or-glow-effect}

Para ajustar un efecto de sombra o resplandor, seleccione el nombre correspondiente en la lista de capas. Cambie los valores que tiene asignados en el área Propiedades de la capa:

* **[!UICONTROL Color]** : seleccione el botón Color y elija una muestra de color para cambiar el color de la sombra o el resplandor. También puede introducir un valor de color en el cuadro.

* **[!UICONTROL Opacidad]** : arrastre el control deslizante para determinar la intensidad del efecto. Cuanto menor sea el valor de opacidad, mayor será la transparencia del efecto.

* **[!UICONTROL Modo de fusión]** : para simular uno de los modos de mezcla disponibles en Photoshop, elija una opción. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla.

* **[!UICONTROL Tamaño]** : introduzca las medidas en el cuadro X e Y para ampliar o reducir el efecto de sombra. Las opciones de tamaño son aplicables a sombras interiores y paralelas.

* **[!UICONTROL Crecer]** : arrastre el control deslizante para ampliar el efecto hacia dentro o hacia fuera.

* **[!UICONTROL Desenfoque]** : arrastre el control deslizante para controlar el desvanecimiento en los bordes del efecto. Cuanto mayor sea el desenfoque, mayor será el calado.

## Máscara de capas {#masking-layers}

El botón Máscara, disponible en la lista de capas, permite especificar el uso de la máscara o el canal alfa de una capa. Con este botón puede aplicar el efecto de una capa de fondo a una capa concreta, o a toda la capa principal de la plantilla. Seleccione una capa en la lista Capas y seleccione **[!UICONTROL Máscara]** para recorrer estos estados:

* El fondo de la capa es opaco.
* El contenido de la capa se invierte y el fondo de ésta se rellena de negro sólido.
* El fondo de la capa se rellena de negro sólido.
