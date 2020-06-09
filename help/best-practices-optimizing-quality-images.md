---
title: Prácticas recomendadas para optimizar la calidad de las imágenes
seo-title: Prácticas recomendadas para optimizar la calidad de las imágenes
description: nulo
seo-description: Conozca las prácticas recomendadas para optimizar la calidad de las imágenes.
uuid: 102e83fe-ee2a-443b-ba92-6ad5cc3daef0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 8164466e-2520-482a-88ec-6191fdc77ea3
translation-type: tm+mt
source-git-commit: 707afa544ffcea8885631c9fca8b432bc7af6860
workflow-type: tm+mt
source-wordcount: '1527'
ht-degree: 60%

---


# Prácticas recomendadas para optimizar la calidad de las imágenes{#best-practices-for-optimizing-the-quality-of-your-images}

La optimización de la calidad de las imágenes puede ser un proceso lento, ya que intervienen muchos factores para conseguir resultados aceptables. El resultado es en parte subjetivo porque distintas personas perciben la calidad de las imágenes de forma distinta. La clave es la experimentación estructurada.

Dynamic Media Classic incluye más de 100 comandos de servicio de imágenes para ajustar y optimizar imágenes y procesar resultados. Las directrices siguientes pueden ayudarle a agilizar el proceso y a obtener buenos resultados con rapidez utilizando ciertos comandos esenciales y prácticas recomendadas.

