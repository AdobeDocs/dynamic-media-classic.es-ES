---
title: Adobe Dynamic Media Classic Desktop
description: Obtenga más información sobre la aplicación de escritorio de Adobe Dynamic Media Classic que ya está disponible.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 0%

---

# Ya disponible: aplicación de escritorio de Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Los usuarios de Adobe Dynamic Media Classic ahora tienen acceso a una nueva experiencia de aplicación de escritorio que ya no depende de la tecnología Adobe Flash en el navegador.

Esta nueva aplicación ya está disponible para Windows® y macOS.

>[!IMPORTANT]
>
>Adobe recomienda instalar la nueva aplicación de escritorio de Adobe Dynamic Media Classic antes del 1 de octubre de 2020. Al hacerlo, se garantiza una transición sin problemas antes de que Adobe Flash Player quede obsoleto el 31 de diciembre de 2020. Después de esta fecha, no podrá iniciar sesión en la versión del explorador de la interfaz de usuario de Adobe Dynamic Media Classic, etiquetada como Adobe Dynamic Media Classic en el producto.

Ver las preguntas frecuentes para el [nuevo inicio de sesión de Adobe Dynamic Media Classic ya disponible.](/help/using/new-ui-2020.md)

## Requisitos del sistema para la aplicación de escritorio de Adobe Dynamic Media Classic {#system-requirements-dmc-app}

La aplicación de escritorio de Adobe Dynamic Media Classic es compatible con los siguientes sistemas operativos:

* macOS 10.10 o posterior.
* Windows® 7 o posterior.

Consulte los requisitos completos del sistema en [Requisitos del sistema para la aplicación de escritorio de Adobe Dynamic Media Classic](/help/using/system-requirements.md).

No se ha generado una notificación de actualización en la aplicación de escritorio de Adobe Dynamic Media Classic para *versiones menores*. Los clientes que se benefician de las correcciones en una versión menor pueden actualizar.

## Solo se ha corregido en la última versión (20.22.2) de macOS {#release-feb2022}

