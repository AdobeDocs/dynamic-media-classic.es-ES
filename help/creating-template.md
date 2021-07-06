---
title: Crear una plantilla
description: Obtenga información sobre cómo crear una plantilla en Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '3382'
ht-degree: 52%

---

# Crear una plantilla {#creating-a-template}

Para crear una plantilla, haga clic en **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de la plantilla]**. Seleccione Diseñador o Desarrollador. En esta página puede añadir capas de imagen y de texto. También puede cambiar el orden de las capas, modificar el tamaño y la posición de éstas y aplicarles efectos de sombra y resplandor.

>[!NOTE]
>
>Si edita una plantilla creada en una versión anterior de Dynamic Media Classic, una solicitud le preguntará al guardar &quot;¿Desea añadir una capa de lienzo?&quot; Haga clic en **[!UICONTROL No]** para evitar agregar una capa base. Si accidentalmente hace clic en **[!UICONTROL Yes]**, elimine los modificadores `&allowCanvasPrompt` y `&layer=0` en la dirección URL y pulse **[!UICONTROL Enter]** o **[!UICONTROL Return]**.

## Creación de la plantilla inicial {#creating-the-initial-template}

Al crear un conjunto de plantillas, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| **[!UICONTROL ¿Publicar después de]** guardar está seleccionada la opción antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

Puede crear una plantilla a partir de una existente. Abra la plantilla, haga clic en **[!UICONTROL Guardar como]** y escriba otro nombre en el cuadro de diálogo Guardar como.

**Para crear el conjunto de plantillas inicial:**

1. Para crear la plantilla inicial, utilice uno de los siguientes métodos:

   * **Seleccione primero**  el PSD o las imágenes: en el panel Examinar, seleccione el archivo PSD o las imágenes que desee para la plantilla y haga clic en  **[!UICONTROL Generar]**  > Conceptos básicos de  **[!UICONTROL plantilla]**.

   * **Comenzar desde la pantalla**  Plantilla: haga clic en  **[!UICONTROL Generar]**  > Conceptos básicos  **[!UICONTROL de plantilla]**. Seleccione Diseñador o Desarrollador.

1. En el cuadro de diálogo Introducir tamaño de lienzo, introduzca los valores de anchura y altura de la plantilla.
1. Seleccione una carpeta en la biblioteca de recursos y arrastre el archivo PSD o las imágenes requeridas hasta la pantalla Plantilla.
1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **[!UICONTROL Guardar]**.
1. Seleccione una carpeta para guardar la plantilla, asigne un nombre a la plantilla y seleccione el botón **[!UICONTROL Enviar]**.

   Dynamic Media Classic reduce las imágenes si es necesario para ajustarlas al lienzo, el área de la pantalla Plantilla para definir la plantilla.

## Edición de un conjunto de plantillas {#editing-a-template-set}

Tanto si edita un conjunto publicado como un conjunto de plantillas sin publicar, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL ¿Publicar después de]** guardar una opción seleccionada antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de plantillas:**

1. En la vista de cuadrícula, vaya a un conjunto de plantillas y, a continuación, debajo de la imagen, haga clic en **[!UICONTROL Editar]**.
1. Cambie la plantilla según sea necesario.
1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, especifique un nombre para el conjunto y haga clic en **[!UICONTROL Guardar]**.

## Eliminación de una plantilla {#deleting-a-template}

Cuando se elimina un conjunto de plantillas, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar una plantilla:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione una o varias plantillas.
1. En la barra de navegación global, haga clic en **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.

## Explicación de la pantalla Plantilla {#understanding-the-template-screen}

La pantalla Plantilla contiene herramientas de edición y parametrización de capas.

Use estas herramientas en la pantalla Plantilla para crear plantillas:

* **Herramienta Panorámica** : permite seleccionar capas, moverlas por el lienzo, cambiar su tamaño o girarlas.

