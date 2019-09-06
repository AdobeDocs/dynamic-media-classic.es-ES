---
title: Ajustes personales
seo-title: Ajustes personales
description: nulo
seo-description: Todos los usuarios pueden cambiar la configuración de la pantalla Ajustes personales de Dynamic Media Classic.
uuid: 29 cb 825 a-f 158-4 a 1 e -9 d 5 f -7636 ee 411 b 6 e
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/setup
discoiquuid: 6314 e 7 b 7-5 bde -4 fe 2-8674-e 4 fc 525 d 4 d 1 c
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Ajustes personales {#personal-setup}

Todos los usuarios pueden cambiar la configuración de la página Ajustes personales. Para abrir la pantalla Ajustes personales, haga clic en Ajustes &gt; Ajustes personales.

>[!NOTE]
>
>En la pantalla Ajustes personales se muestra su función de usuario dentro de Scene7 Publishing System: administrador de empresa, administrador o usuario.

La configuración de Ajustes personales determina el comportamiento predeterminado del panel Examinar, la manera en que se recibe correo electrónico y la configuración de la contraseña. No olvide hacer clic en Guardar después de cambiar la configuración.

## Información de mi cuenta

Identifica el nombre de la cuenta, el nombre, el nombre de usuario (dirección de correo electrónico) y la función de usuario asignada.

### Versión de escritorio

Haga clic en Instalar ahora para instalar la versión de escritorio de Scene7 Publishing System en su unidad de disco duro local. También puede hacer clic en Volver a instalar ahora para instalar la versión de escritorio de nuevo.

### Plugin de Illustrator para impresión virtual

En equipos con Windows 7 o 8, deberá disponer de privilegios de administrador e iniciar sesión como tal en Windows para poder instalar y actualizar el plugin de Illustrator para impresión virtual. Después de instalar el plugin, estará disponible en Adobe Illustrator.

El plugin es compatible con las siguientes versiones de Adobe Illustrator:

* Adobe Illustrator 18 en Adobe Creative Cloud 2014.
* Adobe Illustrator 17 en Adobe Creative Cloud.
* Adobe Illustrator 16 en Adobe Creative Suite 6.

Entre las plataformas compatibles con Adobe Illustrator se incluyen:

* Apple Mac OS X 10.7 o superior.
* Windows 8 de 32 bits y 64 bits.
* Windows 7 de 32 bits y 64 bits.
* Windows XP de 32 bits y 64 bits (solo para Adobe Illustrator 16 en Adobe Creative Suite 6).

Consulte también [Publicación de plantillas](quick-start-template-publishing.md).

## Para instalar el plugin en la unidad de disco duro local

1. En la página Ajustes personales de Scene7 Publishing System, debajo del plugin de Illustrator para impresión virtual, haga clic en **Descargar ahora** para descargar el archivo **Plugin de Illustrator para impresión virtual**.
1. Descomprima el archivo ZIP en una carpeta temporal.

   Se incluye un archivo Léame en la raíz del archivo descomprimido que le proporcionará información adicional sobre el plugin.

1. Según el sistema operativo instalado, realice una de las acciones siguientes:

### Windows

| Si dispone de | Haga lo siguiente |
|--- |--- |
| Adobe Illustrator 18 en Adobe Creative Cloud 2014 | <ul><li>Desde la raíz de la carpeta sin comprimir, haga clic en CC-2014.</li><li>Según la versión de bits Adobe Illustrator que esté utilizando, haga clic en win32 o win64.</li><li>Haga clic en Bibliotecas &gt; flame y copie `aflame.dll` en la carpeta ejecutable de Adobe Illustrator. Por ejemplo, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Nota**: Esta ruta de ejemplo es para la ubicación de 64 bits; La ubicación de 32 bits puede encontrarse en Archivos de programa (x 86). <br/><ul><li>Vuelva a la misma carpeta Bibliotecas, haga clic en Flamingo y copie `aflamingo.dll` en la misma carpeta ejecutable de Adobe Illustrator que haya utilizado en el paso anterior. </li><li>Vuelva a la carpeta win32 o win64 seleccionada en el paso 2 y copie `AdobeS7FXGFileFormat.aip` en la carpeta de plugins de Adobe Illustrator. Por ejemplo, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Nota**: Esta ruta de ejemplo es para la ubicación de 64 bits; La ubicación de 32 bits puede encontrarse en Archivos de programa (x 86). |
| Adobe Illustrator 17 en Adobe Creative Cloud | <ul><li>Desde la raíz de la carpeta sin comprimir, haga clic en CC. </li><li>Según la versión de bits Adobe Illustrator que esté utilizando, haga clic en win32 o win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. Por ejemplo, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Nota**: Esta ruta de ejemplo es para la ubicación de 64 bits; La ubicación de 32 bits puede encontrarse en Archivos de programa (x 86). |
| Adobe Illustrator 16 en Adobe Creative Suite 6 | <ul><li>Desde la raíz de la carpeta sin comprimir, haga clic en 6.0. </li><li>Según la versión de bits Adobe Illustrator que esté utilizando, haga clic en win32 o win64. </li><li>Copie·AdobeS7FXGFileFormat.aip en la carpeta de plugins de Adobe Illustrator. Por ejemplo, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Nota**: Esta ruta de ejemplo es para la ubicación de 64 bits; La ubicación de 32 bits puede encontrarse en Archivos de programa (x 86). |

### Mac

| Si dispone de | Haga lo siguiente |
|--- |--- |
| Adobe Illustrator 18 en Adobe Creative Cloud 2014 | <ul><li>Desde la raíz de la carpeta sin comprimir, haga clic en CC-2014 &gt; mac64.</li><li>Haga clic en Bibliotecas &gt; flame y copie la carpeta `aflame.framework` en la carpeta de contenido del paquete de Adobe Illustrator. Por ejemplo, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Para abrir la carpeta de contenido del paquete de Adobe Illustrator, haga clic con el botón derecho en el icono de Adobe illustrator CC 2014 y haga clic en Mostrar contenido del paquete en menú contextual).</li><li>Vuelva a la misma carpeta Bibliotecas, haga clic en `flamingo` y copie la carpeta `aflamingo.framework` en la misma carpeta de contenido del paquete de Adobe Illustrator que haya utilizado en el paso anterior.</li><li>Vuelva a la carpeta mac64 seleccionada en el paso 1 y copie la carpeta `AdobeS7FXGFileFormat.aip` en la carpeta de plugins de Adobe Illustrator. Por ejemplo, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 en Adobe Creative Cloud | <ul><li>Desde la raíz de la carpeta sin comprimir, haga clic en CC &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Por ejemplo, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 en Adobe Creative Suite 6 | <ul><li>Desde la raíz de la carpeta sin comprimir, haga clic en 6.0 &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Por ejemplo, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

