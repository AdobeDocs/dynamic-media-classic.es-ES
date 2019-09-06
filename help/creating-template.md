---
title: Creación de una plantilla
seo-title: Creación de una plantilla
description: nulo
seo-description: Aprenda a crear una plantilla en Dynamic Media Classic.
uuid: c 762224 b -7 c 6 c -4434-bada-c 26570079645
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template_ basics
discoiquuid: 8 f 7093 da-d 215-4337-ac 95-69 f 0 a 5 bf 8648
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Creación de una plantilla {#creating-a-template}

Para crear una plantilla, haga clic en Generar &gt; Funciones básicas de plantilla. Seleccione Diseñador o Desarrollador. En esta página puede añadir capas de imagen y de texto. También puede cambiar el orden de las capas, modificar el tamaño y la posición de éstas y aplicarles efectos de sombra y resplandor.

>[!NOTE]
>
>Si edita una plantilla creada en una versión anterior de Scene7 Publishing System, al guardar puede recibir un mensaje con la pregunta: "¿Desea añadir una capa de lienzo?". Seleccione No para evitar agregar una nueva capa base. Si por error selecciona Sí, elimine los modificadores "&amp; allowCanvasPrompt" y "&amp; layer=0" de la URL y pulse Intro o Retorno.

## Creación de la plantilla inicial {#creating-the-initial-template}

Al crear un conjunto de plantillas, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

Puede crear una plantilla a partir de una existente. Abra la plantilla, haga clic en **Guardar como** y escriba otro nombre en el cuadro de diálogo Guardar como.

**Para crear el conjunto de plantillas inicial**

1. Para crear la plantilla, utilice uno de los métodos siguientes:

   **Seleccione el PSD o las imágenes primero** en el panel Examinar, seleccione el archivo PSD o las imágenes que desee para su plantilla, haga clic en Generar &gt; Funciones básicas de plantilla.

   **Comience desde la pantalla Plantilla** haga clic en Generar &gt; Funciones básicas de plantilla. Seleccione Diseñador o Desarrollador.

1. En el cuadro de diálogo Introducir tamaño de lienzo, introduzca los valores de anchura y altura de la plantilla.
1. Seleccione una carpeta en la biblioteca de recursos y arrastre el archivo PSD o las imágenes requeridas hasta la pantalla Plantilla.
1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **Publicar después de guardar** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **Guardar**.
1. Seleccione una carpeta para guardar la plantilla, asigne un nombre a la plantilla y seleccione el botón **Enviar**.

   Dynamic Media Classic reduce las imágenes si es necesario para ajustarlas al lienzo, el área de la pantalla Plantilla para definir la plantilla.

## Edición de un conjunto de plantillas {#editing-a-template-set}

Según si edita un conjunto de plantillas publicado o sin publicar, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Ya se ha publicado el conjunto? | ¿Se ha seleccionado la opción “Publicar después de Guardar” antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservan su estado publicado. Todos los miembros nuevos que agregue durante la edición conservarán su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de plantillas**

1. En la vista de cuadrícula, busque un conjunto de plantillas y, debajo de la imagen, haga clic en **Editar**.
1. Realice los cambios necesarios en la plantilla.
1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **Publicar después de guardar** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **Guardar**, seleccione una carpeta de almacenamiento, especifique un nombre para el conjunto y haga clic en **Guardar**.

## Eliminación de una plantilla {#deleting-a-template}

Cuando se elimina un conjunto de plantillas, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar una plantilla**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione una o varias plantillas.
1. En la barra de navegación global, haga clic en **Archivo** &gt; **Eliminar** &gt; **Eliminar**.

## Información sobre la pantalla Plantilla {#understanding-the-template-screen}

La pantalla Plantilla contiene herramientas de edición y parametrización de capas.

Use estas herramientas en la pantalla Plantilla para crear plantillas:

**Herramienta de desplazamiento** Le permite seleccionar capas, moverlas alrededor del lienzo, cambiar su tamaño o rotarlas.

**Herramienta** Texto Crea una capa de texto. Arrastre el puntero sobre el lienzo para crear una capa de texto e introduzca el texto en la capa. Consulte Creación de una capa de texto.

**Botón Vista previa** Abre la pantalla Vista previa y muestra la plantilla en un visor de zoom. La plantilla aparece tal y como la verán los usuarios que accedan al sitio web o utilicen la aplicación.

**Botón Resumen de parámetros** Abre la pantalla Resumen de parámetros. Puede ver el nombre de cada una de las capas de una plantilla y, en cada capa, los nombres de los parámetros que se han activado.

**Editor de texto v 4.3 y v 4.2** , puede elegir utilizar el editor de texto más reciente y con más funciones, el Editor de texto v 4.3 o el anterior, el Editor de texto v 4.2. Al crear nuevas plantillas, el Editor de texto v 4.3 está seleccionado de forma predeterminada. Al editar plantillas antiguas, se seleccionará por defecto el Editor de texto 4.2. El Editor de texto v4.3 no admite el ajuste de palabras, de modo que si desea editar plantillas antiguas que utilicen ajuste de palabras, deberá utilizar el Editor de texto v4.2 para mantener intacta la fidelidad de la plantilla. Si la plantilla antigua no utiliza ajuste de palabras, puede seleccionar el Editor de texto v4.3 para aprovechar las nuevas funciones que este ofrece, como Aumentar márgenes, Reducir márgenes, Establecer texto en Todo en mayúsculas y Copiar texto de ajuste.

***nota**: El Editor de texto v 4.2 se eliminará finalmente como opción en Dynamic Media Classic, por lo que se recomienda utilizar el Editor de texto 4.3 siempre que sea posible. La opción de ajuste de palabras se incluirá en una versión posterior del Editor de texto.*

**Designer y Desarrollador** Seleccione la opción que mejor describe su función.

**Lienzo** Define el área total disponible, en píxeles, para definir la plantilla. El tamaño predeterminado es 300 x 300 píxeles. La capas se colocan en el lienzo.

**Lista de capas** Muestra el nombre de las capas de la plantilla. Para seleccionar una capa, seleccione su nombre en esta lista. La lista de capas ofrece herramientas para agregar efectos a capas, eliminar y parametrizar capas y modificar el orden de éstas. Consulte Uso de capas.

**Área de propiedades de la capa** Ofrece herramientas para cambiar el color de fondo, la opacidad, el tamaño y la posición de una capa, así como el color de fondo, la opacidad y el tamaño del lienzo. También es posible ajustar efectos de sombra y resplandor. Consulte Uso de capas.

## Creación de capas de imagen {#creating-image-layers}

1. Arrastre la imagen desde la biblioteca de recursos al lienzo.

   El ID de la imagen aparece en la lista de capas.

>[!NOTE]
>
>Si es necesario, Dynamic Media Classic reduce las imágenes para que quepan en el lienzo al crear una capa de imagen.

## Creación de una capa de texto {#creating-a-text-layer}

1. Haga clic en la herramienta Texto.
1. Arrastre para crear un cuadro de texto en el lienzo o en una imagen.
1. En la pantalla Texto que aparece, agregue texto mediante uno de los siguientes procedimientos en la ficha Vista previa:

   * Escriba el texto en el cuadro de texto. Seleccione Copiar texto de ajuste para ajustar el texto al cuadro de texto.
   * Pegue el texto desde el portapapeles en el cuadro de texto. 

1. Haga clic en Aplicar y cierre la pantalla de texto.

### Formateo de texto {#format-text}

Siga estos pasos para dar formato al texto en una capa de texto:

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. En el cuadro de texto, seleccione el texto al que desea dar formato. Puede seleccionar todo o parte del texto, o caracteres individuales.
1. Especifique las siguientes opciones de formato y, a continuación, haga clic en Aplicar.

   **Fuente** Elija una fuente en el menú Fuente. Si el tipo de letra que desea no aparece en el menú, puede cargarlo en Scene7 Publishing System. Consulte Fuentes.

   **Tamaño de fuente** Elija un tamaño de fuente en el menú, escriba un tamaño específico en el cuadro o haga clic en las flechas hacia arriba o hacia abajo para aumentar o disminuir el tamaño en dos puntos.

   **Clic en color** para elegir un color para el texto.

   **Negrita, Cursiva o Subrayado** Seleccione el texto y, a continuación, haga clic en el icono para el tipo de formato que desee aplicar al texto.

   **Todas las mayúsculas, Superíndice o Subíndice** Seleccione el texto y, a continuación, haga clic en el icono para el tipo de formato que desee aplicar al texto.

   **Alineaciónseleccione un** botón de alineación para alinear a la izquierda, centrar o alinear a la derecha texto de la capa de texto.

   **Tipo de seguimiento** o seleccione un valor numérico según el cual ajustar la cantidad de espacio entre palabras.

   **Tipo de kerning** o seleccione un valor numérico según el cual ajustar la cantidad de espacio entre caracteres.

   **Tipo de interlineado** o seleccione un valor numérico según el cual ajustar la cantidad de espacio entre líneas.

   **Tipo de desplazamiento** base o seleccione un valor numérico por el cual mover un carácter seleccionado hacia arriba o hacia abajo en relación con la línea base del texto que lo rodea. Esta opción resulta especialmente útil al definir fracciones manualmente o al ajustar la posición de gráficos integrados.

>[!NOTE]
>
>Haga clic en Deshacer para deshacer la última acción. Haga clic en Rehacer si cambia de opinión acerca de deshacer una acción después de hacer clic en Deshacer.

### Formateo de párrafos {#format-paragraphs}

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. Seleccione el párrafo al que desea dar formato.
1. Especifique las siguientes opciones de formato y, a continuación, haga clic en Aplicar.

   **Haga clic en** Hacer clic para especificar el tipo de alineación: alinea a la izquierda, al centro, a la derecha o justificado.

   **Final de justificación de párrafo** Haga clic para especificar el tipo de justificación de la última línea del párrafo: la última línea se alinea a la izquierda; alineación de la última línea; y la última línea la derecha.

   **Tipo de interlineado** o seleccione un valor numérico según el cual ajustar la cantidad de espacio entre todas las líneas del párrafo.

   **Sangría en Todos** los clics para aumentar la cantidad de sangría del texto.

   **Eliminar sangría** Haga clic para reducir la sangría del texto.

   **Sangría en primera línea** Especifique la cantidad por la que desea sangrar la primera línea de texto.

   **Espacio antes del párrafo** Especifique la cantidad de espacio que desea que aparezca encima de la primera línea de texto del párrafo.

   **Espacio después del párrafo** Especifique la cantidad de espacio que desea que aparezca debajo de la última línea de texto del párrafo.

   **Alineación vertical** Seleccione dónde desea que aparezca el texto verticalmente dentro del cuadro de texto: Arriba, Centro, Abajo.

   **Dirección del texto** Seleccione la dirección en la que desea que se muestre el texto: De derecha a izquierda o de izquierda a derecha.

### Ajuste de propiedades de capas de texto {#adjust-text-layer-properties}

1. En la pantalla Funciones básicas de plantilla, seleccione el cuadro de texto que desea ajustar.
1. En el panel Propiedades de la capa, seleccione cualquiera de los siguientes:

   **Reducir texto (solo en el Editor de texto v 4.2)** Seleccione para reducir el texto y ajustarlo al cuadro de texto.

   **Ajuste de Word (solo en el Editor de texto v 4.2)** Seleccione una opción de ajuste para especificar si se ajusta o no el texto:

   **Ajustar** ajusta el texto para ajustarlo a un cuadro de texto demasiado pequeño horizontalmente.

   **Sin ajuste** no ajusta el texto cuando el cuadro de texto es demasiado pequeño horizontalmente y, en su lugar, se corta una parte del texto.

   **Ajuste** de ajuste NB (ajuste de no separación) Ajusta el texto para ajustarlo a un cuadro de texto y no separa las palabras.

   **Posición** Especifica la ubicación del cuadro de texto en el lienzo.

   **Relleno** Añade márgenes o recorta el rectángulo de la capa. Especifique el número de píxeles que agregar o eliminar de izquierda, arriba, abajo, y derecha. Introduzca números positivos para agregar un margen; introduzca números negativos para recortarlos.

### Visualización y edición de texto del código fuente {#view-and-edit-text-source-code}

La información que se proporciona en la ficha Origen del Editor de texto es para su referencia. Modifique el texto únicamente si está familiarizado con la edición de código fuente.

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. Haga clic en la ficha Origen del Editor de texto para mostrar el código fuente del texto.
1. Vea o edite el texto según lo necesite.

   Los cambios se mantienen intactos al alternar entre la vista previa y la vista de código fuente.

1. Haga clic en Aplicar para efectuar los cambios.

## Uso de capas {#working-with-layers}

Use la lista de capas y el área Propiedades de la capa para trabajar con capas. Puede reordenar las capas, modificar su tamaño y posición, girarlas y determinar el color de fondo, color de primer plano, opacidad y modo de mezcla de una capa.

También es posible modificar el tamaño del lienzo y especificar su color de fondo y opacidad.

### Reordenación de las capas {#reordering-layers}

Cambiar el orden de las capas puede afectar a su apariencia, especialmente cuando se trata de la transparencia o la sobreimpresión. Asegúrese de comprobar el resultado mediante una vista previa antes de confirmar los cambios.

1. Use una de estas técnicas para cambiar el orden de las capas de una plantilla:

   * Seleccione una capa en la lista de capas. A continuación, haga clic en el botón Subir o Bajar las veces necesarias para colocar la capa en la posición deseada en la lista.
   * Arrastre una capa a una posición superior o inferior en la lista.

### Cambio del tamaño y la posición de las capas y el lienzo {#changing-the-size-and-position-of-layers-and-the-canvas}

El tamaño de las capas no debe superar las restricciones del lienzo. Puede modificar el tamaño de una capa o el del lienzo manualmente o introduciendo las medidas requeridas. Puede modificar la posición de una capa manualmente o introduciendo los valores de desfase requeridos. También puede rotar una capa.

>[!NOTE]
>
>Dynamic Media Classic recomienda crear un ajuste preestablecido de imagen con el tamaño exacto de la plantilla. De este modo se asegura una definición correcta de las opciones de enfoque y el tamaño de salida final de la plantilla. Después de crear este ajuste de imagen preestablecido, está disponible en el menú Ajustes preestablecidos, en la pantalla Vista previa de plantilla. La pantalla muestra el aspecto que tendrá la imagen procedente del servidor. Consulte [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

**Cambio del tamaño de una capa**

Para modificar el tamaño de una capa o el del lienzo, seleccione la capa o el lienzo en la lista de capas y use una de estas técnicas:

**Cambio manual de tamaño** Seleccione y arrastre una esquina de la capa o del lienzo. Con las capas de texto, también puede arrastrar un lado de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño pero manteniendo la proporción de aspecto (la forma).

**Introducción de medidas de tamaño de capa** Introduzca mediciones de píxeles en los cuadros de texto W (Anchura) y H (Altura) en el área Propiedades de la capa.

Además de cambiar el tamaño, también es posible añadir un margen a la capa. Para ello, introduzca un valor de margen en los cuadros Izquierda, Derecha, Superior e Inferior del área Propiedades de la capa. Se insertará un margen entre la capa actual y el perímetro de la capa base. El margen es útil para hacer más visibles efectos de sombra paralela o resplandor exterior añadidos. El margen incrementa el tamaño de una capa y muestra su color de fondo en el área extendida. La posición de la capa base se ajusta con relación al nuevo tamaño de la capa. Por ejemplo, si la capa actual está centrada en la capa base, al extenderse el lado izquierdo de la capa ésta se desplaza hacia la derecha de la capa base.

**Cambio de la posición de una capa**

Para modificar la posición de una capa o la del lienzo, seleccione el nombre en la lista de capas y use una de estas técnicas:

**Cambiar la posición manualmente** 
Mueva el puntero cerca de un límite de capa, pero no lo hace, y cuando vea el cursor de flecha con cuatro puntas, haga clic y arrastre.

**Introducción de medidas de compensación de posición** Introduzca los valores de desplazamiento X e Y en los cuadros de texto X e Y. Esto valores representan el desfase x, y del punto de anclaje, medido en píxeles.

**Rotación de una capa**

El cuadro Rotar indica el ángulo de rotación de la capa. Para rotar una capa, seleccione el nombre de ésta en la lista de capas y use una de estas técnicas:

**Rotación manual** de mueva el cursor cerca de una esquina de la capa, pero no sobre ella. Cuando aparezca el cursor de rotación, arrastre la esquina de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para rotar en incrementos de 15 grados.

**Introducción de una medición** de grados Introduzca el número de grados para rotar la capa. Se aplica una rotación hacia la derecha; para rotar la capa hacia la izquierda, debe introducir un valor negativo.

**Ocultación de una capa o un efecto de capa**

Puede ocultar una capa o efecto de capa haciendo clic en el icono del ojo  junto al nombre de la capa o del efecto. Las capas ocultas no aparecen en las vistas previas o en el resultado final. La información de la capa no se elimina de la URL. En su lugar, se agrega "hide=1" a la URL para señalar que la capa está oculta a la vista. Por ejemplo:

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;hide=1&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

### Configuración del color de fondo, la opacidad y el modo de fusión {#determining-the-background-color-opacity-and-blend-mode}

Para definir el color de fondo, la opacidad y el modo de fusión de una capa o del lienzo, seleccione la capa o el lienzo y use una de esta técnicas:

**Color frontal** Haga clic en el botón Color frontal y elija una muestra de color para cambiar el color de la sombra o del resplandor. También puede introducir un valor de color en el cuadro. El color de fondo solo se aplica a las capas con transparencia. Se puede utilizar, por ejemplo, en una capa con transparencia parcial de una etiqueta de precio o en el fondo de un campo de texto. Las capas que consisten en una imagen PSD, TIFF o PNG con transparencia activada pueden tener fondos transparentes.

**Color de fondo** Haga clic en el botón Color de fondo y elija una muestra de color para cambiar el color de las áreas con relleno.

**Opacidad** Arrastre el control deslizante Opacidad para crear cualquier capa translúcida para que se muestre parte de la imagen subyacente. El valor 100 representa la opacidad total y el valor 0 la transparencia.

**Modo de fusión** Elija una opción para simular uno de los modos de fusión disponibles en Photoshop. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla. Estas opciones están disponibles para capas únicamente, no son aplicables a lienzos.

## Utilización de efectos de sombra y resplandor en las capas {#using-shadow-and-glow-effects-on-layers}

Puede aplicar una sombra o un resplandor a una capa. La sombra o el resplandor se aplican al perímetro de la capa y se extienden hacia dentro o hacia fuera, según la opción elegida. Si la plantilla se ha creado a partir de un archivo PSD con efectos de sombra y resplandor, puede ajustar estos efectos en Scene7 Publishing System.

Después de aplicar un efecto de sombra o resplandor, puede ajustar su tamaño, color, opacidad y posición en el área Propiedades de la capa, en la pantalla Plantilla.

### Aplicación de un efecto de sombra o resplandor a una capa {#applying-a-shadow-or-glow-effect-to-a-layer}

Para aplicar un efecto de sombra o resplandor:

1. Seleccione una capa en la lista de capas.
1. Seleccione el menú Agregar efecto y elija una opción:

   **Sombra paralela** Aplica una sombra a la parte inferior y derecha de la capa.

   **Sombra interior** Aplica un efecto de sombra dentro de todos los bordes de la capa.

   **Resplandor** exterior Aplica un resplandor alrededor de todos los bordes de la capa.

   **Resplandor** interior Aplica un resplandor dentro de todos los bordes de la capa.

Después de aplicar un efecto, el nombre del mismo aparece en la lista de capas. Para eliminar un efecto, seleccione el nombre correspondiente en la lista de capas y luego seleccione el botón Eliminar.

>[!NOTE]
>
>Si la capa subyacente es demasiado pequeña para mostrarlo, puede que no sea visible un efecto de sombra paralela o resplandor externo aplicado. De ser así, puede añadir valores de margen a la capa, o cambiar el orden de las capas. Consulte [Cambio del tamaño y la posición de las capas y el lienzo](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) y [Reordenación de las capas](creating-template.md#reordering_layers).

### Ajuste de un efecto de sombra o resplandor {#adjusting-a-shadow-or-glow-effect}

Para ajustar un efecto de sombra o resplandor, seleccione el nombre correspondiente en la lista de capas. Cambie los valores que tiene asignados en el área Propiedades de la capa:

**Color** Seleccione el botón Color y elija una muestra de color para cambiar el color de la sombra o del resplandor. También puede introducir un valor de color en el cuadro.

**Opacidad** Arrastre el control deslizante para determinar la intensidad del efecto. Cuanto menor sea el valor de opacidad, mayor será la transparencia del efecto.

**Modo de fusión** Elija una opción para simular uno de los modos de fusión disponibles en Photoshop. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla.

**Tamañointroduzca** las medidas en el cuadro X e Y para ampliar o reducir el efecto de sombra. Las opciones de tamaño son aplicables a sombras interiores y paralelas.

**Aumentar** el deslizador para extender el efecto hacia dentro o hacia fuera.

**Desenfoque** Arrastre el control deslizante para controlar el calado en los bordes del efecto. Cuanto mayor sea el desenfoque, mayor será el calado.

## Creación de máscaras en capas {#masking-layers}

El botón Máscara, disponible en la lista de capas, permite especificar el uso de la máscara o el canal alfa de una capa. Con este botón puede aplicar el efecto de una capa de fondo a una capa concreta, o a toda la capa principal de la plantilla. Seleccione una capa en la lista de capas y luego seleccione el botón Máscara  para acceder a estos estados:

* El fondo de la capa es opaco.
* El contenido de la capa se invierte y el fondo de ésta se rellena de negro sólido.
* El fondo de la capa se rellena de negro sólido.

