---
title: Ajustes de aplicación
seo-title: Ajustes de aplicación
description: Obtenga información sobre cómo configurar el área de aplicación de Dynamic Media Classic.
seo-description: Obtenga información sobre cómo configurar el área de aplicación de Dynamic Media Classic.
uuid: 3e2f1d30-8f33-4a9d-bbe4-e8c3dbc968f8
contentOwner: admin
content-type: referencia
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: ae2d1895-a437-4463-bface-3960c8027551
translation-type: tm+mt
source-git-commit: 8216ac64ba418987c7f5ed84c4cb957189645bd9

---


# Ajustes de aplicación{#application-setup}

Puede utilizar las páginas Ajustes de aplicación para introducir ajustes generales, crear ajustes preestablecidos de imagen, ajustes preestablecidos de codificación de vídeo, ajustes preestablecidos de visor o definir visores predeterminados y metadatos. También puede configurar ajustes preestablecidos de conjuntos de lotes para automatizar, por ejemplo, la creación de conjuntos de giros 2D, la configuración de publicación y la configuración de la optimización para motores de búsqueda de vídeos.

>[!NOTE]
>
>Solo los administradores de Scene7 Publishing System pueden cambiar la configuración de las páginas Ajustes de aplicación.

## Configuración general {#general-settings}

To open the Application General Settings page, on the Global Navigation bar, click **[!UICONTROL Setup &gt; Application Setup &gt; General Settings]**.

### Servidores

Al crear la cuenta, Dynamic Media Classic proporciona automáticamente los servidores asignados a la empresa. Estos servidores se utilizan para crear cadenas URL para su página web y sus aplicaciones. Estas llamadas mediante URL son específicas para su cuenta.

