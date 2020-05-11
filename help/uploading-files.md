---
title: Carga de archivos
seo-title: Carga de archivos
description: nulo
seo-description: Obtenga información sobre cómo cargar archivos.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
translation-type: tm+mt
source-git-commit: d5dcc67200b636cafcf1c87b2ecdfb2271b7b9a2
workflow-type: tm+mt
source-wordcount: '3867'
ht-degree: 51%

---


# Carga de archivos{#uploading-files}

Antes de cargar archivos de recursos en Scene7 Publishing System, asegúrese de que tienen el nombre correcto y que la estructura de carpetas está organizada de la forma que desea. Puede cargar archivos desde un sitio FTP proporcionado por Dynamic Media Classic o directamente desde el equipo o la red. Dynamic Media Classic oferta opciones para optimizar los archivos al cargarlos. Si ha instalado la aplicación de escritorio de Adobe Scene7 Publishing System, puede cargar archivos y carpetas arrastrándolos directamente desde el equipo. (Consulte [Configuración general de la aplicación](application-setup.md#general_settings)).

## Preparación de los recursos y las carpetas para la carga {#preparing-your-assets-and-folders-for-uploading}

Antes de cargar recursos en Scene7 Publishing System, asegúrese de que tienen el tamaño y el formato correcto. También debe observar las reglas de Dynamic Media Classic para asignar nombres a los recursos. La creación de una estructura de carpetas para los archivos facilita la búsqueda y el uso de éstos.

### Formatos de archivo de recurso admitidos {#supported-asset-file-formats}

Esta tabla muestra los formatos de archivo de recurso que Scene7 Publishing System admite. For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formatos de archivo de recurso | Descripción |
|--- |--- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Hoja de estilos en cascada | CSS |
| Perfiles de color | ICC, ICM |
| Fuentes | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Imágenes | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (solo Windows), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG y RAW de cámara |
| PostScript | EPS, PS |
| Creación de imágenes de Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

La carga de archivos TAR y ZIP incluye una casilla de verificación para seleccionar si desea descomprimir los archivos.

### Formatos de imagen no admitidos en Dynamic Media {#unsupported-image-formats-dynamic-media}

La siguiente lista describe los subtipos de formatos de archivo de imagen rasterizada que *no son* compatibles con Dynamic Media.

Consulte también [Detección de formatos de archivo no compatibles para Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Archivos PNG con un tamaño de fragmento IDAT bueno de 100 MB.
* Archivos PSB.
* Los archivos PSD con un espacio de color distinto de CMYK, RGB, escala de grises o mapa de bits no son compatibles. No se admiten los espacios de color DuoTone, Lab e Indexed.
* Archivos PSD con una profundidad buena de 16.
* Archivos TIFF que tienen datos de coma flotante.
* Archivos TIFF que tienen espacio de color Lab.

### Tipos de recursos {#asset-types}

Para obtener resultados óptimos con la plataforma de Dynamic Media Classic, asegúrese de utilizar los formatos y tamaños de archivo recomendados. Esta tabla muestra los tipos de recursos, algunos con los formatos y tamaños de archivos recomendados para los recursos más comunes.

| Tipo de recurso | Descripción/Recomendaciones |
|--- |--- |
| Audio | Los formatos de recursos de audio de entrada incluyen AAC, HE-AAC, AC3, WAV, WMA, AIFF y MP3. Puede transcodificar audio a los formatos siguientes: MP3, AAC y HE-AAC. |
| Imágenes (para cambio de tamaño de imagen, zoom, conjuntos de imágenes, conjuntos de giros) | El tamaño mínimo de las imágenes debe ser de 2.000 píxeles a lo largo; el tamaño típico suele ser entre 1.500 y 2.500 píxeles. Se recomiendan los formatos de imagen sin pérdida (incluidos TIFF y PNG). Con imágenes JPEG, use los valores más altos de calidad. Los archivos GIF animados se gestionan como cualquier otro contenido estático. |
| Catálogos electrónicos | Use archivos PDF de alta resolución creados en Adobe® Acrobat® o una aplicación de Creative Suite guardados como &quot;listos para publicación&quot;. Los archivos PDF incluyen todas las fuentes, imágenes y máscaras requeridas, así como elementos gráficos a los que se hace referencia, ya sea en formato de página única, doble o multipágina. Asigne un nombre alfanumérico a los archivos para ordenar las páginas. Coloque todos los PDF para el catálogo electrónico en una misma carpeta, para facilitar la tarea de carga. Puede seleccionar opciones de recorte para quitar de los archivos marcas de recorte, destinos de registro o barras de color. La mayoría de archivos PDF listos para imprenta utilizan un espacio de color CMYK, por lo que es importante obtener el perfil de color CMYK ICC utilizado con los archivos. |
| Plantillas | Las imágenes o los diseños con capas pueden incluir texto, imágenes y capas. Las capas de imagen, las cadenas de texto y los atributos, tales como el color y tamaño, pueden parametrizarse para personalizar los datos variables. Los requisitos de imagen cuando se utilizan plantillas son los mismos que para otros tipos de imagen. Prepare los gráficos en Photoshop u otro programa de edición de imágenes. Guarde cada gráfico como archivo acoplado transparente, en formato TIFF o PNG. Asegúrese de que la resolución de la imagen es apropiada para el uso previsto. Las imágenes para impresión deben ser de 300 ppp. |
| Vídeos | Dynamic Media Classic admite archivos de vídeo guardados en formato OGV y MP4. Puede transcodificar los archivos al formato MP4 al cargarlos.Consulte Formatos [de archivo de recursos](#supported-static-file-formats)admitidos. |
| Fuentes | Fuentes TrueType, Type1 (solo Windows), OpenType y PhotoFonts cargadas. |
| Imágenes | Imágenes y archivos de imagen con capas. |
| Conjuntos de imágenes y conjuntos de muestras | Un conjunto de imágenes se compone de imágenes relacionadas que se pueden mostrar en un visor. |
| Perfiles ICC | Perfil de color que se puede usar para convertir una imagen cargada de su espacio de color de origen a uno diferente. |
| Viñetas | Imágenes creadas con el programa Image Authoring, así como archivos relacionados. |
| Archivos de contenido | Archivos de contenido de Adobe InDesign, Illustrator o Photoshop. |
| Archivos FXG | Archivos con formato gráfico independiente de la resolución que puede utilizar para crear plantillas personalizadas para impresión, web, correo electrónico, escritorio y dispositivos. |
| Archivos SVG | Archivos gráficos vectoriales escalables que los servidores para servicio de imágenes pueden procesar. |
| Archivos XML | Archivos que definen reglas de preprocesamiento utilizadas para modificar la ruta y las partes de consulta de las solicitudes. |
| Archivos de hoja de estilos en cascada | Cargue apariencias de CSS para personalizar los visores de HTML5. |
| Archivos JavaScript | Los archivos JavaScript se utilizan para la instrumentación del visor con el fin de contener la información de la cuenta. El equipo de seguridad de Adobe solo los recomienda para las cuentas de cliente que dispongan de un dominio independiente en uso para la entrega (a fin de evitar la aplicación de scripts en distintos sitios). |

>[!NOTE]
>
>Al cargar archivos de imagen y PDF en SPS, el sistema convierte estos archivos de origen a formato P-TIFF (Pyramid TIFF). Estos P-TIFF son los archivos que se publican posteriormente en los servidores de imágenes de Dynamic Media. Dynamic Media Classic utiliza el formato de archivo Pyramid Tiff, ya que contiene varias relaciones de zoom que permiten un zoom rápido al visualizarse con un visor de zoom Dynamic Media Classic.

### Formatos de archivo estático compatibles {#supported-static-file-formats}

Dynamic Media Classic admite varios formatos de archivo estáticos. El contenido estático es cualquier recurso publicado &quot;tal cual&quot;, como CSS, PDF, SVG, XML, etc.

Los siguientes tipos de archivo pueden publicarse:

* GIF animado
* Archivos de sonido
* CSS
* JavaScript (cuando la empresa se configura con su propio dominio)
* Vídeo maestro
* PDF (cuando PDF se marca específicamente para la publicación tras la carga con el fin de evitar la entrega de todos los archivos PDF para el flujo de trabajo existente de catálogos electrónicos/PDF)
* Vídeo PrX
* SVG
* XML
* ZIP

Dynamic Media Classic no ofrece la opción de generar una URL de previsualización de contenido estático.

### Requisitos de nombre de archivo {#filename-requirements}

Dado que las extensiones de nombre de archivo se quitan durante el proceso de carga, el sistema no permite que haya archivos con el mismo nombre raíz. En el sistema de Dynamic Media Classic, el nombre de archivo del recurso menos la extensión de nombre de archivo se convierte en el ID del recurso. Por esta razón no puede haber dos recursos con el mismo nombre.

Asegúrese de que todos los usuarios de la empresa entienden las reglas de designación de archivos.

* El sistema no admite identificadores de recurso con un nombre idéntico.
* Los nombres de ID de recursos distinguen entre mayúsculas y minúsculas.
* Como práctica recomendada, compruebe que los ID de recursos no contienen espacios en blanco (por ejemplo, chaqueta negra.tif o chaqueta azul.jpg). Dynamic Media Classic codifica los espacios en blanco en los nombres de recursos cuando utiliza nombres de recursos para construir cadenas URL. Estos códigos ASCII son difíciles de leer, lo que dificulta la lectura de las direcciones URL.
* Los caracteres específicos de idioma están permitidos en los nombres de archivo. No obstante, los siguientes caracteres se permiten en los nombres de archivo:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Si un nombre de archivo contiene uno o varios de los caracteres anteriores, los caracteres se eliminan del nombre durante la carga.

En la mayoría de los casos, un nombre de archivo de recurso puede coincidir con el número de elemento, la SKU de producto u otro nombre tal y como se indica:

| Elemento | Nombre de archivo | ID de recurso |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organización y estructura de carpetas {#folder-organization-and-structure}

Organice y estructure carpetas y subcarpetas en Scene7 Publishing System antes de cargar el contenido en el sistema. Esto aporta dos ventajas:

* Al cargar el contenido en SPS por medio de FTP, puede indicar al sistema que reproduzca la estructura de carpetas durante la carga. De esta forma, el contenido en SPS se organiza en las mismas carpetas y subcarpetas que en el ordenador o la red del usuario. Para reproducir la estructura de carpetas en SPS, seleccione la opción Incluir subcarpetas al cargar recursos a través de FTP.
* La reorganización de carpetas dentro del sistema después de cargar los archivos resulta más difícil que un punto de partida con una estructura de carpetas ya probada.

A la hora de elegir unas convenciones de nomenclatura y estructura para almacenar contenido en Scene7 Publishing System es preciso tener en cuenta los requisitos de cada empresa. A continuación se citan algunos ejemplos de estructura de carpetas:

**Las carpetas basadas** en SKU reciben nombres según los números de artículo o SKU. Por ejemplo, se crean carpetas distintas para las series de números 0-, 20-, 30-, etc.

**Basado** en la marca Para los fabricantes con varias líneas de marca y los minoristas que comercializan otras marcas desde otras compañías, separe los archivos en carpetas de productos con nombres para distintas marcas.

**Las carpetas basadas** en proyectos están organizadas según la fecha de implementación/colocación o el nombre del proyecto. Es el método favorito de los clientes que producen principalmente catálogos electrónicos.

**Reflejo de la jerarquía** de carpetas del sitio web Esta estructura refleja la estructura de carpetas del sitio web, con las carpetas denominadas, por ejemplo, para categorías de productos.

## Acerca de la carga de archivos {#uploading-your-files}

Puede cargar archivos individuales desde el escritorio o cargar carpetas enteras mediante FTP. If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Si ha instalado la aplicación de escritorio de Scene7 Publishing System, puede arrastrar archivos y carpetas directamente desde el escritorio a la carpeta de carga de destino.

Scene7 Publishing System le enviará un mensaje de correo electrónico para confirmar cuándo comienza y termina el trabajo de carga, y para notificar posibles problemas.

Durante un trabajo de carga grande, o inmediatamente después, algunos elementos nuevos pueden mostrar el mensaje &quot;La imagen no está optimizada todavía&quot;. Este mensaje aparece porque los archivos aún no se han procesado completamente y se han agregado a SPS. Puede optimizar estos archivos posteriormente. (Consulte [Optimización de archivos](application-setup.md#optimize_files)).

### Carga de archivos mediante la ficha DESKTOP FROM {#upload-files-using-sps-desktop-application}

La aplicación Scene7 Publishing System Desktop le permite cargar archivos y carpetas arrastrándolos.

1. En la aplicación Scene7 Publishing System Desktop, en la barra de navegación global, haga clic en **Cargar**.
1. On the Upload page, click the **FROM DESKTOP** tab.
1. En la parte izquierda de la página Cargar, en el área **Seleccionar archivos para cargar** , haga clic en **Examinar** para seleccionar los archivos o carpetas que desea cargar y, a continuación, haga clic en **Abrir**.
1. En la parte derecha de la página Cargar, en el área **Elegir destino** de la carpeta, navegue a la carpeta de destino donde desee agregar los archivos o carpetas cargados.
1. (Opcional) Cerca de la parte inferior de la página Cargar, en el campo Nombre **del** trabajo, especifique el nuevo nombre del trabajo de carga. O bien, puede utilizar el nombre predeterminado generado por el sistema que proporciona SPS. El trabajo, junto con otros de carga y publicación, se grabará en la página Trabajos, donde puede comprobar el estado de los trabajos. Consulte [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files).
1. (Opcional) Cerca de la parte inferior de la página de carga, seleccione **Publicar tras la carga** si desea publicar automáticamente los recursos que cargue.
Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Tenga en cuenta que esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
1. (Opcional) Cerca de la parte inferior de la página de carga, seleccione **Sobrescribir en cualquier carpeta, el mismo nombre de recurso base, independientemente de la extensión** , si desea que los archivos que cargue sustituyan los archivos existentes con los mismos nombres. Tenga en cuenta que esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Consulte [Opciones de carga](uploading-files.md#upload_options).

1. En el cuadro de diálogo Opciones de trabajo de carga, haga clic en **Guardar**.
1. En la esquina inferior derecha de la página Cargar, haga clic en **Enviar carga**.
Para ver el progreso de la carga, haga clic en **Trabajos** en la barra de navegación global. Puede continuar trabajando en Scene7 Publishing System y regresar a la pantalla Trabajos en cualquier momento para consultar un trabajo en curso. Para cancelar un trabajo de carga que se encuentre en curso, seleccione **Cancelar** junto al tiempo de duración.

### Carga de archivos mediante la ficha VIA FTP {#upload-files-using-via-ftp}

1. Inicie sesión en el sitio FTP de Dynamic Media Classic que sea específico de su región en particular. Utilice el nombre de usuario y la contraseña FTP que ha recibido del administrador.
1. En Dynamic Media Classic, en la barra de navegación global, haga clic en **Cargar**.
1. On the Upload page, click the **VIA FTP** tab.
1. En la parte izquierda de la página Cargar, en el área **Elegir carpeta FTP para la carga** , elija una carpeta FTP desde la que cargar los archivos.
1. En la parte derecha de la página Cargar, en el área **Elegir destino** de la carpeta de SPS, elija una carpeta de destino en Scene7 Publishing System.
1. (Opcional) Cerca de la parte inferior de la página Cargar, en el campo Nombre **del** trabajo, especifique el nuevo nombre del trabajo de carga. O bien, puede utilizar el nombre predeterminado generado por el sistema que proporciona SPS. El trabajo, junto con otros de carga y publicación, se grabará en la página Trabajos, donde puede comprobar el estado de los trabajos. Consulte [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files).
1. (Opcional) Cerca de la parte inferior de la página de carga, seleccione **Publicar tras la carga** si desea publicar automáticamente los recursos que cargue.
Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Tenga en cuenta que esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
1. (Opcional) Cerca de la parte inferior de la página de carga, seleccione **Sobrescribir en cualquier carpeta, el mismo nombre de recurso base, independientemente de la extensión** , si desea que los archivos que cargue sustituyan los archivos existentes con los mismos nombres. Tenga en cuenta que esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. (Opcional; disponible sólo si ha hecho clic en la ficha **MEDIANTE FTP** ) Cerca de la parte inferior de la página de carga, seleccione **Descomprimir archivos comprimidos o archivos de la barra al cargar** si desea extraer automáticamente todos los archivos del archivo ZIP o TAR cargado. Tenga en cuenta que esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Consulte [Opciones de carga](uploading-files.md#upload_options).

1. En el cuadro de diálogo Opciones de trabajo de carga, haga clic en **Guardar**.
1. En la esquina inferior derecha de la página Cargar, haga clic en **Enviar carga**.

   Para ver el progreso de la carga, en la barra de navegación global, haga clic en **Trabajos**. La página Trabajos muestra el progreso de la carga. Puede continuar trabajando en Scene7 Publishing System y regresar a la pantalla Trabajos en cualquier momento para consultar un trabajo en curso.

Para cancelar un trabajo de carga que se encuentre en curso, haga clic en **Cancelar** junto al tiempo de duración.

## Cuadro de diálogo Opciones de trabajo de carga {#upload-options}

Al cargar archivos, puede elegir entre las siguientes opciones del cuadro de diálogo Opciones de trabajo de carga:

* **TRABAJO** — Haga clic en **TRABAJO** para elegir las opciones que afectan a todo el trabajo de carga.

   Tenga en cuenta que también puede elegir las opciones *predeterminadas* para cargar trabajos mediante el cuadro de diálogo Opciones **de carga** predeterminadas en Configuración general. Haga clic en **Ajustes > Ajustes de aplicación > Configuración general > Opciones** de carga predeterminadas y, a continuación, defina las opciones predeterminadas que desee.

   * **Cuándo** — La opción **Cuándo** solo está disponible si ha seleccionado la ficha **MEDIANTE FTP** .
      * **Una vez** — Especifique un trabajo de carga que se ejecute una vez. Las opciones son las siguientes:
         * **Ahora** — Ejecuta el trabajo de carga inmediatamente después de hacer clic en **Guardar** en el cuadro de diálogo Opciones de trabajo de carga y, a continuación, haga clic en **Enviar carga** en la página de carga.
         * **Programar para después** — Seleccione el año, mes, día y hora (en incrementos de 15 minutos) que desea que se ejecute el trabajo de carga.
      * **Recurrente** — Especifique un trabajo de carga que se ejecute diariamente, semanalmente o mensualmente. O bien, personalice el trabajo de carga según sus propias especificaciones.
         * **Diario** — Defina la hora a la que desea que se ejecute el trabajo todos los días. Si desea que el trabajo se ejecute solamente de lunes a viernes, seleccione Solo **días de semana**.
         * **Semanal** — Elija un día específico de la semana y la hora en que desea que se ejecute el trabajo.
         * **Mensual** — Elija un día específico del mes o día de la semana, incluida la hora de inicio, que desea que se ejecute el trabajo.
         * **Personalizado** — Personalice un intervalo de tiempo de trabajo de carga o publicación según sus propias especificaciones. Consulte [Creación de un intervalo personalizado para un trabajo de carga o publicación](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Publicar tras la carga** — Disponible si ha seleccionado la ficha **DESKTOP** O **MEDIANTE FTP** . Seleccione esta opción para publicar automáticamente los recursos que cargue. Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Esta opción también está disponible en la página de carga.

   * **Sobrescribir en cualquier carpeta, el mismo nombre de recurso base, independientemente de la extensión** — Disponible si ha seleccionado la ficha **DESKTOP** O **MEDIANTE FTP** . Seleccione esta opción si desea que los archivos que cargue sustituyan archivos existentes con los mismos nombres. Esta opción también está disponible en la página de carga. The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.

   * **Descomprimir archivos comprimidos o de etiquetas durante la carga** — Disponible si ha seleccionado la ficha **DESKTOP** O **MEDIANTE FTP** .
Seleccione esta opción si desea extraer automáticamente todos los archivos del archivo ZIP o TAR cargado. Tenga en cuenta que esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.

   * **Incluir subcarpetas** — Solo está disponible si ha seleccionado la ficha **MEDIANTE FTP** .
Seleccione esta opción si desea cargar subcarpetas de la carpeta que va a cargar. Los nombres de la carpeta y las subcarpetas que cargue se introducirán automáticamente en SPS.

   * **Procesar archivos** de metadatos — Solo está disponible si ha seleccionado la ficha **VIA FTP** . Seleccione esta opción si desea cargar un archivo delimitado por tabuladores o XML para agregar metadatos a varios recursos. Consulte [Importación de datos (mediante FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPCIONES** DE RECORTE — Para recortar automáticamente píxeles de espacio en blanco de una imagen, abra el menú Recortar, elija Manual e introduzca las medidas en píxeles en los campos Superior, Derecha, Inferior e Izquierda para recortar desde los lados. También puede seleccionar Recortar del menú Recortar y elegir estas opciones:

   * **Recortar basándose en** — Elija si desea recortar según el color o la transparencia:

      * **Color** — Elija la opción Color. A continuación, seleccione el menú Esquina y elija la esquina de la imagen que mejor represente el color de espacio en blanco que desea recortar.

         Recorte basado en el color: Especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color.

      * **Transparencia** —  Elija la opción Transparencia.

         Recorte basado en transparencia: Especifique 0 para recortar píxeles solo si son totalmente transparentes; los números más cercanos a 1 permiten una mayor transparencia.

      * **Tolerancia** — Arrastre el control deslizante para especificar una tolerancia de 0 a 1.

* **OPCIONES** DE PERFIL DE COLOR — Seleccione una conversión de color cuando cree archivos optimizados que se utilicen para el envío dinámico de Dynamic Media Classic:

   * **Conservación** de color predeterminada — Mantiene los colores de la imagen de origen siempre que las imágenes contengan información de espacio de color; no hay conversión de color. Casi todas las imágenes actuales ya tienen incrustado el perfil de color adecuado. Sin embargo, si la imagen de origen CMYK no contiene un perfil de color incrustado, los colores se convierten al espacio de color sRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

   * **Mantener espacio** de color original: Conserva los colores originales sin ninguna conversión de color en el punto de ingestión en Scene7 Publishing System. Para las imágenes sin un perfil de color incrustado, las conversiones de color necesarias para procesar solicitudes de la imagen se realizan con los perfiles de color predeterminados como están configurados en Configuración de publicación. Puede ser que estos perfiles de color no coincidan con el color en los archivos creados con esta opción. Por lo tanto, se recomienda utilizar la opción Conservación de color predeterminada.

   * **Personalizar De > A** — Abre menús para que pueda elegir un espacio de color Convertir de y Convertir a. Esta opción avanzada sustituye cualquier información de color incrustada en el archivo de origen. Solo debe seleccionar esta opción cuando todas las imágenes que envía contienen datos de perfil de color incorrectos o que faltan.

* **OPCIONES** DE EDICIÓN DE IMÁGENES — Puede conservar las máscaras de recorte &lt;> en las imágenes y elegir un perfil de color.
Consulte [Opciones de edición de imágenes al cargarlas](image-editing-options-upload.md#image-editing-options-at-upload).

* **OPCIONES** POSTSCRIPT — Puede rasterizar archivos PostScript®, recortar archivos, mantener fondos transparentes, elegir una resolución y elegir un espacio de color.
Consulte [Uso de archivos de PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPCIONES** DE PHOTOSHOP: Puede crear plantillas a partir de archivos de Adobe® Photoshop®, mantener las capas, especificar el nombre de las capas, extraer texto y especificar cómo se anclan las imágenes en las plantillas.
Consulte [Opciones de carga de archivos PSD](psd-files.md#psd_upload_options).

* **OPCIONES** DE PDF — Puede rasterizar los archivos, extraer palabras de búsqueda y vínculos, generar automáticamente un catálogo electrónico, definir la resolución y elegir un espacio de color.
Consulte [Opciones de carga de PSD](pdfs.md#pdf_upload_options).

* **OPCIONES** DE ILLUSTRATOR — Puede rasterizar archivos de Adobe Illustrator®, mantener fondos transparentes, elegir una resolución y elegir un espacio de color.
Consulte [Uso de archivos de PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPCIONES** DE EVIDEO — Puede transcodificar un archivo de vídeo seleccionando un ajuste preestablecido de vídeo.
Consulte [Uso de ajustes preestablecidos de codificación de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **METADATOS** ADICIONALES — Escriba las palabras clave que describan los archivos que va a cargar. Separe las palabras clave con una coma. Las palabras clave facilitan la búsqueda de recursos. Consulte [Búsqueda avanzada](searching-assets.md#conducting_an_advanced_search).

* **AJUSTES PREESTABLECIDOS** DE CONJUNTOS DE LOTES — Si desea crear un conjunto de imágenes, un conjunto de giros de varios ejes o un conjunto de muestras a partir de los archivos cargados, haga clic en la columna Activo del ajuste preestablecido que desee utilizar. Puede seleccionar varios ajustes preestablecidos. Los ajustes preestablecidos se crean en la página Ajustes de aplicación/Valores preestablecidos de conjunto por lotes.
Consulte [Valores preestablecidos de conjunto por lotes](application-setup.md#batch_set_presets).

* **AVANZADO** — Consulte [Seguir una carga con otro trabajo](uploading-files.md#follow-an-upload-with-another-job).

## Ejecución de trabajos a continuación de la carga {#follow-an-upload-with-another-job}

Al cargar elementos por medio de FTP, puede programar el inicio del trabajo siguiente para el momento en que termine la carga. (Si hay otros trabajos programados para ese mismo momento, los trabajos que programe aquí se colocarán detrás de ellos).

El nuevo trabajo envía una notificación a la dirección especificada para activar el código de esa ubicación. Este trabajo de publicación que sigue recibe el mismo nombre que el trabajo de carga pero se le añade el prefijo *Pub_*.

**Para seguir una carga con otro trabajo**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. En el cuadro de diálogo Opciones de trabajo de carga, expanda la sección **AVANZADA** .
1. Elija una de las siguientes opciones en la lista desplegable **Seguir carga con otro trabajo** :

   * Ninguno
   * Solicitud HTTP
   * Publicación para servicio de imágenes
   * Procesador de imágenes
   * Publicación de vídeo

1. Especifique la dirección HTTP.
1. Especifique si desea ejecutar solo si se han cargado archivos.
1. Indique si desea ejecutar esta solicitud cada vez que termine este trabajo o solo si se han publicado archivos.

   >[!NOTE]
   >
   >La programación periódica de los trabajos no garantiza la publicación de ningún archivo.

>[!MORELIKETHIS]
>
>* [Uso de carpetas de recursos](asset-folders.md#working_with_asset_folders)
>* [Gestión de trabajos recurrentes de carga y publicación](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Uso de un trabajo de carga o publicación como desencadenador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

