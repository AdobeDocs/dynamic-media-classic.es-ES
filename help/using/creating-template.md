---
title: Creación de una plantilla
description: Obtenga información sobre cómo crear una plantilla en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '3427'
ht-degree: 36%

---

# Creación de una plantilla

Para crear una plantilla, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de plantilla]**. Seleccione Diseñador o Desarrollador. En esta página puede añadir capas de imagen y de texto. También puede cambiar el orden de las capas, modificar el tamaño y la posición de éstas y aplicarles efectos de sombra y resplandor.

Consulte también [Conceptos básicos de plantilla](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de formación.

>[!NOTE]
>
>Si edita una plantilla creada en una versión anterior de Adobe Dynamic Media Classic, un mensaje le preguntará al guardar &quot;¿Desea agregar una capa de lienzo?&quot; Seleccionar **[!UICONTROL No]** para evitar agregar una capa base. Si selecciona accidentalmente **[!UICONTROL Sí]**, elimine la `&allowCanvasPrompt` y `&layer=0` en la URL y pulse **[!UICONTROL Entrar]** o **[!UICONTROL Volver]**.

## Creación de la plantilla inicial {#creating-the-initial-template}

Cuando se crea un conjunto de plantillas, la variable **[!UICONTROL Publicar tras guardar]** afecta a los miembros set y set de las siguientes maneras:

| **[!UICONTROL Publicar tras guardar]** opción seleccionada antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

Puede crear una plantilla a partir de una existente. Abra la plantilla y seleccione **[!UICONTROL Guardar como]** y escriba un nombre nuevo en el cuadro de diálogo Guardar como.

**Para crear la plantilla inicial:**

1. Para crear la plantilla inicial, utilice uno de los siguientes métodos:

   * **Seleccione primero el PSD o las imágenes**: en el panel Examinar, seleccione el archivo o las imágenes de PSD que desee para la plantilla y vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de plantilla]**.

   * **Empezar desde la pantalla Plantilla**: Vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de plantilla]**. Seleccione Diseñador o Desarrollador.

1. En el cuadro de diálogo Especificar tamaño de lienzo, escriba las medidas de anchura y altura para la plantilla.
1. Seleccione una carpeta en la biblioteca de recursos y arrastre el archivo PSD o las imágenes requeridas hasta la pantalla Plantilla.
1. Cuando termine, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar tras guardar]** está seleccionado (predeterminado).
1. Seleccionar **[!UICONTROL Guardar]**.
1. Seleccione una carpeta para almacenar la plantilla, introduzca un nombre para ella y seleccione **[!UICONTROL Enviar]**.

   Adobe Dynamic Media Classic reduce el tamaño de las imágenes si es necesario para ajustarlas al lienzo, el área de la pantalla Plantilla para definir la plantilla.

## Edición de un conjunto de plantillas {#editing-a-template-set}

Tanto si edita un conjunto de plantillas publicadas como si no, la variable **[!UICONTROL Publicar tras guardar]** afecta a los miembros set y set de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL Publicar tras guardar]** opción seleccionada antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de plantillas:**

1. En la vista de cuadrícula, busque un conjunto de plantillas y, debajo de la imagen, seleccione **[!UICONTROL Editar]**.
1. Cambie la plantilla según sea necesario.
1. Cuando termine de editar, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar tras guardar]** está seleccionado (predeterminado).
1. Seleccionar **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar una plantilla

Al eliminar un conjunto de plantillas, el propio conjunto se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar una plantilla:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione una o varias plantillas.
1. En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.

## Explicación de la pantalla Plantilla {#understanding-the-template-screen}

La pantalla Plantilla contiene herramientas de edición y parametrización de capas.

Utilice estas herramientas en la pantalla Plantilla para poder crear plantillas:

* **[!UICONTROL Panorámica]**: permite seleccionar capas, moverlas por el lienzo, cambiar su tamaño o girarlas.

