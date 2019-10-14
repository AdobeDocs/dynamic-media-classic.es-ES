---
title: Creación de documentos PDF
seo-title: Creación de documentos PDF
description: nulo
seo-description: Obtenga información sobre cómo crear un documento PDF mediante el proceso de impresión virtual en Dynamic Media Classic.
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: referencia
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Creación de documentos PDF {#creating-a-pdf-document}

El paso final en el proceso de impresión virtual consiste en generar el PDF personalizado. Después de que los usuarios finales personalicen la plantilla con la aplicación web que ha creado, crean un documento PDF definitivo. Por lo general, este PDF definitivo se envía a un proveedor de servicios de impresión para conseguir una impresión profesional. Para asegurarse de que el PDF definitivo se imprime como debe, los desarrolladores usan el archivo de opciones del trabajo correcto y configuran las fuentes, las marcas de impresión y los colores correctamente.

## Configuración de ajustes preestablecidos de PDF {#setting-up-pdf-presets}

Especifique el nivel de compatibilidad con PDF y la configuración de la impresora creando y cargando un archivo de opciones de trabajo de PDF en el servidor de Dynamic Media Classic. Por ejemplo, seleccione una salida PDF compatible con PDF/X-4 (se recomienda para flujos de trabajo de publicación de impresiones PDF). El archivo de opciones de trabajos se puede crear en un software de creación (como Adobe Illustrator) o en Acrobat. Consulte siempre al encargado de la impresión, que puede indicarle la configuración de opciones adecuada para los trabajos de impresión.

Para obtener más información sobre la creación de archivos de opciones de trabajos y del archivo de opciones de trabajo en Acrobat, consulte la ayuda de Adobe Acrobat.

Para crear un archivo de opciones de trabajos en Illustrator:

1. Seleccione Edición &gt; Ajustes preestablecidos de Adobe PDF.
1. En el cuadro de diálogo, seleccione el ajuste preestablecido que desee utilizar.

   Dynamic Media Classic admite las siguientes opciones de trabajo:

   | Opción de trabajo | Descripción |
   |--- |--- |
   | General | <ul><li>Compatibilidad </li><li>Compresión de nivel de objetos</li><li>Incrustar miniaturas</li><li>Optimizar para vista rápida en Web</li></ul> |
   | Imágenes | <ul><li>Disminuir resolución</li><li>Resolución</li><li>Umbral</li><li>Compresión para color, gris y mono</li></ul> |
   | Fuentes | <ul><li>Incrustar todas las fuentes (las fuentes se incrustan de manera predeterminada)</li><li>Incrustar fuentes OpenType</li><li>Crear subconjunto de fuentes incrustadas cuando el porcentaje de caracteres utilizado sea menor que</li><li>Lista Incrustar siempre</li><li>Lista No incrustar nunca</li></ul> |
   | Color | <ul><li>Estrategia de color (el etiquetado exclusivo de imágenes se interpreta como etiquetar todo)</li><li>Calidad de representación del documento</li><li>Solo se admiten los espacios de trabajo siguientes en 4.2.5. 4.3 permitirá utilizar cualquier perfil proporcionado por el cliente que se haya cargado en IPS</li><li>Como solución alternativa, puede especificar el espacio de color de destino para el diseño que se va a convertir utilizando los perfiles de color predeterminados de la empresa</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Flat XYZ (XYZ plano)</li><li>Linear ROMM-RGB (ROMM-RGB lineal)</li><li>ROMM-RGB</li><li>sYCC 8-bit (sYCC de 8 bits)</li><li>e-sYCC 8-bit (e-sYCC de 8 bits)</li></ul> |
   | Gris | <ul><li>Gris Gamma 1.8</li><li>Gris Gamma 2.2</li><li>Dot Gain 10%</li><li>Dot Gain 15%</li><li>Dot Gain 20%</li><li>Dot Gain 25%</li><li>Dot Gain 30%</li><li>sGray</li></ul> |
   | Mantener valores CMYK para espacios de color CMYK calibrados |  |
   | Avanzado | Conservar comentarios OPI (siempre activado) |
   | Estándares | Estándar de compatibilidad |

   >[!NOTE]
   >
   >Dynamic Media Classic ignora la configuración de marca de impresora en el archivo de opciones de trabajo. En su lugar, las marcas de impresora se configuran mediante el uso de comandos URL de Dynamic Media Classic.

1. Haga clic en Exportar y, a continuación, especifique un nombre y una ubicación y haga clic en Guardar.
1. Cargue el archivo de opciones de trabajos como recurso en Scene7 Publishing System.

   Úselo con la plantilla publicada haciendo referencia a él en la URL. Por ejemplo:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Preparación de PDF para la impresión {#preparing-the-pdf-for-print}

Antes de finalizar el PDF para la impresión, no olvide seguir las instrucciones de esta sección.

**Imágenes**

Asegúrese de que todas las imágenes del trabajo de publicación se han cargado en el servidor de Dynamic Media Classic y se han publicado.

**Fuentes**

Asegúrese de que todas las fuentes del trabajo de publicación se han cargado en el servidor de Dynamic Media Classic y se han publicado. Cerciórese de que tiene los derechos legales adecuados para alojar las fuentes si desea permitir que los usuarios finales las cambien.

**Resolución de imagen (píxeles por pulgada)**

El servidor de Dynamic Media Classic conserva la resolución de las imágenes de mapa de bits en archivos PDF generados listos para imprimir. Si es necesario, Dynamic Media Classic aumenta la resolución de la imagen. Para conseguir resultados óptimos, deje el valor predeterminado de resolución (por lo general, 72 ppp) para la vista previa en Web. La resolución predeterminada de todas las imágenes de la empresa se define en la sección Resolución de impresión predeterminada de la ventana Configuración de publicación/Servidor de imágenes. Si la resolución es alta (por ejemplo, 300 ppp), el resultado puede ser un tiempo de procesamiento más prolongado, por lo que solo se debe aplicar a PDF listos para imprimir. Use el comando imageRes= de la URL para anular manualmente la resolución predeterminada de los trabajos en PDF.

**Gestión de color**

El documento y las imágenes pueden utilizar la escala de grises, CMYK, tintas planas con nombre, RGB o modelos de color Lab. Cada modelo puede estar calibrado o no empleando un perfil de color ICC. Para obtener unos resultados óptimos, incruste el perfil en el PDF generado listo para la impresión. El servidor de Dynamic Media Classic lo hace de forma predeterminada. Asegúrese de que todos los perfiles de color necesarios se han cargado en la plataforma de Dynamic Media Classic. Es preferible que las opciones de administración de color definidas en la aplicación de diseño coincidan con las definidas en el servidor de Dynamic Media Classic:

* **Configuración de la gestión del color en la aplicación de diseño**: en la configuración del color de la aplicación de creación (por ejemplo, Adobe Illustrator), especifique los perfiles de color RGB y CMYK en la sección de los espacios de trabajo.

* **** Configuración de la administración de color de Dynamic Media Classic: Normalmente, la configuración de administración de color de la aplicación de diseño debe coincidir con los perfiles de color predeterminados del servidor de Dynamic Media Classic. Esta configuración se encuentra en la ventana Ajustes de publicación/Servidor de imágenes.

## Visualización de marcas de impresora {#displaying-printer-marks}

Puede crear un archivo PDF para cualquiera de estos casos:

* Documentos terminados
* Documentos intermedios como películas o placas que se pueden enviar a una impresora para producción

Los documentos intermedios pueden incluir contenido de producción adicional como márgenes de sangrado, marcas de impresora, etc. Este contenido suele aparecer fuera de los límites de la página terminada.

Todas las marcas disponibles en la pantalla "Agregar marcas de impresora" en Acrobat son compatibles. Las marcas de impresora se controlan con el parámetro `printerMark`. La sintaxis es la siguiente `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

Al preparar un documento para su impresión, las marcas de impresora pueden ayudar al servicio de impresión a alinear las películas de separación para generar pruebas, establecer la calibración y la densidad de tinta correctas de la película, recortar la película con el tamaño adecuado, etc. Las marcas de impresora indican los límites de los cuadros del documento, por ejemplo, de los rectángulos de corte y sangrado. El contenido relacionado con la producción puede incluir lo siguiente:

* **Cuadro** MedioLímites del medio físico en el que se imprimirá la página. Se puede descartar el contenido que está fuera del rectángulo sin que se modifique el archivo.

* **Cuadro** Sangrado La región a la que se recorta el contenido de la página cuando se genera un resultado en un entorno de producción. Este rectángulo puede incluir áreas necesarias por las limitaciones físicas de los equipos de corte, plegado o recorte. El valor predeterminado es el cuadro de recorte de la página.

* **Cuadro** Recortar Las dimensiones deseadas de la página final después del recorte. Este rectángulo puede ser más pequeño que el rectángulo del soporte a fin de dejar sitio para contenido relacionado con la producción, por ejemplo, instrucciones de impresión, marcas de corte o barras de colores. El valor predeterminado es el cuadro de recorte de la página.

* **Cuadro** de arte El alcance del contenido significativo de la página (incluido el posible espacio en blanco) según lo previsto por el creador de la página. El valor predeterminado es el cuadro de recorte de la página.

Los modificadores de la tabla siguiente permiten replicar las marcas de impresora disponibles en Adobe Illustrator, InDesign y Acrobat:

| Modificador y valores | Descripción |
|--- |--- |
| bleedMargin = top, left, bottom, right | Se especifica en Acrobat con la opción Definir cuadros de página. Seleccione BleedBox y, a continuación, especifique los márgenes con la opción Controles de margen.<br><br>Los valores representan la distancia a los bordes superior, izquierdo, inferior y derecho desde los bordes originales del diseño (esto es, el rectángulo del soporte) hacia adentro. Los valores (0-1000) están en puntos.<br><br>Nueva altura = altura original - (superior + inferior)<br><br>Nueva anchura= anchura original - (izquierda + derecha) |
| mediaMargin = top, left, bottom, right | Se especifica en Acrobat con la opción Definir cuadros de página. Modifique el tamaño de página personalizado en la opción Cambiar tamaño de página.<br><br>Los valores representan la distancia a los bordes superior, izquierdo, inferior y derecho desde los bordes originales del diseño (esto es, el rectángulo del soporte) hacia afuera. Los valores (0-1000) están en puntos.<br><br>Nueva altura = superior + inferior +<br><br>altura originalNueva anchura = superior + inferior +<br><br>anchura originalLos nuevos valores de altura y nueva anchura determinan el nuevo tamaño de página del PDF generado.<br><br>Una vez definido un nuevo MediaBox, todos los cálculos de los márgenes de corte y sangrado deben tener en cuenta el nuevo MediaBox como borde del diseño. |
| trimMargin = top, left, bottom, right | Se especifica en Acrobat con la opción Definir cuadros de página. Seleccione TrimBox y, a continuación, especifique los márgenes con la opción Controles de margen.<br><br>Los valores representan la distancia a los bordes superior, izquierdo, inferior y derecho desde los bordes originales del diseño (esto es, el rectángulo del soporte) hacia adentro. Los valores (0-1000) están en puntos.<br><br>Nueva altura = altura original - (superior + inferior)<br><br>Nueva anchura = anchura original - (izquierda + derecha) |
| printerMark = trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed | Los valores son los siguientes:<br><br>trim marks = 0,1 (el valor predeterminado es 0)<br><br>bleed marks = 0,1 (el valor predeterminado es 0)<br><br>registration marks = 0,1 (el valor predeterminado es 0)<br><br>color bars = 0,1 (el valor predeterminado es 0)<br><br>page information = 0,1 (el valor predeterminado es 0)<br><br>style = Default, InDesignJ1, InDesignJ2, Illustrator, illustrator, illustratorJ, illustrator QuarkXPress (el valor predeterminado es Predeterminado)<br><br>line weight= 0.125-0.2, ambos valores inclusive (el valor predeterminado es 0.25)<br><br>layer embed = 0, 1, con 1 creando una nueva capa que contenga todas las marcas de impresora (el valor predeterminado es 1)<br><br>Según el estilo que se utilice, las marcas y las barras de color aparecen diferentes y coinciden con los estilos correspondientes utilizados por Acrobat. |

Tenga en cuenta lo siguiente sobre las marcas de impresora:

* Especifique los márgenes de sangrado, de corte y de medios mediante llamadas mediante URL al especificar las marcas de impresora. Si se especifican las marcas de impresora sin especificar estos márgenes, las marcas aparecen fuera de la región visible del PDF generado. Además, las marcas de corte y sangrado se superponen.
* Si se especifican los mismos valores para los márgenes de corte y sangrado, las marcas de corte y sangrado se superponen en caso de que ambos indicadores estén definidos en 1 en `&printerMark`.
* Si se especifican formatos fmt=swf/image mediante llamadas mediante URL, se obtiene una salida sin ningún margen ni ninguna marca de impresora porque esta función es específica de salidas en PDF.
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. No obstante, para definir el enésimo elemento en ON, es preciso especificar todos los parámetros (n-1) mediante URL.
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* En los PDF de varias páginas, los márgenes y las marcas de impresora se aplican a todas las páginas (en Acrobat, los usuarios pueden seleccionar intervalos de páginas para los márgenes o las marcas de impresora).
* La salida de un PDF en el que se han activado los márgenes o las marcas de impresora coincide exactamente con Acrobat X a menos que se especifique lo contrario.

Si desea crear un archivo PDF compatible con PDF/X-4 con el modificador &amp;joboption en la URL, debe tener en cuenta las limitaciones relacionadas con las marcas de impresora especificadas en el PDF ISO_15930-7-2008.pdf:

* Cada uno de los objetos de página de un archivo PDF incluye un MediaBox. Cada uno de los objetos de página de un archivo conforme con PDF/X-4 debe incluir un TrimBox o un ArtBox, pero no ambos. Se puede incluir un MediaBox por herencia.
* Si hay un BleedBox, el ArtBox o el TrimBox no se debe extender más allá de los límites del BleedBox. Si hay un CropBox, ni el ArtBox, ni el TrimBox ni el BleedBox se deben extender más allá de los límites del CropBox.
* Ni el ArtBox, ni el TrimBox, ni el CropBox ni el BleedBox se deben extender más allá de los límites del MediaBox.
* Algunas prácticas del sector exigen el uso del BleedBox. Se deben seguir las prácticas comerciales apropiadas.
* Se recomienda utilizar el TrimBox en lugar del ArtBox.
* Todas las anotaciones que no sean TrapNet y PrinterMark deben tener un valor para Rect que esté completamente fuera del BleedBox (o del TrimBox o del ArtBox si no hay ningún BleedBox). Todas las anotaciones PrinterMark deben tener un valor para Rect que esté completamente fuera del TrimBox o del ArtBox. Es posible que los lectores compatibles con PDF/X-4 ignoren por completo las anotaciones salvo las anotaciones TrapNet de PDF.
* Rect se considera como completamente fuera de un cuadro delimitador si todas sus coordenadas se encuentran fuera del cuadro delimitador o en su borde y la intersección de los dos rectángulos es cero.
* Si el diccionario ViewerPreferences contiene las claves ViewArea, ViewClip, PrintArea o PrintClip, cada una de las que haya debe tener el valor MediaBox o, si hay un BleedBox en todos los objetos de página del archivo, el valor BleedBox.

