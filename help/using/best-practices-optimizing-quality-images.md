---
title: Recomendaciones para optimizar la calidad de las imágenes
description: Conozca las prácticas recomendadas para optimizar la calidad de las imágenes.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:42.316Z'
TQID: 'https://experienceleague.adobe.com/kw-spdqv6ArVEWk8ID4mnQjYrS25RZntKOJ7-tESasY'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: bcc5edb5-84c3-4940-9f84-ed88b6c16274id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: b29d7cc6962ca9e7724bb43987947b08af5cd4d7
workflow-type: tm+mt
source-wordcount: 1591
ht-degree: 27%

---

# Prácticas recomendadas para optimizar la calidad de las imágenes{#best-practices-for-optimizing-the-quality-of-your-images}

La optimización de la calidad de la imagen puede llevar mucho tiempo. Muchos factores contribuyen a obtener resultados aceptables. El resultado es en parte subjetivo porque distintas personas perciben la calidad de las imágenes de forma distinta. La experimentación estructurada es esencial.

Adobe Dynamic Media Classic incluye más de 100 comandos de servidor de imágenes para ajustar y optimizar imágenes y procesar resultados. Las directrices siguientes pueden ayudarle a agilizar el proceso y a obtener buenos resultados con rapidez utilizando ciertos comandos esenciales y prácticas recomendadas.

