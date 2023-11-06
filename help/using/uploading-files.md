---
title: Carga de archivos
description: Obtenga información sobre cómo cargar archivos en Adobe Dynamic Media Classic.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 597b7d6bd98c59a644984baeecb888f86a8975c9
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 30%

---

# Carga de archivos{#uploading-files}

Antes de cargar archivos de recursos en Adobe Dynamic Media Classic, asegúrese de que los archivos de recursos tienen un nombre correcto y de que la estructura de carpetas está configurada y organizada del modo que desee. Puede cargar archivos desde un sitio FTP proporcionado por Adobe Dynamic Media Classic o directamente desde el equipo o la red. Adobe Dynamic Media Classic ofrece opciones para optimizar los archivos a medida que se cargan. Si ha instalado la aplicación de escritorio de Adobe Dynamic Media Classic, puede cargar archivos y carpetas arrastrándolos directamente desde el escritorio. Consulte [Configuración general de la aplicación](application-setup.md#general_settings).

## Preparación de recursos y carpetas para su carga {#preparing-your-assets-and-folders-for-uploading}

Antes de cargar recursos en Adobe Dynamic Media Classic, asegúrese de que tengan el formato y el tamaño correctos. También debe observar las reglas de Adobe Dynamic Media Classic para nombrar los recursos. La creación de una estructura de carpetas para los archivos facilita la búsqueda y el uso de éstos.

### Formatos de archivo de recurso admitidos {#supported-asset-file-formats}

En esta tabla se enumeran los formatos de archivo de recursos compatibles con Adobe Dynamic Media Classic. Para obtener información sobre los archivos Camera Raw admitidos, consulte [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Formatos de archivo de recurso | Descripción |
| --- | --- |
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
| Creación de imágenes de Adobe Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

La carga de archivos TAR y ZIP incluye una casilla de verificación para seleccionar si desea descomprimir los archivos.

### Formatos de imagen no compatibles en Dynamic Media {#unsupported-image-formats-dynamic-media}

En la lista siguiente se describen los subtipos de formatos de archivo de imagen rasterizada que son *no* compatible con Dynamic Media.

Consulte también [Detectar formatos de archivo no compatibles para Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Archivos PNG con un tamaño de fragmento IDAT superior a 100 MB.
* Archivos PSB.
* Los archivos de PSD con un espacio de color distinto de CMYK, RGB, escala de grises o mapa de bits no son compatibles. No se admiten los espacios de color DuoTone, Lab e Indexed.
* Archivos PSD con una profundidad de bits superior a 16.
* Archivos de TIFF que tienen datos de punto flotante.
* Archivos de TIFF con espacio de color Lab.

### Tipos de recursos {#asset-types}

Para lograr resultados óptimos con el programa Adobe Dynamic Media Classic, asegúrese de utilizar los formatos y tamaños de archivo recomendados. Esta tabla muestra los tipos de recursos, algunos con los formatos y tamaños de archivos recomendados para los recursos más comunes.

| Tipo de recurso | Descripción/Recomendaciones |
| --- | --- |
| Audio | Los formatos de recursos de audio de entrada incluyen AAC, HE-AAC, AC3, WAV, WMA, AIFF y MP3. Puede transcodificar audio a los formatos siguientes: MP3, AAC y HE-AAC. |
| Imágenes (para cambio de tamaño de imagen, zoom, conjuntos de imágenes, conjuntos de giros) | Las imágenes deben tener al menos 2000 píxeles en el tamaño más largo; los tamaños de imagen típicos oscilan entre 1500 y 2500 píxeles en el tamaño más largo. Se recomiendan los formatos de imagen sin pérdida (incluidos TIFF y PNG). Con imágenes JPEG, use los valores más altos de calidad. Los archivos del GIF de animación se gestionan como cualquier otro contenido estático. |
| Catálogos electrónicos | Utilice archivos de PDF de alta resolución creados en Adobe Acrobat o una aplicación de Creative Suite de Adobe guardada como &quot;preparada para la prensa&quot;. Los archivos PDF incluyen todas las fuentes, imágenes y máscaras requeridas, así como elementos gráficos a los que se hace referencia, ya sea en formato de página única, doble o multipágina. Asigne un nombre alfanumérico a los archivos para ordenar las páginas. Coloque todos los PDF para el catálogo electrónico en una misma carpeta, para facilitar la tarea de carga. Puede seleccionar opciones de recorte para quitar de los archivos marcas de recorte, destinos de registro o barras de color. La mayoría de archivos PDF listos para imprenta utilizan un espacio de color CMYK, por lo que es importante obtener el perfil de color CMYK ICC utilizado con los archivos. |
| Plantillas | Las imágenes o los diseños con capas pueden incluir texto, imágenes y capas. Las capas de imagen, las cadenas de texto y los atributos, tales como el color y tamaño, pueden parametrizarse para personalizar los datos variables. Los requisitos de imagen cuando se utilizan plantillas son los mismos que para otros tipos de imagen. Prepare los gráficos en Photoshop u otro programa de edición de imágenes. Guarde cada gráfico como archivo acoplado transparente, en formato TIFF o PNG. Asegúrese de que la resolución de la imagen es apropiada para el uso previsto. Las imágenes para impresión son de 300 ppp. |
| Vídeos | Adobe Dynamic Media Classic admite archivos de vídeo guardados en formato OGV y MP4. Puede transcodificar los archivos a formato MP4 en el momento de realizar la carga. Consulte [Formatos de archivo de recursos admitidos](#supported-static-file-formats) |
| Fuentes | TrueType cargado, `Type1` (Solo Windows®), OpenType ® fuentes y PhotoFonts. |
| Imágenes | Imágenes y archivos de imagen con capas. |
| Conjuntos de imágenes y conjuntos de muestras | Un conjunto de imágenes se compone de imágenes relacionadas que se pueden mostrar en un visor. |
| Perfiles ICC | Un perfil de color que puede utilizar para convertir una imagen cargada desde su espacio de color de origen a un espacio de color diferente. |
| Viñetas | Imágenes creadas con el programa Image Authoring y archivos relacionados. |
| Archivos de contenido | Archivos de contenido de Adobe InDesign, Illustrator o Photoshop. |
| Archivos FXG | Archivos con formato gráfico independiente de la resolución que puede utilizar para crear plantillas personalizadas para impresión, web, correo electrónico, escritorio y dispositivos. |
| Archivos SVG | Archivos gráficos vectoriales escalables que los servidores para servicio de imágenes pueden procesar. |
| Archivos XML | Archivos que definen reglas de preprocesamiento utilizadas para modificar la ruta y las partes de consulta de las solicitudes. |
| Archivos de hoja de estilos en cascada | Cargue apariencias de CSS para personalizar los visores de HTML5. |
| Archivos JavaScript | Los archivos JavaScript se utilizan en la instrumentación del visor para guardar información de la cuenta. Adobe Security recomienda este tipo de recurso únicamente para las cuentas de cliente que tengan un dominio independiente en uso para la entrega (para evitar scripts entre sitios). |

>[!NOTE]
>
>Al cargar archivos de imagen y PDF en Adobe Dynamic Media Classic, el sistema convierte estos archivos de origen en archivos P-TIFF (TIFF piramidal). Estos TIFF P son los archivos que se publican posteriormente en los servidores de imágenes de Dynamic Media. Adobe Dynamic Media Classic utiliza el formato de archivo Tiff piramidal porque contiene varias relaciones de zoom que permiten un zoom rápido cuando se visualiza con un visor de zoom de Adobe Dynamic Media Classic.

### Formatos de archivo estático compatibles {#supported-static-file-formats}

Adobe Dynamic Media Classic admite varios formatos de archivo estático. El contenido estático es cualquier recurso que se publica &quot;tal cual&quot;, como CSS, PDF, SVG y XML.

Los siguientes tipos de archivo pueden publicarse:

* GIF animado
* Archivos de sonido
* CSS
* JavaScript (cuando la empresa se configura con su propio dominio)
* Vídeo principal
* PDF (cuando el PDF está marcado para publicarse después de la carga, para evitar la entrega de todos los PDF para el flujo de trabajo de catálogo electrónico/PDF existente)
* Vídeo PrX
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic no proporciona la opción de generar una URL de vista previa de contenido estático.

### Requisitos de nombre de archivo {#filename-requirements}

Dado que las extensiones de nombre de archivo se quitan durante el proceso de carga, el sistema no permite que haya archivos con el mismo nombre raíz. En el sistema de Adobe Dynamic Media Classic, el nombre del archivo del recurso menos la extensión del nombre del archivo se convierte en el ID del recurso. Por esta razón no puede haber dos recursos con el mismo nombre.

Asegúrese de que todos los usuarios de su empresa comprendan estas reglas para asignar nombres a los archivos:

* El sistema no admite identificadores de recurso con un nombre idéntico.
* Los nombres de ID de recurso distinguen entre mayúsculas y minúsculas.
* Como práctica recomendada, compruebe que los ID de recursos no contienen espacios en blanco (por ejemplo, chaqueta negra.tif o chaqueta azul.jpg). Adobe Dynamic Media Classic ASCII codifica los espacios en blanco en los nombres de los recursos cuando utiliza nombres de recursos para construir cadenas de URL. Estos códigos ASCII son difíciles de leer, lo que dificulta la lectura de las direcciones URL.
* Los caracteres específicos de idioma están permitidos en los nombres de archivo. No obstante, los siguientes caracteres se permiten en los nombres de archivo:

  \ ; / ? : @ &amp; = + $ , &#42; &quot; &lt; > | &#39; { } %

  Si un nombre de archivo contiene uno o varios de los caracteres anteriores, los caracteres se eliminan del nombre durante la carga.

Normalmente, un nombre de archivo de recurso puede ser el mismo que su número de artículo, SKU de producto u otro nombre, como en el siguiente ejemplo:

| Elemento | Nombre de archivo | ID de recurso |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organización y estructura de carpetas {#folder-organization-and-structure}

Organice y organice carpetas y subcarpetas para el contenido en Adobe Dynamic Media Classic antes de cargar el contenido en el sistema. Esto aporta dos ventajas:

* Al cargar el contenido en Adobe Dynamic Media Classic mediante FTP, puede indicar al sistema que duplique la estructura de carpetas durante la carga. De este modo, el contenido se organiza en las mismas carpetas y subcarpetas de Adobe Dynamic Media Classic que en el equipo o la red. (Para replicar la estructura de carpetas en Adobe Dynamic Media Classic, seleccione la opción Incluir subcarpetas al cargar recursos mediante FTP).
* La reorganización de carpetas dentro del sistema después de cargar los archivos resulta más difícil que un punto de partida con una estructura de carpetas ya probada.

El método de asignación de nombres a carpetas y la estructura que elija para almacenar el contenido en Adobe Dynamic Media Classic dependen de las necesidades de su organización. A continuación se citan algunos ejemplos de estructura de carpetas:

**basado en SKU** : las carpetas se nombran según los SKU o los números de artículo. Por ejemplo, se crean carpetas distintas para las series de números 0-, 20-, 30-, etc.

**Basado en marca** - Para fabricantes con varias líneas de marcas y minoristas que comercializan otras marcas de otras empresas, separe los archivos en carpetas de productos denominadas para diferentes marcas.

**Basado en proyectos** : las carpetas se organizan según la fecha de despliegue o de colocación o el nombre del proyecto. Es el método favorito de los clientes que producen principalmente catálogos electrónicos.

**Espejo de la jerarquía de carpetas del sitio web** : Esta estructura de carpetas refleja la estructura de carpetas del sitio web, con las carpetas denominadas, por ejemplo, para las categorías de productos.

## Acerca de la carga {#uploading-your-files}

Puede cargar archivos individuales desde el escritorio o cargar carpetas mediante FTP. Si desea cargar más de 100 MB de archivos o cargar carpetas y subcarpetas completas, seleccione la opción **A TRAVÉS DE FTP** pestaña.

Adobe Dynamic Media Classic le envía un mensaje de correo electrónico para confirmar cuándo comienza y finaliza el trabajo de carga y para notificarle cualquier problema.

Durante (o inmediatamente después) un trabajo de carga grande, algunos elementos nuevos podían mostrar el mensaje &quot;Imagen aún no optimizada&quot;. Este mensaje aparece porque los archivos aún no se han procesado completamente y no se han agregado a Adobe Dynamic Media Classic. Puede optimizar estos archivos posteriormente. Consulte [Optimización de archivos](application-setup.md#optimize_files).

### Carga de archivos mediante la pestaña Desde el escritorio {#upload-files-using-sps-desktop-application}

La aplicación Adobe Dynamic Media Classic Desktop permite cargar archivos y carpetas arrastrándolos.

1. En la aplicación Adobe Dynamic Media Classic Desktop, en la barra de navegación global, seleccione **[!UICONTROL Cargar]**.
1. En la página Cargar, seleccione **[!UICONTROL Desde el escritorio]** pestaña.
1. En la parte izquierda de la página Cargar, en **[!UICONTROL Seleccionar archivos para cargar]** , seleccione **[!UICONTROL Examinar]** para seleccionar los archivos o carpetas que desea cargar, seleccione **[!UICONTROL Abrir]**.
1. En el lado derecho de la página Cargar, en **Elegir carpeta de destino** , vaya a una carpeta de destino en la que desee agregar los archivos o carpetas cargados.
1. (Opcional) Cerca de la parte inferior de la página Cargar, en el campo de texto Nombre del trabajo, introduzca el nuevo nombre del trabajo de carga. O bien, puede utilizar el nombre predeterminado generado por el sistema que proporciona Adobe Dynamic Media Classic. El trabajo, junto con otros de carga y publicación, se grabará en la página Trabajos, donde puede comprobar el estado de los trabajos. Consulte [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files).
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Publicar tras la carga]** si desea publicar automáticamente los recursos que carga.
Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Esta misma opción también está disponible en el cuadro de diálogo Opciones del trabajo.
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Sobrescribir en cualquier carpeta con mismo nombre de recurso base independientemente de la extensión]** si desea que los archivos que cargue reemplacen a los archivos existentes con los mismos nombres. Esta misma opción también está disponible en el cuadro de diálogo Opciones del trabajo.
El nombre de esta opción podría ser diferente, según la configuración de **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Configuración general]** > **[!UICONTROL Cargar en la aplicación]** > **[!UICONTROL Sobrescribir imágenes]**.
1. Cerca de la esquina inferior derecha de la página Cargar, seleccione **[!UICONTROL Opciones de trabajo]** y, a continuación, especifique las opciones que desee.

   Consulte [Opciones de carga](uploading-files.md#upload_options).

1. En el cuadro de diálogo Opciones del trabajo de carga, seleccione **[!UICONTROL Guardar]**.
1. En la esquina inferior derecha de la página Cargar, seleccione **[!UICONTROL Cargar envío]**.
Para ver el progreso de la carga, seleccione **[!UICONTROL Trabajos]** en la barra de navegación global. Puede seguir trabajando en Adobe Dynamic Media Classic y volver a la página Trabajos en cualquier momento para revisar un trabajo en curso. Para cancelar un trabajo de carga que se encuentre en curso, seleccione **[!UICONTROL Cancelar]** junto al tiempo de duración.

### Carga de archivos mediante la pestaña VIA FTP {#upload-files-using-via-ftp}

1. Inicie sesión en el sitio FTP de Adobe Dynamic Media Classic específico para su región. Utilice el nombre de usuario y la contraseña FTP que ha recibido del administrador.
1. En Adobe Dynamic Media Classic, en la barra de navegación global, seleccione **[!UICONTROL Cargar]**.
1. En la página Cargar, seleccione **[!UICONTROL A TRAVÉS DE FTP]** pestaña.
1. En la parte izquierda de la página Cargar, en **[!UICONTROL Elegir carpeta FTP de carga]** , elija una carpeta FTP desde la que cargar los archivos.
1. En el lado derecho de la página Cargar, en **[!UICONTROL Elegir carpeta Dynamic Media de Adobe de destino]** , elija una carpeta de destino en Adobe Dynamic Media Classic.
1. (Opcional) Cerca de la parte inferior de la página Cargar, en el campo de texto Nombre del trabajo, introduzca el nuevo nombre del trabajo de carga. O bien, puede utilizar el nombre predeterminado generado por el sistema que proporciona Adobe Dynamic Media Classic. El trabajo, junto con otros de carga y publicación, se grabará en la página Trabajos, donde puede comprobar el estado de los trabajos. Consulte [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files).
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Publicar tras la carga]** si desea publicar automáticamente los recursos que carga.
Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Esta misma opción también está disponible en el cuadro de diálogo Opciones del trabajo.
1. (Opcional) Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Sobrescribir en cualquier carpeta con mismo nombre de recurso base independientemente de la extensión]** si desea que los archivos que cargue reemplacen a los archivos existentes con los mismos nombres. Esta misma opción también está disponible en el cuadro de diálogo Opciones del trabajo.
El nombre de esta opción podría ser diferente, según la configuración de **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Configuración general]** > **[!UICONTROL Cargar en la aplicación]** > **[!UICONTROL Sobrescribir imágenes]**.
1. Opcional; sólo disponible si ha seleccionado la variable **[!UICONTROL A TRAVÉS DE FTP]** pestaña. Cerca de la parte inferior de la página Cargar, seleccione **[!UICONTROL Descomprimir archivos Zip o Tar al cargar]** si desea extraer automáticamente todos los archivos del archivo ZIP o TAR cargado. Esta misma opción también está disponible en el cuadro de diálogo Opciones del trabajo.
1. Cerca de la esquina inferior derecha de la página Cargar, seleccione **[!UICONTROL Opciones de trabajo]** y, a continuación, especifique las opciones que desee.

   Consulte [Opciones de carga](uploading-files.md#upload_options).

1. En el cuadro de diálogo Opciones del trabajo de carga, seleccione **[!UICONTROL Guardar]**.
1. En la esquina inferior derecha de la página Cargar, seleccione **[!UICONTROL Cargar envío]**.

   Para ver el progreso de la carga, en la barra de navegación global, seleccione **[!UICONTROL Trabajos]**. La página Trabajos muestra el progreso de la carga. Puede seguir trabajando en Adobe Dynamic Media Classic y volver a la página Trabajos en cualquier momento para revisar un trabajo en curso.

Para cancelar un trabajo de carga que se encuentre en curso, seleccione **[!UICONTROL Cancelar]** junto al tiempo de duración.

## Cuadro de diálogo Cargar opciones de trabajo {#upload-options}

Al cargar archivos, puede elegir entre las siguientes opciones del cuadro de diálogo Opciones del trabajo de carga:

* **TRABAJO** - Seleccionar **[!UICONTROL TRABAJO]** para elegir las opciones que afectan a todo el trabajo de carga.

  También puede elegir *predeterminado* opciones para cargar trabajos mediante la variable **[!UICONTROL Opciones de carga predeterminadas]** en Configuración general. Ir a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Configuración general]** > **[!UICONTROL Opciones de carga predeterminadas]** y, a continuación, establezca las opciones predeterminadas que desee.

   * **[!UICONTROL Cuándo]** : Esta opción solo está disponible si ha seleccionado la variable **[!UICONTROL A TRAVÉS DE FTP]** pestaña.
      * **[!UICONTROL Único]** : especifique un trabajo de carga que se ejecute una vez. Las opciones son las siguientes:
         * **[!UICONTROL Ahora]** : ejecuta el trabajo de carga inmediatamente después de seleccionar **[!UICONTROL Guardar]** en el cuadro de diálogo Opciones de carga de trabajo, seleccione **[!UICONTROL Cargar envío]** en la página Cargar.
         * **[!UICONTROL Programar para más tarde]** : seleccione el año, el mes, el día y la hora (en incrementos de 15 minutos) en los que desea que se ejecute el trabajo de carga.
      * **[!UICONTROL Recurrente]** : especifique un trabajo de carga que se ejecute diariamente, semanalmente o mensualmente. O bien, personalice el trabajo de carga según sus propias especificaciones.
         * **[!UICONTROL Diario]** - Establezca la hora a la que desea que se ejecute el trabajo todos los días. Si desea que el trabajo se ejecute sólo de lunes a viernes, seleccione **[!UICONTROL Solo entre semana]**.
         * **[!UICONTROL Semanalmente]** : elija un día de la semana y una hora específicos a los que desea ejecutar el trabajo.
         * **[!UICONTROL Mensual]** : elija un día específico del mes o de la semana, incluida la hora de inicio, en el que desea ejecutar el trabajo.
         * **[!UICONTROL Personalizado]** : personalice un intervalo de tiempo de trabajo de carga o publicación según sus propias especificaciones. Consulte [Crear un intervalo de tiempo de trabajo de carga o publicación personalizado](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Publicar tras la carga]** - Disponible si ha seleccionado la opción **[!UICONTROL DESDE EL ESCRITORIO]** o la pestaña **[!UICONTROL A TRAVÉS DE FTP]** pestaña. Seleccione esta opción para publicar automáticamente los recursos que cargue. Al publicar archivos, se envían a servidores interactivos. Las URL para estos archivos se pueden utilizar en sitios Web y aplicaciones externas. Esta opción también está disponible en la página de carga.

   * **[!UICONTROL Sobrescribir en cualquier carpeta con mismo nombre de recurso base independientemente de la extensión]** - Disponible si ha seleccionado la opción **[!UICONTROL DESDE EL ESCRITORIO]** o la pestaña **[!UICONTROL A TRAVÉS DE FTP]** pestaña. Seleccione esta opción si desea que los archivos que cargue sustituyan archivos existentes con los mismos nombres. Esta opción también está disponible en la página de carga. El nombre de esta opción podría ser diferente, según la configuración de **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Configuración general]** > **[!UICONTROL Cargar en la aplicación]** > **[!UICONTROL Sobrescribir imágenes]**.

   * **[!UICONTROL Descomprimir archivos Zip o Tar al cargar]** - Disponible si ha seleccionado la opción **[!UICONTROL DESDE EL ESCRITORIO]** o la pestaña **[!UICONTROL A TRAVÉS DE FTP]** pestaña.