Consulte también Imágenes [inteligentes](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

## Prácticas recomendadas para el formato de imágenes (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Los formatos JPG o PNG son las mejores opciones para distribuir imágenes con una buena calidad y con un tamaño y peso manejables.
* Si no se proporciona ningún comando de formato en la dirección URL, el servicio de imágenes de Dynamic Media tiene el valor predeterminado JPG para envío.
* JPG comprime en una proporción de 10:1 y generalmente ofrece tamaños de archivo de imagen más pequeños. PNG se comprime a una proporción de aproximadamente 2:1, excepto en algunos casos, como cuando las imágenes contienen un fondo vacío. Normalmente, los tamaños de archivo PNG son mayores que los archivos JPG.
* JPG utiliza compresión con pérdidas, lo que significa que elementos de la imagen (píxeles) se eliminan durante la compresión. PNG utiliza la compresión sin pérdidas.
* JPG a menudo comprime imágenes fotográficas con una mejor fidelidad que las imágenes sintéticas con contraste y bordes y nítidos.
* Si las imágenes contienen transparencias, utilice PNG porque JPG no admite transparencias.

As a best practice for image format, start with the most common setting `&fmt=JPG`.

## Prácticas recomendadas para el tamaño de imagen {#best-practices-for-image-size}

La reducción dinámica del tamaño de la imagen es una de las tareas más comunes que realiza el servicio de imágenes de Dynamic Media. Requiere especificar el tamaño y, opcionalmente, el modo de disminución de resolución que se utiliza para reducir el tamaño de la imagen.

* For image sizing, the best and most straightforward approach is to use `&wid=<value>` and `&hei=<value>` or just `&hei=<value>`. Estos parámetros establecen la anchura de la imagen automáticamente según la proporción de aspecto.
* `&resMode=<value>` controla el algoritmo utilizado para la disminución de resolución. Inicio con `&resMode=sharp2`. Este valor proporciona la mejor calidad de imagen. While using the downsampling value `=bilin` is faster, it often results in the aliasing of artifacts.

Como práctica recomendada para cambiar el tamaño, el uso `&wid=<value>&hei=<value>&resMode=sharp2` o `&hei=<value>&resMode=sharp2`

## Prácticas recomendadas para el enfoque de imágenes {#best-practices-for-image-sharpening}

El enfoque de imágenes es el aspecto más complejo del control de imágenes en su sitio Web y en el que se producen muchos errores. Tómese el tiempo para obtener más información sobre el funcionamiento del enfoque y la máscara de enfoque en Dynamic Media Classic haciendo referencia a los siguientes recursos útiles:

Documento técnico de prácticas recomendadas [Enfoque de imágenes en Adobe Scene7 Publishing System y en el servidor](/help/assets/s7_sharpening_images.pdf)de imágenes.

Consulte también [Enfoque de imágenes con máscara](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html)de enfoque.

Con Dynamic Media Classic, puede enfocar imágenes durante la ingesta, en el envío o en ambos. En la mayoría de los casos, no obstante, deberá enfocar las imágenes con un método u otro, pero no ambos. Normalmente, el enfoque de imágenes durante la distribución, en una URL, ofrece los mejores resultados.

Puede utilizar dos métodos de enfoque de imágenes:

* Simple sharpening ( `&op_sharpen`) - Similar to the sharpen filter used in Photoshop, simple sharpening applies basic sharpening to the final view of the image following dynamic resizing. Sin embargo, este método no puede configurarse. The best practice is to not use `&op_sharpen` unless required.
* Unsharp masking ( `&op_USM`) - Unsharp masking is an industry standard sharpening filter. La práctica recomendada es enfocar imágenes con la máscara de enfoque siguiendo las directrices siguientes. Las máscaras de enfoque permiten controlar los tres parámetros siguientes:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (cantidad= (0-5, intensidad del efecto).
      * `radius` (radio) (0-250, anchura de las “líneas de enfoque” dibujadas alrededor del objeto enfocado, medidas en píxeles.)

         Keep in mind that the parameters `radius` and `amount` work against each other. La reducción `radius` se puede compensar aumentando `amount`. `Radius` permite un control más preciso, ya que un valor más bajo enfoca solo los píxeles de borde, mientras que un valor más alto enfoca una banda más ancha de píxeles.

      * `threshold` (0-255, sensibilidad del efecto).

         Este parámetro determina la diferencia entre los píxeles enfocados y el área circundante antes de que se consideren píxeles de borde y el filtro los enfoque. El umbral ayuda a evitar el exceso de áreas de enfoque con colores similares, como los tonos de piel. Por ejemplo, un valor de umbral de 12 ignora las ligeras variaciones en el brillo del tono de la piel para evitar agregar “ruido”, mientras que al mismo tiempo agrega contraste al borde de las áreas de alto contraste, como cuando las pestañas tocan la piel.
      Para obtener más información sobre la configuración de estos tres parámetros, incluidas las prácticas recomendadas de uso del filtro, consulte los siguientes recursos:

      Tema de ayuda de Dynamic Media Classic sobre el [enfoque de imágenes](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html).

      Documento técnico de prácticas recomendadas [Enfoque de imágenes en Adobe Scene7 Publishing System y en el servidor](/help/assets/s7_sharpening_images.pdf)de imágenes.

   * Dynamic Media Classic también le permite controlar un cuarto parámetro: monocromo ( `0,1`). Este parámetro determina si la máscara de enfoque se aplica a cada componente de color por separado mediante el valor `0` o al brillo o la intensidad de la imagen con el valor `1`.


La práctica recomendada es comenzar con el parámetro de radio de máscara de enfoque. Puede comenzar con las configuraciones de radio siguientes:

* Sitio web: 0,2-0,3 píxeles
* Impresión fotográfica (250-300 ppp): 0,3-0,5 píxeles
* Impresión en offset (266-300 ppp): 0,7-1,0 píxeles
* Impresión de lienzo (150 ppp): 1,5-2,0 píxeles

Aumente gradualmente la cantidad de 1,75 a 4. Si el enfoque aún no aparece como desea, aumente el radio en un decimal y ejecute de nuevo la cantidad de 1,75 a 4. Repita el proceso tantas veces como sea necesario.

Deje la configuración del parámetro monocromo en 0.

## Prácticas recomendadas para la compresión de JPEG (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Este parámetro controla la calidad de codificación de JPG. Un valor más alto significa una mejor calidad de imagen pero un tamaño mayor de archivo; por lo contrario, un valor inferior significa una imagen de menor calidad pero un tamaño de archivo más pequeño. El rango de este parámetro es 0-100.
* Para optimizar la calidad, no defina el valor del parámetro a 100. La diferencia entre un ajuste de 90 o 95 y 100 es casi imperceptible, pero 100 aumenta innecesariamente el tamaño de archivo de la imagen. Therefore, to optimize for quality but avoid image files becoming too large, set the `qlt=` value to 90 or 95.
* To optimize for a small image file size but keep image quality at an acceptable level, set the `qlt=` value to 80. Los valores por debajo de 70 a 75 degradan considerablemente la calidad de imagen.
* As a best practice, to stay in the middle, set the `qlt=` value to 85 to stay in the middle.
* Utilización del indicador de cromatismo en `qlt=`

   * The `qlt=` parameter has a second setting that lets you turn on RGB chromaticity downsampling using the normal value `,0` (default), or turn it off using the value `,1`.
   * Para simplificar, empiece con la disminución de resolución de cromaticidad RGB desactivada ( `,1`). Este ajuste normalmente ofrece una mejor calidad de imagen, especialmente en imágenes sintéticas con muchos bordes nítidos y contraste.

La práctica recomendada de compresión JPG es `&qlt=85,0`.

## Prácticas recomendadas para el tamaño JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` es un parámetro muy útil si desea asegurarse de que una imagen no supere un determinado tamaño para la distribución en dispositivos con memoria limitada.

* Este parámetro se establece en kilobytes ( `jpegSize=<size_in_kilobytes>`). Define el tamaño máximo permitido para la distribución de imágenes.
* `&jpegSize=` interactúa con el parámetro de compresión JPG `&qlt=`. If the JPG response with the specified JPG compression parameter ( `&qlt=`) does not exceed the `jpegSize` value, the image is returned with `&qlt=` as defined. Otherwise, `&qlt=` is gradually decreased until the image fits in the maximum allowed size, or until the system determines it cannot fit and returns an error.

As a best practice, set `&jpegSize=` and add the parameter `&qlt=` if you are delivering JPG images to devices with limited memory.

## Resumen de prácticas recomendadas {#best-practices-summary}

Como práctica recomendada, para lograr una alta calidad de imagen y un tamaño de archivo pequeño, comience con esta combinación de parámetros:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Esta combinación da resultados excelentes en la mayoría de circunstancias.

Si necesita optimizar la imagen aún más, ajuste gradualmente los parámetros de enfoque (la máscara de enfoque) comenzando con un radio definido en 0,2 o 0,3. A continuación, aumente gradualmente la cantidad desde 1,75 a 4 (equivalente al 400% en Photoshop). Compruebe si se ha obtenido el resultado deseado.

Si los resultados de enfoque aún no son satisfactorios, aumente el radio en incrementos decimales. Tras cada incremento decimal, vuelva a ajustar la cantidad en 1,75 y auméntela gradualmente a 4. Repita este proceso hasta lograr el resultado deseado. Aunque los valores anteriores son un método validado por los estudios creativos, recuerde que puede empezar con otros valores y seguir otras estrategias. Si los resultados son satisfactorios o no es una cuestión subjetiva y, por lo tanto, la clave es la experimentación estructurada.

Al experimentar, también puede encontrar las sugerencias generales siguientes útiles para optimizar el flujo de trabajo:

* Pruebe distintos parámetros en tiempo real, ya sea directamente en una URL de Dynamic Media Classic o mediante la función de ajuste de imagen de Scene7 Publishing System, que proporciona previsualizaciones en tiempo real para las operaciones de ajuste.
* Como práctica recomendada, recuerde que puede agrupar comandos de servicio de imágenes de Dynamic Media en un ajuste preestablecido de imagen. An image preset is basically URL command macros with custom preset names such as `$thumb_low$` and `&product_high$`. El nombre del ajuste preestablecido personalizado en una ruta URL invoca estos ajustes preestablecidos. Esta funcionalidad le ayudará a administrar comandos y ajustes de calidad para diferentes modelos de uso de imágenes en su sitio web y reducirá la longitud total de la URL.
* Dynamic Media Classic también ofrece formas más avanzadas de ajustar la calidad de imagen, como la aplicación de imágenes de enfoque durante la ingesta. En el caso de usos avanzados, en los que es necesaria esta opción para perfeccionar y optimizar aún más los resultados del procesamiento, Adobe Professional Service puede ayudarle con prácticas recomendadas y sugerencias personalizadas.

