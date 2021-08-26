---
title: Carga de archivos
description: Obtenga información sobre cómo cargar archivos.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '3863'
ht-degree: 36%

---

# Carga de archivos{#uploading-files}

Antes de cargar archivos de recursos en Adobe Dynamic Media Classic, asegúrese de que los archivos de recursos tengan los nombres adecuados y de que la estructura de carpetas esté configurada y organizada del modo que desee. Puede cargar archivos desde un sitio FTP proporcionado por Dynamic Media Classic de Adobe o directamente desde su equipo o red. Adobe Dynamic Media Classic ofrece opciones para optimizar archivos a medida que los carga. Si ha instalado la aplicación de escritorio de Adobe Dynamic Media Classic, puede cargar archivos y carpetas arrastrándolos directamente desde el escritorio. Consulte [Configuración general de la aplicación](application-setup.md#general_settings).

## Preparación de los recursos y las carpetas para la carga {#preparing-your-assets-and-folders-for-uploading}

Antes de cargar recursos en Adobe Dynamic Media Classic, asegúrese de que tengan el formato y el tamaño adecuados. También debe observar las reglas de Adobe de Dynamic Media Classic para asignar nombres a los recursos. La creación de una estructura de carpetas para los archivos facilita la búsqueda y el uso de éstos.

### Formatos de archivo de recurso admitidos {#supported-asset-file-formats}

En esta tabla se enumeran los formatos de archivo de recursos que admite Adobe Dynamic Media Classic. Para obtener información sobre los archivos Camera Raw admitidos, consulte [https://www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formatos de archivo de recurso | Descripción |
|--- |--- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Hoja de estilos en cascada | CSS |
| Perfiles de color | ICC, ICM |
| Fuentes | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Imágenes | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (solo Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG y RAW de cámara |
| PostScript | EPS, PS |
| Creación de imágenes en Adobe Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

La carga de archivos TAR y ZIP incluye una casilla de verificación para seleccionar si desea descomprimir los archivos.

### Formatos de imagen no compatibles en Dynamic Media {#unsupported-image-formats-dynamic-media}

La siguiente lista describe los subtipos de formatos de archivo de imagen de trama que *no* son compatibles con Dynamic Media.

Consulte también [Detectar formatos de archivo no compatibles para Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Los archivos PNG que tienen un tamaño de fragmento IDAT tienen un tamaño bueno de más de 100 MB.
* Archivos PSB.
* Los archivos PSD con un espacio de color distinto de CMYK, RGB, escala de grises o mapa de bits no son compatibles. Los espacios de color DuoTone, Lab e Indexed no son compatibles.
* Los archivos PSD con una profundidad buena superior a 16.
* Archivos TIFF con datos de coma flotante.
* Archivos TIFF que tienen espacio de color Lab.

### Tipos de recursos {#asset-types}

Para obtener resultados óptimos con el programa Adobe Dynamic Media Classic, asegúrese de utilizar los formatos y tamaños de archivo recomendados. Esta tabla muestra los tipos de recursos, algunos con los formatos y tamaños de archivos recomendados para los recursos más comunes.

| Tipo de recurso | Descripción/Recomendaciones |
|--- |--- |
| Audio | Los formatos de recursos de audio de entrada incluyen AAC, HE-AAC, AC3, WAV, WMA, AIFF y MP3. Puede transcodificar audio a los formatos siguientes: MP3, AAC y HE-AAC. |
| Imágenes (para cambio de tamaño de imagen, zoom, conjuntos de imágenes, conjuntos de giros) | Las imágenes deben tener al menos 2000 píxeles con el tamaño más largo; los tamaños de imagen típicos varían de 1500 a 2500 píxeles en el tamaño más largo. Se recomiendan los formatos de imagen sin pérdida (incluidos TIFF y PNG). Con imágenes JPEG, use los valores más altos de calidad. Los archivos GIF animados se gestionan como cualquier otro contenido estático. |
| Catálogos electrónicos | Use archivos PDF de alta resolución creados en Adobe® Acrobat® o una aplicación de Creative Suite guardados como &quot;listos para publicación&quot;. Los archivos PDF incluyen todas las fuentes, imágenes y máscaras requeridas, así como elementos gráficos a los que se hace referencia, ya sea en formato de página única, doble o multipágina. Asigne un nombre alfanumérico a los archivos para ordenar las páginas. Coloque todos los PDF para el catálogo electrónico en una misma carpeta, para facilitar la tarea de carga. Puede seleccionar opciones de recorte para quitar de los archivos marcas de recorte, destinos de registro o barras de color. La mayoría de archivos PDF listos para imprenta utilizan un espacio de color CMYK, por lo que es importante obtener el perfil de color CMYK ICC utilizado con los archivos. |
| Plantillas | Las imágenes o los diseños con capas pueden incluir texto, imágenes y capas. Las capas de imagen, las cadenas de texto y los atributos, tales como el color y tamaño, pueden parametrizarse para personalizar los datos variables. Los requisitos de imagen cuando se utilizan plantillas son los mismos que para otros tipos de imagen. Prepare los gráficos en Photoshop u otro programa de edición de imágenes. Guarde cada gráfico como archivo acoplado transparente, en formato TIFF o PNG. Asegúrese de que la resolución de la imagen es apropiada para el uso previsto. Las imágenes para imprimir son de 300 ppi. |
| Vídeos | Adobe Dynamic Media Classic admite archivos de vídeo guardados en los formatos OGV y MP4. Puede transcodificar los archivos a formato MP4 en el momento de realizar la carga. Consulte [Formatos de archivo de recursos admitidos](#supported-static-file-formats) |
| Fuentes | Fuentes TrueType, Type1 (solo Windows®), OpenType® y PhotoFonts cargados |
| Imágenes | Imágenes y archivos de imagen con capas. |
| Conjuntos de imágenes y conjuntos de muestras | Un conjunto de imágenes se compone de imágenes relacionadas que se pueden mostrar en un visor. |
| Perfiles ICC | Perfil de color que se puede usar para convertir una imagen cargada de su espacio de color de origen a uno diferente. |
| Viñetas | Imágenes creadas con el programa de creación de imágenes y archivos relacionados. |
| Archivos de contenido | Archivos de contenido de Adobe InDesign, Illustrator o Photoshop. |
| Archivos FXG | Archivos con formato gráfico independiente de la resolución que puede utilizar para crear plantillas personalizadas para impresión, web, correo electrónico, escritorio y dispositivos. |
| Archivos SVG | Archivos gráficos vectoriales escalables que los servidores para servicio de imágenes pueden procesar. |
| Archivos XML | Archivos que definen reglas de preprocesamiento utilizadas para modificar la ruta y las partes de consulta de las solicitudes. |
| Archivos de hoja de estilos en cascada | Cargue apariencias de CSS para personalizar los visores de HTML5. |
| Archivos JavaScript™ | Los archivos JavaScript™ se utilizan para la instrumentación del visor con el fin de almacenar información de la cuenta. Adobe Security recomienda este tipo de recurso solo para cuentas de cliente que tengan un dominio independiente en uso para la entrega (para evitar la creación de scripts en sitios cruzados). |

>[!NOTE]
>
>Cuando se cargan archivos de imagen y archivos PDF en Adobe Dynamic Media Classic, el sistema convierte estos archivos de origen en archivos P-TIFF (Pyramid TIFF). Estos P-TIFF son los archivos que se publican posteriormente en los servidores de imágenes de Dynamic Media. Adobe Dynamic Media Classic utiliza el formato de archivo Pyramid Tiff porque contiene varias relaciones de zoom que permiten un zoom rápido al visualizarlo con un visor de zoom Dynamic Media Classic de Adobe.

### Formatos de archivo estático compatibles {#supported-static-file-formats}

Adobe Dynamic Media Classic admite varios formatos de archivo estáticos. El contenido estático es cualquier recurso publicado tal cual, como CSS, PDF, SVG y XML.

Los siguientes tipos de archivo pueden publicarse:

* GIF animado
* Archivos de sonido
* CSS
* JavaScript™ (cuando la empresa está configurada con su propio dominio)
* Vídeo maestro
* PDF (cuando PDF está marcado para su publicación después de la carga, para evitar la entrega de todos los PDF para el flujo de trabajo existente de catálogo electrónico/PDF)
* Vídeo PrX
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic no proporciona la opción de generar una URL de vista previa de contenido estático.

### Requisitos de nombre de archivo {#filename-requirements}

Dado que las extensiones de nombre de archivo se quitan durante el proceso de carga, el sistema no permite que haya archivos con el mismo nombre raíz. En el sistema de Adobe Dynamic Media Classic, el nombre de archivo del recurso menos la extensión del nombre del archivo se convierte en el ID del recurso. Por esta razón no puede haber dos recursos con el mismo nombre.

Asegúrese de que todos los usuarios de la empresa entienden las reglas de designación de archivos.

* El sistema no admite identificadores de recurso con un nombre idéntico.
* Los nombres de los ID de recurso distinguen entre mayúsculas y minúsculas.
* Como práctica recomendada, compruebe que los ID de recursos no contienen espacios en blanco (por ejemplo, chaqueta negra.tif o chaqueta azul.jpg). Adobe Dynamic Media Classic ASCII codifica espacios en blanco en los nombres de recursos cuando utiliza nombres de recursos para construir cadenas de URL. Estos códigos ASCII son difíciles de leer, lo que dificulta la lectura de las direcciones URL.
* Los caracteres específicos de idioma están permitidos en los nombres de archivo. No obstante, los siguientes caracteres se permiten en los nombres de archivo:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Si un nombre de archivo contiene uno o varios de los caracteres anteriores, los caracteres se eliminan del nombre durante la carga.

Normalmente, un nombre de archivo de recurso puede ser el mismo que su número de artículo, SKU de producto u otro nombre que en el siguiente ejemplo:

| Elemento | Nombre de archivo | ID de recurso |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organización y estructura de carpetas {#folder-organization-and-structure}

Organice y estructura carpetas y subcarpetas para su contenido en Adobe Dynamic Media Classic antes de cargar el contenido en el sistema. Esto aporta dos ventajas:

* Al cargar el contenido en Adobe Dynamic Media Classic a través de FTP, puede indicar al sistema que duplique la estructura de carpetas durante la carga. De este modo, el contenido se organiza en las mismas carpetas y subcarpetas de Adobe Dynamic Media Classic que en su equipo o red. (Para replicar la estructura de carpetas en Adobe Dynamic Media Classic, seleccione la opción Incluir subcarpetas al cargar recursos mediante FTP).
* La reorganización de carpetas dentro del sistema después de cargar los archivos resulta más difícil que un punto de partida con una estructura de carpetas ya probada.

El método de asignación de nombres a carpetas y la estructura que elija para almacenar el contenido en el Adobe Dynamic Media Classic dependen de las necesidades de su organización. A continuación se citan algunos ejemplos de estructura de carpetas:

**Basado en SKU** : los nombres de las carpetas dependen de los SKU o los números de artículo. Por ejemplo, se crean carpetas distintas para las series de números 0-, 20-, 30-, etc.

**Basado en la marca** : para los fabricantes con varias líneas de marca y los minoristas que comercializan otras marcas de otras empresas, separe los archivos en carpetas de productos con nombres para diferentes marcas.

**Basado en proyectos** : las carpetas se organizan en función de la fecha de lanzamiento/colocación o el nombre del proyecto. Es el método favorito de los clientes que producen principalmente catálogos electrónicos.

**Mirror of web site folder hierarchy** : esta estructura de carpetas refleja la estructura de carpetas del sitio web, con las carpetas denominadas, por ejemplo, para categorías de productos.

## Acerca de la carga de archivos {#uploading-your-files}

Puede cargar archivos individuales desde el escritorio o cargar carpetas enteras mediante FTP. Si desea cargar más de 100 MB de archivos o cargar carpetas y subcarpetas completas, seleccione la pestaña **VIA FTP**.

Adobe Dynamic Media Classic le envía un mensaje de correo electrónico para confirmar cuándo comienza y finaliza el trabajo de carga y para notificarle cualquier problema.

Durante (o inmediatamente después) un trabajo de carga grande, algunos elementos nuevos podrían mostrar el mensaje &quot;Imagen aún no optimizada&quot;. Este mensaje aparece porque los archivos aún no se han procesado y agregado completamente a Adobe Dynamic Media Classic. Puede optimizar estos archivos posteriormente. Consulte [Optimizar archivos](application-setup.md#optimize_files).

### Carga de archivos mediante la ficha Desde escritorio {#upload-files-using-sps-desktop-application}

La aplicación de escritorio de Adobe Dynamic Media Classic permite cargar archivos y carpetas arrastrando.

1. En la aplicación de escritorio de Adobe Dynamic Media Classic, en la barra de navegación global, haga clic en **[!UICONTROL Cargar]**.
1. En la página Cargar , haga clic en la pestaña **[!UICONTROL Desde escritorio]**.
1. En el lado izquierdo de la página Cargar, en el área **[!UICONTROL Seleccionar archivos para cargar]**, haga clic en **[!UICONTROL Examinar]** para seleccionar los archivos o carpetas que desea cargar y, a continuación, haga clic en **[!UICONTROL Abrir]**.
1. En el lado derecho de la página Cargar, en el área **Elegir destino de carpeta**, vaya a la carpeta de destino en la que desee agregar los archivos o carpetas cargados.
1. (Opcional) Cerca de la parte inferior de la página Cargar, en el campo **[!UICONTROL Nombre del trabajo]**, especifique el nuevo nombre del trabajo de carga. O bien, simplemente puede utilizar el nombre predeterminado generado por el sistema que proporciona el Adobe Dynamic Media Classic. El trabajo, junto con otros de carga y publicación, se grabará en la página Trabajos, donde puede comprobar el estado de los trabajos. Consulte [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files).
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Publicar después de cargar]** si desea publicar automáticamente los recursos que carga.
Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Sobrescribir en cualquier carpeta, el mismo nombre de recurso base independientemente de la extensión]** si desea que los archivos que cargue reemplacen los archivos existentes con los mismos nombres. Esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
El nombre de esta opción puede ser diferente, dependiendo de la configuración en **Configuración de la aplicación > Configuración general > Cargar a la aplicación > Sobrescribir imágenes**.
1. Cerca de la esquina inferior derecha de la página Cargar, haga clic en **[!UICONTROL Opciones de trabajo]** y, a continuación, especifique las opciones que desee.

   Consulte [Opciones de carga](uploading-files.md#upload_options).

1. En el cuadro de diálogo Opciones de trabajo de carga, haga clic en **[!UICONTROL Guardar]**.
1. En la esquina inferior derecha de la página Cargar, haga clic en **[!UICONTROL Enviar carga]**.
Para ver el progreso de la carga, haga clic en **[!UICONTROL Trabajos]** en la barra de navegación global. Puede seguir trabajando en Adobe Dynamic Media Classic y volver a la página Trabajos en cualquier momento para revisar un trabajo en curso. Para cancelar un trabajo de carga que se encuentre en curso, seleccione **[!UICONTROL Cancelar]** junto al tiempo de duración.

### Carga de archivos mediante la ficha VIA FTP {#upload-files-using-via-ftp}

1. Inicie sesión en el sitio FTP de Adobe Dynamic Media Classic que sea específico de su región en particular. Utilice el nombre de usuario y la contraseña FTP que ha recibido del administrador.
1. En Adobe Dynamic Media Classic, en la barra de navegación global, haga clic en **[!UICONTROL Cargar]**.
1. En la página Cargar , haga clic en la pestaña **[!UICONTROL VIA FTP]**.
1. En la parte izquierda de la página Cargar, en el área **[!UICONTROL Elegir carpeta FTP para cargar]**, elija una carpeta FTP desde la que cargar los archivos.
1. En el lado derecho de la página Cargar, en el área **[!UICONTROL Elegir destino de carpeta de Dynamic Media de Adobe]**, elija una carpeta de destino en Adobe Dynamic Media Classic.
1. (Opcional) Cerca de la parte inferior de la página Cargar, en el campo **[!UICONTROL Nombre del trabajo]**, especifique el nuevo nombre del trabajo de carga. O bien, simplemente puede utilizar el nombre predeterminado generado por el sistema que proporciona el Adobe Dynamic Media Classic. El trabajo, junto con otros de carga y publicación, se grabará en la página Trabajos, donde puede comprobar el estado de los trabajos. Consulte [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files).
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Publicar después de la carga]** si desea publicar automáticamente los recursos que carga.
Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Sobrescribir en cualquier carpeta, el mismo nombre de recurso base independientemente de la extensión]** si desea que los archivos que cargue reemplacen los archivos existentes con los mismos nombres. Esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
El nombre de esta opción puede ser diferente, dependiendo de la configuración en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración general]** > **[!UICONTROL Cargar a la aplicación]** > **[!UICONTROL Sobrescribir imágenes]**.
1. Opcional; solo está disponible si ha hecho clic en la pestaña **[!UICONTROL VIA FTP]**. Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Descomprimir archivos comprimidos o tar en la carga]** si desea extraer automáticamente todos los archivos de su archivo ZIP o TAR cargado. Esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.
1. Cerca de la esquina inferior derecha de la página Cargar, haga clic en **[!UICONTROL Opciones de trabajo]** y, a continuación, especifique las opciones que desee.

   Consulte [Opciones de carga](uploading-files.md#upload_options).

1. En el cuadro de diálogo Opciones de trabajo de carga, haga clic en **[!UICONTROL Guardar]**.
1. En la esquina inferior derecha de la página Cargar, haga clic en **[!UICONTROL Enviar carga]**.

   Para ver el progreso de la carga, en la barra de navegación global, haga clic en **[!UICONTROL Trabajos]**. La página Trabajos muestra el progreso de la carga. Puede seguir trabajando en Adobe Dynamic Media Classic y volver a la página Trabajos en cualquier momento para revisar un trabajo en curso.

Para cancelar un trabajo de carga que se encuentre en curso, haga clic en **[!UICONTROL Cancelar]** junto al tiempo de duración.

## Cuadro de diálogo Cargar opciones de trabajo {#upload-options}

Al cargar archivos, puede elegir entre las siguientes opciones del cuadro de diálogo Opciones de carga de trabajo:

* **TRABAJO** : haga clic en  **** TRABAJO para elegir las opciones que afectan a todo el trabajo de carga.

   También puede elegir las opciones *predeterminadas* para cargar trabajos mediante el cuadro de diálogo **[!UICONTROL Opciones de carga predeterminadas]** en Configuración general. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración general]** > **[!UICONTROL Opciones de carga predeterminadas]** y, a continuación, defina las opciones predeterminadas que desee.

   * **Cuando** : esta opción solo está disponible si ha seleccionado la pestaña  **[!UICONTROL VIA]** FTP.
      * **Una sola vez** : especifique un trabajo de carga que se ejecute una vez. Las opciones incluyen las siguientes:
         * **Ahora** : ejecuta el trabajo de carga inmediatamente después de hacer clic en  **** Guardar en el cuadro de diálogo Opciones de carga de trabajo y, a continuación, haga clic en  **[!UICONTROL Enviar]** carga en la página Cargar.
         * **Programar para después** : seleccione el año, el mes, el día y la hora (en incrementos de 15 minutos) en que desea que se ejecute el trabajo de carga.
      * **Recurrente** : especifique un trabajo de carga que se ejecute de forma diaria, semanal o mensual. O bien, personalice el trabajo de carga según sus propias especificaciones.
         * **Diario** : configure la hora a la que desea que se ejecute el trabajo todos los días. Si desea que el trabajo se ejecute solo de lunes a viernes, seleccione **[!UICONTROL Solo días de la semana]**.
         * **Semanal** : elija un día específico de la semana y la hora en que desea que se ejecute el trabajo.
         * **Mensualmente** : elija un día específico del mes o del día de la semana, incluida la hora de inicio, en el que desea que se ejecute el trabajo.
         * **Personalizado** : personalice un intervalo de tiempo de trabajo de carga o publicación según sus propias especificaciones. Consulte [Creación de un intervalo personalizado para un trabajo de carga o publicación](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Publicar después de la carga** : está disponible si ha seleccionado la pestaña  **[!UICONTROL DESKTOP o]** DESKTOP o la  **[!UICONTROL pestaña]** FTP. Seleccione esta opción para publicar automáticamente los recursos que cargue. Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Esta opción también está disponible en la página de carga.

   * **Sobrescriba en cualquier carpeta, el mismo nombre de recurso base independientemente de la extensión** . Está disponible si ha seleccionado la pestaña  **[!UICONTROL DESKTOP o]** DESKTOP o la pestaña  **[!UICONTROL VIA]** FTP. Seleccione esta opción si desea que los archivos que cargue sustituyan archivos existentes con los mismos nombres. Esta opción también está disponible en la página de carga. El nombre de esta opción puede ser diferente, dependiendo de la configuración en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración general]** > **[!UICONTROL Cargar a la aplicación]** > **[!UICONTROL Sobrescribir imágenes]**.

   * **Descomprimir archivos comprimidos o tar al cargar** : está disponible si ha seleccionado la pestaña  **[!UICONTROL DESKTOP de]** DESKTOP o  **[!UICONTROL VIA]** FTP.
Seleccione esta opción si desea extraer automáticamente todos los archivos de su archivo ZIP o TAR cargado. Esta misma opción también está disponible en el cuadro de diálogo Opciones de trabajo.

   * **Incluir subcarpetas** : solo está disponible si ha seleccionado la pestaña  **[!UICONTROL VIA]** FTP.
Seleccione esta opción si desea cargar subcarpetas de la carpeta que va a cargar. Los nombres de la carpeta y sus subcarpetas que cargue se introducen automáticamente en Adobe Dynamic Media Classic.

   * **Procesar archivos de metadatos** : solo está disponible si ha seleccionado la  **[!UICONTROL pestaña]** VIA FTP. Seleccione esta opción si desea cargar un archivo delimitado por tabuladores o XML para agregar metadatos a varios recursos. Consulte [Importación de datos (mediante FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPTIONS CROP** : para recortar automáticamente píxeles de espacio en blanco de una imagen, abra el  **** menú Recortar, haga clic en  **[!UICONTROL Manual]** e introduzca medidas de píxeles en los campos de texto Superior, Derecha, Inferior e Izquierda para recortar desde los lados. También puede hacer clic en **[!UICONTROL Recortar]** en el menú Recortar y elegir estas opciones:

   * **Separar en función de** : elija si recortar en función del color o la transparencia:
      * **Color** : elija la opción Color. A continuación, seleccione el menú Esquina y elija la esquina de la imagen que mejor represente el color de espacio en blanco que desea recortar.
Recorte basado en el color: Especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color.
      * **Transparencia** : elija la opción  **** Transparencia.
Recorte basado en la transparencia: Especifique 0 para recortar píxeles solo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.
      * **Tolerancia** : arrastre el control deslizante para especificar una tolerancia de 0 a 1.

* **OPTIONS DEL PERFIL DE COLOR** : elija una conversión de color cuando cree archivos optimizados que se utilicen para la entrega dinámica de Dynamic Media Classic de Adobe:

   * **Conservación de color predeterminada** : mantiene los colores de la imagen de origen siempre que las imágenes contienen información de espacio de color; no hay conversión de color. Casi todas las imágenes actuales ya tienen incrustado el perfil de color adecuado. Sin embargo, si la imagen de origen CMYK no contiene un perfil de color incrustado, los colores se convierten al espacio de color sRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.
   * **Conservar espacio de color original** : conserva los colores originales sin conversión de color alguna en el punto de ingesta en Adobe Dynamic Media Classic. En el caso de las imágenes sin un perfil de color incrustado, cualquier conversión de color necesaria para procesar las solicitudes de la imagen se realiza mediante los perfiles de color predeterminados, tal y como se configura en la configuración de publicación . Estos perfiles de color no siempre se alinean con el color en los archivos creados con esta opción. Por lo tanto, se recomienda utilizar la opción Conservación de color predeterminada.
   * **Personalizar de > A** : abre los menús para que pueda elegir un espacio  **[!UICONTROL Convertir]** de y  **[!UICONTROL Convertir]** color de color. Esta opción avanzada sustituye cualquier información de color incrustada en el archivo de origen. Seleccione esta opción solo cuando todas las imágenes que envía contengan datos de perfil de color incorrectos o que falten.

* **OPTIONS**  de EDICIÓN DE IMÁGENES: puede conservar las  &lt;> máscaras de recorte en imágenes y elegir un perfil de color.
Consulte [Opciones de edición de imágenes al cargarlas](image-editing-options-upload.md#image-editing-options-at-upload).

* **OPTIONS de PostScript®** : puede rasterizar archivos de PostScript®, recortar archivos, mantener fondos transparentes, elegir una resolución y elegir un espacio de color.
Consulte [Uso de archivos de PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPTIONS de Photoshop** : puede crear plantillas a partir de archivos de Adobe® Photoshop®, mantener las capas, especificar cómo se denominan las capas, extraer texto y especificar cómo se anclan las imágenes en las plantillas.
Consulte [Opciones de carga de archivos PSD](psd-files.md#psd_upload_options).

* **OPTIONS PDF** : puede rasterizar los archivos, extraer palabras y vínculos de búsqueda, generar automáticamente un catálogo electrónico, establecer la resolución y elegir un espacio de color.
Consulte [Opciones de carga de PSD](pdfs.md#pdf_upload_options).

* **OPTIONS de Illustrator** : puede rasterizar archivos de Adobe Illustrator®, mantener fondos transparentes, elegir una resolución y elegir un espacio de color.
Consulte [Uso de archivos de PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPTIONS EVIDEO** : puede transcodificar un archivo de vídeo eligiendo un ajuste preestablecido de vídeo.
Consulte [Uso de ajustes preestablecidos de codificación de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **METADATOS ADICIONALES** : introduzca palabras clave que describan los archivos que desea cargar. Separe las palabras clave con una coma. Las palabras clave facilitan la búsqueda de recursos. Consulte [Búsqueda avanzada](searching-assets.md#conducting_an_advanced_search).

* **AJUSTES PREESTABLECIDOS DE CONJUNTOS DE LOTES** : si desea crear un conjunto de imágenes, un conjunto de giros de varios ejes o un conjunto de muestras a partir de los archivos cargados, haga clic en la columna Activo del ajuste preestablecido que desee utilizar. Puede seleccionar varios ajustes preestablecidos. Los ajustes preestablecidos se crean en la página Ajustes de aplicación/Valores preestablecidos de conjunto por lotes.
Consulte [Valores preestablecidos de conjunto por lotes](application-setup.md#batch_set_presets).

* **AVANZADO** : consulte  [Seguir una carga con otro trabajo](uploading-files.md#follow-an-upload-with-another-job).

## Ejecución de trabajos a continuación de la carga {#follow-an-upload-with-another-job}

Cuando carga elementos mediante FTP, puede programar un trabajo posterior para que comience cuando se complete la carga. Si hay otros trabajos programados para comenzar, el trabajo que programe aquí se colocará después de ellos.

El nuevo trabajo envía una notificación a la dirección especificada para activar el código de esa ubicación. Este trabajo de publicación que sigue recibe el mismo nombre que el trabajo de carga pero se le añade el prefijo *Pub_*.

**Para seguir una carga con otro trabajo:**

1. Haga clic en **[!UICONTROL Upload]** y, a continuación, haga clic en la pestaña **[!UICONTROL VIA FTP]**.
1. En la esquina inferior derecha de la página Cargar, haga clic en **[!UICONTROL Opciones de trabajo]**.
1. En el cuadro de diálogo Opciones de carga de trabajo , expanda la sección **[!UICONTROL AVANZADA]**.
1. Elija una de las siguientes opciones en la lista desplegable **[!UICONTROL Follow Upload with other job]**:

   * Ninguno
   * Solicitud HTTP
   * Publicación para servicio de imágenes
   * Procesador de imágenes
   * Publicación de vídeo

1. Especifique la dirección HTTP.
1. Especifique si desea ejecutar solo si se cargaron archivos.
1. Indique si desea ejecutar esta solicitud cada vez que termine este trabajo o solo si se han publicado archivos.

   >[!NOTE]
   >
   >Los trabajos programados con regularidad a veces no pueden resultar en la publicación de archivos.

>[!MORELIKETHIS]
>
>* [Uso de carpetas de recursos](asset-folders.md#working_with_asset_folders)
>* [Gestión de trabajos recurrentes de carga y publicación](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Uso de un trabajo de carga o publicación como desencadenador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