* macOS Monterey: La página de carga de archivos se ha congelado en cargas posteriores. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Correcciones en la última versión (20.22.1) {#release-jan2022}

* Al editar una imagen, los botones **[!UICONTROL Guardar]** no funcionaban.
* En los editores de conjuntos, los botones **[!UICONTROL Cerrar]**, **[!UICONTROL Guardar]** y **[!UICONTROL Guardar como]** se desactivan después de desplazarse por los recursos en el panel **[!UICONTROL Agregar Assets]**.
* El botón **[!UICONTROL Reproducir]** de la vista de detalles de vídeo no funcionó.
* No se pudo escribir `d` y `e` en los campos **[!UICONTROL Nombre de usuario]** y **[!UICONTROL Contraseña]** al ejecutar macOS Monterey.
* Se han movido las API de análisis restantes a la versión 2.0.

## Correcciones en la versión 20.21.3 {#release-sept2021}

* Miniaturas rotas para recursos vistos después de un período de inactividad en la aplicación de escritorio.
* La aplicación de escritorio deja de responder, generalmente después de establecer operaciones.
* Modo de bloqueo y ofuscación de solicitud habilitado automáticamente en **[!UICONTROL Probar el servicio de imágenes]**.

  Consulte [El servicio de pruebas seguras](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Se ha actualizado el mecanismo de autenticación con Adobe Analytics. Es relevante para nuevas integraciones o si algunas variables de Analytics deben actualizarse desde la aplicación de escritorio de Dynamic Media Classic.

  Consulte [Iniciar sesión en Adobe Analytics](/help/using/log-analytics.md) para ver los pasos actualizados.

## Correcciones en la versión 20.21.2 {#minor-release}

* Limitación conocida en 20.21.1: la lista desplegable **[!UICONTROL Servidor]** de la pantalla de inicio de sesión estaba vacía.
* En **[!UICONTROL Opciones de trabajo de carga]**, el valor predeterminado del nombre de capa en **[!UICONTROL Opciones de Photoshop]** es ahora **[!UICONTROL Photoshop y Nombre de capa]**. Las capas del archivo PSD se cargan como imágenes independientes.
   * El valor predeterminado anterior de **[!UICONTROL Nombre de capa]**, asignaba a las imágenes el nombre de su nombre o número de capa en el archivo PSD. El número de capa se utilizaba si los nombres de capa del fichero PSD eran nombres de capa de Photoshop por defecto.
   * El nuevo valor predeterminado de **[!UICONTROL Photoshop y Nombre de capa]**, asigna un nombre a las imágenes después del archivo PSD seguido del nombre o número de capa. El número de capa se utiliza si los nombres de capa del fichero PSD son nombres de capa Photoshop por defecto.
   * Dado que las imágenes de capa en Adobe Dynamic Media Classic ahora tienen nombres únicos, no se van a realizar actualizaciones en PSD o Templates existentes (qué nombres de capa compartidos tienen los archivos PSD originales).
* Miniaturas de recursos rotas.

## Correcciones en la versión 20.21.1 {#latest-fixes-desktop-app}

* Problemas de inicio de sesión debido al tiempo de espera, lo que da como resultado el siguiente mensaje: *Este usuario puede asignarse al grupo o grupos sin permiso. Póngase en contacto con el administrador.*
* Los ajustes preestablecidos del visor se duplican con cada intento de contraseña incorrecto.
* La aplicación de escritorio deja de responder debido a muchos recursos de la carpeta raíz. (Se corrigió en Windows®; funciona como se desea en macOS).

## Correcciones en la versión 20.20.2 {#previous-version-fixes-desktop-app}

* No hay limitación en el número de archivos que se pueden cargar a través de la interfaz de usuario de la aplicación de escritorio tanto para macOS como para Windows®.
* No es necesario cerrar la sesión de la aplicación de escritorio para cambiar de empresa.
* La operación Ctrl+V para pegar ahora funciona en Windows®.
* En el futuro, cuando se publique una nueva versión de la aplicación de escritorio, se notificará a los usuarios dentro de la propia aplicación de escritorio.

## Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en macOS o Windows® {#installation-dmc-app}

Consulte también:

* [Descargue e instale de forma silenciosa la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac](#install-silent-mac-dmc-app)
* [Descargue e instale de forma silenciosa la última aplicación de escritorio de Adobe Dynamic Media Classic en Windows](#install-silent-windows-dmc-app)

1. Desinstale las versiones anteriores de la aplicación de escritorio de Adobe Dynamic Media Classic en el sistema.

1. Descargue el último instalador para la aplicación de escritorio de Adobe Dynamic Media Classic.

   * La versión más reciente está disponible en los siguientes enlaces:

      * [macOS (.DMG): Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE): Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * La versión anterior está disponible en los siguientes enlaces:

      * [macOS (.DMG): Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE): Descargar](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Realice una de las siguientes acciones en función del programa de instalación que descargó.

   * **macOS** - En el cuadro de diálogo **[!UICONTROL Arrastrar y soltar para instalar]**, arrastre **[!UICONTROL Adobe Dynamic Media Classic]** y suéltelo en **[!UICONTROL Aplicaciones]**.

     ![Arrastrar y soltar la instalación en macOS](/help/using/assets/dragondrop-install1.png)

   * En la carpeta **[!UICONTROL Aplicaciones]**, pulse el icono Adobe Dynamic Media Classic.
   * En el cuadro de diálogo, pulse **[!UICONTROL Abrir]** para abrir la aplicación de escritorio de Adobe Dynamic Media Classic.

     ![Abrir aplicación descargada](/help/using/assets/open-dmclassicapp1.png)

   * **Windows**: ejecute el binario del instalador y siga las instrucciones que aparecen en la pantalla para instalar la aplicación de escritorio.

1. Al abrir la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Adobe Dynamic Media Classic inició sesión](/help/using/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para que **[!UICONTROL Server]** lo use, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (Norteamérica) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción de Asia-Pacífico (Asia-Pacífico) | https://s7sps5.scene7.com/ |

1. Después de iniciar sesión, observe la experiencia familiar de la interfaz de usuario del explorador. Puede continuar con su actividad diaria de Adobe Dynamic Media Classic como de costumbre en la aplicación de escritorio.

## Descargue e *instale de forma silenciosa* la aplicación de escritorio más reciente de Adobe Dynamic Media Classic en macOS {#install-silent-mac-dmc-app}

Consulte también:

* [Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac o Windows](#installation-dmc-app)
* [Descargue e instale de forma silenciosa la última aplicación de escritorio de Adobe Dynamic Media Classic en Windows](#install-silent-windows-dmc-app)

Para descargar y *instalar en modo silencioso* la versión más reciente de la aplicación de escritorio de Adobe Dynamic Media Classic en macOS:

1. Desinstale las versiones anteriores de la aplicación de escritorio de Adobe Dynamic Media Classic en el sistema.

1. Descargue el último instalador para la aplicación de escritorio de Adobe Dynamic Media Classic para macOS.

   * [macOS (.DMG): Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Monte la imagen de disco descargada (.DMG) en una ubicación de punto de montaje con el siguiente comando:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Copie el archivo .APP en **[!UICONTROL Aplicaciones]** mediante el siguiente comando:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. Al abrir la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Adobe Dynamic Media Classic inició sesión](/help/using/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para que **[!UICONTROL Server]** lo use, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (Norteamérica) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción de Asia-Pacífico (Asia-Pacífico) | https://s7sps5.scene7.com/ |

## Descargue e *instale de forma silenciosa* la aplicación de escritorio más reciente de Adobe Dynamic Media Classic en Windows® {#install-silent-windows-dmc-app}

El comando que utiliza es para una instalación silenciosa MSI básica. Sin embargo, el instalador de la aplicación de escritorio de Adobe Dynamic Media Classic es un instalador MSI de InstallScript creado con InstallShield. Cuando se ejecuta el instalador en modo de registro, cualquier interacción del usuario se registra en un archivo de respuesta. Este archivo de respuesta se utiliza para una instalación silenciosa como se describe en [Ejecución de instalaciones en modo silencioso](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Consulte también:

* [Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac o Windows](#installation-dmc-app)

* [Descargue e instale de forma silenciosa la última aplicación de escritorio de Adobe Dynamic Media Classic en macOS](#install-silent-mac-dmc-app)

Para descargar y *instalar en modo silencioso* la versión más reciente de la aplicación de escritorio de Adobe Dynamic Media Classic en Windows®:

1. Desinstale las versiones anteriores de la aplicación de escritorio de Adobe Dynamic Media Classic en el sistema.

1. Descargue el último instalador para la aplicación de escritorio de Adobe Dynamic Media Classic.

   * [Windows® (.EXE): Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Ejecute el instalador en modo de registro con el siguiente comando:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. En la ventana del instalador de GUI, siga los pasos para instalar de modo que las interacciones/entradas, como la ubicación de instalación, se registren en el archivo `Setup.iss`.

1. Copie el archivo `Setup.iss` creado y `adobe-dynamic-media-classic-20.22.1.exe` a otro equipo.

1. Ejecute el siguiente comando para realizar una instalación silenciosa:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Encontrará detalles sobre los parámetros de línea de comandos en [Setup.exe y Update.exe parámetros de línea de comandos](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Al abrir la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Adobe Dynamic Media Classic inició sesión](/help/using/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para que **[!UICONTROL Server]** lo use, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (Norteamérica) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción de Asia-Pacífico (Asia-Pacífico) | https://s7sps5.scene7.com/ |

## Introducción a vídeo sobre el uso de Adobe Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Vea un recorrido en vídeo de [con la aplicación Adobe Dynamic Media Classic para escritorio](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (duración: 2 minutos y 36 segundos).

## Borrando la caché de imágenes y de recursos del equipo mediante la aplicación de escritorio {#clear-cache}

1. En la aplicación de escritorio de Adobe Dynamic Media Classic, cerca de la esquina superior derecha, pulsa **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**.
1. En la página **[!UICONTROL Configuración personal]**, en el encabezado **[!UICONTROL Escritorio]**, realice una de las siguientes acciones:
   * Para quitar todos los archivos de imagen en caché de Adobe Dynamic Media del equipo, pulse **[!UICONTROL Borrar caché de imágenes]** y, a continuación, pulse **[!UICONTROL Aceptar]**.
   * Para quitar todos los archivos de recursos en caché de Adobe Dynamic Media del equipo, pulse **[!UICONTROL Borrar caché de recursos]** y, a continuación, pulse **[!UICONTROL Aceptar]**.
1. En la esquina inferior derecha de la página, pulse **[!UICONTROL Cerrar]**.

### Borrado manual de la caché de imágenes y la caché de recursos

Además de borrar la caché de imágenes y recursos mediante la aplicación de escritorio, puede borrar manualmente la caché directamente desde el sistema de archivos.

1. En función del sistema operativo, vaya a lo siguiente:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitaciones conocidas en Adobe Dynamic Media Classic 20.21.1

* La lista desplegable **[!UICONTROL Servidor]** está vacía después de actualizar a la aplicación de escritorio de Adobe Dynamic Media Classic 20.21.1: Escenario: instale e inicie sesión en Adobe Dynamic Media Classic 20.20.1 o 20.20.2 y, a continuación, cierre la aplicación. A continuación, actualice a Adobe Dynamic Media Classic 20.21.1. Al intentar iniciar sesión, la lista desplegable **[!UICONTROL Servidor]** del cuadro de diálogo **[!UICONTROL Iniciar sesión en la cuenta]** está vacía. Para solucionar este problema, debe [borrar manualmente la caché](#clear-cache) (ver los pasos anteriores).

## Limitaciones conocidas en Adobe Dynamic Media Classic 20.20.1 (corregidas en 20.20.2)

**_Solo se aplica a Windows®. ¿Hay alguna limitación en la cantidad de archivos que se pueden cargar a través de la interfaz de usuario de la aplicación de escritorio?_**<br>Sí, se pueden cargar un máximo de 150 archivos a la vez mediante la interfaz de usuario de la aplicación de escritorio.

**_Se aplica a Windows® y macOS. ¿Cómo cambio de empresa?_**<br>Para cambiar de empresa, haga lo siguiente:

* En la aplicación de Adobe Dynamic Media Classic, seleccione la nueva empresa en la lista desplegable empresa.
* Cuando aparezca la ventana emergente, pulsa **[!UICONTROL Aceptar]** para cerrar la sesión y cerrar la aplicación.

  ![Para usar la nueva compañía, reinicia la aplicación](/help/using/assets/dmclassic-new-company1.png)

* Reinicie Adobe Dynamic Media Classic y, a continuación, inicie sesión como de costumbre para trabajar con la nueva empresa.

## Sugerencias y trucos

**_No puedo ver el panel Carro de medios en la página de aterrizaje de Adobe Dynamic Media Classic._**<br>En Adobe Dynamic Media Classic, pulse**[!UICONTROL Configuración > Configuración personal ]**. En la sección Explorador, asegúrese de que**[!UICONTROL Mostrar características de MediaPortal ]**está seleccionado (marcado). Pulse**[!UICONTROL Guardar > Cerrar ]**.

**_El estado de publicación (indicador verde) de un recurso no se refleja correctamente._**<br>En la interfaz de usuario del explorador, era necesario volver a iniciar sesión en la interfaz de usuario para ver el estado de publicación correcto de los recursos. En la aplicación de escritorio, Adobe ha incluido el icono**[!UICONTROL Actualizar ]**en la barra de herramientas, a la derecha del botón**[!UICONTROL Seleccionar ninguno ]**. Pulse el icono**[!UICONTROL Actualizar ]**para ver el estado más reciente de todos los recursos de la página dada. No es necesario volver a iniciar sesión, como con la interfaz de usuario del explorador.

![Icono de actualización](/help/using/assets/refresh-icon1.png)
*Icono de actualización*

**_No veo que funcionen los ajustes preestablecidos de conjunto por lotes en la aplicación de escritorio._**<br>Pulse**[!UICONTROL Cargar > Opciones del trabajo > Ajustes preestablecidos de conjunto de lotes ]**. Asegúrese de que el**[!UICONTROL ajuste preestablecido del conjunto de lotes ]**correspondiente esté habilitado. Haga clic en**[!UICONTROL Guardar y enviar carga ]**.