* **Herramienta Texto** : crea una capa de texto. Arrastre el puntero sobre el lienzo para crear una capa de texto e introduzca el texto en la capa. Consulte [Creación de una capa de texto](#creating-a-text-layer).

* **Botón Vista previa** : abre la pantalla Vista previa y muestra la plantilla en un visor de zoom. La plantilla aparece tal y como la verán los usuarios que accedan al sitio web o utilicen la aplicación.

* **Botón Resumen de** parámetrosAbre la pantalla Resumen de parámetros. Puede ver el nombre de cada una de las capas de una plantilla y, en cada capa, los nombres de los parámetros que se han activado.

* **Editor de texto v4.3 y Editor de texto v4.2** : puede elegir usar el editor de texto más reciente y con más funciones, Editor de texto v4.3, o el editor de texto anterior, Editor de texto v4.2. Al crear plantillas, el Editor de texto v4.3 está seleccionado de forma predeterminada. Al editar plantillas antiguas, se seleccionará por defecto el Editor de texto 4.2. El Editor de texto v4.3 no admite el ajuste de palabras, de modo que si desea editar plantillas antiguas que utilicen ajuste de palabras, deberá utilizar el Editor de texto v4.2 para mantener intacta la fidelidad de la plantilla. Si la plantilla anterior no utiliza ajuste de palabras, puede elegir Editor de texto v4.3 para aprovechar las muchas nuevas funciones que ofrece. Por ejemplo, Aumentar márgenes, Reducir márgenes, Establecer texto en mayúsculas y Copiar texto de ajuste.

   >[!NOTE]
   >
   >El Editor de texto v4.2 finalmente se eliminará como opción en Dynamic Media Classic, por lo que se recomienda usar el Editor de texto 4.3 cuando sea posible. La opción de ajuste de palabras se incluirá en una versión posterior del Editor de texto.

* **Diseñador y desarrollador** : seleccione la opción que mejor describe su función.

* **Lienzo** : define el área total disponible, en píxeles, para definir la plantilla. El tamaño predeterminado es 300 x 300 píxeles. La capas se colocan en el lienzo.

* **Lista de capas** : enumera el nombre de las capas de la plantilla. Para seleccionar una capa, seleccione su nombre en esta lista. La lista de capas ofrece herramientas para agregar efectos a capas, eliminar y parametrizar capas y modificar el orden de éstas. Consulte [Uso de capas](#working-with-layers).

* **Área Propiedades de capa** : ofrece herramientas para cambiar el color de fondo, la opacidad, el tamaño y la posición de una capa, así como el color de fondo, la opacidad y el tamaño del lienzo. También es posible ajustar efectos de sombra y resplandor. Consulte [Uso de capas](#working-with-layers).

## Creación de capas de imagen {#creating-image-layers}

1. Arrastre la imagen desde la biblioteca de recursos al lienzo.

   El ID de la imagen aparece en la lista de capas.

   >[!NOTE]
   >
   >Si es necesario, Dynamic Media Classic reduce las imágenes para ajustarlas al lienzo al crear una capa de imagen.

## Creación de una capa de texto {#creating-a-text-layer}

1. Haga clic en la herramienta **[!UICONTROL Texto]**.
1. Arrastre para crear un cuadro de texto en el lienzo o en una imagen.
1. En la pantalla Texto que aparece, agregue texto mediante uno de los siguientes procedimientos en la ficha Vista previa:

   * Escriba el texto en el cuadro de texto. Seleccione Copiar texto de ajuste para ajustar el texto al cuadro de texto.
   * Pegue el texto desde el portapapeles en el cuadro de texto. 

1. Haga clic en **[!UICONTROL Aplicar]** y cierre la pantalla Texto.

### Formateo de texto {#format-text}

Para dar formato al texto de una capa de texto, haga lo siguiente:

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. En el cuadro de texto, seleccione el texto al que desea dar formato. Puede seleccionar todo el texto, partes del texto o caracteres individuales.
1. Especifique cualquiera de estas opciones de formato y haga clic en **[!UICONTROL Aplicar]**.

   * **Fuente** : elija una fuente en el menú Fuente. Si la fuente que desea no aparece en el menú, puede cargarla en Dynamic Media Classic. Consulte Fuentes.

   * **Tamaño de fuente** : elija un tamaño de fuente en el menú, escriba un tamaño específico en el cuadro o haga clic en las  **** flechas  **** inferiores para aumentar o reducir el tamaño en dos puntos.

   * **Color** : haga clic para elegir un color para el texto.

   * **Negrita, cursiva o subrayado** : seleccione el texto y, a continuación, haga clic en el icono del tipo de formato que desee aplicar al texto.

   * **Todo en mayúsculas, superíndice o subíndice** : seleccione el texto y, a continuación, haga clic en el icono del tipo de formato que desee aplicar al texto.

   * **Alineación** : elija un botón Alineación para alinear a la izquierda, al centro o a la derecha en la capa de texto.

   * **Seguimiento** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre palabras.

   * **Interletraje** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre caracteres.

   * **Interlineado** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre líneas.

   * **Desplazamiento vertical** : escriba o seleccione un valor numérico para mover un carácter seleccionado hacia arriba o hacia abajo en relación con la línea base del texto que lo rodea. Esta opción resulta especialmente útil al definir fracciones manualmente o al ajustar la posición de gráficos integrados.

>[!NOTE]
>
>Haga clic en **[!UICONTROL Deshacer]** para invertir la última acción. Haga clic en **[!UICONTROL Rehacer]** si cambia de opinión acerca de revertir una acción después de hacer clic en **[!UICONTROL Deshacer]**.

### Formateo de párrafos {#format-paragraphs}

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. Seleccione el párrafo al que desea dar formato.
1. Especifique cualquiera de estas opciones de formato y haga clic en **[!UICONTROL Aplicar]**.

   * **Alineación** : haga clic en para especificar el tipo de alineación: alinee a la izquierda, alinee el centro, alinee a la derecha o justifique.

   * **Justificación del final del párrafo** : haga clic en para especificar el tipo de justificación de la última línea del párrafo: la última línea se alinea a la izquierda; la última línea alinea el centro; y la última línea se alinea a la derecha.

   * **Interlineado** : escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre todas las líneas del párrafo.

   * **Aplicar sangría a todo** : haga clic en para aumentar la sangría del texto.

   * **Quitar sangría** : haga clic en para reducir la sangría del texto.

   * **Sangría en primera línea** : especifique la cantidad en la que desea sangrar la primera línea de texto.

   * **Espacio antes del párrafo** : especifique el espacio que desea que aparezca encima de la primera línea de texto del párrafo.

   * **Espacio después del párrafo** : especifique el espacio que desea que aparezca debajo de la última línea de texto del párrafo.

   * **Alineación vertical** : seleccione dónde desea que aparezca el texto verticalmente dentro del cuadro de texto: Arriba, Centro, Abajo.

   * **Dirección del texto** : seleccione la dirección en la que desea que se muestre el texto: De derecha a izquierda o de izquierda a derecha.

### Ajuste de propiedades de capas de texto {#adjust-text-layer-properties}

1. En la pantalla Funciones básicas de plantilla, seleccione el cuadro de texto que desea ajustar.
1. En el panel Propiedades de la capa, seleccione cualquiera de los siguientes:

   * **Reducir texto (solo Editor de texto v4.2)** : para ajustar dentro del cuadro de texto, seleccione reducir el texto.

   * **Ajuste de texto (solo Editor de texto v4.2)** : para especificar si el texto se ajusta o cómo se ajusta, seleccione una opción de ajuste:

   * **Ajustar** : ajusta el texto para que quepa en un cuadro de texto que sea demasiado pequeño horizontalmente.

   * **Sin ajuste** : no ajusta el texto cuando el cuadro de texto es demasiado pequeño horizontalmente y, en su lugar, corta una parte del texto.

   * **Ajuste NB** : (ajuste de no separación) ajusta el texto para que quepa en un cuadro de texto y no rompe las palabras.

   * **Posición** : especifica la ubicación del cuadro de texto en el lienzo.

   * **Relleno** : Añade márgenes o recorta el rectángulo de la capa. Especifique el número de píxeles que agregar o eliminar de izquierda, arriba, abajo, y derecha. Introduzca números positivos para añadir un margen o números negativos a recortar.

### Visualización y edición de texto del código fuente {#view-and-edit-text-source-code}

La información que se proporciona en la ficha Origen del Editor de texto es para su referencia. Modifique el texto únicamente si está familiarizado con la edición de código fuente.

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. Para mostrar el código fuente del texto, haga clic en la pestaña **[!UICONTROL Source]** en el Editor de texto.
1. Vea o edite el texto según lo necesite.

   Los cambios se mantienen intactos al alternar entre la vista previa y la vista de código fuente.

1. Haga clic en **[!UICONTROL Aplicar]** para procesar las ediciones.

## Uso de capas {#working-with-layers}

Use la lista de capas y el área Propiedades de la capa para trabajar con capas. Puede reordenar las capas, modificar su tamaño y posición, girarlas y determinar el color de fondo, color de primer plano, opacidad y modo de mezcla de una capa.

También es posible modificar el tamaño del lienzo y especificar su color de fondo y opacidad.

### Reordenación de las capas {#reordering-layers}

Cambiar el orden de las capas puede afectar al aspecto, especialmente cuando se trata de transparencia o sobreimpresión. Asegúrese de comprobar el resultado mediante una vista previa antes de confirmar los cambios.

1. Use una de estas técnicas para cambiar el orden de las capas de una plantilla:

   * Seleccione una capa en la lista de capas. A continuación, haga clic **[!UICONTROL Up]** o **[!UICONTROL Down]** tantas veces como sea necesario para colocarlo en la posición correcta de la lista.
   * Arrastre una capa a una posición superior o inferior en la lista.

### Cambio del tamaño y la posición de las capas y el lienzo {#changing-the-size-and-position-of-layers-and-the-canvas}

El tamaño de las capas no debe superar las restricciones del lienzo. Puede modificar el tamaño de una capa o el del lienzo manualmente o introduciendo las medidas requeridas. Puede modificar la posición de una capa manualmente o introduciendo los valores de desfase requeridos. También puede rotar una capa.

>[!NOTE]
>
>Dynamic Media Classic recomienda crear un ajuste preestablecido de imagen que sea del tamaño exacto de la plantilla. De este modo se asegura una definición correcta de las opciones de enfoque y el tamaño de salida final de la plantilla. Después de crear este ajuste de imagen preestablecido, está disponible en el menú Ajustes preestablecidos, en la pantalla Vista previa de plantilla. La pantalla muestra el aspecto que tendrá la imagen procedente del servidor. Consulte [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

* **Cambio del tamaño de una capa** : para cambiar el tamaño de una capa o del lienzo, seleccione la capa o el lienzo en la lista Capas y utilice una de estas técnicas:

* **Cambio manual de tamaño** : seleccione y arrastre una esquina de la capa o del lienzo. Con las capas de texto, también puede arrastrar un lado de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño pero manteniendo la proporción de aspecto (la forma).

* **Introducción de medidas de tamaño de capa** : introduzca medidas de píxeles en los cuadros de texto W (ancho) y H (alto) del área Propiedades de capa.

Además de cambiar el tamaño, también es posible añadir un margen a la capa. Para ello, introduzca un valor de margen en los cuadros Izquierda, Derecha, Superior e Inferior del área Propiedades de la capa. Se insertará un margen entre la capa actual y el perímetro de la capa base. El margen es útil para hacer más visibles efectos de sombra paralela o resplandor exterior añadidos. El margen incrementa el tamaño de una capa y muestra su color de fondo en el área extendida. La posición de la capa base se ajusta con relación al nuevo tamaño de la capa. Por ejemplo, si la capa actual está centrada en la capa base, al extenderse el lado izquierdo de la capa ésta se desplaza hacia la derecha de la capa base.

* **Cambio de la posición de una capa** : para cambiar la posición de una capa en el lienzo, seleccione su nombre en la lista Capas y utilice una de estas técnicas:

* **Cambio manual de posición** : mueva el puntero cerca de un límite de capa pero no sobre él y, cuando vea el cursor de flecha de cuatro puntas, haga clic en y comience a arrastrar.

* **Introducción de medidas de desvío de posición** : introduzca las medidas de desvío X e Y en los cuadros de texto X e Y. Esto valores representan el desfase x, y del punto de anclaje, medido en píxeles.

* **Rotación de una capa** : el cuadro Rotar muestra el ángulo al que giró la capa. Para rotar una capa, seleccione el nombre de ésta en la lista de capas y use una de estas técnicas:

* **Giro manual** : mueva el cursor cerca de una esquina de la capa, pero no sobre ella. Cuando aparezca el cursor de rotación, arrastre la esquina de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para rotar en incrementos de 15 grados.

* **Introducción de una medición de grado** : introduzca el número de grados para rotar la capa. Se aplica una rotación hacia la derecha; para rotar la capa hacia la izquierda, debe introducir un valor negativo.

**Ocultación de una capa o un efecto de capa:**

Puede ocultar una capa o efecto de capa haciendo clic en el icono del ojo  junto al nombre de la capa o del efecto. Las capas ocultas no aparecen en las vistas previas o en el resultado final. La información de la capa no se elimina de la URL. En su lugar, se agrega `hide=1` a la dirección URL para tener en cuenta que la capa está oculta a la vista. Por ejemplo:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Configuración del color de fondo, la opacidad y el modo de fusión {#determining-the-background-color-opacity-and-blend-mode}

Para definir el color de fondo, la opacidad y el modo de fusión de una capa o del lienzo, seleccione la capa o el lienzo y use una de esta técnicas:

* **Color de primer plano** : haga clic en  **[!UICONTROL Color de]** primer plano y elija una muestra de color para cambiar el color de la sombra o el resplandor. También puede introducir un valor de color en el cuadro. El color de fondo solo se aplica a las capas con transparencia. Se puede utilizar, por ejemplo, en una capa con transparencia parcial de una etiqueta de precio o en el fondo de un campo de texto. Las capas que consisten en una imagen PSD, TIFF o PNG con transparencia activada pueden tener fondos transparentes.

* **Color de fondo** : haga clic en  **[!UICONTROL Color de]** fondo y elija una muestra de color para cambiar el color de las áreas acolchadas.

* **Opacidad** : arrastre el control deslizante de Opacidad para que cualquier capa sea translúcida de modo que parte de la imagen subyacente se muestre. La configuración del 100% es opaca; 0 es transparente.

* **Modo de fusión** : para simular uno de los modos de mezcla disponibles en Photoshop, elija una opción. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla. Estas opciones están disponibles para capas únicamente, no son aplicables a lienzos.

## Utilización de efectos de sombra y resplandor en las capas {#using-shadow-and-glow-effects-on-layers}

Puede aplicar una sombra o un resplandor a una capa. La sombra o el resplandor se aplican al perímetro de la capa y se extienden hacia dentro o hacia fuera, según la opción elegida. Si la plantilla se originó con un archivo PSD con efectos de sombra y resplandor, puede ajustar estos efectos en Dynamic Media Classic.

Después de aplicar un efecto de sombra o resplandor, puede ajustar su tamaño, color, opacidad y posición en el área Propiedades de la capa, en la pantalla Plantilla.

### Aplicación de un efecto de sombra o resplandor a una capa {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Seleccione una capa en la lista de capas.
1. Seleccione el menú Agregar efecto y elija una opción:

   * **Sombra paralela** : aplica una sombra a los lados inferior y derecho de la capa.

   * **Sombra interna** : aplica un efecto de sombra dentro de todos los bordes de la capa.

   * **Resplandor exterior** : aplica un efecto de resplandor alrededor de todos los bordes de la capa.

   * **Resplandor interior** : aplica un efecto de resplandor dentro de todos los bordes de la capa.

Después de aplicar un efecto, el nombre del mismo aparece en la lista de capas. Para eliminar un efecto, seleccione su nombre en la lista Capas y haga clic en **[!UICONTROL Eliminar]**.

>[!NOTE]
>
>A veces no se puede ver el efecto de una sombra paralela o un resplandor exterior si la capa subyacente no es lo suficientemente grande para mostrarla. Si no puede ver la sombra o el resplandor, considere añadir valores de relleno a la capa o reordenar la capa. Consulte [Cambio del tamaño y la posición de las capas y el lienzo](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) y [Reordenación de las capas](creating-template.md#reordering_layers).

### Ajuste de un efecto de sombra o resplandor {#adjusting-a-shadow-or-glow-effect}

Para ajustar un efecto de sombra o resplandor, seleccione el nombre correspondiente en la lista de capas. Cambie los valores que tiene asignados en el área Propiedades de la capa:

* **Color** : seleccione el botón Color y elija una muestra de color para cambiar el color de la sombra o el resplandor. También puede introducir un valor de color en el cuadro.

* **Opacidad** : arrastre el control deslizante para determinar la intensidad del efecto. Cuanto menor sea el valor de opacidad, mayor será la transparencia del efecto.

* **Modo de fusión** : para simular uno de los modos de mezcla disponibles en Photoshop, elija una opción. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla.

* **Tamaño** : introduzca las medidas en el cuadro X e Y para ampliar o reducir el efecto de sombra. Las opciones de tamaño son aplicables a sombras interiores y paralelas.

* **Crecer** : arrastre el control deslizante para ampliar el efecto hacia dentro o hacia fuera.

* **Desenfoque** : arrastre el control deslizante para controlar el desvanecimiento en los bordes del efecto. Cuanto mayor sea el desenfoque, mayor será el calado.

## Creación de máscaras en capas {#masking-layers}

El botón Máscara, disponible en la lista de capas, permite especificar el uso de la máscara o el canal alfa de una capa. Con este botón puede aplicar el efecto de una capa de fondo a una capa concreta, o a toda la capa principal de la plantilla. Seleccione una capa en la lista Capas y haga clic en **[!UICONTROL Máscara]** para recorrer estos estados:

* El fondo de la capa es opaco.
* El contenido de la capa se invierte y el fondo de ésta se rellena de negro sólido.
* El fondo de la capa se rellena de negro sólido.