Seleccione esta opción si desea extraer automáticamente todos los archivos del archivo ZIP o TAR cargado. Esta misma opción también está disponible en el cuadro de diálogo Opciones del trabajo.

   * **[!UICONTROL Incluir subcarpetas]** - Disponible solo si ha seleccionado la variable **[!UICONTROL A TRAVÉS DE FTP]** pestaña.
Seleccione esta opción si desea cargar subcarpetas de la carpeta que va a cargar. Los nombres de la carpeta y sus subcarpetas que carga se introducen automáticamente en Adobe Dynamic Media Classic.

   * **[!UICONTROL Procesar archivos de metadatos]** - Disponible solo si ha seleccionado la opción **[!UICONTROL A TRAVÉS DE FTP]** pestaña. Seleccione esta opción si desea cargar un archivo delimitado por tabuladores o XML para agregar metadatos a varios recursos. Consulte [Importación de datos (mediante FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Opciones de recorte** : Para recortar automáticamente los píxeles de espacio en blanco de una imagen, abra el **[!UICONTROL Recorte]** menú, seleccione **[!UICONTROL Manual]** y especifique las medidas de los píxeles en los campos de texto Superior, Derecha, Inferior e Izquierda para recortar desde los lados. También puede seleccionar **[!UICONTROL Recortar]** en el menú Recortar y elija estas opciones:

   * **[!UICONTROL Recortar basándose en]** - Elija si desea recortar en función del color o la transparencia:
      * **[!UICONTROL Color]** - Elija la opción Color. A continuación, seleccione el menú Esquina y elija la esquina de la imagen que mejor represente el color de espacio en blanco que desea recortar.
Recorte basado en el color: especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color.
      * **[!UICONTROL Transparencia]** - Elija el **[!UICONTROL Transparencia]** opción.
Recorte basado en la transparencia: especifique 0 para recortar píxeles solo si son transparentes; los números cercanos a 1 permiten una mayor transparencia.
      * **[!UICONTROL Tolerancia]** : Arrastre el regulador para especificar una tolerancia de 0 a 1.

* **Opciones de perfil de color** - Elija una conversión de color cuando cree archivos optimizados que se utilizan para la entrega dinámica de Adobe Dynamic Media Classic:

   * **[!UICONTROL Conservación de color predeterminado]** - Mantiene los colores de la imagen de origen siempre que las imágenes contengan información del espacio de color; no hay conversión de color. Casi todas las imágenes actuales ya tienen incrustado el perfil de color adecuado. Sin embargo, si la imagen de origen CMYK no contiene un perfil de color incrustado, los colores se convierten al espacio de color sRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.
   * **[!UICONTROL Mantener el espacio de color original]** - Conserva los colores originales sin ninguna conversión de color en el punto de ingesta en Adobe Dynamic Media Classic. En el caso de las imágenes sin un perfil de color incrustado, cualquier conversión de color necesaria para procesar las solicitudes de la imagen se realiza mediante los perfiles de color predeterminados, según se ha configurado en la configuración de Publicación. Estos perfiles de color no siempre se alinean con el color en los archivos creados con esta opción. Por lo tanto, se recomienda utilizar la opción Conservación de color predeterminada.
   * **[!UICONTROL Personalizar desde]** > **[!UICONTROL Hasta]** - Abre menús para que pueda elegir una **[!UICONTROL Convertir de]** y **[!UICONTROL Convertir a]** espacio de color. Esta opción avanzada sustituye cualquier información de color incrustada en el archivo de origen. Seleccione esta opción solo cuando todas las imágenes que está enviando contengan datos de perfil de color incorrectos o que falten.

* **Opciones de edición de imágenes** - Puede conservar las máscaras de recorte &lt;> en las imágenes y elegir un perfil de color.
Consulte [Opciones de ajuste de imagen al cargar](image-editing-options-upload.md#image-editing-options-at-upload).

* **opciones de PostScript®** - Puede rasterizar archivos de PostScript®, recortar archivos, mantener fondos transparentes, elegir una resolución y elegir un espacio de color.
Consulte [Uso de archivos PostScript y Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opciones de Photoshop** : puede crear plantillas a partir de archivos de Adobe ® Photoshop®, mantener las capas, especificar cómo se asignan los nombres a las capas, extraer el texto y especificar cómo se anclan las imágenes en las plantillas.
Consulte [Opciones de carga de archivos PSD](psd-files.md#psd_upload_options).

* **Opciones del PDF** : Puede rasterizar los archivos, extraer palabras de búsqueda y vínculos, generar automáticamente un catálogo electrónico, establecer la resolución y elegir un espacio de color.
Consulte [Opciones de carga de PSD](pdfs.md#pdf_upload_options).

* **Opciones de Illustrator** - Puede rasterizar archivos Adobe Illustrator®, mantener fondos transparentes, elegir una resolución y elegir un espacio de color.
Consulte [Uso de archivos PostScript y Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opciones de EVIDEO** - Puede transcodificar un archivo de vídeo seleccionando un ajuste preestablecido de vídeo.
Consulte [Trabajar con ajustes preestablecidos de codificación de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Metadatos adicionales** : introduzca palabras clave que describan los archivos que desea cargar. Separe las palabras clave con una coma. Las palabras clave facilitan la búsqueda de recursos. Consulte [Realización de una búsqueda avanzada](searching-assets.md#conducting_an_advanced_search). Consulte también [Cargar palabras clave](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) vídeo de formación.

* **Ajustes preestablecidos del conjunto de lotes** - Si desea crear un conjunto de imágenes, un conjunto de giros o un conjunto de muestras a partir de los archivos cargados, seleccione la opción **[!UICONTROL Activo]** para el ajuste preestablecido que desea utilizar. Puede seleccionar varios ajustes preestablecidos. Los ajustes preestablecidos se crean en la página Ajustes de aplicación/Valores preestablecidos de conjunto por lotes.
Consulte [Valores preestablecidos de conjunto por lotes](application-setup.md#batch_set_presets).

* **Avanzadas** - Consulte [Seguir una carga con otro trabajo](uploading-files.md#follow-an-upload-with-another-job).

## Ejecución de trabajos a continuación de la carga {#follow-an-upload-with-another-job}

Cuando cargue elementos mediante FTP, puede programar un trabajo posterior para que comience cuando se complete la carga. Si hay otros trabajos programados para comenzar, el trabajo que programa aquí se pone en cola después de ellos.

El nuevo trabajo envía una notificación a la dirección especificada para que se pueda activar el código de esa ubicación. Este trabajo de publicación que sigue recibe el mismo nombre que el trabajo de carga pero se le añade el prefijo *Pub_*.

**Para seguir una carga con otro trabajo:**

1. Seleccionar **[!UICONTROL Cargar]**, luego seleccione la **[!UICONTROL A TRAVÉS DE FTP]** pestaña.
1. En la esquina inferior derecha de la página Cargar, seleccione **[!UICONTROL Opciones de trabajo]**.
1. En el cuadro de diálogo Opciones del trabajo de carga, expanda **[!UICONTROL AVANZADO]** sección.
1. Elija una de las siguientes opciones de la **[!UICONTROL Seguir carga con otro trabajo]** lista desplegable:

   * Ninguno
   * Solicitud HTTP
   * Publicación para servicio de imágenes
   * Procesador de imágenes
   * Publicación de vídeo

1. Especifique la dirección HTTP.
1. Especifique si desea ejecutar solo si los archivos se han cargado.
1. Indique si desea ejecutar esta solicitud cada vez que termine este trabajo o solo si se han publicado archivos.

   >[!NOTE]
   >
   >Los trabajos programados con regularidad a veces pueden hacer que no se publique ningún archivo.

>[!MORELIKETHIS]
>
>* [Trabajo con carpetas de recursos](asset-folders.md#working_with_asset_folders)
>* [Gestión de trabajos recurrentes de carga y publicación](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Uso de un trabajo de carga o publicación como déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
