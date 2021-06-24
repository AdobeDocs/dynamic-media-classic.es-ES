---
title: Ajustes de aplicación
description: Aprenda a configurar el área Aplicación de Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Administrator
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: 223bbacab2f244b91763de2ea324a5c8d777feb9
workflow-type: tm+mt
source-wordcount: '10917'
ht-degree: 57%

---

# Ajustes de aplicación{#application-setup}

Puede utilizar las páginas Ajustes de aplicación para introducir ajustes generales, crear ajustes preestablecidos de imagen, ajustes preestablecidos de codificación de vídeo, ajustes preestablecidos de visor o para definir visores predeterminados y metadatos. Puede configurar ajustes preestablecidos de conjuntos de lotes para automatizar también la generación de conjuntos de giros 2D (por ejemplo), la configuración de publicación y la configuración de SEO de vídeo.

>[!NOTE]
>
>Solo los administradores de Dynamic Media Classic pueden cambiar la configuración en las páginas Ajustes de aplicación .

## Configuración general {#general-settings}

Para abrir la página Configuración general de la aplicación, haga clic en **[!UICONTROL Ajustes > Ajustes de aplicación > Configuración general]** en la barra de navegación global.

### Servidores

Al crear la cuenta, Dynamic Media Classic proporciona automáticamente los servidores asignados a su empresa. Estos servidores se utilizan para crear cadenas URL para su página web y sus aplicaciones. Estas llamadas mediante URL son específicas para su cuenta.

