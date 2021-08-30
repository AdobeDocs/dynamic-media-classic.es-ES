---
title: Ajustes personales
description: Todos los usuarios pueden cambiar la configuración en la pantalla Ajustes personales de Adobe Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Ajustes personales {#personal-setup}

Todos los usuarios pueden cambiar la configuración de la página Ajustes personales. Para abrir la pantalla Ajustes personales, vaya a **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes personales]**.

>[!NOTE]
>
>La pantalla Ajustes personales muestra la función de usuario que tiene en Adobe Dynamic Media Classic: Administrador de la empresa, Administrador o Usuario.

La configuración de Ajustes personales determina el comportamiento del panel Examinar, la manera en que recibe correo electrónico y la configuración de la contraseña. Recuerde seleccionar **[!UICONTROL Guardar]** después de cambiar esta configuración.

## Información de mi cuenta

Identifica el nombre de la cuenta, el nombre, el nombre de usuario (dirección de correo electrónico) y la función de usuario asignada.

## Ordenador

* **Borrar caché de imágenes** : quita de su equipo todos los archivos de imagen en caché de Dynamic Media de Adobe.
* **Borrar caché de recursos** : Quita de su equipo todos los archivos de recursos almacenados en caché de Dynamic Media de Adobe.

Además de borrar la imagen y la caché de recursos mediante la aplicación de escritorio, puede borrar manualmente la caché directamente desde el sistema de archivos. En función del sistema operativo, vaya a lo siguiente:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Para instalar la extensión del Creative Suite Dynamic Media de Adobe:**

1. En Adobe Dynamic Media Classic, en la barra de herramientas, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**, en Extensión de Creative Suite, seleccione **[!UICONTROL Descargar ahora]** para descargar el archivo `s7csxs.zxp`.
1. Seleccione los vínculos **[!UICONTROL Installation]** y **[!UICONTROL System Requirements]** para obtener información adicional sobre la extensión.

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
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Explorador

* **[!UICONTROL Tamaño de las miniaturas]** : determina el tamaño predeterminado de las imágenes en miniatura en la vista de cuadrícula en el panel Examinar.
* **[!UICONTROL Vista predeterminada de la biblioteca de recursos]** : determina si los recursos de la biblioteca de recursos para conjuntos de versiones aparecen como miniaturas o por nombre. Si trabaja con numerosos recursos de la biblioteca de recursos, puede visualizarlos por nombre. Por ejemplo, si va a crear un catálogo electrónico con muchos archivos PDF, puede ver los recursos por nombre para que la lista sea más pequeña.
* **[!UICONTROL Orden de exploración predeterminado]** : determina el orden en que aparecen los recursos de forma predeterminada en el panel Examinar. Elija un criterio de orden en el menú y seleccione si desea un orden ascendente o descendente.
* **[!UICONTROL Ubicación de exploración predeterminada]** : le permite establecer la ubicación de exploración en la ubicación predeterminada, en la última carpeta explorada o en una ubicación específica a la que vaya e identifique. También puede definir que los archivos y las carpetas aparezcan por orden ascendente o descendente en la ubicación de exploración.
* **[!UICONTROL Vista de exploración predeterminada]** : determina si la vista de cuadrícula o la vista de lista es la vista predeterminada que se ve al abrir el panel Examinar por primera vez.
* **[!UICONTROL Pantalla de bienvenida]** : determina si se ve alguna pantalla de inicio, incluida la pantalla de bienvenida.
* **[!UICONTROL Mostrar información del objeto]** : determina si la información del objeto aparece al mover el puntero sobre botones, menús y vínculos de navegación. Las informaciones de objeto describen los elementos de la interfaz de usuario en pantalla.
* **[!UICONTROL Fondo de tablero de ajedrez]** : muestra una capa de tablero de ajedrez detrás de las imágenes, lo que permite ver fácilmente las áreas transparentes de una imagen que tiene un canal alfa.
* **[!UICONTROL Mostrar tamaño de archivo]** : muestra el tamaño de archivo de un recurso cuando está explorando.
* **[!UICONTROL Incluir UDF en la búsqueda]** : para mejorar el rendimiento del sistema en la mayoría de las búsquedas de metadatos que ejecute, anule la selección (predeterminado).

   Si necesita incluir los campos personalizables en la mayoría de sus búsquedas de metadatos, puede seleccionar esta opción para activarla. Si lo prefiere, puede utilizar la búsqueda avanzada para permitir una búsqueda más rápida y directa sin incluir todos los campos personalizables.

   Consulte [Búsqueda avanzada](searching-assets.md#conducting_an_advanced_search).

   Consulte también [Campos personalizables](application-setup.md#user_defined_fields).

* **[!UICONTROL Tipo de búsqueda básica]** : puede seleccionar entre dos opciones:  **** Contiene busca en la cadena completa el valor especificado;  **** StartsWithSearch desde el principio de la cadena y devuelve los resultados más rápido que  **[!UICONTROL Contains]**. Cualquiera de las opciones anula el valor predeterminado que el administrador establece en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración general de la aplicación]**.
* **[!UICONTROL Mostrar comentarios del comando]** : seleccione esta opción para activar la visualización de las solicitudes de comando al servidor; anule la selección para desactivarla.
* **[!UICONTROL Mostrar cuadro de diálogo durante la exportación]** : seleccione esta opción para mostrar un cuadro de diálogo emergente durante una exportación. Si anula la selección (desactiva) de esta opción, aún puede ir a la página Trabajos para recuperar los resultados de la exportación.

## Correo electrónico

* **[!UICONTROL Opciones de correo electrónico]** : elija cómo desea que Adobe Dynamic Media Classic le informe por correo electrónico cuando se completen los trabajos de carga y publicación. Puede recibir notificaciones sobre la finalización de un trabajo solo cuando aparezcan advertencias o se produzcan errores.
* **[!UICONTROL Ámbito de correo electrónico]** : determina si recibe todo el correo electrónico del trabajo de su empresa o solo el correo electrónico sobre los trabajos de carga y publicación que inicie.
* **[!UICONTROL Tipos de correo electrónico]** : determina si se le informa cuando se completan los trabajos de carga y publicación.

## Idioma

* **[!UICONTROL Idioma preferido]** : determina el idioma que desea utilizar para la interfaz.

## Contraseña

* **[!UICONTROL Contraseña actual]** : introduzca la contraseña de su contraseña actual.
* **[!UICONTROL Nueva contraseña]** : introduzca una contraseña nueva y válida. La contraseña debe cumplir los siguientes requisitos:
   * Tener entre 8 y 25 caracteres.
   * Incluir al menos una letra minúscula.
   * Incluir al menos una letra en mayúsculas.
   * Incluir al menos un número.
   * Incluir al menos uno de los siguientes caracteres especiales: `# $ & - _ : { }`
* **[!UICONTROL Volver a escribir la contraseña]** : vuelva a introducir la nueva contraseña para confirmar que la ha introducido correctamente.
* **[!UICONTROL Caducidad de la contraseña]** : determina si la contraseña caduca después de 72 días como medida de seguridad. Si selecciona Sí, se le pedirá que cree una contraseña dentro de 72 días.