Consulte también [Imágenes inteligentes](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Pruebe y descubra las ventajas de los modificadores de imagen de Dynamic Media y de las imágenes inteligentes con Dynamic Media [_Snapshot_](https://snapshot.scene7.com/).
>
> Snapshot es una herramienta de demostración visual diseñada para ilustrar las capacidades de Dynamic Media para la entrega de imágenes optimizadas y dinámicas. Experimente con imágenes de prueba o URL de Dynamic Media para poder observar visualmente la salida de varios modificadores de imagen de Dynamic Media y optimizaciones de imágenes inteligentes para lo siguiente:
>
>* Tamaño de archivo (con envío WebP y AVIF)
>* Ancho de banda de red
>* DPR (proporción de píxeles del dispositivo)
>
>Para aprender a usar Snapshot, vea el [vídeo de entrenamiento de Snapshot](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 minutos y 17 segundos).


## Prácticas recomendadas para el formato de imágenes (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Los formatos JPG o PNG son las mejores opciones para distribuir imágenes con una buena calidad y con un tamaño y peso manejables.
* Si no se proporciona ningún comando de formato en la dirección URL, el servicio de imágenes de Dynamic Media toma el valor predeterminado de JPG para la entrega.
* JPG comprime en una proporción de 10:1 y generalmente ofrece tamaños de archivo de imagen más pequeños. PNG comprime en una proporción de aproximadamente 2:1, excepto cuando las imágenes contienen fondos transparentes. Normalmente, el tamaño de los archivos PNG es mayor que el de los archivos JPG.
* JPG utiliza compresión con pérdidas, lo que significa que elementos de la imagen (píxeles) se eliminan durante la compresión. PNG utiliza la compresión sin pérdidas.
* JPG a menudo comprime imágenes fotográficas con una mejor fidelidad que las imágenes sintéticas con contraste y bordes y nítidos.
* Si las imágenes contienen transparencias, utilice PNG porque JPG no admite transparencias.

Como práctica recomendada para el formato de imagen, comience con la configuración más común `&fmt=JPG`.

## Prácticas recomendadas para el tamaño de imagen {#best-practices-for-image-size}

La reducción dinámica del tamaño de la imagen es una de las tareas más comunes que realiza el servicio de imágenes de Dynamic Media. Requiere especificar el tamaño y, opcionalmente, el modo de disminución de resolución que se utiliza para reducir el tamaño de la imagen.

* Para cambiar el tamaño de la imagen, use `&wid=<value>` y `&hei=<value>`. Estos parámetros establecen automáticamente el ancho de la imagen de acuerdo con la relación de aspecto.
* `&resMode=<value>`: controla el algoritmo utilizado para la disminución de resolución. Comience por `&resMode=sharp2`. Este valor proporciona la mejor calidad de imagen. Aunque el uso del valor de disminución de resolución `bilin` es más rápido, a menudo produce defectos de solapamiento.

Como práctica recomendada para el tamaño de la imagen, use `&wid=<value>&hei=<value>&resMode=sharp2`. `&hei=<value>&resMode=sharp2`

## Prácticas recomendadas para el enfoque de imágenes {#best-practices-for-image-sharpening}

El enfoque de imágenes es el aspecto más complejo del control de imágenes en el sitio web y en el que se producen muchos errores. Para obtener más información sobre cómo funcionan el enfoque y la máscara de enfoque en Adobe Dynamic Media Classic, consulte los siguientes recursos útiles:

Prácticas recomendadas en el documento técnico de PDF denominado [Enfoque de imágenes en Adobe Dynamic Media Classic y en Image Server](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

En Adobe Dynamic Media Classic, puede enfocar las imágenes durante la ingesta, la entrega o ambas cosas. Sin embargo, normalmente las imágenes se enfocan con un método, pero no con ambos. El enfoque de imágenes en el envío a través de una dirección URL suele proporcionarle los mejores resultados.

Existen dos métodos de enfoque de imágenes que puede utilizar:

* Enfoque simple (`&op_sharpen`): de forma similar al filtro de enfoque utilizado en Adobe Photoshop, el enfoque simple aplica un enfoque básico a la vista final de la imagen tras el cambio de tamaño dinámico. Sin embargo, este método no puede configurarse. Se recomienda evitar el uso de `&op_sharpen` a menos que sea necesario.
* Máscara de enfoque (`&op_USM`): la máscara de enfoque es un filtro estándar del sector para el enfoque. La práctica recomendada es enfocar imágenes con la máscara de enfoque siguiendo las directrices siguientes. Las máscaras de enfoque permiten controlar los tres parámetros siguientes:

  * `&op_sharpen=amount,radius,threshold`

    * `amount` (0-5, intensidad del efecto).
    * `radius` (0-250, ancho de las &quot;líneas de enfoque&quot; dibujadas alrededor del objeto enfocado, medido en píxeles.)

      Tenga en cuenta que los parámetros `radius` y `amount` tienen una relación inversa. La reducción de `radius` se puede compensar aumentando `amount`. `Radius` permite un control más preciso ya que un valor más bajo enfoca únicamente los píxeles del borde, mientras que un valor más alto enfoca un intervalo más amplio de píxeles.

    * `threshold` (0-255, sensibilidad del efecto.)

      Este parámetro determina hasta qué punto deben ser distintos los píxeles enfocados respecto al área que los rodea para poder considerarse píxeles de borde y por tanto enfocarse. El umbral ayuda a evitar el exceso de áreas de enfoque con colores similares, como los tonos de piel. Por ejemplo, un valor de umbral de 12 ignora las ligeras variaciones en el brillo del tono de la piel para evitar añadir &quot;ruido&quot;, mientras que al mismo tiempo agrega contraste al borde de las áreas de alto contraste, como cuando las pestañas tocan la piel.

      Para obtener más información acerca de cómo establecer estos tres parámetros, incluidas las prácticas recomendadas para usar con el filtro, consulte [Enfoque de imágenes en Adobe Dynamic Media Classic y en Image Server](/help/using/assets/s7_sharpening_images.pdf).

    * Adobe Dynamic Media Classic también le permite controlar un cuarto parámetro: monocromo ( `0,1`). Este parámetro determina si se aplica la máscara de enfoque a cada componente de color por separado usando el valor `0` o al brillo/intensidad de la imagen usando el valor `1`.

La práctica recomendada es comenzar con el parámetro de radio de máscara de enfoque. Puede comenzar con las configuraciones de radio siguientes:

* Sitio web: 0,2-0,3 píxeles
* Impresión fotográfica (250-300 ppp): 0,3-0,5 píxeles
* Impresión en offset (266-300 ppp): 0,7-1,0 píxeles
* Impresión de lienzo (150 ppp): 1,5-2,0 píxeles

Aumente gradualmente la cantidad de 1,75 a 4. Si el enfoque sigue sin ser el resultado deseado, aumente el radio en un incremento decimal y vuelva a establecer la cantidad de 1,75 a 4. Repita el proceso tantas veces como sea necesario.

Deje la configuración del parámetro monocromo en 0.

## Prácticas recomendadas para la compresión de JPEG (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Este parámetro controla la calidad de codificación de JPG. Un valor más alto significa una mejor calidad de imagen pero un tamaño mayor de archivo; por lo contrario, un valor inferior significa una imagen de menor calidad pero un tamaño de archivo más pequeño. El rango de este parámetro es 0-100.
* Para optimizar la calidad, no defina el valor del parámetro a 100. La diferencia entre un ajuste de 90 o 95 y 100 es casi imperceptible. Sin embargo, 100 aumenta innecesariamente el tamaño del archivo de imagen. Por lo tanto, para optimizar la calidad pero evitar que los archivos de imagen se vuelvan demasiado grandes, establezca el valor de `qlt=` en 90 o 95.
* Para optimizar para un archivo de imagen pequeño pero mantener la calidad de la imagen en un nivel aceptable, establezca el valor `qlt=` en 80. Los valores por debajo de 70 a 75 dan como resultado una degradación significativa de la calidad de imagen.
* Para permanecer en el medio, establezca el valor `qlt=` en 85 como práctica recomendada.
* Usando el indicador de croma `qlt=`

  * El parámetro `qlt=` tiene una segunda configuración que le permite activar la disminución de resolución de cromaticidad de RGB con el valor normal `,0` (predeterminado), o desactivarla con el valor `,1`.
  * Comience con la disminución de resolución de cromaticidad de RGB desactivada ( `,1`). Este ajuste normalmente ofrece una mejor calidad de imagen, especialmente en imágenes sintéticas con muchos bordes nítidos y contraste.

Como práctica recomendada para la compresión de JPG, use `&qlt=85,0`.

## Prácticas recomendadas para el tamaño JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

El parámetro `jpegSize` es útil si desea garantizar que una imagen no supere un tamaño determinado. Este parámetro se utiliza para la entrega a dispositivos con memoria limitada.

* Este parámetro se establece en kilobytes ( `jpegSize=<size_in_kilobytes>`). Define el tamaño máximo permitido para la distribución de imágenes.
* `&jpegSize=` interactúa con el parámetro de compresión de JPG `&qlt=`. Si la respuesta de JPG con el parámetro de compresión de JPG especificado (`&qlt=`) no supera el valor `jpegSize`, la imagen se devuelve con `&qlt=` tal como se definió. De lo contrario, `&qlt=` se reducirá gradualmente hasta que la imagen se ajuste al tamaño máximo permitido. Como alternativa, el sistema devuelve un error si no cabe en la imagen.

Se recomienda configurar `&jpegSize=` e incluir el parámetro `&qlt=` cuando envíe imágenes de JPG a dispositivos con memoria limitada.

## Resumen de prácticas recomendadas {#best-practices-summary}

Como práctica recomendada, para lograr una alta calidad de imagen y un tamaño de archivo pequeño, comience con la siguiente combinación de parámetros:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Esta combinación de ajustes produce resultados excelentes en la mayoría de las circunstancias.

Si la imagen requiere una mayor optimización, ajuste gradualmente los parámetros de enfoque (máscara de enfoque) empezando por un radio establecido en 0,2 o 0,3. A continuación, aumente gradualmente la cantidad de 1,75 a un máximo de 4 (equivalente a 400% en [!DNL Adobe Photoshop]). Compruebe si se ha obtenido el resultado deseado.

Si los resultados de enfoque aún no son satisfactorios, aumente el radio en incrementos decimales. Para cada incremento decimal, restablezca la cantidad a 1,75 y aumente gradualmente a 4. Repita este proceso hasta lograr el resultado deseado. Aunque los valores anteriores son un enfoque que los estudios creativos han validado, tenga en cuenta que puede utilizar otros valores y seguir otros procedimientos. Si los resultados son satisfactorios o no es una cuestión subjetiva; por lo tanto, se requiere experimentación estructurada.

A medida que experimenta, las siguientes sugerencias generales son útiles para optimizar el flujo de trabajo:

* Pruebe diferentes parámetros en tiempo real, directamente en una dirección URL o usando [!DNL Adobe Dynamic Media Classic] herramientas de ajuste de imagen. Este último proporciona previsualizaciones en tiempo real para operaciones de ajuste.
* Como práctica recomendada, recuerde que puede agrupar comandos de servicio de imágenes de Dynamic Media en un ajuste preestablecido de imagen. Un ajuste preestablecido de imagen es un conjunto de macros de comandos de URL con nombres de ajustes preestablecidos personalizados, como `$thumb_low$` y `$product_high$`. El nombre del ajuste preestablecido personalizado en una ruta URL llama a estos ajustes preestablecidos. Esta funcionalidad le ayudará a administrar comandos y ajustes de calidad para diferentes modelos de uso de imágenes en su sitio web y reducirá la longitud total de la URL.
* Adobe Dynamic Media Classic también proporciona formas más avanzadas de ajustar la calidad de la imagen, como aplicar enfoque de imagen al ingerir. En los casos de uso avanzados en los que una opción es seguir ajustando y optimizando los resultados procesados, Adobe Professional Services puede ayudarle con la insight personalizada y con las prácticas recomendadas.
