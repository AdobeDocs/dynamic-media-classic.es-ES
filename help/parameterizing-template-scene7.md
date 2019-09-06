---
title: Parametrización de una plantilla en Dynamic Media Classic
seo-title: Parametrización de una plantilla en Dynamic Media Classic
description: nulo
seo-description: Aprenda a parametrizar una plantilla en Dynamic Media Classic
uuid: 27 c 8 c 8 b 4-47 f 3-4270-a 6 db-d 304648 ba 357
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/template-publishing
discoiquuid: df 1 a 9 ff 5-a 5 ba -4480-ba 0 d-a 19 bc 665 f 907
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Parametrización de una plantilla en Dynamic Media Classic{#parameterizing-a-template-in-scene}

Después de cargar una plantilla de Illustrator guardada como FXG de Dynamic Media Classic en Scene 7 Publishing System, puede definir sus elementos variables. Para ello, parametrice los elementos variables en las pantallas Generar y Vista previa de Publicación de plantillas. Dynamic Media Classic ofrece herramientas para definir parámetros de texto y objetos en capas y sus respectivas propiedades. También puede crear diferentes versiones de una plantilla.

La parametrización de una plantilla FXG le permite personalizar la variabilidad del texto, las imágenes y los gráficos de la plantilla. Por ejemplo, puede parametrizar una línea de texto de forma que los usuarios finales puedan modificar el texto a través de una interfaz de usuario web. Puede definir campos de texto vacíos como variables de forma que los usuarios finales puedan rellenar estos campos con texto personalizado. También puede parametrizar los atributos y las propiedades de los elementos de diseño en la pantalla Generar publicación de Dynamic Media Classic.

>[!NOTE]
>
>No es necesario parametrizar la plantilla en Dynamic Media Classic si planea utilizar la manipulación DOM.

## Definición de parámetros en plantillas FXG {#defining-parameters-in-fxg-templates}

Siga estos pasos en Dynamic Media Classic para definir parámetros para una plantilla FXG:

1. En la ventana Examinar, seleccione el archivo FXG.
1. Click **Build** and choose **Template Publishing**, or click the file’s **Edit** button.

   Se abre la pantalla Publicación de plantilla.

1. Seleccione lrco\ FXG\ Welcome_ Summit_ 10 (archivo FXG) y haga clic **en Generar** &gt; **Publicación de plantillas**.</p>

   ![](assets/wp_fxg_edit.png)

1. En el panel Capas de la pantalla Publicación de plantilla, seleccione la capa que contenga los elementos que desea parametrizar.

   >[!NOTE]
   >
   >Haga clic en el icono del ojo para activarlo o desactivarlo y asegurarse de que selecciona el objeto correcto.

1. En el panel Propiedades, haga clic en un parámetro de la columna Nombre (para parametrizar texto) o Parámetro (para parametrizar objetos).

   **Clic en texto** en el campo de texto (desplácese hasta la parte inferior de la lista Propiedades para encontrarla). Se abrirá el cuadro de diálogo Parámetros. Select the text that you want to parameterize and click **Add**. Puede crear varios parámetros desde la misma propiedad de texto si selecciona diferentes partes del texto y añade parámetros para cada una de ellas. To change the name of the parameter, click it, enter a new name, and click **Close**.

   **Objetos** Haga clic en un cuadro de la columna Parámetro. Se abrirá el cuadro de diálogo Editar parámetro. Enter a name and click **OK**.

   Para personalizar múltiples atributos a la vez con el mismo valor, use el mismo nombre de parámetro para cada atributo. For example, if your template has a rectangle and a star, you can type `newcolor` as the Parameter name for the SolidColor color attribute of each. Whenever you change the `newcolor` value, both the rectangle and the star change to the new color.

1. Especifique un valor predeterminado para el atributo del campo Valor o Datos. Establezca todas las propiedades del objeto seleccionado para especificar la apariencia exacta que desea.
1. (Opcional) Repita los pasos del 3 al 5 para todos los objetos o capas que desee parametrizar.
1. Haga clic en **Guardar** o **Guardar como**.
1. Click **Preview** to open the FXG Preview window and see the parameters you created with their default values.

## Procedimiento para mostrar u ocultar objetos o capas de plantillas FXG {#show-or-hide-an-object-or-layer-in-the-fxg-template}

Los objetos y capas ocultos no son visibles en la vista previa o la salida, pero no se eliminan del archivo. Usted puede hacerlos visibles de nuevo si lo desea. La visibilidad es un atributo que puede hacer variable. Al activar o desactivar el icono de ojo, se establece el valor predeterminado de visibilidad de ese objeto o capa.

1. En el panel Objetos, haga clic en el icono de ojo que aparezca junto a un nombre de objeto o capa para ocultarlo en el archivo.
1. Haga clic de nuevo para que el objeto vuelva a estar visible.

## Creación de versiones diferentes de una plantilla {#create-different-versions-of-a-template}

Es posible editar los atributos para crear varias versiones de las plantillas destinadas a usos distintos.

En la pantalla Publicación de plantilla, haga clic en Guardar como para guardar el archivo como una plantilla FXG nueva sin sobrescribir la plantilla FXG original.

## Uso de texto con trazos {#using-stroked-text}

El texto con trazos es un ejemplo de cómo se pueden parametrizar atributos. Dynamic Media Classic admite estas funciones de texto con trazos:

* Anchura del trazo
* Patrón de trazo discontinuo
* Diferentes estilos de unión
* Diferentes estilos de extremo final
* Sobreimpresión del trazo
* Administración independiente de color del trazo, con compatibilidad con tintas planas

En esta tabla se describen los atributos que admiten texto con trazos.

| Atributo | Descripción |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | Especifica si se permite el relleno del texto. El valor predeterminado es true. |
| s7:stroke `<Boolean>` (S7FXG Only) | Especifica si se permite el trazo en el texto. El valor predeterminado es false. |
| s7:weight `<number>` (S7FXG Only) | Especifica el grosor del trazo del texto en puntos. El valor predeterminado es 1 punto. |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | Especifica el tipo de unión del trazo. El valor predeterminado es round. |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | Especifica el tipo de extremo del trazo. El valor predeterminado es round. |
| s7:miterLimit `<number>` (S7FXG Only) | Especifica el límite del ángulo cuando la unión del trazo es una unión en ángulo. El valor predeterminado es 4. |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | Especifica si se permite la sobreimpresión del trazo. El valor predeterminado es false. |
| s7:strokeColorName (solo S7FXG) | Es igual que s7:colorName con la salvedad de que define el nombre del color del trazo. |
| s7:strokeColorValue (solo S7FXG) | Es igual que s7:colorValue con la salvedad de que define el valor del color que se utiliza para el trazo. |
| s7:strokeColorspace (solo S7FXG) | Es igual que s7:colorspace con la salvedad de que define el espacio de color del trazo. |
| flm:dashPattern `<array>` (S7FXG Only) | De manera predeterminada, no hay ningún patrón de guiones y huecos. Este atributo define el patrón de guiones y huecos del trazo. El primer valor es el guión del trazo. El segundo es el hueco que hay entre los guiones. La matriz se puede ampliar del mismo modo especificando varios valores alternativos de guión y hueco. |

## Uso de texto deformado {#using-warped-text}

El texto deformado permite modificar el aspecto del texto con efectos como onda, bandera, estirar, etc.

El texto deformado es compatible con los objetos de texto enriquecido. El texto puede ser horizontal o vertical, y puede ser texto de punto, de área y de ruta de texto. Para poder aplicar la deformación debe haberse seleccionado previamente todo el objeto de texto.

En Adobe Illustrator se puede crear texto deformado.

Al deformar texto, se pueden definir los siguientes atributos:

* Estilo
* Dirección
* Curva
* Distorsión horizontal
* Distorsión vertical

Cada atributo contiene un conjunto de valores.

| Atributo | Valores | Predeterminado |
|--- |--- |--- |
| Estilos 7: Warpstyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | ninguno |
| Direcciones 7: Warpdirection | horizontalvertical | horizontal |
| Finaliza 7: Warpbend | -1 a 1 | 0,5 |
| Distorsión horizontal 7: Warphorizontaldistortion | -1 a 1 | 0 |
| Distorsión vertical de distorsión vertical 7: Warpverticaldistortion | -1 a 1 | 0 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

Para obtener más información acerca de cómo crear y usar texto deformado, consulte la documentación de Adobe Illustrator.

>[!MORELIKETHIS]
>
>* [Creación de la plantilla inicial en Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Carga de archivos para publicación de plantillas](upload-files-template-publishing.md#upload_files_for_template-publishing)