El plugin está ahora disponible para utilizarlo en Adobe Illustrator.

### Explorador

* **Tamaño de miniatura**
   * Determina el tamaño predeterminado de las imágenes en miniatura en la vista de cuadrícula del panel Examinar.
* **Vista de biblioteca de recursos predeterminada**
   * Determina si los recursos de la biblioteca de recursos para crear conjuntos aparecen por nombre o como miniaturas. Si trabaja con numerosos recursos de la biblioteca de recursos, puede visualizarlos por nombre. Por ejemplo, si va a crear un catálogo electrónico con muchos archivos PDF, puede ver los recursos por nombre para que la lista sea más pequeña.
* **Orden de exploración predeterminado**
   * Determina el orden predeterminado en que los recursos aparecen en el panel Examinar. Elija un criterio de orden en el menú y seleccione si desea un orden ascendente o descendente.
* **Ubicación de exploración predeterminada**
   * Permite definir la ubicación de exploración en la ubicación predeterminada, la última carpeta explorada o la ubicación concreta que busque e identifique. También puede definir que los archivos y las carpetas aparezcan por orden ascendente o descendente en la ubicación de exploración.
* **Vista de exploración predeterminada**
   * Determina la vista predeterminada al abrir el panel Examinar por primera vez: vista de cuadrícula o de lista.