Consulte también [Prueba del servicio Secure Testing](testing-assets-making-them-public.md#testing_the_secure_testing_service).

**Nombre** del servidor publicado Este servidor es el servidor CDN activo que se utiliza en todas las llamadas URL generadas por el sistema específicas de su cuenta. No cambie este nombre de servidor a menos que un técnico de soporte de Dynamic Media Classic le indique que lo haga.

**Nombre** del servidor de origen Este servidor se utiliza solamente para la prueba de control de calidad. No cambie este nombre de servidor a menos que un técnico de soporte de Dynamic Media Classic le indique que lo haga.

**Nombre** del servidor AGM Este servidor se utiliza para plantillas de impresión virtual. Este servidor se configura para toda la empresa. No cambie este nombre de servidor a menos que un técnico de soporte de Dynamic Media Classic le indique que lo haga.

**Nombre** del servidor de Test&amp;Target Su URL de Test&amp;Target, hasta .com inclusive. Para obtener instrucciones sobre cómo obtener esta URL, consulte Integración de Dynamic Media Classic con Target Classic.

**Nombre** del servidor de flujo iOS La URL de su servidor de flujo iOS de Dynamic Media Classic. Este servidor ofrece transmisión de vídeo para los dispositivos basados en iOS utilizando el protocolo HTTP.

**Nombre** del servidor de vídeo progresivo La URL de su servidor de vídeo progresivo de Dynamic Media Classic. Este servidor ofrece vídeo progresivo utilizando el protocolo HTTP.

**Mostrar URL para recursos** sin publicar Seleccione esta opción si desea que Dynamic Media Classic muestre una URL al obtener una vista previa de cualquier recurso, esté publicado o no. Si el recurso no está publicado, la URL no funciona. Sin embargo, puede utilizar la dirección URL para fines de planificación o de organización.

**Permitir la instalación** de AIR Seleccione esta opción para permitir a los usuarios descargar la versión de escritorio de Scene7 Publishing System en sus discos duros locales. Los usuarios instalan la aplicación desde el área Versión de escritorio de la pantalla Ajustes personales.

Los usuarios de AIR deben desinstalar manualmente la aplicación existente y volver a la instalarla desde la versión web de Scene7 Publishing System (en Configuración personal). Tras esta reinstalación puntual, se le pide que ejecute la actualización cada vez que el servidor disponga de una versión nueva de Scene7 Publishing System AIR. Scene7 Publishing System está integrado con el marco de actualización de la aplicación que facilita el proceso de actualización.

**Plantilla** de invalidación de CDN Especifica la plantilla que se utiliza para invalidar la caché de CDN (red de entrega de contenido).

For example, suppose you enter an image URL (including image presets or modifiers) referencing `<ID>`, instead of a specific image ID as in the following example:

`https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

If the Template just contains `<ID>`, then SPS fills in the `https://<server>/is/image`, where `<server>` is the Publish Server Name that is defined in General Settings.

Si se define una plantilla de inutilización de CDN, se selecciona una imagen con el nombre Backpack_B y se hace clic en **Archivo** &gt; **Inutilizar en CDN**, se crea la siguiente URL en la interfaz de inutilización de CDN:

`https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

En el cuadro de lista de URL, haga clic en **Continuar** para borrar la caché de esa llamada de URL a la imagen específica. Tenga en cuenta que también puede agregar una URL escribiéndola o pegándola en el cuadro de lista de URL, por lo que no es necesario establecer la plantilla por adelantado.

Después de seleccionar la plantilla de inutilización de CDN y realizar la solicitud de Inutilizar en CDN, aparecerá un indicador en la interfaz de usuario que le proporciona una idea de cuánto tiempo tardará en borrarse la caché.

Del mismo modo, si se seleccionan varias imágenes de SPS cuando se hace clic en **Archivo** &gt; **Inutilizar en CDN**, se hace referencia a cada imagen en la plantilla URL guardada. Por lo tanto, se puede definir una plantilla de invalidación de CDN que haga referencia a cada URL a la que se hace referencia en su sitio web (por ejemplo, los detalles del producto, los resultados de la búsqueda, etc.). A continuación, cuando se seleccione una o varias imágenes para la invalidación desde la caché, las direcciones URL rellenan automáticamente la interfaz.

Consulte [Caché de contenido](scene7-platform-overview.md#content_caching).

Consulte [Segunda publicación de recursos y retrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

**Examinar**

**Mostrar proyectos** Determina si los proyectos están disponibles como medio para organizar los recursos de Dynamic Media Classic. Consulte Organización del trabajo con proyectos.

**Mostrar contenido** de eVideo de muestra Active o desactive la visualización del contenido de muestra de eVideo.

**Mostrar contenido** generado En carpetas, muestra el contenido generado a partir de un recurso. Por ejemplo, cuando se rasteriza un archivo PDF a medida que se carga, Dynamic Media Classic crea una imagen para cada página del PDF original. Si la opción Mostrar contenido generado está seleccionada, cada imagen generada durante la carga del PDF original aparecerá junto con el PDF en la carpeta en la que se cargó.

**Mostrar vídeos** codificados sin seleccionar (desactivado) de forma predeterminada.

Para buscar vídeos rápidamente en Scene7 Publishing System sin tener que navegar por varios derivados codificados del mismo vídeo, deje esta opción sin seleccionar (predeterminada). En la interfaz de usuario solo se muestra la miniatura del Vídeo principal, que es el vídeo de origen que ha cargado y utilizado para crear todos los derivados, y la miniatura del Conjunto de vídeos adaptable “principal”, que contiene todos los derivados “secundarios” del conjunto de vídeos codificado.

Sin embargo, puede seguir teniendo acceso a vídeos codificados individuales en el vídeo principal o en el conjunto de vídeos adaptable. Para ello, haga doble clic en la imagen en miniatura del vídeo para abrir la vista de detalles. A continuación, haga clic en **Vídeos codificados** en el panel derecho para tener acceso a todos los vídeos "secundarios".

También puede utilizar **Archivo &gt; Volver a procesar** para crear más vídeos "secundarios" codificados directamente desde un conjunto de vídeos adaptable. Scene7 Publishing System busca automáticamente el vídeo "principal" del conjunto adaptable y lo utiliza como vídeo de origen en la transcodificación. Sin embargo, cuando se guardan los nuevos vídeos codificados individuales, estos no se ven al buscar o examinar un elemento. No obstante, siguen siendo accesibles desde la ficha Vídeos codificados en la vista de detalles.

Consulte [Carga y transcodificación de vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

Para mantener la capacidad de tener acceso a todos los derivados del vídeo codificado al buscar y examinar, seleccione **Mostrar vídeos codificados**.

Hay ciertas acciones en el menú Generar que solo funcionan, o funcionan de forma opcional, con vídeos individuales. Esta funcionalidad hace que sea necesario mostrar todos los derivados de vídeos codificados que pueda seleccionar, independientemente de cómo haya definido la opción **Mostrar vídeos codificados**. The Build actions that over-ride the **Show Encoded Videos** setting include **Adaptive Video Sets**, and **eCatalogs**.

>[Nota]
>
>Si no ha utilizado Scene7 Publishing System para cargar y codificar recursos de vídeo, Dynamic Media Classic muestra todos los vídeos codificados individuales, aunque esta opción no esté seleccionada.

**Mostrar botón** Actualizar subcarpetas Active o desactive la visualización del botón Actualizar subcarpetas.

**Cuenta de FTP de Dynamic Media Classic**

**Servidor** Muestra el servidor de cuentas FTP.

**Nombre** de usuario Muestra el nombre de usuario de la cuenta de FTP.

**Cargar a la aplicación**

**Sobrescribir imágenes** Dynamic Media Classic no permite que dos archivos tengan el mismo nombre. El ID de Scene7 Publishing System de cada elemento (el nombre de la imagen menos la extensión de nombre de archivo) debe ser único. Debido a esta regla, el cuadro de diálogo Cargar dispone de una opción Sobrescribir. El efecto exacto de esta opción depende de la opción Sobrescribir imágenes especificada. Estas opciones especifican cómo se cargan las imágenes de sustitución: si sustituyen las imágenes originales o si se convierten en imágenes duplicadas. En el caso de las imágenes duplicadas, se cambia su nombre agregando “-1” (por ejemplo, el nombre silla.tif se cambia a silla-1.tif). Estas opciones también afectan a las imágenes cargadas en una carpeta distinta de la original o a las imágenes con una extensión de nombre de archivo diferente de la original (como JPG, TIF o PNG). (Consulte Uso de la opción Sobrescribir imágenes).

**Sobrescribir en la carpeta actual. El nombre base y la extensión de la imagen deben ser los mismos**

Esta opción supone la regla más estricta de sustitución. Exige que la imagen de sustitución se cargue en la misma carpeta y tenga la misma extensión de nombre de archivo que la imagen original. Si no se cumplen estos requisitos, se crea un duplicado.

**Sobrescribir en la carpeta actual. El nombre base del recurso debe ser el mismo, independientemente de su extensión**

Exige que la imagen de sustitución se cargue en la misma carpeta que la imagen original. Sin embargo, la extensión de nombre de archivo puede ser distinta de la original. Por ejemplo, silla.tif sustituye silla.jpg.

**Sobrescribir en cualquier carpeta. La extensión y el nombre base del recurso deben ser los mismos**

Exige que la imagen de sustitución tenga la misma extensión de nombre de archivo que la imagen original (por ejemplo, silla.jpg debe sustituir a silla.jpg, no silla.tif). Sin embargo, puede cargar la imagen de sustitución en otra carpeta distinta de la original. La imagen actualizada reside en la nueva carpeta; el archivo ya no se encuentra en su ubicación original.

**Sobrescribir en cualquier carpeta. El nombre base del recurso debe ser el mismo, independientemente de su extensión**

Esta opción supone la regla de sustitución menos excluyente. Puede cargar la imagen de sustitución en otra carpeta distinta de la original, cargar un archivo con una extensión de nombre de archivo diferente y sustituir el archivo original. Si el archivo original está en otra carpeta, la imagen de sustitución residirá en la nueva carpeta en la que se haya cargado.

**Conservar publicación** Especifica si una imagen de sustitución cargada en Dynamic Media Classic conserva la configuración Listo para publicar de la imagen que está reemplazando o si la configuración se especifica al cargar.

**Perfiles** de color predeterminados Especifica los perfiles de color aplicados como parte de Opciones de perfil de color predeterminadas al agregar imágenes CMYK.

**Opciones** de carga predeterminadas Abre el cuadro de diálogo Opciones de trabajo de carga, donde puede especificar las opciones de carga predeterminadas. Para obtener información sobre estas opciones, consulte Opciones de carga.

**Editor de mapas de imagen, a aplicación**

**HREF** de asignación de imágenes predeterminada Define la dirección URL predeterminada que se utiliza para la columna href de asignación de imágenes. Es la dirección URL predeterminada que se muestra cuando se crean mapas de imagen.

**Plantilla** de asignación de imágenes predeterminada Define el JavaScript predeterminado para la plantilla href de asignación de imágenes. Puede especificar el código personalizado que se debe ejecutar al hacer clic en un mapa de imagen.

**Otras opciones, a aplicación**

**La papelera puede limpiar los recursos de advertencias** de la papelera se eliminan automáticamente en un plazo de siete días. Seleccione “Enviar correos electrónicos antes de que los elementos de la papelera se eliminen automáticamente” si desea que se envíen notificaciones a los administradores de la empresa cuando falten cuatro días para que los recursos que hay en la papelera se eliminen de forma permanente. Consulte Gestión de la carpeta Papelera.

## Uso de la opción Sobrescribir imágenes {#using-the-overwrite-images-option}

Dynamic Media Classic no permite que dos archivos tengan el mismo nombre. El ID de Scene7 Publishing System de cada elemento (el nombre de la imagen menos la extensión de nombre de archivo) debe ser único. Debido a esta regla, el cuadro de diálogo Cargar incluye las opciones Sobrescribir imágenes. El efecto exacto de esta opción depende de un ajuste de configuración interna de Scene7 Publishing System de cada empresa.

Si previamente ha cargado las imágenes y, a continuación, ha cambiado los archivos originales (o los ha reemplazado), la opción Sobrescribir seleccionada especifica cómo se reemplazan las imágenes con Dynamic Media Classic. No se modifica ningún dato referente a la imagen sino que la nueva imagen sustituye la antigua. Si la carpeta también contiene imágenes que aún no están en Dynamic Media Classic, se agregan.

Use esta opción si las imágenes cargadas han sufrido alguna variación (por ejemplo, se ha alterado una imagen) pero la referencia a ellas permanece igual. La sobreescritura también resulta de utilidad a la hora de cargar y extraer archivos PDF de Adobe®. To fine-tune how Dynamic Media Classic *rips* the image, adjust the ICC color profile options in the Upload dialog box and re-upload using the Overwrite feature.

Los ID de Dynamic Media Classic que se utilizan para acceder a las imágenes desde los servidores de producción se derivan de los nombres de archivo de imagen. El uso de caracteres en mayúsculas y minúsculas en el nombre del archivo es importante, tanto para la sustitución de archivos existentes como para los ID de Dynamic Media Classic utilizados para acceder a la imagen. Asegúrese de que el uso de caracteres en mayúsculas y minúsculas en los nombres de archivo es correcto antes de cargarlos en Dynamic Media Classic para evitar que los ID de Dynamic Media Classic solo difieran en el caso de la misma imagen.

Al anular la selección de esta opción, todas las imágenes que tengan los mismos nombres de archivo como imágenes existentes se tratan como duplicados y, por consiguiente, no se agregan.

## Ajustes preestablecidos de imagen {#image-presets}

En la pantalla Ajustes preestablecidos de imagen se pueden crear y editar ajustes preestablecidos de imagen. Los ajustes preestablecidos de imagen permiten a Dynamic Media Classic distribuir imágenes de forma dinámica en diferentes tamaños desde la misma imagen principal. Cada ajuste preestablecido de imagen representa una serie de comandos predefinidos de formato y tamaño que determinan la presentación de las imágenes. Cuando se crea un ajuste preestablecido de imagen, debe elegir un tamaño para la distribución de imágenes. También se deben escoger los comandos de formato para que se optimice el aspecto de la imagen al distribuirla para su visualización.

Los administradores pueden crear ajustes preestablecidos para exportar recursos. Los usuarios pueden elegir un ajuste preestablecido al exportar imágenes, lo que corrige el formato de las imágenes de acuerdo con las especificaciones del administrador.

To open the Image Preset screen, on the Global Navigation bar, click **Setup** &gt; **Image Presets**.

Consulte Imágenes [inteligentes](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

### Creación y edición de ajustes preestablecidos de imagen {#creating-and-editing-image-presets}

1. Haga clic en **Ajustes** &gt; **Ajustes preestablecidos de imagen**.
1. Cree un ajuste preestablecido nuevo o empiece a partir de un ajuste preestablecido existente:
   * **Creación de un ajuste preestablecido** de imagen: haga clic en **Agregar**.
   * **Creación de un ajuste preestablecido de imagen a partir de un ajuste preestablecido** existente: seleccione el ajuste preestablecido de imagen más parecido al que desea crear y, a continuación, haga clic en Editar.

1. En la pantalla de adición (o de edición) del ajuste preestablecido, introduzca el nombre que desea darle al ajuste preestablecido.
1. Defina las opciones de ajustes preestablecidos que desea. 

   Consulte [Opciones de ajuste preestablecido de imagen](application-setup.md#image_preset_options).

1. Click **Save**, or if you started from an existing preset, click **Save As**.
1. To preview the preset with your own image, click **Browse** and then select an image. To preview with the default image, click **Reset**.

Puede editar un ajuste preestablecido de imagen si selecciona su nombre en la pantalla Ajustes preestablecidos de imagen y luego hace clic en Editar. Para eliminar un ajuste preestablecido de imagen, selecciónelo y, a continuación, haga clic en Eliminar.

### Opciones de ajuste preestablecido de imagen {#image-preset-options}

En las pantallas de adición y edición de ajustes preestablecidos, encontrará las siguientes opciones de creación y edición de ajustes preestablecidos de imagen:

**Nombre** de ajuste preestablecido Introduzca un nombre descriptivo sin espacios en blanco. Incluya la especificación de tamaño de imagen en el nombre para ayudar a los usuarios a identificar el ajuste preestablecido de imagen.

**Anchura y altura** Introduzca en píxeles el tamaño en el que se distribuye la imagen.

**Formato** Elija un formato en el menú. Al elegir el formato GIF, JPEG, PDF o TIFF, aparecen más opciones:

* Opciones de Cuantificación de color GIF

   **Tipo**

   Seleccione Adaptable (opción predeterminada), Web o Macintosh. Si elige GIF con Alpha, la opción Macintosh® no estará disponible.

   **Tramado**

   Elija entre Difuso o Desactivado.

   **Número de colores**

   Arrastre el control deslizante para introducir 2-255.

   **Lista de colores**

   Escriba una lista separada por comas. Por ejemplo, para blanco, gris y negro, introduzca 000000,888888,ffffff.

* Opciones JPEG

   **Calidad**

   Controla el nivel de compresión JPEG. Esta configuración afecta tanto al tamaño como a la calidad de la imagen. La escala de calidad JPEG es de 1 a 100.

   **Activar disminución de resolución de crominancia JPEG**

   Puesto que el ojo es menos sensible a la información de color de alta frecuencia que a la luminancia de alta frecuencia, las imágenes JPEG dividen la información de la imagen en componentes de color y de luminancia. Al comprimir una imagen JPEG, el componente de luminancia conserva la totalidad de su resolución, mientras que la resolución de los componentes de color se disminuye mediante promedios de grupos de píxeles. La disminución de resolución le resta una mitad o un tercio al volumen de los datos sin tener casi ningún impacto en la calidad percibida. La disminución de resolución no se aplica a las imágenes en escala de grises. Esta técnica reduce la cantidad de compresión, lo cual resulta útil para las imágenes de mayor contraste (por ejemplo, las imágenes con texto superpuesto).

* Opciones PDF y TIFF

   **Compresión**

   Elija un algoritmo de compresión.

**Espacio de color** Elija un espacio de color.

**Enfoque** Seleccione la opción Activar enfoque simple para aplicar un filtro de enfoque básico a la imagen una vez que se haya realizado todo el ajuste de escala. El enfoque puede ayudar a ver mejor las imágenes borrosas que se obtienen al mostrar una imagen en un tamaño diferente. 

Para obtener más información acerca del enfoque, los modos de remuestreo y la máscara de enfoque, consulte [Enfoque de imágenes](sharpening-image.md#sharpening_an_image).

**Modo** de remuestreo Elija una opción de modo de remuestreo. Estas opciones pueden enfocar la imagen cuando se disminuye su resolución:

**B-Lineal** El método de remuestreo más rápido; se pueden apreciar algunos artefactos de solapamiento.

**Bicúbico** Aumenta el uso de CPU en el servidor de imágenes, pero genera imágenes más nítidas con artefactos de solapamiento menos notables.

**Sharp2** Puede producir resultados ligeramente más nítidos que la opción Bicúbico, pero con un costo de CPU aún mayor en el servidor de imágenes.

**Tri-Linear** Utiliza tanto resoluciones altas como resoluciones inferiores, si está disponible; solo se recomienda cuando el solapamiento sea un problema. Este método reduce el tamaño JPEG debido a la reducción de datos de alta frecuencia.

**Máscara** de enfoque Elija estas opciones para ajustar el enfoque:

**Cantidad** Controla la cantidad de contraste aplicado a los píxeles del borde. El valor predeterminado es 1,0. En las imágenes de alta resolución, puede aumentarse hasta 5,0. La cantidad equivaldría a la medida de la intensidad del filtro.

**Radio** Determina el número de píxeles que rodean los píxeles del borde que afectan al enfoque. Para las imágenes de alta resolución, introduzca una cantidad de 1 a 2. Un valor bajo aplica enfoque solo a los píxeles de borde; un valor alto aplica enfoque a un mayor número de píxeles. El valor adecuado depende del tamaño de la imagen.

**Umbral** Determina el rango de contraste que se debe ignorar al aplicar el filtro de máscara de enfoque. Es decir, esta opción determina en qué deben diferenciarse los píxeles enfocados del área que los rodea antes de ser considerados píxeles de borde y por tanto enfocados. Para evitar la introducción de ruido, experimente con valores entre 0,02 y 0,2. El valor predeterminado (6) aplica enfoque a todos los píxeles de la imagen.

**Espacio** de colorDetermina si la imagen utiliza el espacio en el que se creó, normalmente RGB (Original) o un espacio de luminancia (Intensidad).

**Color** Elija estas opciones:

**Perfil** de color de salida Seleccione Usar predeterminado o uno de los perfiles de color ICC disponibles en Scene7 Publishing System.

Consulte también [Perfiles ICC](icc-profiles.md#icc_profiles).

**Calidad** de representación Seleccione una opción si desea anular la interpretación predeterminada del perfil de color. Utilice esta opción cuando uno de los perfiles ICC predeterminados es el espacio de color de destino en una conversión de color, un dispositivo de salida (impresora o monitor) está caracterizado por este perfil y la interpretación especificada es válida para este perfil.

**Incrustar perfil** Seleccione esta opción para que, si abre esta imagen en Adobe® Photoshop®, utilice este perfil.

**Resolución** de impresión Elija una resolución para imprimir esta imagen; 72 píxeles es el valor predeterminado.

**Modificadores** de URL Si prefiere especificar los modificadores de URL que definen el ajuste preestablecido de imagen en lugar de la configuración, introduzca los modificadores aquí.

**URL** de imagen de ejemplo Muestra la cadena URL "sin procesar" que utiliza el servidor de imágenes de Dynamic Media para distribuir imágenes con el ajuste preestablecido de imagen que está agregando o editando. Esta cadena URL codifica la configuración de formato seleccionada en las pantallas de adición o de edición de ajustes preestablecidos.

### Edición, eliminación o desactivación de un ajuste preestablecido de imagen {#editing-removing-or-deactivating-an-image-preset}

1. Haga clic en **Ajustes** &gt; **Ajustes preestablecidos de imagen**.
1. En la pantalla Ajustes preestablecidos de imagen, seleccione un ajuste preestablecido de la tabla y, a continuación, realice una de las siguientes acciones:

   * Click **Edit** and then specify new options in the Edit Preset dialog box.
   * Click **Delete** to remove the preset from the list.
   * Anule la selección de la casilla de verificación Activo que hay junto al nombre de un ajuste preestablecido para quitarlo de toda la interfaz de usuario de Scene7 Publishing System para los usuarios de Media Portal.

## Activación o desactivación de los ajustes preestablecidos de vídeos adaptables {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic ofrece ajustes preestablecidos de codificación de vídeo adaptable. Es una lista maestra de ajustes preestablecidos que combina ajustes preestablecidos de vídeo adaptable de 16:9 y ajustes preestablecidos de vídeo adaptable de 4:3 en un grupo. Estos ajustes preestablecidos predefinidos reflejan la configuración de codificación más común y se han optimizado para la reproducción en dispositivos móviles, tablets y escritorios.

De forma predeterminada solo se activan (habilitan o “encienden”) los ajustes preestablecidos de codificación de “Vídeo adaptable”. Puede desactivarlos, si lo desea. Los ajustes preestablecidos de vídeos adaptables inactivos no aparecen como una opción seleccionable en la sección eVideo del cuadro de diálogo Opciones de trabajo de carga.

Consulte [Carga y codificación de vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Para activar y desactivar ajustes preestablecidos de vídeos adaptables**

1. Cerca de la esquina superior derecha de Scene7 Publishing System, haga clic en **Ajustes** &gt; **Configuración de aplicaciones** &gt; **Ajustes preestablecidos de vídeo** &gt; **Ajustes preestablecidos de vídeo adaptables**.
1. En la página Ajustes preestablecidos de vídeo, anule la selección de la casilla de verificación situada junto al nombre de un ajuste preestablecido para quitarlo de la lista Opciones de eVideo del cuadro de diálogo Opciones de trabajo de carga.
1. Haga clic en **Cerrar**.

## Ajustes preestablecidos de vídeo para la codificación de archivos de vídeo {#video-presets-for-encoding-video-files}

Para seleccionar un ajuste preestablecido de codificación, haga clic en Opc. de trabajo en la esquina inferior derecha de la página de carga. En el cuadro de diálogo Opciones de trabajo de carga, expanda Opciones de eVideo y elija los ajustes preestablecidos de codificación de vídeo que desee.

>[!NOTE]
>
>Aparte de “Vídeo adaptable”, que está activado de forma predeterminada, puede ser que no vea todos los ajustes preestablecidos de codificación única o de vídeos adaptables en el cuadro de diálogo Opciones de trabajo de carga. Los administradores de Dynamic Media Classic determinan los ajustes preestablecidos de codificación de vídeo visibles en el cuadro de diálogo Opciones de trabajo de carga.

* Elija entre los siguientes ajustes preestablecidos de codificación de vídeo adaptable o a ajustes preestablecidos de codificación única:

   **Vídeo adaptable 16:9**

   Cree vídeos con una proporción de aspecto de 16:9 para su distribución en equipos de escritorio, móviles (iPhone, iPad, Android) y tablets (iPad, Android), optimizados con la resolución y la velocidad de bits que mejor se ajusten a la velocidad de conexión del visor.

   **Vídeo adaptable 4:3**

   Cree vídeos con una proporción de aspecto de 4:3 para su distribución en equipos de escritorio, móviles (iPhone, iPad, Android) y tablets (iPad, Android), optimizados con la resolución y la velocidad de bits que mejor se ajusten a la velocidad de conexión del visor.

   **Vídeo adaptable**

   Un ajuste preestablecido de codificación única que funciona con cualquier proporción de aspecto para crear vídeos para su distribución en teléfonos móviles, tablets y equipos de escritorio. Los vídeos originales cargados que se hayan codificado con este ajuste preestablecido se definirán con una altura fija. Sin embargo, la anchura se escalará automáticamente para mantener la proporción de aspecto del vídeo.

   Esta flexibilidad de tener una “Escala automática” también está disponible de forma predeterminada al crear su propio ajuste preestablecido de codificación de vídeo personalizado.

   Consulte [Adición o edición de un ajuste preestablecido de codificación de vídeo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   **Codificación de vídeo adaptable (16:9 o 4:3)**

   Cree vídeos con una proporción de aspecto de 16:9 y 4:3 para su distribución en equipos de escritorio, móviles (iPhone, iPad, Android) y tablets (iPad, Android), optimizados con la resolución y la velocidad de bits que mejor se ajusten a la velocidad de conexión del visor.

   Consulte [Ajustes preestablecidos de vídeo de codificación de vídeo adaptable (16:9 o 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)

   **Ajustes preestablecidos de codificación única**

   >[NOTA]
   >
   >Para publicar vídeo en iPad, puede elegir un ajuste preestablecido de codificación Móvil o Tablet. Los ajustes preestablecidos Tablet están diseñados específicamente para iPad, normalmente con mayor resolución y calidad para aprovechar el tamaño de pantalla más grande y la conexión de ancho de banda más alta. La publicación de archivos de vídeo codificados con un ajuste preestablecido Tablet requiere la inclusión de código de detección de dispositivo en la aplicación o sitio móvil. Este código cambia entre la visualización de vídeo en iPhone o iPad, según el dispositivo de reproducción. Si se selecciona un ajuste preestablecido Móvil para la publicación de archivos de vídeo en iPad, el flujo de trabajo es más simple. El motivo es que puede utilizar el mismo archivo de vídeo para iPhone e iPad. Sin embargo, la calidad se estandariza a la visualización de iPhone de menor resolución.

   * En el grupo Ajustes preestablecidos de codificación, en la lista desplegable Ordenar valores preestablecidos de codificación, seleccione Nombre o Tamaño para ordenar los ajustes preestablecidos por el nombre o el tamaño de resolución.
   * Al elegir el ajuste preestablecido de codificación, tenga en cuenta el tamaño de resolución y el ancho de banda con los que se va a reproducir el vídeo. 
   * Puede seleccionar la codificación de vídeo adaptable y uno o más ajustes preestablecidos de vídeo. Por ejemplo, puede codificar un archivo para escritorio o dispositivo móvil en un trabajo de carga.

Después de hacer clic en **Iniciar carga**, se carga el archivo de vídeo maestro original y se generan a partir de él los archivos codificados.

### Acerca de las opciones de ajustes preestablecidos de codificación {#about-encoding-preset-options}

Los parámetros de las opciones de ajustes preestablecidos de codificación son los siguientes:

**Velocidad** de conexión de Target La velocidad de conexión a Internet del usuario final de destino.

**Sufijo** de archivo codificado El sufijo que se adjunta al archivo de vídeo codificado para fines de identificación.

**Velocidad de bits de vídeo (velocidad de datos)** Cantidad de datos codificados para configurar un solo segundo de reproducción de vídeo (en kilobits por segundo).

**Anchura y altura** de píxeles La dimensión de anchura de la imagen de pantalla, en píxeles; dimensión de altura de la imagen de pantalla (en píxeles).

**Fotograma por segundo (fps)** El número de fotogramas o imágenes fijas para cada segundo de vídeo. En Estados Unidos y Japón, la mayoría de los vídeos se graban a 29,97 fps; en Europa y Asia (excluido Japón), la mayoría se graba a 25 fps. Las películas se graban a 24 fps.

**Velocidad** de bits de audio La cantidad de datos codificados para configurar un solo segundo de reproducción de audio, en kilobits por segundo.

En las siguientes tablas se muestran las mejores prácticas recomendadas para seleccionar ajustes preestablecidos de vídeo y las convenciones de designación que se utilizan para dar nombre a los archivos codificados.

### Vídeo adaptable (predeterminado) {#adaptive-video-default}

Un ajuste preestablecido de codificación que funciona con cualquier proporción de aspecto para crear vídeos para su distribución en teléfonos móviles, tablets y equipos de escritorio. Los vídeos originales cargados que se codifiquen con este ajuste preestablecido (valor predeterminado y una práctica recomendada) se definen con una altura fija, mientras que la anchura se escala automáticamente para mantener la proporción de aspecto del vídeo.

**Vídeo adaptable (predeterminado)**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Automático x360, 800 kbps | _Mobile_Autox360p_800K | 800 | Autox360 | Igual que el origen | 64 | Para móvil (iPhone, iPad, Android) |
| 2 | Automático x 480, 1400 kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | Igual que el origen | 96 | Para tablet (iPad, Android) |
| 3 | Automático x 720, 2600 kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | Igual que el origen | 128 | Para escritorio |

### Ajustes preestablecidos de vídeo de codificación de vídeo adaptable (16:9 o 4:3){#adaptive-video-encoding-or-video-presets}

Estos ajustes preestablecidos de codificación de vídeo adaptable combinan una serie de ajustes preestablecidos de codificación individuales que se seleccionan automáticamente en función de la proporción de vídeo que cargue. Por ejemplo, si carga un vídeo de 4:3, se codificará automáticamente con los cinco ajustes preestablecidos de 4:3 de la lista maestra de ajustes preestablecidos en la opción **Codificación de vídeo adaptable (16:9 o 4:3)** .

Para obtener más información sobre los parámetros de las opciones de codificación, consulte [Acerca de las opciones de ajustes preestablecidos de codificación](application-setup.md#about_encoding_preset_options).

**Ajustes preestablecidos de codificación de vídeo adaptable (16:9 o 4:3)**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 51 2 x 288, Móvil (iPhone, iPad, Android), (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 2 | 4:3, 384 x 288 px, Móvil (iPhone, iPad, Android), (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 3 | 16:9, 512 x 288, Móvil (iPhone, iPad, Android), (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 4 | 4:3, 384 x 288, Móvil (iPhone, iPad, Android), (600 Kbps) | 700 | _Mobile_384x288_600 | 600 | 384 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 5 | 16:9, 640 x 360, Tablet (iPad, Android), (800 Kbps) | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Igual que el origen | 80 | Resolución media, WiFi |
| 6 | 4:3, 640 x 480, Tablet (iPad, Android), (800 Kbps) | 900 | _iPad_640x480_800K | 800 | 640 x 480 | Igual que el origen | 80 | Resolución media, WiFi |
| 7 | 16:9, 768 x 432, Tablet (iPad, Android), (1200 Kbps) | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768 x 432 | Igual que el origen | 96 | Alta resolución, WiFi |
| 8 | 4:3, 768 x 576, Tablet (iPad, Android), (1200 Kbps) | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768 x 576 | Igual que el origen | 96 | Alta resolución, WiFi |
| 9 | 16:9, 1280 x 720, Escritorio, (2000 kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280 x 720 | Igual que el origen | 128 | Pantalla ancha de alta definición |
| 10 | 4:3, 1280 x 960, Escritorio, (2000 kbps) | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280 x 960 | Igual que el origen | 128 | Alta definición |

### Ajustes preestablecidos de codificación de vídeo para equipos de escritorio {#desktop-video-encoding-presets}

Ajustes preestablecidos de codificación de vídeo para MP4 y OGV en ordenadores de escritorio.

Para obtener más información sobre los parámetros de las opciones de codificación, consulte [Acerca de las opciones de ajustes preestablecidos de codificación](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2, audio AAC, extensión de archivo MP4**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Igual que el origen | 64 | Pantalla ancha de baja resolución |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640 x 360 | Igual que el origen | 80 | Resolución media para pantalla ancha |
| 3 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Igual que el origen | 96 | Resolución media/alta |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280 x 720 | Igual que el origen | 128 | Pantalla ancha de alta definición |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320 x 240 | Igual que el origen | 64 | Baja resolución |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Igual que el origen | 80 | Resolución media |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640 x 480 | Igual que el origen | 96 | Resolución media/alta |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280 x 960 | Igual que el origen | 128 | Alta definición |

**OGG Theora Vorbis - extensión de archivo OGV**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Igual que el origen | 64 | Pantalla ancha de baja resolución |
| 2 | 16:9, 640x360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Igual que el origen | 80 | Resolución media para pantalla ancha |
| 3 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | Igual que el origen | 96 | Resolución media/alta |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280 x 720 | Igual que el origen | 128 | Pantalla ancha de alta definición |
| 5 | 4:3, 320x240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Igual que el origen | 64 | Baja resolución |
| 6 | 4:3, 480x360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Igual que el origen | 80 | Resolución media |
| 7 | 4:3, 640x480 (1200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640 x 480 | Igual que el origen | 96 | Resolución media/alta |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280 x 960 | Igual que el origen | 128 | Alta definición |

### Ajustes preestablecidos de codificación de vídeo para dispositivos móviles {#mobile-video-encoding-presets}

Igual que fps del origen. Ajustes preestablecidos de codificación de vídeo para iPhone, iPad y dispositivos móviles Android.

Para obtener más información sobre los parámetros de opciones de codificación, consulte [Acerca de las opciones de ajustes preestablecidos de codificación](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1, audio AAC, extensión de archivo MP4**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de bits de vídeo (Kbps) | Anchura y altura en píxeles | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288 , Móvil (400 kbps) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 2 | 16:9, 512 x 288 , Móvil (600 kbps) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 3 | 16:9, 512 x 288 , Móvil (800 kbps) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Igual que el origen | 80 | Resolución media, Wi-Fi |
| 4 | 16:9, 512 x 288 , Móvil (1000 kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1.000 | 512 x 288 | Igual que el origen | 80 | Alta resolución, Wi-Fi |
| 5 | 16:9, 512 x 288 , Móvil (1200 kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512 x 288 | Igual que el origen | 96 | Alta resolución, Wi-Fi |
| 6 | 4:3, 384 x 288 , Móvil (400 kbps) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 7 | 4:3, 384 x 288 , Móvil (600 kbps) | 700 | _Mobile_384x288_600K | 600 | 384 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 8 | 4:3, 448 x 336 , Móvil (800 kbps) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Igual que el origen | 80 | Resolución media, Wi-Fi |
| 9 | 4:3, 448 x 336 , Móvil (1000 kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1.000 | 448 x 336 | Igual que el origen | 80 | Alta resolución, Wi-Fi |
| 10 | 4:3, 448 x 336 , Móvil (1200 kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448 x 336 | Igual que el origen | 96 | Alta resolución, Wi-Fi |

## Ajustes preestablecidos de visor {#viewer-presets}

>[!NOTE]
>
>**Aviso** de fin de vida útil de visores Flash: a partir del 31 de enero de 2017, Adobe Scene7 Publishing System ha dejado de ofrecer asistencia técnica para la plataforma de visor Flash. Para obtener más información sobre este cambio importante, consulte el siguiente sitio web de preguntas más frecuentes: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

Un *ajuste preestablecido de visor* es una serie de opciones que determinan la manera en que los usuarios verán los recursos de medios enriquecidos en la pantalla de su ordenador y dispositivos móviles. Como administrador, puede crear ajustes preestablecidos de visor. Se pueden configurar varias opciones de configuración para los visores. Por ejemplo, puede cambiar el tamaño, el comportamiento del zoom, las combinaciones de colores, los bordes y las fuentes del visor.

Se recomienda utilizar los visores de vídeo HTML5 de Dynamic Media Classic. Los ajustes preestablecidos utilizados en los visores de vídeo HTML5 son reproductores de vídeo sólidos. Al combinar en un solo reproductor la capacidad para diseñar los componentes de reproducción mediante HTML5 y CSS, tener la reproducción incorporada y usar flujo adaptable y progresivo en función de la capacidad del explorador, se amplía el alcance del contenido de medios enriquecidos para los usuarios de móviles, tablets y de escritorio y se garantiza una experiencia optimizada de vídeo.

Consulte [Acerca de los visores](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) HTML5 en la Guía de referencia de visores de Adobe.

Consulte Tabla [de compatibilidad de ajustes preestablecidos de visor de](application-setup.md#scene7_viewer_preset_compatibility_matrix)Dynamic Media Classic.

Consulte [Práctica recomendada: Uso del visor de vídeo HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Dependiendo del visor, puede añadir funciones de comunidad. Las funciones de la comunidad incluyen los botones de incrustación, enlace y visita al sitio. Estos botones permiten a las personas que utilizan los visores compartir el visor con otros usuarios o abrir el sitio web de Dynamic Media Classic.

Consulte también Ejemplos [de la biblioteca de referencia de visores de](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)Adobe.

### Compatibilidad de los visores para páginas web diseñadas para interactividad {#viewer-support-for-responsive-designed-web-pages}

Diferentes páginas Web tienen diferentes necesidades. A veces deseará que la página web proporcione un vínculo que abra el visor HTML5 en otra ventana del explorador. En otros casos, puede ser necesario incrustar el visor HTML5 directamente en la página de alojamiento. En este último caso, la página web puede tener un diseño estático. O bien, puede ser “interactiva” y mostrarse de forma diferente en diferentes dispositivos o diferentes tamaños de ventana de explorador. Para satisfacer estas necesidades, los visores HTML5 que vienen con Dynamic Media Classic admiten páginas web estáticas y páginas web diseñadas con capacidad de respuesta.

Consulte [Biblioteca de imágenes estáticas interactivas](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)en la Ayuda *de la API de servicio de imágenes de* Adobe para obtener más información sobre cómo incrustar visores interactivos en sus páginas web.

### Tipos de ajustes preestablecidos {#viewer-preset-types}

Los administradores pueden crear y personalizar los siguientes tipos de valores preestablecidos de visor:

**Visor** de catálogos electrónicos Simula la experiencia de leer un catálogo impreso. Puede moverse de una página a otra, acercar o alejar elementos de una página, utilizar mapas de imagen para ver más información sobre los elementos de la página o buscar en el catálogo. También puede incluir un panel de información para mostrar información detallada y un elemento de mapa de imagen si el área del mapa tiene un atributo rollover_key válido. Para incluir un panel de información, especifique una dirección URL del servidor de información en la configuración del panel de información de la ventana de ajuste preestablecido de visor de catálogo electrónico.

**Visor** de conjuntos de muestras Muestra una imagen en un color, material, textura, acabado o tela diferentes. Los usuarios deben hacer clic en una miniatura para ver las variaciones en la imagen.

**Visor** de conjuntos de medios mixtos Muestra diferentes tipos de medios en un visor. Puede incluir conjuntos de muestras, conjuntos de giros, imágenes y vídeos. Puede configurar fichas que contengan distintos tipos de contenido, como una ficha para conjuntos de imágenes y otra ficha para vídeos. Los vídeos que se reproducen desde un conjunto de medios mixtos usan un visor de vídeo estándar con una línea de tiempo y controles de vídeo, como Detener, Pausa, Rebobinar y Reproducir. Al configurar un ajuste preestablecido de visor de conjuntos de medios mixtos, debe especificar qué visores desea usar para los diferentes tipos de recursos en su conjunto de medios mixtos. También puede usar el visor de cuadrícula o carrusel para ver un conjunto de medios mixtos.

**Visor** de conjuntos de giros Proporciona varias vistas de una imagen para que los usuarios puedan girar el objeto y examinar los diferentes lados y ángulos.

**Visor** de vídeos Muestra vídeos con las dimensiones de resolución del archivo de origen o un tamaño personalizado. Dynamic Media Classic incluye muchos ajustes preestablecidos de visor predefinidos para reproducir vídeo y, si es un administrador, puede crear ajustes preestablecidos de visor de vídeo personalizados. Hay más de una docena de opciones de configuración diferentes para personalizar el visor de vídeo. Puede configurar el tamaño, el color de primer plano y fondo, los controles de audio y vídeo, la barra de progreso, la apariencia de la interfaz del usuario, las funciones sociales y la ayuda del visor.

**Visores** de zoom Ofrece tres tipos de visor de zoom:

**Visor** de zoom Permite a los usuarios acercarse al área haciendo clic en él. Pueden hacer clic en los controles para acercarse, alejarse y restablecer la imagen a su tamaño predeterminado.

**Visor de zoom: Desplegable** Muestra una segunda imagen del área ampliada junto a la imagen original. No hay controles, los usuarios simplemente mueven la selección sobre la zona que desean ver.

Al determinar el uso del ancho de banda completo para este visor, tenga en cuenta que tanto la imagen principal como la imagen flotante se muestran en el visor. El tamaño de imagen principal (la anchura y altura de escenario) y el factor de zoom determinan el tamaño de la imagen flotante. Para evitar que el tamaño del archivo flotante sea demasiado grande, equilibre estos dos valores: si el tamaño de la imagen principal es muy grande, reduzca el valor de Factor de zoom. (Los valores de Anchura flotante y Altura flotante determinan el tamaño de la ventana flotante, pero no el tamaño de la imagen que se muestra en el visor).

Por ejemplo, si el tamaño de la imagen principal es 350 x 350 píxeles, con un factor de zoom de 3, el tamaño de la imagen flotante que resultará será de 1050 x 1050 píxeles. Si el tamaño de la imagen principal es de 300 x 300 píxeles, con un factor de zoom de 4, el tamaño de la imagen flotante será de 1200 x 1200 píxeles. Según el ajuste de calidad JPEG (el recomendado es entre 80 y 90), podrá reducir el tamaño del archivo en gran medida. Los factores de zoom recomendados son de 2,5 a 4, según el tamaño de la imagen principal.

### Tabla de compatibilidad de ajustes preestablecidos de visor de Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Aviso** de fin de vida útil de visores Flash: A partir del 31 de enero de 2017, Adobe Scene7 Publishing System dejó de ofrecer asistencia técnica para la plataforma de visor Flash.

Para obtener más información sobre este cambio importante, consulte el siguiente sitio web de preguntas más frecuentes: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

La siguiente tabla identifica los ajustes preestablecidos de visor de Dynamic Media Classic disponibles actualmente. En la tabla también se especifica la compatibilidad del visor con los ordenadores y los dispositivos móviles, así como la tecnología empleada para cada visor.

Consulte también Ejemplos [de la biblioteca de referencia de visores de](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)Adobe.

Para obtener información sobre las versiones de sistema operativo y navegador web admitidas para los visores, consulte las notas de la versión de los visores.

Consulte las Notas [de la versión de referencia de visores de](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/)Adobe.

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de imágenes |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de muestras |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de catálogos electrónicos |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(incluye compatibilidad con medios sociales y búsqueda de catálogos). | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(incluye compatibilidad con medios sociales y búsqueda de catálogos). | HTML5 | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de giros |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visores de eVideo**

Dynamic Media Classic admite la reproducción de vídeo móvil para vídeo MP4 H.264.

* Puede encontrar los dispositivos Blackberry compatibles con este formato de vídeo en: Formatos de vídeo [admitidos en Blackberry](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* También puede encontrar dispositivos Windows compatibles con este formato de vídeo en los siguientes:Formatos de vídeo[admitidos en Windows Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android | Smartphone Blackberry | Teléfono de Windows |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(incluye compatibilidad con subtítulos opcionales). Consulte [Práctica recomendada: Uso del visor de vídeo universal HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(incluye compatibilidad con subtítulos opcionales y medios sociales). | HTML5 | X | X | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de medios mixtos |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Tabla de gestos de visores móviles admitidos {#supported-mobile-viewers-gestures-matrix}

En la siguiente tabla se identifican los gestos del visor móvil que admiten los dispositivos iOS, Android 2.x y Android 3.x.

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de imágenes |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Sobre la pantalla Valor predeterminado del visualizador {#about-the-viewer-preset-screen}

Esta pantalla permite crear y gestionar ajustes preestablecidos de visor. Para abrir esta pantalla, haga clic en **Ajustes** &gt; **Ajustes preestablecidos de visor**.

La pantalla Ajustes preestablecidos de visor ofrece una serie de herramientas para realizar las siguientes tareas:

**Adición de un ajuste preestablecido** Haga clic en Agregar y seleccione las opciones deseadas en el cuadro de diálogo Añadir ajuste preestablecido de visor.

Consulte [Adición y edición de ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

**Edición de un ajuste preestablecido** Seleccione un ajuste preestablecido y, a continuación, haga clic en **Editar**.

Consulte [Adición y edición de ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

**Eliminación de un ajuste preestablecido** Seleccione un ajuste preestablecido y, a continuación, haga clic en **Eliminar**.

**Exportación de un ajuste preestablecido** Seleccione un ajuste preestablecido de visor HTML5 y, a continuación, haga clic en Exportar para descargar la apariencia del visor de modo que pueda utilizarla como base para crear y añadir un nuevo ajuste preestablecido de visor.

Consulte [Exportación de ajustes preestablecidos](application-setup.md#exporting_an_html5_viewer_preset)de visor HTML5.

**Filtrado de la lista** Ajustes preestablecidos de visor Utilice estas herramientas para filtrar la lista:

* Abra la lista desplegable de **activo/inactivo** y seleccione una opción para mostrar los ajustes preestablecidos activos, los inactivos o todos.
* Abra la lista desplegable **Visor** y elija una opción para ver únicamente los visores de un tipo concreto. Seleccione **Todos los visores** para mostrarlos todos.

**Clasificación de ajustes preestablecidos** Haga clic en un encabezado de columna (Activo, Tipo, Ajuste preestablecido o Plataforma) para ordenar la lista en una columna. Vuelva a hacer clic en el encabezado de columna para ordenar la lista en orden descendente (o ascendente).

**Activación y desactivación de ajustes preestablecidos** Seleccione un ajuste preestablecido y haga clic en su opción Activa para activarlo o desactivarlo.

Consulte [Activación o desactivación de ajustes preestablecidos de visor](application-setup.md#activating_or_deactivating_viewer_presets).

>[!NOTE]
>
>Haga clic en Vista previa a la derecha de la pantalla Ajustes preestablecidos de visor y compruebe qué aspecto tiene el recurso con el ajuste preestablecido de visor seleccionado. Si desea ver otro recurso, haga clic en Examinar en la pantalla Ajustes preestablecidos de visor y seleccione otro recurso en el cuadro de diálogo Seleccionar recurso para vista previa.

### Adición y edición de ajustes preestablecidos de visor {#adding-and-editing-viewer-presets}

Además de añadir ajustes preestablecidos de visor con Agregar en la interfaz de usuario, también puede usar Exportar para hacerlo. Basta con exportar un ajuste preestablecido de visor HTML5 existente y utilizarlo como base para el nuevo ajuste preestablecido.

Consulte [Exportación de ajustes preestablecidos](application-setup.md#exporting_an_html5_viewer_preset)de visor HTML5.

**Para añadir y editar ajustes preestablecidos de visor**

1. Cerca de la esquina superior derecha de Scene7 Publishing System, haga clic en **Ajustes** &gt; **Ajustes preestablecidos de visor**.

   Puede filtrar la lista de ajustes preestablecidos. Por ejemplo, para ver solo los ajustes preestablecidos para los visores de vídeos, seleccione Visor de vídeos en el menú desplegable de visores que hay en la barra de herramientas, justo encima de la tabla.

1. En la pantalla Ajustes preestablecidos de visor, añada o edite el ajuste preestablecido de visor oportuno.

   **Adición** Haga clic en Agregar en la barra de herramientas. En el cuadro de diálogo Añadir ajuste preestablecido de visor, elija una plataforma y seleccione un tipo de recurso de medios enriquecidos.

   Haga clic en **Guardar como** cuando termine de crear el ajuste preestablecido de visor.

   **Adición a partir de un ajuste preestablecido** de visor existente En la tabla, seleccione un ajuste preestablecido de visor de vídeo y, a continuación, haga clic en Editar en la barra de herramientas.

   Después de volver a configurar el visor de vídeo, haga clic en **Guardar como** para guardar el ajuste preestablecido con otro nombre en el campo de texto Nombre de ajuste preestablecido.

   **Edición** Seleccione un ajuste preestablecido de visor existente y, a continuación, haga clic en **Editar**.

1. En la pantalla Configurar visor, en el campo Nombre de ajuste preestablecido, escriba o edite el nombre.
1. Defina las opciones restantes que desee.

   >[NOTA]
   >
   >Seleccione Igual que el origen para ajustar automáticamente el tamaño del visor de vídeos al tamaño de resolución del vídeo codificado. Si elige esta opción, no puede introducir la anchura ni la altura del escenario sino que estas opciones proceden del propio vídeo. Si selecciona Igual que el origen, configure la opción de tamaño de margen para que refleje las dimensiones de aspecto fuera del área de reproducción de vídeo. Este tamaño de margen es la altura y anchura de píxel de los controles de vídeo. La siguiente ilustración le ayuda a determinar los tamaños de margen que se deben utilizar.*

   ![](assets/vs_video_viewer_configure_margin.png)

1. Realice una de las siguientes acciones:

   * Haga clic en **Guardar como** si ha agregado un ajuste preestablecido de visor a partir de uno existente.
   * Haga clic en **Guardar** si ha agregado o editado un ajuste preestablecido de visor.

### Exportación de un ajuste preestablecido de visor HTML5 {#exporting-an-html-viewer-preset}

Puede exportar un ajuste preestablecido de visor HTML5 existente para utilizarlo como base para crear un nuevo ajuste preestablecido de visor HTML5. Esta opción de exportación resulta útil porque no tiene que crear el visor de cero, sino que puede exportar un ajuste preestablecido con un aspecto y un comportamiento parecidos a los deseados y, luego, usarlo como punto de partida para realizar ajustes de diseño.

Tenga en cuenta que todos los archivos CSS preestablecidos de visor predeterminados y listos para usar en SPS utilizan rutas de servicio de imágenes relativas que apuntan a recursos ubicados en `Scene7SharedAssets`. Por ejemplo, la siguiente es una ruta relativa a un recurso de imagen en un archivo CSS preestablecido de visor ubicado en `Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`Sin embargo, si aloja archivos CSS de visor en su propio sitio, debe resolver esta ruta de imagen relativa mediante una ruta explícita al servidor de imágenes en su propio entorno. Por motivos ilustrativos, si se actualizara la ruta relativa anterior a una ruta explícita, podría tener el aspecto siguiente, donde `https://s7d1.scene7.com` es la ruta directa al servidor de imágenes: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Para exportar un ajuste preestablecido de visor HTML5**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Haga clic en **Ajustes** &gt; **Ajustes preestablecidos de visor**.
1. On the Viewer Presets toolbar, in the second drop-down list from the left, select **HTML5**.
1. En la tercera lista desplegable desde la izquierda, seleccione **Todos los visores**.
1. Seleccione el ajuste preestablecido de visor que desee utilizar como base para un nuevo ajuste preestablecido de visor HTML5.
1. En la barra de herramientas, haga clic en **Exportar**.
1. En el cuadro de diálogo Exportar recursos seleccionados, haga clic en **Enviar exp.**.

   Tras la exportación, se obtiene un archivo CSS. Descargue y descomprima el archivo.

1. Abra el archivo CSS en un editor de CSS, realice los cambios oportunos y, a continuación, guarde el archivo.
1. Cargue el archivo CSS en Scene7 Publishing System.

   Consulte [Carga de archivos](uploading-files.md#uploading_files).

1. Publique el archivo CSS en el servidor de imágenes de Dynamic Media.

   Consulte [Publicación de archivos](publishing-files.md#publishing_files).

1. Añada el nuevo ajuste preestablecido de visor del modo habitual. Seleccione el archivo CSS del visor que ha cargado.

   Consulte [Adición y edición de ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

### Activación o desactivación de ajustes preestablecidos de visor {#activating-or-deactivating-viewer-presets}

Para crear una URL y mostrar los recursos, los usuarios deben abrir la lista desplegable Ajustes preestablecidos del cuadro de diálogo Vista previa, seleccionar un Ajuste preestablecido de visor y hacer clic en Copiar URL (consulte [Copia de la dirección URL de un ajuste preestablecido de visor](application-setup.md#copying_the_url_of_a_viewer_preset)). La lista Ajustes preestablecidos contiene unos ajustes que los administradores pueden agregar y gestionar desde la pantalla Ajustes preestablecidos de visor. Por ejemplo, cuando un usuario obtiene una vista previa de un catálogo electrónico, todos los ajustes preestablecidos de visor del catálogo activo aparecen en la lista desplegable Ajustes preestablecidos, en el cuadro de diálogo Vista previa.

Si no desactiva los ajustes preestablecidos de visor en su pantalla correspondiente, la lista desplegable de ajustes del cuadro de diálogo Ajustes preestablecidos puede llenarse demasiado. 

**Para activar o desactivar ajustes preestablecidos de visor**

1. Choose **Setup** &gt; **Viewer Presets** to open the Viewer Presets screen.
1. Seleccione o anule la selección de opciones activas para activar o desactivar ajustes preestablecidos de visor.

### Copia de la dirección URL de un ajuste preestablecido de visor {#copying-the-url-of-a-viewer-preset}

Tras publicar un recurso, puede copiar una URL para mostrar el recurso con la configuración de un ajuste preestablecido de visor.

La URL se copiará en el portapapeles. Podrá utilizarla como sea necesario en el código HTML de su página web, dispositivo móvil o aplicación.

**Para copiar la dirección URL de un ajuste preestablecido de visor**

1. Seleccione el recurso en el panel Examinar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **Copiar URL** a la derecha del visor que desee.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** debajo de la imagen en miniatura.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** a la derecha de la imagen en miniatura.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** &gt; **Lista del visor**.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

### Copia del código incrustado de un ajuste preestablecido de visor  {#copying-the-embed-code-of-a-viewer-preset}

El uso de la función de código incrustado permite revisar el código del ajuste preestablecido de visor seleccionado. También puede copiar el código en el portapapeles para pegarlo en sus páginas web para la implementación del visor. 

No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un ajuste preestablecido de visor**

1. Seleccione el recurso en el panel de exploración de recursos.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel Direcciones URL de la derecha, haga clic en **Código incrustado**.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** debajo de la imagen en miniatura.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** a la derecha de la imagen en miniatura.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** &gt; **Lista del visor**.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

1. En el cuadro de diálogo Código incrustado, haga clic en **Copiar al portapapeles**.
1. Haga clic en **Cerrar**.

## Configuración de los visores predeterminados {#configuring-default-viewers}

Puede utilizar visores predeterminados para configurar el visor predeterminado que está asociado con un recurso cuando se utiliza la opción Vista previa en Scene7 Publishing System. Puede configurar la experiencia de previsualización por defecto para los siguientes tipos de recursos:

* Imagen
* Vídeo
* Conjunto de giros
* Catálogo
* Conjunto de imágenes
* Conjunto de muestras
* Conjunto de medios

**Para configurar los visores predeterminados**

1. In the Setup drop-down list, click **Application Setup**.
1. In the Setup window, in the left pane, expand **Application Setup** &gt; **Viewers**
1. Click **Default Viewers**.
1. En la ventana Visores predeterminados, en la lista desplegable para cada tipo de recurso, seleccione el visor que desee asociar con la vista previa del recurso.
1. In the lower-right corner of the Default Viewers window, click **Save Settings**.
1. In the lower-right corner of the Setup window, click **Close** to return to the Asset window.

## Vistas de metadatos {#metadata-views}

Los *metadatos* constituyen un conjunto de información estandarizada sobre un recurso. Puede utilizar metadatos para perfeccionar el flujo de trabajo, organizar sus recursos y mejorar las búsquedas. Dynamic Media Classic admite el estándar IPTC (International Press Telecommunications Council) y el estándar XMP (Extensible Metadata Platform). Antes de que los usuarios vean o introduzcan los metadatos de un recurso en la vista de detalles, pueden abrir el menú Vistas de metadatos y seleccionar el conjunto de campos de metadatos que deseen ver o utilizar para describir el recurso.

Dynamic Media Classic incluye vistas de metadatos predefinidas y los administradores pueden crear sus propias vistas de metadatos para que los usuarios puedan elegir cuándo introducen metadatos.

### Creación de una vista de metadatos {#creating-a-metadata-view}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Views**.
1. Haga clic en **Agregar**.
1. En el campo de texto Nombre de ajuste preestablecido, introduzca un nombre para la vista.
1. (Optional) Check **Make Default** to make this view the one that users see when they open the Metadata panel in Detail View.
1. (Optional) Select **Include UDF** to include user-defined fields in the view. Los campos definidos por el usuario aparecen en la parte superior del panel Metadatos en la vista de detalles.
1. Select the fields you want for the view (click **Select All** to select all the fields).
1. Haga clic en **Guardar**.

   Las categorías y los campos seleccionados de la vista aparecen en el panel Vista previa.

### Gestión de vistas de metadatos {#managing-metadata-views}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Views**.
1. Realice una de las siguientes acciones:

   * Para obtener una vista previa de una vista, selecciónela. Los campos de la vista aparecen en el panel Vista previa.
   * To edit a view, select it and then click **Edit**. Then select or deselect field names on the Preview panel, and select or deselect the **Include UDF** option.
   * To delete a view, select it and then click **Delete**.
   * To make a view the default, select it and then click **Make Default**. La vista predeterminada es aquella que ven los usuarios cuando abren un recurso en la vista de detalles y acceden al panel Metadatos.

## Ajustes preestablecidos de metadatos {#metadata-presets}

Los ajustes preestablecidos ofrecen a los administradores un método para controlar y regular metadatos que se asignan a los recursos. En la vista de detalles, un usuario puede introducir metadatos sobre un recurso en los campos que se proporcionan para ese propósito. Por ejemplo, un usuario puede introducir el nombre de un propietario, la descripción de derechos de autor y la dirección. Para asegurarse de que los usuarios introducen esta información de un modo preciso y completo, puede crear ajustes preestablecidos de metadatos. La elección de un ajuste preestablecido de metadatos en la Vista de detalles rellena los campos de metadatos con valores predefinidos. Por ejemplo, el nombre de un propietario, la descripción de derechos de autor y la dirección se rellenan de forma automática.

Cree un ajuste preestablecido de metadatos para cada conjunto de valores de metadatos que desee que los usuarios puedan introducir de forma automática en la vista de detalles para describir un recurso. 

### Creación o edición de un ajuste preestablecido de metadatos {#creating-or-editing-a-metadata-preset}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Presets** .
1. En la pantalla Ajustes preestablecidos de metadatos, realice lo siguiente:

   * To create a preset, click **Add**. En el campo de texto Nombre de plantilla de metadatos, escriba un nombre para el ajuste preestablecido, haga clic en Vistas **de** metadatos y elija una vista en la lista desplegable (consulte Vistas [de](application-setup.md#metadata_views)metadatos).
   * To edit an existing preset, select the preset from the Metadata Presets list and then click **Edit**.

1. Expanda los encabezados que desee incluir en el ajuste preestablecido e introduzca los valores en los distintos campos que desee incluir en este ajuste.
1. Haga clic en **Guardar**.

   Las categorías y los campos seleccionados para el ajuste preestablecido aparecen en el panel Vista previa.

### Gestión de ajustes preestablecidos de metadatos {#managing-metadata-presets}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Presets**.
1. Realice una de las siguientes acciones:

   * Para obtener la vista previa de un ajuste preestablecido, selecciónelo. La información del ajuste preestablecido (categorías y campos) aparece en la pantalla Ajuste preestablecido.
   * To delete a preset, select the preset, and then click **Delete**.

## Campos personalizables {#user-defined-fields}

Un administrador de Media Portal o un administrador de empresa pueden crear campos de metadatos personalizables o personalizados. Los campos personalizados pueden ayudarle a organizar los recursos en Scene7 Publishing System. Puede marcar los campos como activos, según sea necesario. Cuando están activados, los nombres de estos campos de metadatos personalizados aparecen en el panel Metadatos, en la vista de detalles. Los usuarios pueden introducir información en los campos de metadatos definidos por el usuario para describir los recursos. También pueden utilizar un campo de metadatos definido por el usuario como criterio de búsqueda.

Un uso efectivo de los campos de metadatos personalizables es retardar el tiempo de activación de un recurso para un lanzamiento o una oferta específicos. El campo "activación" se define en función del tipo *Fecha*. Then, using the **Metadata** panel in **Detail** view or **File** &gt; **Edit Info**, you can specify when the asset is activated. Scene7 Publishing System comprueba el estado y el historial de publicación de un recurso. Si no se encuentra dentro del tiempo de activación, el estado de publicación se muestra como "No publicado".

>[!NOTE]
>
>Para que los campos definidos por el usuario aparezcan en el panel Metadatos de la vista de detalles, inclúyalos en las vistas de detalles. En la pantalla Vistas de metadatos, seleccione la opción Incluir UDF (campos definidos por el usuario). Para obtener más información, consulte [Vistas de metadatos](application-setup.md#metadata_views).

>[!NOTE]
>
>Para buscar recursos utilizando los campos personalizados o personalizables, haga clic en **Ajustes** &gt; **Ajustes personales** y seleccione **Incluir UDF en la búsqueda**. Consulte [Ajustes personales](personal-setup.md#personal_setup).

### Creación de un campo de metadatos definido por el usuario {#creating-a-user-defined-metadata-field}

1. Haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Metadatos** &gt; **Campos personalizables**.
1. Haga clic en **Agregar**.
1. En el cuadro de diálogo Campo personalizado, seleccione las opciones que desee.

   **Nombre** Introduzca un nombre para el campo de metadatos.

   **Tipo** Elija una opción que defina el tipo de información que los usuarios pueden introducir en el campo de metadatos:

   **Cadena** Una cadena de texto.

   **Int** Un entero.

   **Flotante** Un número de coma flotante.

   **Sí/No** Un valor booleano sí/no.

   **Fecha** Una fecha. Se acepta el formato MM/DD/AAAA.

   **Nombre** de archivo El nombre de un archivo.

   **Color** El nombre de un color.

   **Dimensión** El ancho y el alto del recurso.

   **Sin tipo** Para compatibilidad con versiones anteriores. No seleccione esta opción.

   **Valor** predeterminado De forma opcional, introduzca el valor que los usuarios tienen más probabilidades de introducir en el campo. El valor introducido se convertirá en el valor predeterminado del campo que cree.

   **Se aplica** de forma opcional, elija un tipo de recurso si desea que el campo de metadatos se aplique solo a un tipo específico de recurso.

   ***Note**: Choose an **Applies To** option carefully because you cannot change the **Applies To** option after you create a user-defined field. Dynamic Media Classic lets you edit the name, type, and default value of a user-defined field, but not the **Applies To** setting. *

1. Haga clic en **Guardar** cuando termine de crear el campo de metadatos.

### Gestión de campos personalizables {#manage-user-defined-fields}

La pantalla Campos personalizables ofrece comandos para gestionar campos de metadatos personalizados definidos por el usuario.

Solo un administrador de Media Portal o un administrador de empresa pueden administrar campos personalizables.

Para abrir esta pantalla, haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Metadatos** &gt; **Campos personalizables**.

**Edición de un campo** Seleccione el campo y, a continuación, haga clic en **Editar**.

**Eliminación de un campo** Seleccione el campo y, a continuación, haga clic en **Eliminar**.

**Activar campo** Haga clic para seleccionar o anular la selección de la opción Activo junto al nombre de un campo. Si tiene la función de Administración de empresa, puede ser que no se muestre esta opción. Como esta opción está relacionada con MediaPortal, debe seleccionar (activar) Mostrar funciones de MediaPortal en Ajustes personales para ver los campos de activación.

## Optimización de archivos {#optimize-files}

Cuando carga archivos en Scene7 Publishing System, el sistema los optimiza para su almacenamiento y publicación. Sin embargo, si se interrumpe el proceso de carga, no se pueden optimizar todas las imágenes. De ser así, aparecerá el mensaje "La imagen no está optimizada todavía". Si es un administrador podrá optimizar estos archivos.

Scene7 Publishing System realiza una búsqueda entre los archivos y optimiza solo las imágenes que no hayan sido optimizadas anteriormente.

1. Elija **Ajustes** &gt; Ajustes **de aplicación** y, a continuación, seleccione **Optimizar archivos**.
1. Enter information for the optimization job and click **Submit**.

   Si trabaja con más de una empresa, optimice los archivos de cada una de forma independiente.

## Valores preestablecidos de conjuntos de lotes {#batch-set-presets}

Utilice los valores preestablecidos de conjuntos de lotes para crear automáticamente conjuntos de imágenes o conjuntos de giros mientras se ejecuta un trabajo para cargar recursos en Scene7 Publishing System.

Los administradores de la empresa definen en primer lugar las convenciones de nombres de los recursos que desean agrupar en un conjunto. Puede crear un ajuste preestablecido de conjunto de lotes para hacer referencia a estas imágenes. Cada valor preestablecido tiene un nombre exclusivo y un conjunto de instrucciones independiente para crear el conjunto con imágenes que coincidan con las convenciones de nombre definidas en el ajuste preestablecido.

Todos los ajustes preestablecidos de conjunto de lotes activos aparecen en el cuadro de diálogo Opciones de trabajo de carga para que pueda especificar qué ajuste preestablecido desea aplicar durante cada sesión de carga. Los administradores de empresa pueden ver todos los valores preestablecidos de conjuntos activos e inactivos. Al cargar archivos, Dynamic Media Classic crea automáticamente un conjunto con todos los archivos que coinciden con la convención de nombre definida en los ajustes preestablecidos activos.

### Nombre por defecto {#default-naming}

El administrador de empresa crea una convención de nombre predeterminada que se utiliza en las fórmulas de los ajustes preestablecidos de conjunto de lotes. La convención de nombre predeterminada seleccionada en la definición del ajuste preestablecido de conjunto de lotes puede ser todo lo que la empresa necesita para la generación de conjuntos de lotes para todos los sitios web. Se crea un ajuste preestablecido de conjunto de lotes para utilizar la convención de nombre predeterminada que defina. Puede crear tantos ajustes preestablecidos de conjunto de lotes como desee con diferentes convenciones de nombre personalizadas necesarias para un conjunto particular de contenido en casos en los que hay una excepción en el nombre predeterminado definido de la empresa. 

Al configurar una convención de nombre predeterminada no es necesario utilizar la funcionalidad de ajuste preestablecido de conjunto de lotes, la práctica recomendada es utilizar la convención de nombre predeterminada para definir todos los elementos de la convención con nombre que desee agrupar en un conjunto para agilizar la creación de conjuntos de lotes.

1. Haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes preestablecidos de conjunto por lotes** &gt; **Nombre por defecto**.
1. Seleccione **Ver formulario** o **Ver código** para determinar cómo desea ver e introducir la información de cada elemento.

   Puede seleccionar la casilla de verificación Ver código para ver la creación del valor de expresión regular junto con las selecciones de formulario. Puede introducir o alterar estos valores para ayudar a definir los elementos de la convención de nombre, si la vista del formulario le limita por alguna razón. Si los valores no se pueden analizar en la vista del formulario, los campos del formulario se volverán inactivos.

   >[!NOTE]
   Los campos del formulario desactivados no indican ninguna expresión regular no válida. No hay certeza de que las expresiones regulares sean correctas. Verá los resultados de la expresión regular que está creando para cada elemento después de la línea de resultados. La expresión regular completa está visible en la parte inferior de la página.

1. Expanda los elementos necesarios e introduzca las convenciones de nombres que desee usar.
1. Si es necesario, haga clic en **Agregar** para añadir otra convención de nombre para un elemento. O bien, haga clic en **Eliminar** para eliminar la convención de nombre de un elemento. 
1. Haga clic en **Guardar como** y escriba un nombre para el ajuste preestablecido. También puede hacer clic en **Guardar** si está editando un ajuste preestablecido existente.

También puede usar la visualización de código sin campos de formulario disponibles. En esta vista, puede crear las definiciones de convención de nombre con expresiones regulares.

Hay dos elementos disponibles para la definición: la coincidencia y el nombre base. Estos campos le permiten definir todos los elementos de una convención de nombre e identificar la parte de la convención utilizada para dar nombre al conjunto que los contiene. Una convención de nombre individual de una empresa puede hacer uso de una o más líneas de definición para cada uno de esos elementos. Puede utilizar tantas líneas como necesite para su definición única y agruparlas en distintos elementos, como imagen principal, elemento de color, elemento de vista alternativa y elemento de muestra.

### Creación de un ajuste preestablecido de conjunto de lotes {#creating-a-batch-set-preset}

Dynamic Media Classic utiliza ajustes preestablecidos de conjunto de lotes para organizar recursos que comparten información o contenido común en conjuntos de imágenes para mostrarlos en los visores. Las fórmulas de ajustes preestablecidos de conjunto de lotes se ejecutan automáticamente junto con los trabajos de importación de recursos programados en Dynamic Media Classic.

En la pantalla Ajustes preestablecidos de conjunto por lotes, cree, edite y gestione sus valores preestablecidos de conjunto de lotes. Puede crear tantos valores preestablecidos de conjunto de lotes como necesite para cubrir todos los trabajos de ingesta de recursos requeridos. Hay dos formas de definiciones de ajustes preestablecidos de conjunto por lotes, una para una convención de nombre predeterminada que haya configurado y otra para convenciones de nombre personalizadas que puede crear sobre la marcha.

Puede utilizar el método de campo de formulario para definir un ajuste preestablecido de conjunto de lotes o el método de código, que le permite utilizar expresiones regulares. En Nombre por defecto, puede elegir la vista de código al mismo tiempo que define la vista de formulario y utiliza las expresiones regulares para crear las definiciones. También puede desactivar la vista para utilizar una u otra exclusivamente.

Consulte también [Creación de un ajuste preestablecido de conjunto de lotes para la generación automática de conjuntos de giros 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Creación de un ajuste preestablecido de conjunto de lotes**

1. Haga clic en **Ajustes &gt;****Ajustes de aplicación** &gt; **Ajustes preestablecidos de conjunto por lotes** &gt; **Valor preestablecido de conjunto de lotes**. **Ver formulario**, definido en la esquina superior derecha de la página Detalles, es la opción predeterminada.
1. En el panel Lista de ajustes preestablecidos, haga clic en **Añadir** para activar los campos de definición en el panel Detalles del lateral derecho de la pantalla.
1. En el panel Detalles, en el campo Nombre de ajuste preestablecido, escriba un nombre para el ajuste preestablecido.
1. En el menú desplegable Tipo de conjunto de lotes, seleccione un tipo de ajuste preestablecido.

   Para generar un conjunto de giros 2D, seleccione **Conjunto de giros con varios ejes** en la lista desplegable Tipo de conjunto de lotes.

1. Realice una de las acciones siguientes:

   * Si está utilizando una convención de nombres predeterminada configurada previamente en Ajustes de aplicación &gt; Valores preestablecidos de conjuntos de lotes &gt; Nombre por defecto, amplíe **Convenciones de nombres de recursos** y haga clic en **Predeterminado** en la lista desplegable Nombres de archivo.
   * Para definir una convención de nombre al configurar el ajuste preestablecido, amplíe **Convenciones de nombres de recursos** y haga clic en **Personalizado** en la lista desplegable Nombres de archivo.

1. Para el orden de secuencia, defina el orden de las imágenes después de que el conjunto se agrupe en Dynamic Media Classic. De forma predeterminada, los recursos se ordenan de forma alfanumérica. Sin embargo, puede utilizar una lista de expresiones regulares separada por comas para definir el orden.
1. Para las convenciones de nombres de conjuntos y opciones de creación, especifique el sufijo o prefijo en el nombre base que definió en Convenciones de nombres de recursos. También defina dónde se creará el conjunto de imágenes en la estructura de carpetas de Dynamic Media Classic.

   Si define un gran número de conjuntos de imágenes, es posible que prefiera mantenerlos separados de las carpetas que contienen los propios recursos. Algunos clientes crean la carpeta Conjuntos de imágenes y redirigen la aplicación para colocar aquí los conjuntos de lotes generados.

1. Haga clic en **Guardar** en el panel Detalles.

### Creación de un ajuste preestablecido de conjunto de lotes para la generación automática de conjuntos de giros 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Puede utilizar el Tipo de conjunto de lotes **Conjunto de giros con varios ejes** para crear una “fórmula” que automatizará la creación de conjuntos de giros 2D. La agrupación de imágenes utiliza expresiones regulares de fila y columna para alinear los recursos de imagen correctamente en la ubicación correspondiente de la matriz multidimensional.

Consulte también [Creación de un ajuste preestablecido de conjunto de lotes](application-setup.md#creating_a_batch_set_preset).

No hay un número máximo o mínimo de filas o columnas para un conjunto de giros de varios ejes.

Por ejemplo, supongamos que desea crear un conjunto de giros de varios ejes denominado *spin-2dspin*. Tiene un grupo de imágenes de conjunto de giros que contiene tres filas, con 12 imágenes por fila. Las imágenes se denominan de la forma siguiente:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Con esta información, puede crear esta fórmula de tipo de conjunto de lotes:

![](assets/se_batch_set_recipe.png)

La agrupación de la parte compartida del nombre de recurso del conjunto de giros se añade al campo **Coincidencia** (zona resaltada). La parte variable del nombre de recurso que contiene la fila y la columna se añade a los campos **Fila** y **Columna** respectivamente.

Cuando se cargue y publique el conjunto de giros, se activará el nombre de la fórmula de conjunto de giros 2D que se muestra en **Ajustes preestablecidos de conjunto por lotes** en el cuadro de diálogo **Opciones de trabajo de carga**.

**Creación de un ajuste preestablecido de conjunto de lotes para la generación automática de conjuntos de giros 2D**

1. Elija **Ajustes &gt;****Ajustes de aplicación** &gt; **Valores preestablecidos de conjunto por lotes** &gt; **Valor preestablecido de conjunto de lotes**. **Ver formulario**, definido en la esquina superior derecha de la página Detalles, es la opción predeterminada.
1. En el panel Lista de ajustes preestablecidos, haga clic en **Añadir** para activar los campos de definición en el panel Detalles del lateral derecho de la pantalla.
1. En el panel Detalles, en el campo Nombre de ajuste preestablecido, escriba un nombre para el ajuste preestablecido.
1. En el menú desplegable Tipo de conjunto de lotes, seleccione **Conjunto de recursos**.
1. En la lista desplegable Subtipo, seleccione **Conjunto de giros con varios ejes**.
1. Amplíe **Convenciones de nombres de recursos** y, a continuación, haga clic en **Personalizado** en la lista desplegable Nombre de archivos.
1. Utilice los atributos **Coincidencia** y, si lo desea, **Nombre base** para definir una expresión regular para la denominación de los recursos de imágenes que conforman el grupo.

   Por ejemplo, la expresión regular Coincidencia literal puede tener el siguiente aspecto:

   `(\w+)-\w+-\w+`

1. Amplíe **Posición de columna/fila** y defina el formato de nombre para la posición del recurso de imágenes en la matriz Conjunto de giros 2D.

   Ponga entre corchetes la posición de la fila o la columna en el nombre de archivo.

   Por ejemplo, la expresión regular de fila puede tener el aspecto siguiente:

   `\w+-R([0-9]+)-\w+`

   o

   `\w+-(\d+)-\w+`

   La expresión regular de columna puede tener el aspecto siguiente:

   `\w+-\w+-C([0-9]+)`

   o

   `\w+-\w+-C(\d+)`

   Recuerde que solo son ejemplos. Puede crear su expresión regular como prefiera según sus necesidades.

   >[!NOTE]
   Si la combinación de expresiones regulares de columna y fila no puede determinar la posición del recurso en la matriz de conjunto de giros multidimensional, ese recurso no se añadirá al conjunto y se registrará un error.

1. Para las convenciones de nombres de conjuntos y opciones de creación, especifique el sufijo o prefijo en el nombre base que definió en Convenciones de nombres de recursos. También defina dónde se creará el conjunto de imágenes en la estructura de carpetas de Dynamic Media Classic.

   Si define un gran número de conjuntos de imágenes, es posible que prefiera mantenerlos separados de las carpetas que contienen los propios recursos. Algunos clientes crean la carpeta Conjuntos de imágenes y redirigen la aplicación para colocar aquí los conjuntos de lotes generados.

1. Haga clic en **Guardar** en el panel Detalles.
1. Cargue y publique el conjunto de giros de la forma habitual, asegurándose de activar el nombre del conjunto de giros 2D en el cuadro de diálogo Opciones de carga de trabajo, en Valores preestablecidos de conjunto por lotes.

>[!MORELIKETHIS]
* [Previsualización de un recurso](previewing-asset.md#previewing_an_asset)
* [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets)
* [Visualización, adición y exportación de metadatos](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files)