* **[!UICONTROL Texto]**: crea una capa de texto. Arrastre el puntero sobre el lienzo para crear una capa de texto e introduzca el texto en la capa. Consulte [Creación de una capa de texto](#creating-a-text-layer).

* **[!UICONTROL Previsualizar]**: abre la pantalla Vista previa y muestra la plantilla en un Visor de zoom. Verá el aspecto que tendrá la plantilla para los usuarios de su sitio web o aplicación.

* **[!UICONTROL Resumen de parámetros]** Abre la pantalla Resumen de parámetros. Puede ver el nombre de cada una de las capas de una plantilla y, en cada capa, los nombres de los parámetros que se han activado.

* **[!UICONTROL Editor de texto v4.3 y Editor de texto v4.2]**: utilice el editor de texto más reciente y con más funciones. Puede elegir utilizar el Editor de texto v4.3 o el Editor de texto anterior, Editor de texto v4.2. Al crear plantillas, Editor de texto v4.3 está seleccionado de forma predeterminada. Al editar plantillas antiguas, se seleccionará por defecto el Editor de texto 4.2. El Editor de texto v4.3 no admite actualmente el ajuste de palabras, por lo que al editar plantillas antiguas que utilizan el ajuste de palabras, utilice el Editor de texto v4.2 para mantener la fidelidad de la plantilla totalmente intacta. Si la plantilla anterior no utiliza ajuste de línea, puede elegir Editor de texto v4.3 para aprovechar las numerosas funciones nuevas que ofrece. Por ejemplo, Aumentar márgenes, Reducir márgenes, Definir texto en mayúsculas y Copiar texto de ajuste.

  >[!NOTE]
  >
  >Se ha planificado la eliminación del Editor de texto v4.2 como opción en Adobe Dynamic Media Classic. Se recomienda utilizar el Editor de texto 4.3 cuando sea posible. El **[!UICONTROL Ajuste de palabras]** se incorporará a una versión futura del Editor de texto.

* **[!UICONTROL Diseñador y desarrollador]**: seleccione la opción que mejor describa su función.

* **[!UICONTROL Lienzo]**: define el área total disponible, en píxeles, para definir la plantilla. El tamaño predeterminado es de 300 × 300 píxeles. La capas se colocan en el lienzo.

* **[!UICONTROL Lista de capas]**: Muestra el nombre de las capas de la plantilla. Para seleccionar una capa, seleccione su nombre en esta lista. La lista de capas ofrece herramientas para agregar efectos a capas, eliminar y parametrizar capas y modificar el orden de éstas. Consulte [Trabajo con capas](#working-with-layers).

* **[!UICONTROL Área Propiedades de la capa]**: Esta área ofrece herramientas para cambiar el color de fondo, la opacidad, el tamaño y la posición de una capa. También puede cambiar el color de fondo, la opacidad y el tamaño del lienzo. También es posible ajustar efectos de sombra y resplandor. Consulte [Trabajo con capas](#working-with-layers).

## Creación de capas de imagen {#creating-image-layers}

1. Arrastre la imagen desde la biblioteca de recursos al lienzo.

   El ID de la imagen aparece en la lista de capas.

   >[!NOTE]
   >
   >Si es necesario, Adobe Dynamic Media Classic reduce el tamaño de las imágenes para que quepan en el lienzo cuando se crea una capa de imagen.

## Creación de una capa de texto {#creating-a-text-layer}

1. Seleccione el **[!UICONTROL Texto]** herramienta.
1. Arrastre para crear un cuadro de texto en el lienzo o en una imagen.
1. En la pantalla Texto que se abre, agregue texto mediante cualquiera de las siguientes acciones en la pestaña Vista previa:

   * Escriba el texto en el cuadro de texto. Seleccione Copiar texto de ajuste para ajustar el texto al cuadro de texto.
   * Pegue el texto desde el portapapeles en el cuadro de texto. 

1. Seleccionar **[!UICONTROL Aplicar]** y, a continuación, cierre la pantalla Texto.

### Formateo de texto {#format-text}

Para dar formato al texto en una capa de texto, haga lo siguiente:

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. En el cuadro de texto del Editor de texto, seleccione el texto al que desee dar formato. Puede seleccionar todo el texto, partes del texto o caracteres individuales.
1. Especifique cualquiera de las siguientes opciones de formato y seleccione **[!UICONTROL Aplicar]**.

   * **[!UICONTROL Fuente]**: elija una fuente en el menú Fuente. Si una fuente que desea no aparece en el menú, puede cargarla en Adobe Dynamic Media Classic. Consulte Fuentes.

   * **[!UICONTROL Tamaño de fuente]**: elija un tamaño de fuente en el menú, escriba un tamaño específico en el cuadro o seleccione la opción **[!UICONTROL Arriba]** o **[!UICONTROL Abajo]** para aumentar o disminuir el tamaño en dos puntos.

   * **[!UICONTROL Color]**: seleccione para elegir un color para el texto.

   * **[!UICONTROL Negrita]**, **[!UICONTROL Cursiva]**, o **[!UICONTROL Subrayado]**: seleccione el texto y, a continuación, seleccione el icono para el tipo de formato que desea aplicar al texto.

   * **[!UICONTROL Todo en mayúsculas]**, **[!UICONTROL Superíndice]**, o **[!UICONTROL Subíndice]**: seleccione el texto y, a continuación, seleccione el icono para el tipo de formato que desea aplicar al texto.

   * **[!UICONTROL Alineación]**: elija un botón Alineación para alinear a la izquierda, centrar o alinear a la derecha el texto en la capa de texto.

   * **[!UICONTROL Seguimiento]**: escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre palabras.

   * **[!UICONTROL Kerning]**: escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre caracteres.

   * **[!UICONTROL Interlineado]**: escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre líneas.

   * **[!UICONTROL Desplazamiento vertical]**: escriba o seleccione un valor numérico mediante el cual mover un carácter seleccionado hacia arriba o hacia abajo en relación con la línea de base del texto que lo rodea. Esta opción es especialmente útil cuando se configuran a mano fracciones o se ajusta la posición de gráficos en línea.

>[!NOTE]
>
>Seleccionar **[!UICONTROL Deshacer]** si desea revertir la última acción. Seleccionar **[!UICONTROL Rehacer]** si cambia de opinión sobre la reversión de una acción después de seleccionar **[!UICONTROL Deshacer]**.

### Formateo de párrafos {#format-paragraphs}

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. Seleccione el párrafo al que desea dar formato.
1. Especifique cualquiera de las siguientes opciones de formato y seleccione **[!UICONTROL Aplicar]**.

   * **[!UICONTROL Alineación]**: especifique el tipo de alineación haciendo clic en **[!UICONTROL Alinear izquierda]**, **[!UICONTROL Alinear al centro]**, **[!UICONTROL Alinear a la derecha]**, o **[!UICONTROL Justificar]**.

   * **[!UICONTROL Justificación de fin de párrafo]**: seleccione esta opción para especificar el tipo de justificación de la última línea del párrafo: la última línea se alinea a la izquierda, la última línea se alinea al centro y la última línea se alinea a la derecha.

   * **[!UICONTROL Interlineado]**: escriba o seleccione un valor numérico para ajustar la cantidad de espacio entre todas las líneas del párrafo.

   * **[!UICONTROL Sangrar todo]**: seleccione esta opción para aumentar la cantidad de sangría del texto.

   * **[!UICONTROL Eliminar sangría]**: seleccione esta opción para reducir la cantidad de sangría del texto.

   * **[!UICONTROL Sangría en primera línea]**: especifique la cantidad en que desea sangrar la primera línea de texto.

   * **[!UICONTROL Espacio antes del párrafo]**: especifique la cantidad de espacio que desea que aparezca sobre la primera línea de texto del párrafo.

   * **[!UICONTROL Espacio después del párrafo]**: especifique la cantidad de espacio que desea que aparezca debajo de la última línea de texto del párrafo.

   * **[!UICONTROL Alineación vertical]**: seleccione el lugar donde desee que aparezca el texto verticalmente dentro del cuadro de texto: Superior, Medio, Inferior.

   * **[!UICONTROL Dirección del texto]**: seleccione la dirección en la que desea que se muestre el texto: De derecha a izquierda o de izquierda a derecha.

### Ajuste de propiedades de capas de texto {#adjust-text-layer-properties}

1. En la pantalla Funciones básicas de plantilla, seleccione el cuadro de texto que desea ajustar.
1. En el panel Propiedades de la capa, seleccione cualquiera de los siguientes:

   * **[!UICONTROL Reducir texto (solo Editor de texto v4.2)]**: seleccione esta opción para reducir el texto de modo que se ajuste al cuadro de texto.

   * **[!UICONTROL Ajuste de palabras (solo Editor de texto v4.2)]**: para especificar si el texto se ajusta o cómo, seleccione una opción de ajuste:

   * **[!UICONTROL Ajuste]**: ajusta el texto en un cuadro de texto que es demasiado pequeño horizontalmente.

   * **[!UICONTROL Sin ajuste]**: no ajusta el texto cuando el cuadro de texto es demasiado pequeño horizontalmente y, en su lugar, corta una parte del texto.

   * **[!UICONTROL Ajuste de no separación]**: Ajusta el texto para que quepa en un cuadro de texto y no divide las palabras.

   * **[!UICONTROL Posición]**: especifica la ubicación del cuadro de texto en el lienzo.

   * **[!UICONTROL Relleno]**: añade márgenes o recorta el rectángulo de capa. Especifique el número de píxeles que desea añadir o quitar para izquierda, arriba, abajo y derecha. Introduzca números positivos si desea añadir un margen o números negativos al recorte.

### Visualización y edición de texto del código fuente {#view-and-edit-text-source-code}

La información proporcionada en la pestaña Fuente del Editor de texto es para su referencia. Modifique el texto únicamente si está familiarizado con la edición de código fuente.

1. En la lista Capas, haga doble clic en el nombre del cuadro de texto que contenga el texto que desee editar. Accederá al Editor de texto.
1. En el Editor de texto, para mostrar el código fuente del texto, seleccione **[!UICONTROL Origen]** en el Editor de texto.
1. Vea o edite el texto según lo necesite.

   Los cambios se mantienen intactos al alternar entre la vista previa y la vista de código fuente.

1. Seleccionar **[!UICONTROL Aplicar]** para procesar las ediciones.

## Trabajo con capas {#working-with-layers}

Use la lista de capas y el área Propiedades de la capa para trabajar con capas. Puede reordenar las capas, modificar su tamaño y posición, girarlas y determinar el color de fondo, color de primer plano, opacidad y modo de mezcla de una capa.

También es posible modificar el tamaño del lienzo y especificar su color de fondo y opacidad.

### Reordenar capas {#reordering-layers}

Cambiar el orden de las capas puede afectar al aspecto, especialmente cuando hay transparencia o sobreimpresión. Asegúrese de comprobar el resultado mediante una vista previa antes de confirmar los cambios.

1. Use una de estas técnicas para cambiar el orden de las capas de una plantilla:

   * Seleccione una capa en la lista de capas. A continuación seleccione **[!UICONTROL Arriba]** o **[!UICONTROL Abajo]** tantas veces como sea necesario para colocarlo en la posición correcta de la lista.
   * Arrastre una capa a una posición superior o inferior en la lista.

### Cambiar el tamaño y la posición de las capas y el lienzo {#changing-the-size-and-position-of-layers-and-the-canvas}

El tamaño de las capas no debe superar las restricciones del lienzo. Puede modificar el tamaño de una capa o el del lienzo manualmente o introduciendo las medidas requeridas. Puede modificar la posición de una capa manualmente o introduciendo los valores de desfase requeridos. También puede rotar una capa.

>[!NOTE]
>
>Adobe Dynamic Media Classic recomienda crear un ajuste preestablecido de imagen que sea del tamaño exacto de la plantilla. De este modo se asegura una definición correcta de las opciones de enfoque y el tamaño de salida final de la plantilla. Después de crear este ajuste preestablecido de imagen, puede elegirlo en el menú Aplicar ajuste preestablecido de la pantalla Vista previa de plantilla. La pantalla muestra el aspecto que tendrá la imagen procedente del servidor. Consulte [Configurar ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

* **Modificación del tamaño de una capa**: para cambiar el tamaño de una capa o del lienzo, seleccione la capa o el lienzo en la lista Capas y utilice una de estas técnicas:

* **Cambio manual del tamaño**: seleccione y arrastre una esquina de la capa o el lienzo. Con las capas de texto, también puede arrastrar un lado de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño pero mantener la relación de aspecto (la forma).

* **Introducción de medidas de tamaño de capa**: introduzca las medidas de los píxeles en los cuadros de texto An (Anchura) y Al (Altura) del área Propiedades de la capa.

Además de cambiar el tamaño, también es posible añadir un margen a la capa. Para ello, introduzca un valor de margen en los cuadros Izquierda, Derecha, Superior e Inferior del área Propiedades de la capa. Se insertará un margen entre la capa actual y el perímetro de la capa base. El margen es útil para hacer más visibles efectos de sombra paralela o resplandor exterior añadidos. El margen incrementa el tamaño de una capa y muestra su color de fondo en el área extendida. La posición de la capa base se ajusta con relación al nuevo tamaño de la capa. Por ejemplo, si la capa actual está centrada en la capa base, al extenderse el lado izquierdo de la capa ésta se desplaza hacia la derecha de la capa base.

* **Cambio de la posición de una capa**: para cambiar la posición de una capa en el lienzo, seleccione su nombre en la lista Capas y utilice una de estas técnicas:

* **Cambio manual de posición**: Mueva el puntero cerca del límite de una capa, pero no sobre él, y cuando vea el cursor de flecha de cuatro puntas, seleccione y comience a arrastrar.

* **Introducción de medidas de desplazamiento de posición**: introduzca las medidas de desvío X e Y en los cuadros de texto X e Y. Esto valores representan el desfase x, y del punto de anclaje, medido en píxeles.

* **Rotación de una capa**: el cuadro Rotar enumera el ángulo al que se giró la capa. Para rotar una capa, seleccione el nombre de ésta en la lista de capas y use una de estas técnicas:

* **Rotación manual**: mueva el cursor cerca de una esquina de la capa, pero no sobre ella. Cuando aparezca el cursor de rotación, arrastre la esquina de la capa. Mantenga pulsada la tecla Mayús mientras arrastra para rotar en incrementos de 15 grados.

* **Introducción de una medición de grado**: introduzca el número de grados para girar la capa. Se aplica una rotación hacia la derecha; para rotar la capa hacia la izquierda, debe introducir un valor negativo.

**Ocultar una capa o un efecto de capa:**

Para ocultar una capa o un efecto de capa, seleccione el icono del ojo junto al nombre de una capa o un nombre de efecto. Las capas ocultas no aparecen en las vistas previas o en el resultado final. La información de la capa no se elimina de la URL. En su lugar, `hide=1` se añade a la dirección URL para indicar que la capa no se ve. Por ejemplo:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Determinar el color de fondo, la opacidad y el modo de fusión

Para definir el color de fondo, la opacidad y el modo de fusión de una capa o del lienzo, seleccione la capa o el lienzo y use una de esta técnicas:

* **Color frontal**: Seleccionar **[!UICONTROL Color frontal]** y elija una muestra de color para cambiar el color de la sombra o el resplandor. También puede introducir un valor de color en el cuadro. El color de fondo solo se aplica a las capas con transparencia. Se puede utilizar, por ejemplo, en una capa con transparencia parcial de una etiqueta de precio o en el fondo de un campo de texto. Las capas que consisten en una imagen PSD, TIFF o PNG con transparencia activada pueden tener fondos transparentes.

* **Color de fondo**: Seleccionar **[!UICONTROL Color de fondo]** y elija una muestra de color para cambiar el color de las áreas acolchadas.

* **Opacidad**: arrastre el control deslizante Opacidad para que cualquier capa sea translúcida y que se muestre parte de la imagen subyacente. El valor del 100 por ciento es opaco; 0 es transparente.

* **Modo de fusión**: Para simular uno de los modos de fusión disponibles en Photoshop, elija una opción. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla. Estas opciones están disponibles para capas únicamente, no son aplicables a lienzos.

## Uso de efectos de sombra y resplandor en las capas {#using-shadow-and-glow-effects-on-layers}

Puede aplicar una sombra o un resplandor a una capa. La sombra o el resplandor se aplica al perímetro de la capa y se extiende hacia dentro o hacia fuera, según la opción de sombra o resplandor que elija. Si la plantilla se originó con un archivo PSD con efectos de sombreado y resplandor, puede ajustar estos efectos en Adobe Dynamic Media Classic.

Después de aplicar un efecto de sombra o resplandor, puede ajustar su tamaño, color, opacidad y posición en el área Propiedades de la capa, en la pantalla Plantilla.

### Aplicar un efecto de sombra o resplandor a una capa {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Seleccione una capa en la lista de capas.
1. Seleccione el **[!UICONTROL `Add Effect`]** y elija una opción:

   * **[!UICONTROL Sombra paralela]**: aplica una sombra a la parte inferior y derecha de la capa.

   * **[!UICONTROL Sombra interna]**: aplica un efecto de sombra dentro de todos los bordes de la capa.

   * **[!UICONTROL Resplandor exterior]**: aplica un efecto de resplandor alrededor de todos los bordes de la capa.

   * **[!UICONTROL Resplandor interior]**: aplica un efecto de resplandor dentro de todos los bordes de la capa.

Después de aplicar un efecto, el nombre del mismo aparece en la lista de capas. Para eliminar un efecto, seleccione su nombre en la lista Capas y seleccione **[!UICONTROL Eliminar]**.

>[!NOTE]
>
>A veces no puede ver el efecto de una sombra paralela o un resplandor exterior si la capa subyacente no es lo suficientemente grande como para mostrarla. Si no puede ver la sombra o el resplandor, considere la posibilidad de agregar valores de relleno a la capa o reordenar la capa. Consulte [Cambio del tamaño y la posición de las capas y el lienzo](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) y [Reordenación de las capas](creating-template.md#reordering_layers).

### Ajuste de un efecto de sombra o resplandor {#adjusting-a-shadow-or-glow-effect}

Para ajustar un efecto de sombra o resplandor, seleccione el nombre correspondiente en la lista de capas. Cambie los valores que tiene asignados en el área Propiedades de la capa:

* **[!UICONTROL Color]**: seleccione el botón Color y elija una muestra de color para cambiar el color de la sombra o el resplandor. También puede introducir un valor de color en el cuadro.

* **[!UICONTROL Opacidad]**: Arrastre el control deslizante para determinar la intensidad del efecto. Cuanto menor sea el valor de opacidad, mayor será la transparencia del efecto.

* **[!UICONTROL Modo de fusión]**: Para simular uno de los modos de fusión disponibles en Photoshop, elija una opción. Las opciones son Normal, Disolver, Aclarar, Oscurecer, Multiplicar y Pantalla.

* **[!UICONTROL Tamaño]**: introduzca las medidas en los cuadros X e Y para aumentar o reducir el efecto de sombra. Las opciones de tamaño son aplicables a sombras interiores y paralelas.

* **[!UICONTROL Aumentar]**: arrastre el control deslizante para extender el efecto hacia dentro o hacia fuera.

* **[!UICONTROL Desenfocar]**: arrastre el regulador para controlar el calado en los bordes del efecto. Cuanto mayor sea el desenfoque, mayor será el calado.

## Capas de máscara {#masking-layers}

El botón Máscara, disponible en la lista de capas, permite especificar el uso de la máscara o el canal alfa de una capa. Con este botón puede aplicar el efecto de una capa de fondo a una capa concreta, o a toda la capa principal de la plantilla. Seleccione una capa en la lista Capas (Layers) y seleccione **[!UICONTROL Máscara]** para recorrer estos estados:

* El fondo de la capa es opaco.
* El contenido de la capa se invierte y el fondo de ésta se rellena de negro sólido.
* El fondo de la capa se rellena de negro sólido.