* **Presentación de pantalla de bienvenida**
   * Determina si se mostrarán las pantallas de bienvenida.
* **Mostrar información de objetos**
   * Determina si se mostrará la información sobre herramientas al mover el puntero sobre botones, menús y vínculos de navegación. La información de objeto describe los elementos en pantalla.
* **Fondo de tablero de ajedrez**
   * Muestra una capa de tablero de ajedrez detrás de las imágenes, de modo que resulta más fácil distinguir las áreas transparentes de imágenes con un canal alfa.
* **Mostrar tamaño del archivo**
   * Muestra el tamaño de archivo del recurso mientras explora.
* **Confirmar al salir de SPS**
   * Muestra una ventana de confirmación antes de salir de Scene7 Publishing System.
* **Incluir UDF en la búsqueda**
   * Se anula la selección de forma predeterminada para mejorar el rendimiento del sistema para la mayoría de las búsquedas de metadatos.

Si necesita incluir los campos personalizables en la mayoría de sus búsquedas de metadatos, puede seleccionar esta opción para activarla. Si lo prefiere, puede utilizar la búsqueda avanzada para permitir una búsqueda más rápida y directa sin incluir todos los campos personalizables.

Consulte [Búsqueda avanzada](searching-assets.md#conducting_an_advanced_search).

Consulte también [Campos personalizables](application-setup.md#user_defined_fields).

* **Tipo de búsqueda básica**
   * Seleccione un tipo de búsqueda predeterminado, Contiene o Empieza por.
* **Mostrar funciones de Media Portal**
   * Seleccione esta opción para acceder a las funciones de Media Portal, como puede ser Carro Multimedia.
* **Mostrar comentarios de comando**
   * Muestra las solicitudes de comando al servidor.
* **Mostrar cuadro de diálogo al exportar**
   * Muestra un cuadro de diálogo cuando se realiza una exportación. Aunque anule la selección de esta opción, puede recuperar los resultados de la exportación desde a la página Trabajos.

## Correo electrónico

* **Opciones de correo electrónico**
   * Elija cómo desea que Dynamic Media Classic le informe por correo electrónico cuando se completen los trabajos de carga y publicación. Puede recibir notificaciones sobre la finalización de un trabajo solo cuando aparezcan advertencias o se produzcan errores.
* **Ámbito de correo electrónico**
   * Determina si recibirá correos electrónicos para todos los trabajos de su empresa o si solo para los trabajos de carga y publicación que usted haya iniciado.
* **Tipos de correos electrónicos**
   * Determina si recibe una notificación al completarse los trabajos de carga y publicación.
* **Idioma**
* **Idioma preferido**
   * Determina el idioma de la interfaz.
* **Contraseña**
* **Nueva contraseña**
   * Introduzca una contraseña nueva válida. Su contraseña debe cumplir los requisitos siguientes:
      * Tener entre 8 y 25 caracteres de longitud
      * Contener por lo menos una letra minúscula
      * Contener por lo menos una letra mayúscula
      * Contener al menos un número
      * Contener al menos uno de los siguientes caracteres especiales: # $ &amp;-_: {}}

* **Vuelva a escribir la contraseña**
   * Vuelva a introducir la nueva contraseña para asegurarse de que la ha introducido correctamente.
* **Caducidad de contraseña**
   * Determina si la contraseña caducará a los 72 días, como medida de seguridad. Si selecciona Sí, se le pedirá que cree una nueva contraseña dentro de 72 días.