Consulte también [Prueba del servicio Secure Testing](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **Nombre del servidor publicado** : este servidor es el servidor de red de entrega de contenido (CDN) activo que se utiliza en todas las llamadas URL generadas por el sistema específicas de su cuenta. No cambie este nombre de servidor a menos que un técnico de asistencia de Dynamic Media Classic le indique que lo haga.

* **Nombre del servidor de origen** : este servidor se utiliza solo para la prueba de control de calidad. No cambie este nombre de servidor a menos que un técnico de asistencia de Dynamic Media Classic le indique que lo haga.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by a Dynamic Media Classic support technician. -->

* **Nombre del servidor de Test&amp;Target** : su URL de Test&amp;Target, hasta .com inclusive. Para obtener instrucciones sobre cómo obtener esta URL, consulte Integración de [!DNL Dynamic Media Classic] con [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **Nombre del servidor de transmisión de iOS** : la URL de su servidor de flujo de  [!DNL Dynamic Media Classic] iOS. Este servidor ofrece transmisión de vídeo para los dispositivos basados en iOS utilizando el protocolo HTTP.

* **Nombre del servidor de vídeo progresivo** : la URL de su servidor de vídeo  [!DNL Dynamic Media Classic] progresivo. Este servidor ofrece vídeo progresivo utilizando el protocolo HTTP.

* **Mostrar URL para recursos no publicados** : seleccione esta opción si desea mostrar una URL  [!DNL Dynamic Media Classic] al obtener una vista previa de cualquier recurso, tanto si se ha publicado como si no. Si el recurso no está publicado, la URL no funciona. Sin embargo, puede utilizar la dirección URL para fines de planificación o de organización.

<!-- **Allow AIR install** Select this option to allow users to download Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Dynamic Media Classic AIR. Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **Plantilla de invalidación de CDN** : especifica la plantilla que se utiliza para invalidar la caché de la CDN (red de entrega de contenido).

   Por ejemplo, supongamos que introduce una URL de imagen (incluidos los ajustes preestablecidos de imagen o modificadores) que hace referencia a `<ID>`, en lugar de un ID de imagen específico, como en el siguiente ejemplo:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Si la plantilla solo contiene `<ID>`, Dynamic Media Classic rellena el `https://<server>/is/image`, donde `<server>` es el nombre del servidor de publicación definido en Configuración general.

   Si se define una plantilla de inutilización de CDN, se selecciona una imagen con el nombre Backpack_B y se hace clic en **Archivo** > **Inutilizar en CDN**, se crea la siguiente URL en la interfaz de inutilización de CDN:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   En el cuadro de lista de URL, haga clic en **[!UICONTROL Continuar]** para borrar la caché de esa llamada de URL a la imagen específica. También puede agregar direcciones URL escribiendo o pegándolas en el cuadro de lista de direcciones URL; no es necesario que establezca la plantilla de antemano.

   Después de seleccionar la plantilla de invalidación de CDN y de realizar una solicitud de Invalidar CDN, aparece un indicador en la interfaz de usuario. Proporciona una estimación del tiempo que se tarda en borrar la caché.

   Del mismo modo, si se seleccionan varias imágenes en Dynamic Media Classic al hacer clic en **Archivo** > **Invalidar CDN**, se hace referencia a cada imagen en la URL de plantilla guardada. Por lo tanto, puede definir una plantilla de invalidación de CDN que haga referencia a cada URL a la que se hace referencia en el sitio web (como detalles del producto y resultados de búsqueda). A continuación, al seleccionar una o varias imágenes para la invalidación desde la caché, las direcciones URL rellenan automáticamente la interfaz.

   Consulte [Caché de contenido](dmc-platform-overview.md#content_caching).

   Consulte [Segunda publicación de recursos y retrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Examinar

* **Mostrar proyectos** : determina si los proyectos están disponibles como medio para organizar los recursos de Dynamic Media Classic. Consulte Organización del trabajo con proyectos.

* **Mostrar contenido de eVideo de muestra** : active o desactive la visualización del contenido de ejemplo de eVideo.

* **Mostrar contenido generado** : en las carpetas, muestra el contenido generado a partir de un recurso. Por ejemplo, cuando se rasteriza un archivo PDF a medida que se carga, Dynamic Media Classic crea una imagen para cada página del PDF original. Si la opción Mostrar contenido generado está seleccionada, cada imagen generada durante la carga del PDF original aparecerá junto con el PDF en la carpeta en la que se cargó.

* **Mostrar vídeos codificados** : deseleccionado (desactivado) de forma predeterminada.

   Para buscar vídeos rápidamente en Dynamic Media Classic sin tener que navegar por varios derivados codificados del mismo vídeo, deje esta opción sin seleccionar (predeterminada). En la interfaz de usuario solo se muestra la miniatura del Vídeo principal, que es el vídeo de origen que ha cargado y utilizado para crear todos los derivados, y la miniatura del Conjunto de vídeos adaptable “principal”, que contiene todos los derivados “secundarios” del conjunto de vídeos codificado.

   Sin embargo, puede seguir teniendo acceso a vídeos codificados individuales en el vídeo principal o en el conjunto de vídeos adaptable. Para ello, haga doble clic en la imagen en miniatura del vídeo para abrir la vista de detalles. A continuación, haga clic en **[!UICONTROL Vídeos codificados]** en el panel derecho para tener acceso a todos los vídeos &quot;secundarios&quot;.

   También puede utilizar **[!UICONTROL File]** > **[!UICONTROL Reprocess]** para crear más vídeos &quot;secundarios&quot; codificados directamente desde un conjunto de vídeos adaptables. Dynamic Media Classic encuentra automáticamente el vídeo maestro &quot;principal&quot; del conjunto de vídeos adaptables y lo utiliza como el vídeo de origen para la transcodificación. Sin embargo, cuando se guardan los nuevos vídeos codificados individuales, estos no se ven al buscar o examinar un elemento. No obstante, siguen siendo accesibles desde la ficha Vídeos codificados en la vista de detalles.

   Consulte [Carga y transcodificación de vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Para mantener la capacidad de tener acceso a todos los derivados del vídeo codificado al buscar y examinar, seleccione **Mostrar vídeos codificados**.

   Hay ciertas acciones en el menú Generar que solo funcionan, o funcionan de forma opcional, con vídeos individuales. Esta funcionalidad hace que sea necesario mostrar todos los derivados de vídeos codificados que pueda seleccionar, independientemente de cómo haya definido la opción **Mostrar vídeos codificados**. Las acciones de compilación que anulan la configuración **Mostrar vídeos codificados** incluyen **Conjuntos de vídeos adaptables** y **catálogos electrónicos**.

   >[!NOTE]
   >
   >Si no utilizó Dynamic Media Classic para cargar y codificar los recursos de vídeo, Dynamic Media Classic muestra todos los vídeos codificados individuales, aunque esta opción no esté seleccionada.

* **Mostrar botón Actualizar subcarpetas** : active o desactive la visualización del botón Actualizar de las subcarpetas.

### Cuenta de FTP de Dynamic Media Classic

* **Servidor** : enumera el servidor de cuentas de FTP.

* **Nombre de usuario** : enumera el nombre de usuario de la cuenta de FTP.

### Cargar a la aplicación

* **Sobrescribir imágenes** : Dynamic Media Classic no permite que dos archivos tengan el mismo nombre. El ID de Dynamic Media Classic de cada elemento (el nombre de imagen menos la extensión de nombre de archivo) debe ser único. Debido a esta regla, el cuadro de diálogo Cargar dispone de una opción Sobrescribir. El efecto exacto de esta opción depende de la opción Sobrescribir imágenes especificada. Estas opciones especifican cómo se cargan las imágenes de sustitución: si sustituyen las imágenes originales o si se convierten en imágenes duplicadas. En el caso de las imágenes duplicadas, se cambia su nombre agregando “-1” (por ejemplo, el nombre silla.tif se cambia a silla-1.tif). Estas opciones también afectan a las imágenes cargadas en una carpeta distinta de la original o a las imágenes con una extensión de nombre de archivo diferente de la original (como JPG, TIF o PNG). (Consulte Uso de la opción Sobrescribir imágenes).

   * **Sobrescribir en la carpeta actual, el mismo nombre/extensión de imagen base** : esta opción es la regla más estricta para reemplazar. Exige que la imagen de sustitución se cargue en la misma carpeta y tenga la misma extensión de nombre de archivo que la imagen original. Si no se cumplen estos requisitos, se crea un duplicado.

   * **Sobrescribir en la carpeta actual, el mismo nombre de recurso base independientemente de la extensión** : requiere que cargue la imagen de reemplazo en la misma carpeta que el original, aunque la extensión del nombre de archivo puede ser diferente del original. Por ejemplo, silla.tif sustituye silla.jpg.

   * **Sobrescribir en cualquier carpeta, el mismo nombre/extensión de recurso base** : requiere que la imagen de reemplazo tenga la misma extensión de nombre de archivo que la imagen original (por ejemplo, chair.jpg debe reemplazar a chair.jpg, no chair.tif). Sin embargo, puede cargar la imagen de sustitución en otra carpeta distinta de la original. La imagen actualizada reside en la nueva carpeta; el archivo ya no se encuentra en su ubicación original.

   * **Sobrescribir en cualquier carpeta, el mismo nombre de recurso base independientemente de la extensión** : esta opción es la regla de reemplazo más inclusiva. Puede cargar la imagen de sustitución en otra carpeta distinta de la original, cargar un archivo con una extensión de nombre de archivo diferente y sustituir el archivo original. Si el archivo original está en otra carpeta, la imagen de sustitución residirá en la nueva carpeta en la que se haya cargado.

* **Retener publicación** : especifica si una imagen de reemplazo cargada en Dynamic Media Classic conserva la configuración Listo para publicar de la imagen que está reemplazando o si la configuración se especifica en la carga.

* **Perfiles de color predeterminados** : especifica los perfiles de color aplicados como parte de las Opciones de perfil de color predeterminadas al agregar imágenes CMYK.

* **Opciones de carga predeterminadas** : abre el cuadro de diálogo Opciones de carga de trabajo, donde puede especificar opciones de carga predeterminadas. Para obtener información sobre estas opciones, consulte Opciones de carga.

### Editor de mapas de imagen, a aplicación

* **HREF de asignación de imágenes predeterminada** : define la URL predeterminada utilizada para la columna href de asignación de imágenes. Esta URL es la URL predeterminada que se ve al crear mapas de imagen.

* **Plantilla de asignación de imágenes predeterminada** : define el JavaScript™ predeterminado para la plantilla href de asignación de imágenes. Puede especificar el código personalizado que se debe ejecutar al hacer clic en un mapa de imagen.

### Otras opciones, a aplicación

* **Papelera puede limpiar advertencias** : los activos de la papelera se eliminan automáticamente en un plazo de siete días. Seleccione “Enviar correos electrónicos antes de que los elementos de la papelera se eliminen automáticamente” si desea que se envíen notificaciones a los administradores de la empresa cuando falten cuatro días para que los recursos que hay en la papelera se eliminen de forma permanente. Consulte Gestión de la carpeta Papelera.

## Uso de la opción Sobrescribir imágenes {#using-the-overwrite-images-option}

Dynamic Media Classic no permite que dos archivos tengan el mismo nombre. El ID de Dynamic Media Classic de cada elemento (el nombre de imagen menos la extensión de nombre de archivo) debe ser único. Debido a esta regla, el cuadro de diálogo Cargar incluye las opciones Sobrescribir imágenes. El efecto exacto de esta opción depende de una configuración para la configuración interna de Dynamic Media Classic de cada empresa.

Si anteriormente ha cargado imágenes y después ha cambiado los archivos originales (o los ha reemplazado), la opción Sobrescribir elegida especifica cómo Dynamic Media Classic sustituye las imágenes. No se modifica ningún dato referente a la imagen sino que la nueva imagen sustituye la antigua. Si la carpeta también contiene imágenes que aún no están en Dynamic Media Classic, se añaden estas imágenes.

Use esta opción si las imágenes cargadas han sufrido alguna variación (por ejemplo, se ha alterado una imagen) pero la referencia a ellas permanece igual. La sobreescritura también resulta de utilidad a la hora de cargar y extraer archivos PDF de Adobe®. Para ajustar el modo en que Dynamic Media Classic *copia* la imagen, ajuste las opciones de perfil de color ICC en el cuadro de diálogo Cargar y vuelva a cargar con la función Sobrescribir.

Los ID de Dynamic Media Classic que se utilizan para acceder a imágenes de los servidores de producción se derivan de los nombres de archivo de imagen. El uso de caracteres en mayúsculas y minúsculas en el nombre de archivo es importante, tanto en la sustitución de archivos existentes como para los ID de Dynamic Media Classic que se utilizan para acceder a la imagen. Asegúrese de que el uso de caracteres en mayúsculas y minúsculas en los nombres de archivo sea correcto antes de cargarlos en Dynamic Media Classic para evitar que los ID de Dynamic Media Classic difieran solo en el caso de la misma imagen.

Al anular la selección de esta opción, todas las imágenes que tengan los mismos nombres de archivo como imágenes existentes se tratan como duplicados y, por consiguiente, no se agregan.

## Ajustes preestablecidos de imagen {#image-presets}

En la pantalla Ajustes preestablecidos de imagen se pueden crear y editar ajustes preestablecidos de imagen. Los ajustes preestablecidos permiten a Dynamic Media Classic entregar imágenes de forma dinámica en diferentes tamaños desde la misma imagen maestra. Cada ajuste preestablecido de imagen representa una serie de comandos predefinidos de formato y tamaño que determinan la presentación de las imágenes. Cuando se crea un ajuste preestablecido de imagen, debe elegir un tamaño para la distribución de imágenes. También se deben escoger los comandos de formato para que se optimice el aspecto de la imagen al distribuirla para su visualización.

Los administradores pueden crear ajustes preestablecidos para exportar recursos. Los usuarios pueden elegir un ajuste preestablecido al exportar imágenes, lo que corrige el formato de las imágenes de acuerdo con las especificaciones del administrador.

Para abrir la pantalla Ajuste preestablecido de imagen, en la barra de navegación global, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de imagen]**.

Consulte [Imágenes inteligentes](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Creación y edición de ajustes preestablecidos de imagen {#creating-and-editing-image-presets}

1. Haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes preestablecidos de imagen]**.
1. Cree un ajuste preestablecido o comience desde uno existente:

   * **Creación de un ajuste preestablecido de imagen** : haga clic en  **[!UICONTROL Agregar]**.
   * **Crear un ajuste preestablecido de imagen a partir de un ajuste preestablecido**  existente: seleccione el ajuste preestablecido de imagen que se asemeje más al que desee crear y, a continuación, haga clic en  **[!UICONTROL Editar]**.

1. En la página Agregar (o Editar) ajuste preestablecido, escriba un nombre para el ajuste preestablecido.
1. Defina las opciones de ajustes preestablecidos que desea. 

   Consulte [Opciones de ajuste preestablecido de imagen](application-setup.md#image_preset_options).

1. Haga clic en **[!UICONTROL Guardar]** o, si comenzó a partir de un ajuste preestablecido existente, haga clic en **[!UICONTROL Guardar como]**.
1. Para previsualizar el ajuste preestablecido con su propia imagen, haga clic en **[!UICONTROL Examinar]** y seleccione una imagen. Para obtener una vista previa con la imagen predeterminada, haga clic en **[!UICONTROL Restablecer]**.

Puede editar un ajuste preestablecido de imagen si selecciona su nombre en la pantalla Ajustes preestablecidos de imagen y luego hace clic en Editar. Para eliminar un ajuste preestablecido de imagen, selecciónelo y, a continuación, haga clic en Eliminar.

### Opciones de ajuste preestablecido de imagen {#image-preset-options}

En las pantallas de adición y edición de ajustes preestablecidos, encontrará las siguientes opciones de creación y edición de ajustes preestablecidos de imagen:

* **Nombre de ajuste preestablecido** : introduzca un nombre descriptivo sin espacios en blanco. Para ayudar a los usuarios a identificar este ajuste preestablecido de imagen, incluya la especificación de tamaño de imagen en el nombre.

* **Anchura y altura** : introduzca en píxeles el tamaño en el que se entrega la imagen.

* **Formato** : elija un formato en el menú. Al elegir el formato GIF, JPEG, PDF o TIFF, aparecen más opciones:

   * Opciones de Cuantificación de color GIF

      * **Tipo** : elija Adaptable (opción predeterminada), Web o Macintosh. Si elige GIF con Alpha, la opción Macintosh no estará disponible.

      * **Ditherer** : seleccione Difuminado o Desactivado.

      * **Número de colores** : arrastre el control deslizante para introducir 2-255.

      * **Lista de colores** : introduzca una lista separada por comas. Por ejemplo, para blanco, gris y negro, introduzca 000000,888888,ffffff.
   * Opciones JPEG

      * **Calidad** : controla el nivel de compresión JPEG. Esta configuración afecta tanto al tamaño como a la calidad de la imagen. La escala de calidad JPEG es de 1-100.

      * **Activar el muestreo descendente de crominancia JPG** : como el ojo es menos sensible a la información de color de alta frecuencia que la luminancia de alta frecuencia, las imágenes JPEG dividen la información de la imagen en componentes de luminancia y color. Al comprimir una imagen JPEG, el componente de luminancia conserva la totalidad de su resolución, mientras que la resolución de los componentes de color se disminuye mediante promedios de grupos de píxeles. La disminución de resolución le resta una mitad o un tercio al volumen de los datos sin tener casi ningún impacto en la calidad percibida. La disminución de resolución no se aplica a las imágenes en escala de grises. Esta técnica reduce la cantidad de compresión, lo cual resulta útil para las imágenes de mayor contraste (por ejemplo, las imágenes con texto superpuesto).
   * Opciones PDF y TIFF

      * **Compresión** : elija un algoritmo de compresión.



* **Espacio de color** : elija un espacio de color.

* **Enfoque** : seleccione la opción Habilitar enfoque simple para aplicar un filtro de enfoque básico a la imagen después de que se haya realizado todo el escalado. El enfoque puede ayudar a ver mejor las imágenes borrosas que se obtienen al mostrar una imagen en un tamaño diferente. 

   Para obtener más información acerca del enfoque, los modos de remuestreo y la máscara de enfoque, consulte [Enfoque de imágenes](sharpening-image.md#sharpening_an_image).

* **Modo de remuestreo** : elija una opción de modo de remuestreo. Estas opciones pueden enfocar la imagen cuando se disminuye su resolución:

* **B-Lineal** : el método de remuestreo más rápido; se pueden apreciar algunos artefactos de aliasing.

* **Bicúbico** : Aumenta el uso de CPU en el servidor de imágenes, pero genera imágenes más nítidas con artefactos de alias menos visibles.

* **Sharp2** : puede producir resultados ligeramente más nítidos que la opción Bi-Cubic, pero con un coste de CPU aún mayor en Image Server.

* **Tri-Linear** : Utiliza resoluciones más altas y más bajas, si están disponibles; recomendado solo cuando el alias sea un problema. Este método reduce el tamaño JPEG debido a la reducción de datos de alta frecuencia.

* **Enmascaramiento de enfoque** : elija estas opciones para ajustar el enfoque:

* **Cantidad** : controla la cantidad de contraste aplicado a los píxeles de borde. El valor predeterminado es 1,0. En las imágenes de alta resolución, puede aumentarse hasta 5,0. La cantidad equivaldría a la medida de la intensidad del filtro.

* **Radio** : determina el número de píxeles que rodean los píxeles de borde que afectan al enfoque. Para las imágenes de alta resolución, introduzca una cantidad de 1 a 2. Un valor bajo aplica enfoque solo a los píxeles de borde; un valor alto aplica enfoque a un mayor número de píxeles. El valor adecuado depende del tamaño de la imagen.

* **Umbral** : Determina el intervalo de contraste que se debe ignorar cuando se aplica el filtro de máscara de enfoque. Es decir, esta opción determina en qué deben diferenciarse los píxeles enfocados del área que los rodea antes de ser considerados píxeles de borde y por tanto enfocados. Para evitar la introducción de ruido, experimente con valores entre 0,02 y 0,2. El valor predeterminado (6) aplica enfoque a todos los píxeles de la imagen.

* **Espacio de color** : determina si la imagen utiliza el espacio en el que se creó la imagen, normalmente RGB (original) o un espacio de luminancia (intensidad).

* **** ColorElija estas opciones:

* **Perfil de color de salida** : seleccione Usar predeterminado o uno de los perfiles de color ICC disponibles en Dynamic Media Classic.

   Consulte también [Perfiles ICC](icc-profiles.md#icc_profiles).

* **Renderización** por intenciónSeleccione una opción si desea anular la interpretación predeterminada del perfil de color. Utilice esta opción cuando uno de los perfiles ICC predeterminados es el espacio de color de destino en una conversión de color, un dispositivo de salida (impresora o monitor) está caracterizado por este perfil y la interpretación especificada es válida para este perfil.

* **Incrustar** perfilSeleccione esta opción para que, si abre esta imagen en Adobe® Photoshop®, utilice este perfil.

* **Imprimir** resoluciónElija una resolución para imprimir esta imagen; El valor predeterminado es 72 píxeles.

* **Modificadores** de URLSi prefiere especificar los modificadores de URL que definen el ajuste preestablecido de imagen en lugar de la configuración, introduzca los modificadores aquí.

* **URL de imagen de** ejemploMuestra la cadena URL &quot;sin procesar&quot; que utiliza el servidor de imágenes de Dynamic Media para enviar imágenes con el ajuste preestablecido de imagen que está agregando o editando. Esta cadena URL codifica la configuración de formato seleccionada en las pantallas de adición o de edición de ajustes preestablecidos.

### Edición, eliminación o desactivación de un ajuste preestablecido de imagen {#editing-removing-or-deactivating-an-image-preset}

1. Haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes preestablecidos de imagen]**.
1. En la pantalla Ajustes preestablecidos de imagen, seleccione un ajuste preestablecido de la tabla y, a continuación, realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Editar]** y, a continuación, especifique nuevas opciones en el cuadro de diálogo Editar ajuste preestablecido.
   * Haga clic en **[!UICONTROL Eliminar]** para eliminar el ajuste preestablecido de la lista.
   * Desmarque la casilla **[!UICONTROL Active]** situada junto al nombre de un ajuste preestablecido para eliminarlo de toda la interfaz de usuario de Dynamic Media Classic para los usuarios de MediaPortal.

## Activación o desactivación de los ajustes preestablecidos de vídeos adaptables {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic ofrece ajustes preestablecidos de codificación de vídeo adaptable. Es una lista maestra de ajustes preestablecidos que combina ajustes preestablecidos de vídeo adaptable de 16:9 y ajustes preestablecidos de vídeo adaptable de 4:3 en un grupo. Estos ajustes preestablecidos predefinidos reflejan la configuración de codificación más común y se han optimizado para la reproducción en dispositivos móviles, tablets y escritorios.

De forma predeterminada solo se activan (habilitan o “encienden”) los ajustes preestablecidos de codificación de “Vídeo adaptable”. Puede desactivarlos, si lo desea. Los ajustes preestablecidos de vídeos adaptables inactivos no aparecen como una opción seleccionable en la sección eVideo del cuadro de diálogo Opciones de trabajo de carga.

Consulte [Carga y codificación de vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Para activar y desactivar ajustes preestablecidos de vídeos adaptables:**

1. Cerca de la esquina superior derecha de Dynamic Media Classic, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de vídeo]** > **[!UICONTROL Ajustes preestablecidos de vídeo adaptables]**.
1. En la página Ajustes preestablecidos de vídeo, anule la selección de la casilla de verificación situada junto al nombre de un ajuste preestablecido para quitarlo de la lista Opciones de eVideo del cuadro de diálogo Opciones de trabajo de carga.
1. Haga clic en **[!UICONTROL Cerrar]**.

## Ajustes preestablecidos de vídeo para la codificación de archivos de vídeo {#video-presets-for-encoding-video-files}

Para seleccionar un ajuste preestablecido de codificación, haga clic en Opc. de trabajo en la esquina inferior derecha de la página de carga. En el cuadro de diálogo Opciones de trabajo de carga, expanda Opciones de eVideo y elija los ajustes preestablecidos de codificación de vídeo que desee.

>[!NOTE]
>
>Salvo &quot;Vídeo adaptable&quot;, que está habilitado de forma predeterminada, no puede ver todos los demás ajustes preestablecidos de vídeo adaptable o de codificación de vídeo único en el cuadro de diálogo Opciones de carga de trabajo . Los administradores de Dynamic Media Classic determinan qué ajustes preestablecidos de codificación de vídeo están visibles en el cuadro de diálogo Opciones de carga de trabajo .

* Elija entre los siguientes ajustes preestablecidos de codificación de vídeo adaptable o a ajustes preestablecidos de codificación única:

   * **Vídeo adaptable 16:9** : cree vídeos con una relación de aspecto de 16:9 para su envío a equipos de escritorio, dispositivos móviles (iPhone, iPad, Android™) y tabletas (iPad, Android™), optimizados con la resolución y la velocidad de bits que mejor se adapten a la velocidad de conexión del espectador.

   * **Vídeo adaptable 4:3** : cree vídeos con relación de aspecto 4:3 para su envío a equipos de escritorio, dispositivos móviles (iPhone, iPad, Android™) y tabletas (iPad, Android™), optimizados con la resolución y la velocidad de bits que mejor se adapten a la velocidad de conexión del espectador.

   * **Vídeo adaptable** : un ajuste preestablecido de codificación único que funciona con cualquier proporción de aspecto para crear vídeos para su envío a dispositivos móviles, tabletas y equipos de escritorio. Los vídeos originales cargados que se hayan codificado con este ajuste preestablecido se definirán con una altura fija. Sin embargo, la anchura se escalará automáticamente para mantener la proporción de aspecto del vídeo.

      Esta flexibilidad de tener una “Escala automática” también está disponible de forma predeterminada al crear su propio ajuste preestablecido de codificación de vídeo personalizado.

      Consulte [Adición o edición de un ajuste preestablecido de codificación de vídeo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **Codificación de vídeo adaptable (16:9 o 4:3)** : cree vídeos de relación de aspecto de 16:9 y 4:3 para su envío a equipos de escritorio, dispositivos móviles (iPhone, iPad, Android™) y tabletas (iPad, Android™). Todo optimizado con la resolución y la velocidad de bits que mejor se adapten a la velocidad de conexión del espectador.

      Consulte [Ajustes preestablecidos de vídeo de codificación de vídeo adaptable (16:9 o 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)

   * **Ajustes preestablecidos de codificación única**

      >[!NOTE]
      >
      >Para publicar vídeo en iPad, puede elegir un ajuste preestablecido de codificación Móvil o Tablet. Los ajustes preestablecidos Tablet están diseñados específicamente para iPad, normalmente con mayor resolución y calidad para aprovechar el tamaño de pantalla más grande y la conexión de ancho de banda más alta. La publicación de archivos de vídeo codificados con un ajuste preestablecido Tablet requiere la inclusión de código de detección de dispositivo en la aplicación o sitio móvil. Este código cambia entre la visualización de vídeo en iPhone o iPad, según el dispositivo de reproducción. Si se selecciona un ajuste preestablecido Móvil para la publicación de archivos de vídeo en iPad, el flujo de trabajo es más simple. El motivo es que puede utilizar el mismo archivo de vídeo para iPhone e iPad. Sin embargo, la calidad se estandariza a la visualización de iPhone de menor resolución.

      * En el grupo Ajustes preestablecidos de codificación, en la lista desplegable Ordenar valores preestablecidos de codificación, seleccione Nombre o Tamaño para ordenar los ajustes preestablecidos por el nombre o el tamaño de resolución.
      * Al elegir el ajuste preestablecido de codificación, tenga en cuenta el tamaño de resolución y el ancho de banda con los que se va a reproducir el vídeo. 
      * Puede seleccionar Codificación de vídeo adaptable y uno o varios ajustes preestablecidos de codificación por vídeo. Por ejemplo, puede codificar un archivo para escritorio o dispositivo móvil en un trabajo de carga.

Después de hacer clic en **[!UICONTROL Iniciar carga]**, se carga el archivo de vídeo maestro original y se generan a partir de él los archivos codificados.

### Acerca de las opciones de ajustes preestablecidos de codificación {#about-encoding-preset-options}

Los parámetros de las opciones de ajustes preestablecidos de codificación son los siguientes:

* **Velocidad de conexión de destino** : la velocidad de conexión a Internet del usuario final de destino.

* **Sufijo de archivo codificado** : el sufijo que se adjunta al archivo de vídeo codificado para fines de identificación.

* **Velocidad de bits de vídeo (velocidad de datos)** : cantidad de datos codificados para formar un solo segundo de reproducción de vídeo (en kilobits por segundo).

* **Anchura/altura del píxel** : dimensión de anchura de la imagen de pantalla, en píxeles; la dimensión de altura de la imagen de pantalla (en píxeles).

* **Fotograma por segundo (fps)** : el número de fotogramas o imágenes fijas para cada segundo de vídeo. En Estados Unidos y Japón, la mayoría de los vídeos se graban a 29,97 fps; en Europa y Asia (excluido Japón), la mayoría se graba a 25 fps. Las películas se graban a 24 fps.

* **Velocidad de bits de audio** : cantidad de datos codificados para formar un solo segundo de reproducción de audio, en kilobits por segundo.

En las siguientes tablas se muestran las mejores prácticas recomendadas para seleccionar ajustes preestablecidos de vídeo y las convenciones de designación que se utilizan para dar nombre a los archivos codificados.

### Vídeo adaptable (predeterminado) {#adaptive-video-default}

Un ajuste preestablecido de codificación que funciona con cualquier proporción de aspecto para crear vídeos para su distribución en teléfonos móviles, tablets y equipos de escritorio. Los vídeos originales cargados que se codifiquen con este ajuste preestablecido (valor predeterminado y una práctica recomendada) se definen con una altura fija, mientras que la anchura se escala automáticamente para mantener la proporción de aspecto del vídeo.

**Vídeo adaptable (predeterminado)**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Automático x360, 800 kbps | _Mobile_Autox360p_800K | 800 | Autox360 | Igual que el origen | 64 | Para móvil (iPhone, iPad, Android™) |
| 2 | Automático x 480, 1400 kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | Igual que el origen | 96 | Para tablet (iPad, Android™) |
| 3 | Automático x 720, 2600 kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | Igual que el origen | 128 | Para escritorio |

### Ajustes preestablecidos de vídeo de codificación de vídeo adaptable (16:9 o 4:3) {#adaptive-video-encoding-or-video-presets}

Estos ajustes preestablecidos de codificación de vídeo adaptable combinan una serie de ajustes preestablecidos de codificación individuales que se seleccionan automáticamente en función de la proporción de vídeo que cargue. Por ejemplo, si carga un vídeo de 4:3, se codificará automáticamente con los cinco ajustes preestablecidos de 4:3 de la lista maestra de ajustes preestablecidos en la opción **Codificación de vídeo adaptable (16:9 o 4:3)** .

Para obtener más información sobre los parámetros de las opciones de codificación, consulte [Acerca de las opciones de ajustes preestablecidos de codificación](application-setup.md#about_encoding_preset_options).

**Ajustes preestablecidos de codificación de vídeo adaptable (16:9 o 4:3)**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9, 512 x 288, móvil (iPhone, iPad, Android™), (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 2 | 4:3, 384 x 288 píxeles, móvil (iPhone, iPad, Android™), (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 1 | 16:9, 512 x 288, móvil (iPhone, iPad, Android™), (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 4 | 4:3, 384x288, Móvil (iPhone, iPad, Android™), (600 Kbps) | 700 | _Mobile_384x288_600 | 800 | 384 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 5 | 16:9, 640x360, tableta (iPad, Android™), (800 Kbps) | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Igual que el origen | 80 | Resolución media, WiFi |
| 6 | 4:3, 640 x 480, tableta (iPad, Android™), (800 Kbps) | 900 | _iPad_640x480_800K | 800 | 640 x 480 | Igual que el origen | 80 | Resolución media, Wi-Fi |
| 7 | 16:9, 768 x 432, tableta (iPad, Android™), (1200 Kbps) | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768 x 432 | Igual que el origen | 96 | Alta resolución, Wi-Fi |
| 8 | 4:3, 768 x 576, tableta (iPad, Android™), (1200 Kbps) | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768 x 576 | Igual que el origen | 96 | Alta resolución, Wi-Fi |
| 9 | 16:9, 1280x720, escritorio, (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280 x 720 | Igual que el origen | 128 | Pantalla ancha de alta definición |
| 10 | 4:3, 1280x960, escritorio, (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280 x 960 | Igual que el origen | 128 | Alta definición |

### Ajustes preestablecidos de codificación de vídeo para equipos de escritorio {#desktop-video-encoding-presets}

Ajustes preestablecidos de codificación de vídeo para MP4 y OGV en ordenadores de escritorio.

Para obtener más información sobre los parámetros de las opciones de codificación, consulte [Acerca de las opciones de ajustes preestablecidos de codificación](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2, audio AAC, extensión de archivo MP4**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Igual que el origen | 64 | Pantalla ancha de baja resolución |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640 x 360 | Igual que el origen | 80 | Resolución media para pantalla ancha |
| 1 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Igual que el origen | 96 | Resolución media/alta |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280 x 720 | Igual que el origen | 128 | Pantalla ancha de alta definición |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320 x 240 | Igual que el origen | 64 | Baja resolución |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Igual que el origen | 80 | Resolución media |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640 x 480 | Igual que el origen | 96 | Resolución media/alta |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280 x 960 | Igual que el origen | 128 | Alta definición |

**OGG Theora Vorbis - extensión de archivo OGV**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de datos de vídeo (kbps) | Anchura/Altura (píxeles) | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Igual que el origen | 64 | Pantalla ancha de baja resolución |
| 2 | 16:9, 640 x 360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Igual que el origen | 80 | Resolución media para pantalla ancha |
| 3 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | Igual que el origen | 96 | Resolución media/alta |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280 x 720 | Igual que el origen | 128 | Pantalla ancha de alta definición |
| 5 | 4:3, 320 x 240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Igual que el origen | 64 | Baja resolución |
| 6 | 4:3, 480x360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Igual que el origen | 80 | Resolución media |
| 7 | 4:3, 640 x 480 (1200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640 x 480 | Igual que el origen | 96 | Resolución media/alta |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280 x 960 | Igual que el origen | 128 | Alta definición |

### Ajustes preestablecidos de codificación de vídeo para dispositivos móviles {#mobile-video-encoding-presets}

Igual que fps del origen. Ajustes preestablecidos de codificación de vídeo para dispositivos móviles iPhone, iPad y Android™.

Para obtener más información sobre los parámetros de las opciones de codificación, consulte [Acerca de las opciones de ajustes preestablecidos de codificación](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1, audio AAC, extensión de archivo MP4**

|  | Nombre de ajuste preestablecido de codificación/Texto de información sobre herramientas | Velocidad de conexión de destino (kbps) | Sufijo de archivo codificado | Velocidad de bits de vídeo (Kbps) | Anchura y altura en píxeles | Fps | Velocidad de bits de audio (kbps) | Recomendaciones |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9, 512 x 288 , Móvil (400 kbps) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 2 | 16:9, 512 x 288 , Móvil (600 kbps) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 1 | 16:9, 512 x 288 , Móvil (800 kbps) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Igual que el origen | 80 | Resolución media, Wi-Fi |
| 4 | 16:9, 512 x 288 , Móvil (1000 kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1.000 | 512 x 288 | Igual que el origen | 80 | Alta resolución, Wi-Fi |
| 5 | 16:9, 512 x 288 , Móvil (1200 kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512 x 288 | Igual que el origen | 96 | Alta resolución, Wi-Fi |
| 6 | 4:3, 384 x 288 , Móvil (400 kbps) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Igual que el origen | 64 | Baja resolución, 3G |
| 7 | 4:3, 384 x 288 , Móvil (600 kbps) | 700 | _Mobile_384x288_600K | 800 | 384 x 288 | Igual que el origen | 64 | Resolución media, 3G |
| 8 | 4:3, 448 x 336 , Móvil (800 kbps) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Igual que el origen | 80 | Resolución media, Wi-Fi |
| 9 | 4:3, 448 x 336 , Móvil (1000 kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1.000 | 448 x 336 | Igual que el origen | 80 | Alta resolución, Wi-Fi |
| 10 | 4:3, 448 x 336 , Móvil (1200 kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448 x 336 | Igual que el origen | 96 | Alta resolución, Wi-Fi |

## Ajustes preestablecidos de visor {#viewer-presets}

>[!NOTE]
>
>**Aviso de fin de vida útil de los visores de Flash** : a partir del 31 de enero de 2017, Adobe Dynamic Media Classic dejó de ser compatible con la plataforma del visor de Flash.

Un *ajuste preestablecido de visor* es una serie de opciones que determinan la manera en que los usuarios verán los recursos de medios enriquecidos en la pantalla de su ordenador y dispositivos móviles. Como administrador, puede crear ajustes preestablecidos de visor. Se pueden configurar varias opciones de configuración para los visores. Por ejemplo, puede cambiar el tamaño, el comportamiento del zoom, las combinaciones de colores, los bordes y las fuentes del visor.

Se recomienda utilizar los visores de vídeo HTML5 de Dynamic Media Classic. Los ajustes preestablecidos utilizados en los visores de vídeo HTML5 son reproductores de vídeo sólidos. Al combinar en un solo reproductor la capacidad para diseñar los componentes de reproducción mediante HTML5 y CSS, tener la reproducción incorporada y usar flujo adaptable y progresivo en función de la capacidad del explorador, se amplía el alcance del contenido de medios enriquecidos para los usuarios de móviles, tablets y de escritorio y se garantiza una experiencia optimizada de vídeo.

Consulte [Acerca de los visores HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) en la Guía de referencia de visores de Adobe.

Consulte [Matriz de compatibilidad de ajustes preestablecidos de visor de Dynamic Media Classic](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consulte [Práctica recomendada: Uso del visor de vídeo HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Dependiendo del visor, puede añadir funciones de comunidad. Las funciones de la comunidad incluyen los botones de incrustación, enlace y visita al sitio. Estos botones permiten a las personas que utilizan los visualizadores compartir el visualizador con otras personas o abrir el sitio web de Dynamic Media Classic.

Consulte también [Ejemplos de la biblioteca de referencia de visores de Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Compatibilidad de los visores para páginas web diseñadas para interactividad {#viewer-support-for-responsive-designed-web-pages}

Diferentes páginas Web tienen diferentes necesidades. A veces se desea una página web que proporcione un vínculo que abra el visor HTML5 en una ventana independiente del explorador. En otros casos, es necesario incrustar el visor HTML5 directamente en la página de alojamiento. En este último caso, es probable que la página web tenga un diseño estático. O bien, es &quot;interactivo&quot; y se muestra de forma diferente en diferentes dispositivos o para diferentes tamaños de ventana del navegador. Para satisfacer estas necesidades, los visores HTML5 que se incluyen con Dynamic Media Classic admiten tanto páginas web estáticas como páginas web diseñadas interactivas.

Para obtener más información sobre cómo incrustar visores interactivos en sus páginas web, consulte [Acerca de la biblioteca de imágenes interactivas](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [Uso de la biblioteca de imágenes interactiva](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api) y [Referencia de comandos: atributos de comando](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### Tipos de ajustes preestablecidos {#viewer-preset-types}

Los administradores pueden crear y personalizar los siguientes tipos de valores preestablecidos de visor:

* **eCatalog Viewer** : simula la experiencia de leer un catálogo impreso. Puede moverse de una página a otra, acercar y alejar elementos de una página, usar mapas de imágenes para ver más información sobre los elementos de la página o buscar en el catálogo. También puede incluir un panel de información para mostrar información detallada y un elemento de mapa de imagen si el área del mapa tiene un atributo rollover_key válido. Para incluir un panel de información, especifique una dirección URL del servidor de información en la configuración del panel de información de la ventana de ajuste preestablecido de visor de catálogo electrónico.

* **Visor de conjuntos de muestras** : muestra una imagen en un color, material, textura, acabado o tela diferentes. Los usuarios deben hacer clic en una miniatura para ver las variaciones en la imagen.

* **Visor de conjuntos de medios mixtos** : muestra distintos tipos de medios en un visor. Puede incluir conjuntos de muestras, conjuntos de giros, imágenes y vídeos. Puede configurar fichas que contengan distintos tipos de contenido, como una ficha para conjuntos de imágenes y otra ficha para vídeos. Los vídeos que se reproducen desde un conjunto de medios mixtos usan un visor de vídeo estándar con una línea de tiempo y controles de vídeo, como Detener, Pausa, Rebobinar y Reproducir. Al configurar un ajuste preestablecido de visor de conjuntos de medios mixtos, debe especificar qué visores desea usar para los diferentes tipos de recursos en su conjunto de medios mixtos. También puede usar el visor de cuadrícula o carrusel para ver un conjunto de medios mixtos.

* **Visor de conjuntos de giros** : proporciona varias vistas de una imagen para que los usuarios puedan girar el objeto y examinar los distintos lados y ángulos.

* **Visor de vídeos** : muestra vídeos utilizando las dimensiones de resolución del archivo de origen o un tamaño personalizado. Dynamic Media Classic incluye muchos ajustes preestablecidos de visor predefinidos para reproducir vídeo. Si es administrador, puede crear ajustes preestablecidos de visor de vídeo personalizados. Hay más de una docena de opciones de configuración diferentes para personalizar el visor de vídeo. Puede configurar el tamaño, el color de primer plano y fondo, los controles de audio y vídeo, la barra de progreso, la apariencia de la interfaz del usuario, las funciones sociales y la ayuda del visor.

* **Visualizadores de zoom** : ofrece tres tipos de visor de zoom:

* **Visor de zoom** : permite a los usuarios acercarse al área haciendo clic en ella. Pueden hacer clic en los controles para acercarse, alejarse y restablecer la imagen a su tamaño predeterminado.

* **Visor de zoom: Salida** : muestra una segunda imagen del área ampliada junto a la imagen original. No hay controles, los usuarios simplemente mueven la selección sobre la zona que desean ver.

Al determinar el uso del ancho de banda completo para este visor, tenga en cuenta que tanto la imagen principal como la imagen flotante se muestran en el visor. El tamaño de imagen principal (la anchura y altura de escenario) y el factor de zoom determinan el tamaño de la imagen flotante. Para evitar que el tamaño del archivo flotante sea demasiado grande, equilibre estos dos valores: si el tamaño de la imagen principal es muy grande, reduzca el valor de Factor de zoom. (Los valores de Anchura flotante y Altura flotante determinan el tamaño de la ventana flotante, pero no el tamaño de la imagen que se muestra en el visor).

Por ejemplo, si el tamaño de la imagen principal es 350 x 350 píxeles, con un factor de zoom de 3, el tamaño de la imagen flotante que resultará será de 1050 x 1050 píxeles. Si el tamaño de la imagen principal es de 300 x 300 píxeles, con un factor de zoom de 4, el tamaño de la imagen flotante será de 1200 x 1200 píxeles. Según el ajuste de calidad JPEG (el recomendado es entre 80 y 90), podrá reducir el tamaño del archivo en gran medida. Los factores de zoom recomendados son de 2,5 a 4, según el tamaño de la imagen principal.

### Matriz de compatibilidad con ajustes preestablecidos de visor de Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Aviso** de fin de vida útil para los visualizadores de Flash: A partir del 31 de enero de 2017, Adobe Dynamic Media Classic dejó de ofrecer asistencia para la plataforma del visor de Flash.

La tabla siguiente identifica los ajustes preestablecidos de visor de Dynamic Media Classic actualmente disponibles. En la tabla también se especifica la compatibilidad del visor con los ordenadores y los dispositivos móviles, así como la tecnología empleada para cada visor.

Consulte también [Ejemplos de la biblioteca de referencia de visores de Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Para obtener información sobre las versiones de sistema operativo y navegador web admitidas para los visores, consulte las notas de la versión de los visores.

Consulte [Notas de la versión de referencia de visores de Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de imágenes |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de muestras |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de catálogos electrónicos |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(incluye compatibilidad con medios sociales y búsqueda de catálogos). | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(incluye compatibilidad con medios sociales y búsqueda de catálogos). | HTML5 | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de giros |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visores de eVideo**

Dynamic Media Classic admite la reproducción de vídeo móvil para vídeo MP4 H.264.

* Puede encontrar los dispositivos BlackBerry® compatibles con este formato de vídeo en el siguiente enlace: [Formatos de vídeo compatibles con BlackBerry®](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* También puede encontrar dispositivos Windows® compatibles con este formato de vídeo en el siguiente enlace: [Formatos de vídeo compatibles con Windows® Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ | Smartphone BlackBerry® | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(incluye compatibilidad con subtítulos optativos). Consulte [Práctica recomendada: Uso del visor de vídeo universal HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(incluye compatibilidad con subtítulos y medios sociales). | HTML5 | X | X | X | X | X | X | X |

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de medios mixtos |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Tabla de gestos de visores móviles admitidos {#supported-mobile-viewers-gestures-matrix}

La siguiente tabla identifica los gestos del visor móvil compatibles con los dispositivos iOS, Android™ 2.x y Android™ 3.x.

|  | Tecnología de visor | Ordenador | Apple iPhone | Apple iPad | Smartphone Android™ | Tableta Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visores de conjuntos de imágenes |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Sobre la pantalla Valor predeterminado del visualizador {#about-the-viewer-preset-screen}

Esta pantalla permite crear y gestionar ajustes preestablecidos de visor. Para abrir esta pantalla, haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes preestablecidos de visor]**.

La pantalla Ajustes preestablecidos de visor ofrece una serie de herramientas para realizar las siguientes tareas:

* **Adición de un ajuste preestablecido** : haga clic en  **** Agregar y elija las opciones que desee en el cuadro de diálogo Agregar ajuste preestablecido de visualizador.

       Consulte [Adición y edición de ajustes preestablecidos de visualizador](application-setup.md#adding_and_editing_viewer_presets).
   
* **Edición de un ajuste preestablecido** : seleccione un ajuste preestablecido y, a continuación, haga clic en  **[!UICONTROL Editar]**.

       Consulte [Adición y edición de ajustes preestablecidos de visualizador](application-setup.md#adding_and_editing_viewer_presets).
   
* **Eliminación de un ajuste preestablecido** : seleccione un ajuste preestablecido y, a continuación, haga clic en  **[!UICONTROL Eliminar]**.

* **Exportación de un ajuste preestablecido** : seleccione un ajuste preestablecido de visualizador HTML5 y, a continuación, haga clic en  **** Exportación para descargar el aspecto del visualizador, de modo que pueda utilizarlo como base para crear y añadir otro ajuste preestablecido de visualizador.

       Consulte [Exportación de un ajuste preestablecido de visualizador HTML5](application-setup.md#export_an_html5_viewer_preset).
   
* **Filtrado de la lista Ajustes preestablecidos de visor** : Utilice estas herramientas para filtrar la lista:

       * Abra la lista desplegable **Activo/Inactivo** y elija una opción para mostrar los ajustes preestablecidos activos, inactivos o todos los ajustes preestablecidos.
       * Abra la lista desplegable **Visualizador** y elija una opción para ver solo los visualizadores de un tipo determinado. Seleccione **[!UICONTROL Todos los visualizadores]** para ver todos los visualizadores.
   
* **Ordenar ajustes preestablecidos** : haga clic en un encabezado de columna (**[!UICONTROL Activo]**,  **[!UICONTROL Tipo]**,  **[!UICONTROL Ajuste preestablecido]** o  **[!UICONTROL Plataforma]**) para ordenar la lista en una columna. Vuelva a hacer clic en el encabezado de columna para ordenar la lista en orden descendente (o ascendente).

* **Activación y desactivación de ajustes preestablecidos** : seleccione un ajuste preestablecido y haga clic en su opción Activo para activarlo o desactivarlo.

       Consulte [Activación o desactivación de ajustes preestablecidos de visor](application-setup.md#activating_or_deactivating_viewer_presets).
   
>[!NOTE]
>
>Haga clic en **[!UICONTROL Vista previa]** en el lado derecho de la página Ajustes preestablecidos de visor para ver el aspecto de un recurso en el ajuste preestablecido de visor que ha seleccionado. Para ver otro recurso, haga clic en **[!UICONTROL Examinar]** en la página Ajustes preestablecidos de visor y seleccione otro recurso en el cuadro de diálogo Seleccionar vista previa de recurso.

### Adición y edición de ajustes preestablecidos de visor {#adding-and-editing-viewer-presets}

Además de agregar ajustes preestablecidos de visualizador mediante **[!UICONTROL Add]** en la interfaz de usuario, también puede utilizar **[!UICONTROL Export]** para agregar un ajuste preestablecido de visualizador. Simplemente exporte un ajuste preestablecido de visor HTML5 existente y, a continuación, utilícelo como base para el nuevo ajuste preestablecido.

Consulte [Exportación de un ajuste preestablecido de visor HTML5](application-setup.md#exporting_an_html5_viewer_preset).

**Para añadir y editar ajustes preestablecidos de visor:**

1. Cerca de la esquina superior derecha de Dynamic Media Classic, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visor]**.

   Puede filtrar la lista de ajustes preestablecidos. Por ejemplo, para ver solo los ajustes preestablecidos para los visores de vídeos, seleccione Visor de vídeos en el menú desplegable de visores que hay en la barra de herramientas, justo encima de la tabla.

1. En la página Ajustes preestablecidos de visor , añada o edite el Ajuste preestablecido de visor en la pantalla Ajustes preestablecidos de visor .

   * **Adición** : en la barra de herramientas, haga clic en  **[!UICONTROL Agregar]**. En el cuadro de diálogo Añadir ajuste preestablecido de visor, elija una plataforma y seleccione un tipo de recurso de medios enriquecidos.

          Haga clic en **[!UICONTROL Guardar como]** cuando haya terminado de crear el ajuste preestablecido de visor.
      
   * **Agregar empezando por un ajuste preestablecido de visualizador existente** : en la tabla, seleccione un ajuste preestablecido de visualizador de vídeo y, a continuación, haga clic en Editar en la barra de herramientas.

          Después de volver a configurar el visualizador de vídeo, haga clic en **[!UICONTROL Guardar como]** para guardar el ajuste preestablecido con un nombre diferente en el campo de texto Nombre del ajuste preestablecido .
      
   * **Edición** : seleccione un ajuste preestablecido de visualizador existente y, a continuación, haga clic en  **[!UICONTROL Editar]**.

1. En la pantalla Configurar visor, en el campo Nombre de ajuste preestablecido, escriba o edite el nombre.
1. Defina las opciones restantes que desee.

   >[!NOTE]
   >
   >Haga clic en **[!UICONTROL Igual que el origen]** para cambiar automáticamente el tamaño del visualizador de vídeo según el tamaño de resolución del propio vídeo codificado. Si elige esta opción, no puede introducir la anchura ni la altura del escenario sino que estas opciones proceden del propio vídeo. Si selecciona Igual que el origen, configure la opción de tamaño de margen para que refleje las dimensiones de aspecto fuera del área de reproducción de vídeo. Este tamaño de margen es la altura y anchura de píxel de los controles de vídeo. La siguiente ilustración le ayuda a determinar los tamaños de margen que se deben utilizar.*

   ![Configuración de márgenes del visor de vídeo](assets/vs_video_viewer_configure_margin.png)

1. Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Guardar como]** si ha agregado un ajuste preestablecido de visor a partir de uno existente.
   * Haga clic en **[!UICONTROL Guardar]** si ha agregado o editado un ajuste preestablecido de visor.

### Exportación de un ajuste preestablecido de visor HTML5 {#exporting-an-html-viewer-preset}

Puede exportar un ajuste preestablecido de visor HTML5 existente para utilizarlo como base para crear un ajuste preestablecido de visor HTML5. Esta opción de exportación resulta útil porque no tiene que crear el visor de cero, sino que puede exportar un ajuste preestablecido con un aspecto y un comportamiento parecidos a los deseados y, luego, usarlo como punto de partida para realizar ajustes de diseño.

Todos los archivos CSS preestablecidos de visualizador predeterminados y listos para usar en Dynamic Media Classic utilizan rutas de servicio de imágenes relativas que apuntan a recursos en `Scene7SharedAssets`. Por ejemplo, la siguiente es una ruta relativa a un recurso de imagen en un archivo CSS preestablecido de visor en

`Scene7SharedAsset`:  `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Sin embargo, si aloja archivos CSS de visor en su propio sitio, debe resolver estas rutas de imagen relativas utilizando una ruta explícita al servidor de imágenes en su propio entorno. Con fines ilustrativos, si actualizara la ruta relativa anterior a una ruta explícita, podría parecerse a la siguiente, donde `https://s7d1.scene7.com` es la ruta directa al servidor de imágenes: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Para exportar un ajuste preestablecido de visor HTML5:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes preestablecidos de visor]**.
1. En la barra de herramientas Ajustes preestablecidos de visor, en la segunda lista desplegable de la izquierda, seleccione **[!UICONTROL HTML5]**.
1. En la tercera lista desplegable desde la izquierda, seleccione **[!UICONTROL Todos los visores]**.
1. Seleccione el ajuste preestablecido de visor que desee utilizar como base para un nuevo ajuste preestablecido de visor HTML5.
1. En la barra de herramientas, haga clic en **[!UICONTROL Exportar]**.
1. En el cuadro de diálogo Exportar recursos seleccionados, haga clic en **[!UICONTROL Enviar exp.]**.

   Después de la exportación, obtiene un archivo CSS. Descargue y descomprima el archivo.

1. Abra el archivo CSS en un editor de CSS, realice los cambios oportunos y, a continuación, guarde el archivo.
1. Cargue el archivo CSS en Dynamic Media Classic.

   Consulte [Carga de archivos](uploading-files.md#uploading_files).

1. Publique el archivo CSS en Dynamic Media Image Server.

   Consulte [Publicación de archivos](publishing-files.md#publishing_files).

1. Añada el nuevo ajuste preestablecido de visor del modo habitual. Seleccione el archivo CSS del visor que ha cargado.

   Consulte [Adición y edición de ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

### Activación o desactivación de ajustes preestablecidos de visor {#activating-or-deactivating-viewer-presets}

Para crear una URL y mostrar los recursos, los usuarios deben abrir la lista desplegable Ajustes preestablecidos del cuadro de diálogo Vista previa, seleccionar un Ajuste preestablecido de visor y hacer clic en Copiar URL (consulte [Copia de la dirección URL de un ajuste preestablecido de visor](application-setup.md#copying_the_url_of_a_viewer_preset)). La lista Ajustes preestablecidos contiene unos ajustes que los administradores pueden agregar y gestionar desde la pantalla Ajustes preestablecidos de visor. Por ejemplo, cuando un usuario obtiene una vista previa de un catálogo electrónico, todos los ajustes preestablecidos de visor del catálogo activo aparecen en la lista desplegable Ajustes preestablecidos, en el cuadro de diálogo Vista previa.

Si no desactiva los ajustes preestablecidos de visor en su pantalla correspondiente, la lista desplegable de ajustes del cuadro de diálogo Ajustes preestablecidos puede llenarse demasiado. 

**Para activar o desactivar ajustes preestablecidos de visor:**

1. Seleccione **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visor]**.
1. En la página Ajustes preestablecidos de visor , seleccione o anule la selección de las opciones **[!UICONTROL Active]** para activar o desactivar ajustes preestablecidos de visor.

### Copia de la dirección URL de un ajuste preestablecido de visor {#copying-the-url-of-a-viewer-preset}

Tras publicar un recurso, puede copiar una URL para mostrar el recurso con la configuración de un ajuste preestablecido de visor.

La URL se copiará en el portapapeles. Podrá utilizarla como sea necesario en el código HTML de su página web, dispositivo móvil o aplicación.

**Para copiar la dirección URL de un ajuste preestablecido de visor:**

1. Seleccione el recurso en el panel Examinar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **[!UICONTROL Copiar URL]** a la derecha del visor que desee.
   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** debajo de la imagen en miniatura.

   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Copiar URL]**.

   * Haga clic en **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** a la derecha de la imagen en miniatura.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Copiar URL]**.

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Copiar URL]**.

### Copia del código incrustado de un ajuste preestablecido de visor  {#copying-the-embed-code-of-a-viewer-preset}

El uso de la función de código incrustado permite revisar el código del ajuste preestablecido de visor seleccionado. También puede copiar el código en el portapapeles para pegarlo en sus páginas web para la implementación del visor. 

No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un ajuste preestablecido de visor:**

1. Seleccione el recurso en el panel de exploración de recursos.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel Direcciones URL de la derecha, haga clic en **[!UICONTROL Código incrustado]**.
   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** debajo de la imagen en miniatura.

   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Código incrustado]**.

   * Haga clic en **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** a la derecha de la imagen en miniatura.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Código incrustado]**.

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.
   En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Código incrustado]**.

1. En el cuadro de diálogo Código incrustado, haga clic en **[!UICONTROL Copiar al portapapeles]**.
1. Haga clic en **[!UICONTROL Cerrar]**.

## Configuración de los visores predeterminados {#configuring-default-viewers}

Puede utilizar Visualizadores predeterminados para configurar el visualizador predeterminado asociado a un recurso cuando utilice Vista previa en Dynamic Media Classic. Puede configurar la experiencia de previsualización por defecto para los siguientes tipos de recursos:

* Imagen
* Vídeo
* Conjunto de giros
* Catálogo
* Conjunto de imágenes
* Conjunto de muestras
* Conjunto de medios

**Para configurar los visores predeterminados:**

1. En la lista desplegable Configuración , haga clic en **[!UICONTROL Ajustes de aplicación]**.
1. En la ventana Configuración, en el panel izquierdo, expanda **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Visualizadores]**
1. Haga clic en **[!UICONTROL Visualizadores predeterminados]**.
1. En la ventana Visores predeterminados, en la lista desplegable para cada tipo de recurso, seleccione el visor que desee asociar con la vista previa del recurso.
1. En la esquina inferior derecha de la ventana Visualizadores predeterminados, haga clic en **[!UICONTROL Guardar configuración]**.
1. En la esquina inferior derecha de la ventana Configuración, haga clic en **[!UICONTROL Cerrar]** para volver a la ventana Recurso.

## Vistas de metadatos {#metadata-views}

Los *metadatos* constituyen un conjunto de información estandarizada sobre un recurso. Puede utilizar metadatos para perfeccionar el flujo de trabajo, organizar sus recursos y mejorar las búsquedas. Dynamic Media Classic es compatible con el estándar IPTC (International Press Telecommunications Council) y el estándar XMP (extensible metadata platform). Antes de que los usuarios vean o introduzcan metadatos sobre un recurso en la vista de detalles, pueden abrir el menú Vistas de metadatos . Desde allí, pueden elegir el conjunto de campos de metadatos que desean ver o utilizar para describir el recurso.

Dynamic Media Classic incluye vistas de metadatos predefinidas y los administradores pueden crear sus propias vistas de metadatos para que los usuarios puedan elegir cuándo introducen metadatos.

### Creación de una vista de metadatos {#creating-a-metadata-view}

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Vistas de metadatos]**.
1. Haga clic en **[!UICONTROL Agregar]**.
1. En el campo de texto Nombre de ajuste preestablecido , introduzca un nombre para la vista.
1. (Opcional) Marque **[!UICONTROL Establecer como predeterminado]** para que esta vista sea la que ven los usuarios cuando abren el panel Metadatos en la Vista de detalles.
1. (Opcional) Seleccione **[!UICONTROL Include UDF]** para incluir los campos definidos por el usuario en la vista. Los campos definidos por el usuario aparecen en la parte superior del panel Metadatos en la vista de detalles.
1. Seleccione los campos que desee para la vista (haga clic en **[!UICONTROL Select All]** para seleccionar todos los campos).
1. Haga clic en **[!UICONTROL Guardar]**.

   Las categorías y los campos seleccionados de la vista aparecen en el panel Vista previa.

### Gestión de vistas de metadatos {#managing-metadata-views}

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Vistas de metadatos]**.
1. Realice una de las siguientes acciones:

   * Para obtener una vista previa de una vista, selecciónela. Los campos de la vista aparecen en el panel Vista previa.
   * Para editar una vista, selecciónela y haga clic en **[!UICONTROL Editar]**. A continuación, seleccione o anule la selección de los nombres de campo en el panel Vista previa y seleccione o anule la selección de la opción **[!UICONTROL Incluir UDF]**.
   * Para eliminar una vista, selecciónela y haga clic en **[!UICONTROL Eliminar]**.
   * Para que una vista sea la predeterminada, selecciónela y haga clic en **[!UICONTROL Establecer como predeterminada]**. La vista predeterminada es aquella que ven los usuarios cuando abren un recurso en la vista de detalles y acceden al panel Metadatos.

## Ajustes preestablecidos de metadatos {#metadata-presets}

Los ajustes preestablecidos ofrecen a los administradores un método para controlar y regular metadatos que se asignan a los recursos. En la vista de detalles, un usuario puede introducir metadatos sobre un recurso en los campos que se proporcionan para ese propósito. Por ejemplo, un usuario puede introducir el nombre de un propietario, la descripción de derechos de autor y la dirección. Para asegurarse de que los usuarios introducen esta información de un modo preciso y completo, puede crear ajustes preestablecidos de metadatos. La elección de un ajuste preestablecido de metadatos en la Vista de detalles rellena los campos de metadatos con valores predefinidos. Por ejemplo, el nombre de un propietario, la descripción de derechos de autor y la dirección se rellenan de forma automática.

Cree un ajuste preestablecido de metadatos para cada conjunto de valores de metadatos que desee que los usuarios puedan introducir de forma automática en la vista de detalles para describir un recurso. 

### Creación o edición de un ajuste preestablecido de metadatos {#creating-or-editing-a-metadata-preset}

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Ajustes preestablecidos de metadatos]**.
1. En la pantalla Ajustes preestablecidos de metadatos, realice lo siguiente:

   * Para crear un ajuste preestablecido, haga clic en **[!UICONTROL Add]**. En el campo de texto Nombre de plantilla de metadatos , escriba un nombre para el ajuste preestablecido, haga clic en **[!UICONTROL Vistas de metadatos]** y elija una vista en la lista desplegable (consulte [Vistas de metadatos](application-setup.md#metadata_views)).
   * Para editar un ajuste preestablecido existente, selecciónelo en la lista Ajustes preestablecidos de metadatos y haga clic en **[!UICONTROL Editar]**.

1. Expanda los encabezados que desee incluir en el ajuste preestablecido e introduzca los valores en los distintos campos que desee incluir en este ajuste.
1. Haga clic en **[!UICONTROL Guardar]**.

   Las categorías y los campos seleccionados para el ajuste preestablecido aparecen en el panel Vista previa.

### Gestión de ajustes preestablecidos de metadatos {#managing-metadata-presets}

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Ajustes preestablecidos de metadatos]**.
1. Realice una de las siguientes acciones:

   * Para obtener la vista previa de un ajuste preestablecido, selecciónelo. La información del ajuste preestablecido (categorías y campos) aparece en la pantalla Ajuste preestablecido.
   * Para eliminar un ajuste preestablecido, selecciónelo y haga clic en **[!UICONTROL Eliminar]**.

## Campos personalizables {#user-defined-fields}

Un administrador de Media Portal o un administrador de empresa pueden crear campos de metadatos personalizables o personalizados. Los campos personalizados pueden ayudarle a organizar los recursos en Dynamic Media Classic. Puede marcar los campos como Activo, según sea necesario. Cuando están activados, los nombres de estos campos de metadatos personalizados aparecen en el panel Metadatos, en la vista de detalles. Los usuarios pueden introducir información en los campos de metadatos definidos por el usuario para describir los recursos. También pueden utilizar un campo de metadatos definido por el usuario como criterio de búsqueda.

Un uso efectivo de los campos de metadatos personalizables es retardar el tiempo de activación de un recurso para un lanzamiento o una oferta específicos. Se define un campo &quot;activación&quot;, basado en el tipo *Date*. A continuación, con el panel **[!UICONTROL Metadatos]** en la vista de detalles o **[!UICONTROL Archivo]** > **[!UICONTROL Editar información]**, puede especificar cuándo se activa el recurso. Dynamic Media Classic comprueba el estado de publicación de un recurso y el historial de publicación. Si no se encuentra dentro del tiempo de activación, el estado de publicación se muestra como &quot;No publicado&quot;.

>[!NOTE]
>
>Para que los campos definidos por el usuario aparezcan en el panel Metadatos de la vista de detalles, inclúyalos en las vistas de detalles. En la pantalla Vistas de metadatos, seleccione la opción Incluir UDF (campos definidos por el usuario). Para obtener más información, consulte [Vistas de metadatos](application-setup.md#metadata_views).

>[!NOTE]
>
>Para buscar recursos utilizando los campos personalizados o personalizables, haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes personales]** y seleccione **[!UICONTROL Incluir UDF en la búsqueda]**. Consulte [Ajustes personales](personal-setup.md#personal_setup).

### Creación de un campo de metadatos definido por el usuario {#creating-a-user-defined-metadata-field}

1. Haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Campos personalizables]**.
1. Haga clic en **[!UICONTROL Agregar]**.
1. En el cuadro de diálogo Campo personalizado, seleccione las opciones que desee.

   * **Nombre** : introduzca un nombre para el campo de metadatos.

   * **Tipo** : elija una opción que defina el tipo de información que los usuarios pueden introducir en el campo de metadatos:

   * **Cadena** : una cadena de texto.

   * **Int** : un número entero.

   * **Flotante** : un número de coma flotante.

   * **Sí/No** : un valor booleano sí/no.

   * **Fecha** : una fecha. Se acepta el formato MM/DD/AAAA.

   * **Nombre de archivo** : el nombre de un archivo.

   * **Color** : nombre de un color.

   * **Dimension** : anchura y altura del recurso.

   * **Sin tipo** : para la compatibilidad con versiones anteriores. No seleccione esta opción.

   * **Valor predeterminado** : Opcionalmente, introduzca el valor que es más probable que introduzcan los usuarios en el campo. El valor introducido se convertirá en el valor predeterminado del campo que cree.

   * **Se aplica a** : De forma opcional, elija un tipo de recurso si desea que el campo de metadatos se aplique solo a un tipo específico de recurso.

      >[!NOTE]
      >
      >Elija cuidadosamente una opción **[!UICONTROL Aplica a]** porque no puede cambiar la opción **[!UICONTROL Aplica a]** después de crear un campo definido por el usuario. Dynamic Media Classic permite editar el nombre, el tipo y el valor predeterminado de un campo definido por el usuario, pero no la configuración **[!UICONTROL Se aplica a]**. *

1. Haga clic en **[!UICONTROL Guardar]** cuando termine de crear el campo de metadatos.

### Gestión de campos personalizables {#manage-user-defined-fields}

La pantalla Campos personalizables ofrece comandos para gestionar campos de metadatos personalizados definidos por el usuario.

Solo un administrador de Media Portal o un administrador de empresa pueden administrar campos personalizables.

Para abrir esta pantalla, haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Campos personalizables]**.

* **Edición de un campo** : seleccione el campo y, a continuación, haga clic en  **[!UICONTROL Editar]**.

* **Eliminación de un campo** : seleccione el campo y, a continuación, haga clic en  **[!UICONTROL Eliminar]**.

* **Activar campo** : haga clic en para seleccionar o anular la selección de la  **** opción Activeoption situada junto al nombre de un campo. Si está en una función de administración de la empresa, esta opción no se muestra. Como esta opción está relacionada con MediaPortal, debe seleccionar (activar) Mostrar funciones de MediaPortal en Configuración personal para ver los campos de activación.

## Optimización de archivos {#optimize-files}

A medida que carga archivos en Dynamic Media Classic, el sistema los optimiza para su almacenamiento y publicación. Sin embargo, si se interrumpe el proceso de carga, no se pueden optimizar todas las imágenes. De ser así, aparecerá el mensaje &quot;La imagen no está optimizada todavía&quot;. Si es un administrador podrá optimizar estos archivos.

Dynamic Media Classic busca en los archivos y optimiza solo las imágenes que no se habían optimizado completamente antes.

1. Elija **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** y, a continuación, seleccione **[!UICONTROL Optimizar archivos]**.
1. Introduzca la información del trabajo de optimización y haga clic en **[!UICONTROL Submit]**.

   Si trabaja con más de una empresa, optimice los archivos de cada una de forma independiente.

## Valores preestablecidos de conjuntos de lotes {#batch-set-presets}

Utilice los ajustes preestablecidos de conjuntos de lotes para crear automáticamente conjuntos de imágenes o conjuntos de giros mientras se ejecuta un trabajo para cargar recursos en Dynamic Media Classic.

Los administradores de la empresa definen primero las convenciones de nomenclatura de los recursos que desean agrupar en un conjunto. A continuación, puede crear un ajuste preestablecido de conjunto de lotes para hacer referencia a estas imágenes. Cada valor preestablecido tiene un nombre exclusivo y un conjunto de instrucciones independiente para crear el conjunto con imágenes que coincidan con las convenciones de nombre definidas en el ajuste preestablecido.

Todos los ajustes preestablecidos de conjunto de lotes activos aparecen en el cuadro de diálogo Opciones de trabajo de carga para que pueda especificar qué ajuste preestablecido desea aplicar durante cada sesión de carga. Los administradores de empresa pueden ver todos los valores preestablecidos de conjuntos activos e inactivos. Al cargar archivos, Dynamic Media Classic crea automáticamente un conjunto con todos los archivos que coinciden con la convención de nombres definida en los ajustes preestablecidos activos.

### Nombre por defecto {#default-naming}

El administrador de empresa crea una convención de nombre predeterminada que se utiliza en las fórmulas de los ajustes preestablecidos de conjunto de lotes. La convención de nombres predeterminada seleccionada en la definición del ajuste preestablecido de conjunto de lotes puede ser todo lo que su empresa necesite para generar conjuntos por lotes para todos los sitios web. Se crea un ajuste preestablecido de conjunto de lotes para utilizar la convención de nombre predeterminada que defina. Puede crear tantos ajustes preestablecidos de conjunto de lotes como desee con diferentes convenciones de nombre personalizadas necesarias para un conjunto particular de contenido en casos en los que hay una excepción en el nombre predeterminado definido de la empresa. 

No es necesario configurar una convención de nombres predeterminada para utilizar la funcionalidad preestablecida de conjuntos de lotes. Sin embargo, la práctica recomendada de Adobe recomienda utilizar una convención de nombres predeterminada para definir tantos elementos de la convención de nombres que desee agrupar en un conjunto. Esto ayuda a agilizar la creación de conjuntos de lotes.

1. Haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de conjunto por lotes]** > **[!UICONTROL Nombre por defecto]**.
1. Seleccione **[!UICONTROL Ver formulario]** o **[!UICONTROL Ver código]** para especificar cómo desea ver e introducir información sobre cada elemento.

   Puede seleccionar la casilla de verificación **[!UICONTROL Ver código]** para ver la generación del valor de expresión regular junto con las selecciones de formulario. Puede introducir o alterar estos valores para ayudar a definir los elementos de la convención de nombre, si la vista del formulario le limita por alguna razón. Si los valores no se pueden analizar en la vista de formulario, los campos del formulario se desactivan.

   >[!NOTE]
   >
   >Los campos del formulario desactivados no indican ninguna expresión regular no válida. No hay certeza de que las expresiones regulares sean correctas. Verá los resultados de la expresión regular que está creando para cada elemento después de la línea de resultados. La expresión regular completa está visible en la parte inferior de la página.

1. Expanda los elementos necesarios e introduzca las convenciones de nombres que desee usar.
1. Si es necesario, haga clic en **[!UICONTROL Agregar]** para añadir otra convención de nombre para un elemento. O bien, haga clic en **[!UICONTROL Eliminar]** para eliminar la convención de nombre de un elemento. 
1. Haga clic en **[!UICONTROL Guardar como]** y escriba un nombre para el ajuste preestablecido. También puede hacer clic en **[!UICONTROL Guardar]** si está editando un ajuste preestablecido existente.

También puede usar la visualización de código sin campos de formulario disponibles. En esta vista, se crean las definiciones de convención de nombres utilizando expresiones regulares.

Hay dos elementos disponibles para la definición: la coincidencia y el nombre base. Estos campos le permiten definir todos los elementos de una convención de nombre e identificar la parte de la convención utilizada para dar nombre al conjunto que los contiene. La convención de nombres individual de una empresa podría utilizar una o más líneas de definición para cada uno de estos elementos. Puede utilizar tantas líneas como necesite para su definición única y agruparlas en distintos elementos, como imagen principal, elemento de color, elemento de vista alternativa y elemento de muestra.

### Creación de un ajuste preestablecido de conjunto de lotes {#creating-a-batch-set-preset}

Dynamic Media Classic utiliza ajustes preestablecidos de conjuntos de lotes para organizar los recursos que comparten información o contenido común en conjuntos de imágenes para mostrarlos en los visualizadores. Las fórmulas preestablecidas de conjuntos de lotes se ejecutan automáticamente junto con los trabajos de importación de recursos programados en Dynamic Media Classic.

En la pantalla Ajustes preestablecidos de conjunto por lotes, cree, edite y gestione sus valores preestablecidos de conjunto de lotes. Puede crear tantos valores preestablecidos de conjunto de lotes como necesite para cubrir todos los trabajos de ingesta de recursos requeridos. Existen dos formas de definiciones de ajustes preestablecidos de conjuntos de lotes: una para una convención de nombres predeterminada que haya configurado y otra para las convenciones de nombres personalizadas que cree sobre la marcha.

Se puede utilizar el método de campo de formulario para definir un ajuste preestablecido de conjunto de lotes o el método de código, que permite utilizar expresiones regulares. En Nombre por defecto, puede elegir la vista de código al mismo tiempo que define la vista de formulario y utiliza las expresiones regulares para crear las definiciones. También puede desactivar la vista para utilizar una u otra exclusivamente.

Consulte también [Creación de un ajuste preestablecido de conjunto de lotes para la generación automática de conjuntos de giros 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Creación de un ajuste preestablecido de conjunto de lotes:**

1. Haga clic en **[!UICONTROL Ajustes >]****[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de conjunto por lotes]** > **[!UICONTROL Valor preestablecido de conjunto de lotes]**. **[!UICONTROL Ver formulario]**, definido en la esquina superior derecha de la página Detalles, es la opción predeterminada.
1. En el panel Lista de ajustes preestablecidos, haga clic en **[!UICONTROL Agregar]** para activar los campos de definición en el panel Detalles, en el lado derecho de la página.
1. En el panel Detalles, en el campo Nombre de ajuste preestablecido, escriba un nombre para el ajuste preestablecido.
1. En el menú desplegable Tipo de conjunto de lotes, seleccione un tipo de ajuste preestablecido.

   Para generar un conjunto de giros 2D, seleccione **[!UICONTROL Conjunto de giros con varios ejes]** en la lista desplegable Tipo de conjunto de lotes.

1. Realice una de las acciones siguientes:

   * Si está utilizando una convención de nombres predeterminada que configuró anteriormente en **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de conjuntos de lotes]** > **[!UICONTROL Nombres predeterminados]**, expanda **[!UICONTROL Convenciones de nombres de recursos]** y, a continuación, en la lista desplegable Nombres de archivos, haga clic en **[!UICONTROL Predeterminado]**.
   * Para definir una convención de nombre al configurar el ajuste preestablecido, amplíe **[!UICONTROL Convenciones de nombres de recursos]** y haga clic en **[!UICONTROL Personalizado]** en la lista desplegable Nombres de archivo.

1. En Orden de secuencia, defina el orden de las imágenes después de agrupar el conjunto en Dynamic Media Classic. De forma predeterminada, los recursos se ordenan de forma alfanumérica. Sin embargo, puede utilizar una lista de expresiones regulares separada por comas para definir el orden.
1. Para las convenciones de nombres de conjuntos y opciones de creación, especifique el sufijo o prefijo en el nombre base que definió en Convenciones de nombres de recursos. Defina también dónde se creará el conjunto de imágenes en la estructura de carpetas de Dynamic Media Classic.

   Si define un gran número de conjuntos de imágenes, mantenga estos conjuntos separados de las carpetas que contienen los propios recursos. Algunos clientes crean la carpeta Conjuntos de imágenes y redirigen la aplicación para colocar aquí los conjuntos de lotes generados.

1. Haga clic en **[!UICONTROL Guardar]** en el panel Detalles.

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

Con esta información, la fórmula Tipo de conjunto de lotes se puede crear de la siguiente manera:

![](assets/se_batch_set_recipe.png)

La agrupación de la parte del nombre de recurso compartido del conjunto de giros se agrega al campo Coincidencia (como resaltado). La parte variable del nombre del recurso que contiene la fila y la columna se agrega a los campos Fila y Columna, respectivamente.

Cuando se carga y publica el conjunto de giros, se activa el nombre de la fórmula de conjunto de giros 2D que aparece en **[!UICONTROL Ajustes preestablecidos de conjunto de lotes]** en el cuadro de diálogo Opciones de carga de trabajo.

**Creación de un ajuste preestablecido de conjunto de lotes para la generación automática de conjuntos de giros 2D:**

1. Elija **[!UICONTROL Ajustes >]****[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Valores preestablecidos de conjunto por lotes]** > **[!UICONTROL Valor preestablecido de conjunto de lotes]**. **[!UICONTROL Ver formulario]**, definido en la esquina superior derecha de la página Detalles, es la opción predeterminada.
1. En el panel Lista de ajustes preestablecidos, haga clic en **[!UICONTROL Agregar]** para activar los campos de definición en el panel Detalles del lado derecho de la página.
1. En el panel Detalles, en el campo Nombre de ajuste preestablecido, escriba un nombre para el ajuste preestablecido.
1. En el menú desplegable Tipo de conjunto de lotes, seleccione **[!UICONTROL Conjunto de recursos]**.
1. En la lista desplegable Subtipo, seleccione **[!UICONTROL Conjunto de giros con varios ejes]**.
1. Amplíe **[!UICONTROL Convenciones de nombres de recursos]** y, a continuación, haga clic en **[!UICONTROL Personalizado]** en la lista desplegable Nombre de archivos.
1. Utilice los atributos **[!UICONTROL Coincidencia]** y, opcionalmente, **[!UICONTROL Nombre base]** para establecer una expresión regular para la asignación de nombres a los recursos de imagen que conforman la agrupación.

   Por ejemplo, el literal de expresión regular Match podría tener el siguiente aspecto:

   `(\w+)-\w+-\w+`

1. Amplíe **[!UICONTROL Posición de columna/fila]** y defina el formato de nombre para la posición del recurso de imágenes en la matriz Conjunto de giros 2D.

   Ponga entre corchetes la posición de la fila o la columna en el nombre de archivo.

   Por ejemplo, para la expresión regular de fila, podría tener el siguiente aspecto:

   `\w+-R([0-9]+)-\w+`

   o

   `\w+-(\d+)-\w+`

   Para la expresión regular de su columna, podría tener el siguiente aspecto:

   `\w+-\w+-C([0-9]+)`

   o

   `\w+-\w+-C(\d+)`

   Recuerde que estas expresiones son solo ejemplos. Puede crear su expresión regular como prefiera según sus necesidades.

   >[!NOTE]
   >
   >Si la combinación de expresiones regulares de fila y columna no puede determinar la posición del recurso dentro de la matriz de conjuntos de giros multidimensionales, ese recurso no se agrega al conjunto y se registra un error.

1. Para las convenciones de nombres de conjuntos y opciones de creación, especifique el sufijo o prefijo en el nombre base que definió en Convenciones de nombres de recursos. Defina también dónde se creará el conjunto de imágenes en la estructura de carpetas de Dynamic Media Classic.

   Si define un gran número de conjuntos de imágenes, mantenga estos conjuntos separados de las carpetas que contienen los propios recursos. Algunos clientes crean la carpeta Conjuntos de imágenes y redirigen la aplicación para colocar aquí los conjuntos de lotes generados.

1. Haga clic en **[!UICONTROL Guardar]** en el panel Detalles.
1. Cargue y publique el conjunto de giros de la forma habitual, asegurándose de activar el nombre del conjunto de giros 2D en el cuadro de diálogo Opciones de carga de trabajo, en Valores preestablecidos de conjunto por lotes.

>[!MORELIKETHIS]
>
>* [Previsualización de un recurso](previewing-asset.md#previewing_an_asset)
* [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets)
* [Visualización, adición y exportación de metadatos](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Comprobación de archivos de trabajo](checking-job-files.md#checking_job_files)

