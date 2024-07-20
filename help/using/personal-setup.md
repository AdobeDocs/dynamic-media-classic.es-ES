---
title: Ajustes personales
description: Todos los usuarios pueden cambiar la configuración en la pantalla Configuración personal de Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 19%

---

# Ajustes personales {#personal-setup}

Todos los usuarios pueden cambiar la configuración de la página Ajustes personales. Para abrir la pantalla de configuración personal, ve a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**.

>[!NOTE]
>
>La pantalla Configuración personal indica qué función de usuario tiene en Adobe Dynamic Media Classic: Administrador de la empresa, Administrador o Usuario.

La configuración de Configuración personal controla el comportamiento predeterminado del panel Examinar, cómo recibe el correo electrónico y la configuración de la contraseña. Recuerde seleccionar **[!UICONTROL Guardar]** después de cambiar esta configuración.

## Información de mi cuenta

Identifica el nombre de la cuenta, el nombre, el nombre de usuario (dirección de correo electrónico) y la función de usuario asignada.

## Ordenador

* **Borrar caché de imágenes**: Elimina todos los archivos de imagen en caché de Dynamic Media de Adobe del equipo.
* **Borrar caché de recursos**: Elimina todos los archivos de recursos de la memoria caché de Dynamic Media en Adobe del equipo.

Además de borrar la caché de imágenes y recursos mediante la aplicación de escritorio, puede borrar manualmente la caché directamente desde el sistema de archivos. En función del sistema operativo, vaya a lo siguiente:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Para instalar la extensión de Creative Suite de Dynamic Media de Adobe:**

1. En Adobe Dynamic Media Classic, en la barra de herramientas, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**, en Extensión de Creative Suite, seleccione **[!UICONTROL Descargar ahora]** para descargar el archivo `s7csxs.zxp`.
1. Seleccione los vínculos **[!UICONTROL Instalación]** y **[!UICONTROL Requisitos del sistema]** para obtener información adicional acerca de la extensión.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Explorador

* **[!UICONTROL Tamaño de miniatura]**: Determina el tamaño predeterminado de las imágenes en miniatura en la Vista de cuadrícula del panel Examinar.
* **[!UICONTROL Vista predeterminada de la biblioteca de recursos]**: Determina si los recursos de la biblioteca de recursos de los conjuntos de compilación aparecen como miniaturas o por nombre. Si trabaja con numerosos recursos de la biblioteca de recursos, puede visualizarlos por nombre. Por ejemplo, si va a crear un catálogo electrónico con muchos archivos PDF, puede ver los recursos por nombre para que la lista sea más pequeña.
* **[!UICONTROL Orden de exploración predeterminado]**: Determina el orden en que aparecen los recursos de forma predeterminada en el panel Examinar. Elija un criterio de orden en el menú y seleccione si desea un orden ascendente o descendente.
* **[!UICONTROL Ubicación de exploración predeterminada]**: permite establecer la ubicación de exploración en la ubicación predeterminada, en la última carpeta examinada o en una ubicación específica a la que se desplaza y se identifica. También puede definir que los archivos y las carpetas aparezcan por orden ascendente o descendente en la ubicación de exploración.
* **[!UICONTROL Vista de exploración predeterminada]**: Determina si la vista de cuadrícula o la vista de lista es la vista predeterminada que se ve la primera vez que se abre el panel Examinar.
* **[!UICONTROL Visualización de pantalla de bienvenida]**: Determina si ve alguna pantalla de bienvenida, incluida la pantalla de bienvenida.
* **[!UICONTROL Mostrar información sobre herramientas]**: Determina si aparece información sobre herramientas al mover el puntero sobre botones, menús y vínculos de exploración. La información sobre herramientas describe los elementos de la interfaz de usuario en pantalla.
* **[!UICONTROL Fondo del tablero de ajedrez]**: muestra una capa de tablero de ajedrez detrás de las imágenes, lo que permite ver fácilmente las áreas transparentes de una imagen que tiene un canal alfa.
* **[!UICONTROL Mostrar tamaño de archivo]**: muestra el tamaño de archivo de un recurso al examinar.
* **[!UICONTROL Incluir UDF en la búsqueda]**: Para mejorar el rendimiento del sistema para la mayoría de las búsquedas de metadatos que ejecuta, anule la selección (predeterminado).

  Si necesita incluir los campos personalizables en la mayoría de sus búsquedas de metadatos, puede seleccionar esta opción para activarla. Como alternativa, utilice Búsqueda avanzada para ofrecerle una experiencia de búsqueda más dirigida y rápida que mediante la inclusión de campos definidos por el usuario.

  Consulte [Búsqueda avanzada](searching-assets.md#conducting_an_advanced_search).

  Consulte también [Campos personalizables](application-setup.md#user_defined_fields).

* **[!UICONTROL Tipo de búsqueda básica]**: puede seleccionar entre dos opciones: **[!UICONTROL Contiene]** busca en la cadena completa el valor especificado; **[!UICONTROL Comienza con]** busca desde el principio de la cadena y devuelve resultados más rápidos que **[!UICONTROL Contiene]**. Cualquiera de las opciones anula el valor predeterminado establecido por el administrador en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración general de la aplicación]**.
* **[!UICONTROL Mostrar comentarios de comandos]**: seleccione esta opción para activar la visualización de las solicitudes de comandos al servidor; anule la selección de esta opción para desactivarla.
* **[!UICONTROL Mostrar cuadro de diálogo durante la exportación]**: seleccione esta opción para mostrar un cuadro de diálogo emergente durante la exportación. Si anula la selección de esta opción (o la desactiva), sigue pudiendo ir a la página Trabajos para recuperar los resultados de la exportación.

## Correo electrónico

* **[!UICONTROL Opciones de correo electrónico]**: elija cómo desea que Adobe Dynamic Media Classic le informe por correo electrónico cuando se completen los trabajos de carga y publicación. Puede recibir notificaciones sobre la finalización de un trabajo solo cuando aparezcan advertencias o se produzcan errores.
* **[!UICONTROL Ámbito del correo electrónico]**: Determina si recibe todo el correo electrónico del trabajo de su empresa o sólo el correo electrónico sobre los trabajos de carga y publicación que ha iniciado.
* **[!UICONTROL Tipos de correo electrónico]**: Determina si se le informará cuando se completen los trabajos de carga y publicación.

## Idioma

* **[!UICONTROL Idioma preferido]**: Determina el idioma que desea utilizar para la interfaz.

## Contraseña

* **[!UICONTROL Contraseña actual]**: Escriba la contraseña para la contraseña actual.
* **[!UICONTROL Nueva contraseña]**: escriba una contraseña nueva y válida. La contraseña debe cumplir los siguientes requisitos:
   * Debe tener entre 8 y 25 caracteres.
   * Incluir al menos una letra minúscula
   * Incluir al menos una letra mayúscula
   * Incluir al menos un número
   * Incluir al menos uno de los siguientes caracteres especiales: `# $ &: _ : { }`
* **[!UICONTROL Vuelva a escribir la contraseña]**: Vuelva a escribir la nueva contraseña para confirmar que la ha escrito correctamente.
* **[!UICONTROL Caducidad de contraseña]**: Determina si la contraseña caduca pasados 72 días como medida de seguridad. Si selecciona Sí, se le pedirá que cree una contraseña después de 72 días.
