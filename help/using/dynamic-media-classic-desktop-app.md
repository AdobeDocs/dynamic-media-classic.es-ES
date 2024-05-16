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

Los usuarios de Adobe Dynamic Media Classic ahora tienen acceso a una nueva experiencia de aplicación de escritorio que ya no depende de la tecnología de Flash de Adobe en el navegador.

Esta nueva aplicación ya está disponible para Windows® y macOS.

>[!IMPORTANT]
>
>El Adobe recomienda instalar la nueva aplicación de escritorio de Adobe Dynamic Media Classic antes del 1 de octubre de 2020. Al hacerlo, se garantiza una transición sin problemas antes de que el Flash Player de Adobe quede obsoleto el 31 de diciembre de 2020. Después de esta fecha, no podrá iniciar sesión en la versión del explorador de la interfaz de usuario de Adobe Dynamic Media Classic, etiquetada como Adobe Dynamic Media Classic en el producto.

Consulte las preguntas frecuentes sobre [Ya está disponible el nuevo inicio de sesión de Adobe Dynamic Media Classic.](/help/using/new-ui-2020.md)

## Requisitos del sistema para la aplicación de escritorio de Adobe Dynamic Media Classic {#system-requirements-dmc-app}

La aplicación de escritorio de Adobe Dynamic Media Classic es compatible con los siguientes sistemas operativos:

* macOS 10.10 o posterior.
* Windows® 7 o posterior.

Consulte los requisitos completos del sistema en [Requisitos del sistema para la aplicación de escritorio de Adobe Dynamic Media Classic](/help/using/system-requirements.md).

La notificación de actualización dentro de la aplicación de escritorio de Adobe Dynamic Media Classic no se genera para *menor* versiones. Los clientes que se benefician de las correcciones en una versión menor pueden actualizar.

## Solo se ha corregido en la última versión (20.22.2) de macOS {#release-feb2022}

* macOS Monterey: La página de carga de archivos se ha congelado en cargas posteriores. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Correcciones en la última versión (20.22.1) {#release-jan2022}

* Al editar una imagen, la variable **[!UICONTROL Guardar]** Los botones no funcionaban.
* En los editores de conjuntos, la variable **[!UICONTROL Cerrar]**, **[!UICONTROL Guardar]**, y **[!UICONTROL Guardar como]** Los botones se desactivan después de desplazarse por los recursos en la **[!UICONTROL Añadir recursos]** panel.
* El **[!UICONTROL Reproducir]** El botón en la vista de detalles de vídeo no funcionaba.
* No se ha podido introducir `d` y `e` in **[!UICONTROL Nombre de usuario]** y **[!UICONTROL Contraseña]** al ejecutar macOS Monterrey.
* Se han movido las API de análisis restantes a la versión 2.0.

## Correcciones en la versión 20.21.3 {#release-sept2021}

* Miniaturas rotas para recursos vistos después de un período de inactividad en la aplicación de escritorio.
* La aplicación de escritorio deja de responder, generalmente después de establecer operaciones.
* Modo de bloqueo y ofuscación de solicitudes activado automáticamente en **[!UICONTROL Probar servicio de imágenes]**.

  Consulte [El servicio Secure Testing](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Se ha actualizado el mecanismo de autenticación con Adobe Analytics. Es relevante para nuevas integraciones o si algunas variables de Analytics deben actualizarse desde la aplicación de escritorio de Dynamic Media Classic.

  Consulte [Iniciar sesión en Adobe Analytics](/help/using/log-analytics.md) para ver los pasos actualizados.

## Correcciones en la versión 20.21.2 {#minor-release}

* Limitación conocida en 20.21.1: la variable **[!UICONTROL Servidor]** La lista desplegable de la pantalla de inicio de sesión estaba vacía.
* Entrada **[!UICONTROL Opciones del trabajo de carga]**, el valor predeterminado Nombre de capa en **[!UICONTROL Opciones de Photoshop]**, es ahora **[!UICONTROL Nombre de capa y Photoshop]**. Las capas del archivo de PSD se cargan como imágenes independientes.
   * El valor predeterminado anterior de **[!UICONTROL Nombre de capa]**, asigne a las imágenes un nombre en función del nombre o el número de capa que tengan en el archivo de PSD. El número de capa se utilizaba si los nombres de capa del fichero de PSD eran nombres de capa de Photoshop por defecto.
   * El nuevo valor predeterminado de **[!UICONTROL Nombre de capa y Photoshop]**, asigna un nombre a las imágenes después del archivo de PSD seguido del nombre o número de capa. El número de capa se utiliza si los nombres de capa del fichero de PSD son nombres de capa de Photoshop por defecto.
   * Dado que las imágenes de capa de Adobe Dynamic Media Classic ahora tienen nombres únicos, no se va a realizar ninguna actualización de las plantillas existentes o del PSD (qué nombres de capa compartidos en los archivos de PSD originales).
* Miniaturas de recursos rotas.

## Correcciones en la versión 20.21.1 {#latest-fixes-desktop-app}

* Problemas de inicio de sesión debido al tiempo de espera que resultan en el siguiente mensaje: *Este usuario puede asignarse al grupo o grupos sin permiso. Póngase en contacto con el administrador.*
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

   * **macOS** -En el **[!UICONTROL Arrastrar y soltar para instalar]** cuadro de diálogo, arrastrar **[!UICONTROL Adobe Dynamic Media Classic]** y suéltelo en **[!UICONTROL Aplicaciones]**.

     ![Arrastrar y soltar la instalación en macOS](/help/using/assets/dragondrop-install1.png)

   * En el **[!UICONTROL Aplicaciones]** , pulse el icono Adobe Dynamic Media Classic.
   * En el cuadro de diálogo, pulse **[!UICONTROL Abrir]** para abrir la aplicación de escritorio de Adobe Dynamic Media Classic.

     ![Abrir la aplicación descargada](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** : ejecute el binario del instalador y siga las instrucciones que aparecen en pantalla para instalar la aplicación de escritorio.

1. Al abrir la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Inicio de sesión de Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para el **[!UICONTROL Servidor]** para utilizar, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (Norteamérica) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción de Asia-Pacífico (Asia-Pacífico) | https://s7sps5.scene7.com/ |

1. Después de iniciar sesión, observe la experiencia familiar de la interfaz de usuario del explorador. Puede continuar con su actividad diaria de Adobe Dynamic Media Classic como de costumbre en la aplicación de escritorio.

## Descargar y *silenciosamente* instale la última aplicación de escritorio de Adobe Dynamic Media Classic en macOS {#install-silent-mac-dmc-app}

Consulte también:

* [Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac o Windows](#installation-dmc-app)
* [Descargue e instale de forma silenciosa la última aplicación de escritorio de Adobe Dynamic Media Classic en Windows](#install-silent-windows-dmc-app)

Para descargar y *silenciosamente* instale la última versión de la aplicación de escritorio de Adobe Dynamic Media Classic en macOS:

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

   ![Inicio de sesión de Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para el **[!UICONTROL Servidor]** para utilizar, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (Norteamérica) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción de Asia-Pacífico (Asia-Pacífico) | https://s7sps5.scene7.com/ |

## Descargar y *silenciosamente* instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Windows® {#install-silent-windows-dmc-app}

El comando que utiliza es para una instalación silenciosa MSI básica. Sin embargo, el instalador de la aplicación de escritorio de Adobe Dynamic Media Classic es un instalador MSI de InstallScript creado con InstallShield. Cuando se ejecuta el instalador en modo de registro, cualquier interacción del usuario se registra en un archivo de respuesta. Este archivo de respuesta se utiliza para una instalación silenciosa como se describe en [Ejecución de instalaciones en modo silencioso](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Consulte también:

* [Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac o Windows](#installation-dmc-app)

* [Descargue e instale de forma silenciosa la última aplicación de escritorio de Adobe Dynamic Media Classic en macOS](#install-silent-mac-dmc-app)

Para descargar y *silenciosamente* instale la última versión de la aplicación de escritorio de Adobe Dynamic Media Classic en Windows®:

1. Desinstale las versiones anteriores de la aplicación de escritorio de Adobe Dynamic Media Classic en el sistema.

1. Descargue el último instalador para la aplicación de escritorio de Adobe Dynamic Media Classic.

   * [Windows® (.EXE): Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Ejecute el instalador en modo de registro con el siguiente comando:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. En la ventana del instalador de GUI, siga los pasos para instalar de modo que las interacciones/entradas, como la ubicación de instalación, se registren en `Setup.iss` archivo.

1. Copie el creado `Setup.iss` archivo y `adobe-dynamic-media-classic-20.22.1.exe` a otro equipo.

1. Ejecute el siguiente comando para realizar una instalación silenciosa:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Encontrará detalles sobre los parámetros de la línea de comandos en [Parámetros de línea de comandos Setup.exe y Update.exe](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Al abrir la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Inicio de sesión de Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para el **[!UICONTROL Servidor]** para utilizar, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (Norteamérica) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción de Asia-Pacífico (Asia-Pacífico) | https://s7sps5.scene7.com/ |

## Introducción a vídeo sobre el uso de Adobe Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Ver una [Introducción a vídeo sobre el uso de la aplicación de escritorio de Adobe Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (Duración: 2 minutos y 36 segundos).

## Borrando la caché de imágenes y de recursos del equipo mediante la aplicación de escritorio {#clear-cache}

1. En la aplicación de escritorio de Adobe Dynamic Media Classic, cerca de la esquina superior derecha, pulse **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes personales]**.
1. En el **[!UICONTROL Ajustes personales]** , debajo de la **[!UICONTROL Escritorio]** , realice una de las acciones siguientes:
   * Para quitar todos los archivos de imagen en caché de Dynamic Media de Adobe del equipo, pulse **[!UICONTROL Borrar caché de imágenes]**, y pulse **[!UICONTROL OK]**.
   * Para quitar todos los archivos de recursos en caché de Dynamic Media de Adobe del equipo, pulse **[!UICONTROL Borrar caché de recursos]**, y pulse **[!UICONTROL OK]**.
1. En la esquina inferior derecha de la página, pulse **[!UICONTROL Cerrar]**.

### Borrado manual de la caché de imágenes y la caché de recursos

Además de borrar la caché de imágenes y recursos mediante la aplicación de escritorio, puede borrar manualmente la caché directamente desde el sistema de archivos.

1. En función del sistema operativo, vaya a lo siguiente:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitaciones conocidas en Adobe Dynamic Media Classic 20.21.1

* El **[!UICONTROL Servidor]** La lista desplegable está vacía después de actualizar a la aplicación de escritorio de Adobe Dynamic Media Classic 20.21.1: Escenario: instala e inicia sesión en Adobe Dynamic Media Classic 20.20.1 o 20.20.2 y, a continuación, cierra la aplicación. A continuación, actualice a Adobe Dynamic Media Classic 20.21.1. Cuando intente iniciar sesión, la variable **[!UICONTROL Servidor]** en la lista desplegable de **[!UICONTROL Inicie sesión en su cuenta]** El cuadro de diálogo está vacío. Para solucionar este problema, debe [borrar manualmente la caché](#clear-cache) (consulte los pasos anteriores).

## Limitaciones conocidas en Adobe Dynamic Media Classic 20.20.1 (corregidas en 20.20.2)

**_Solo se aplica a Windows®. ¿Existe una limitación en el número de archivos que se pueden cargar a través de la interfaz de usuario de la aplicación de escritorio?_**<br>Sí, se puede cargar un máximo de 150 archivos a la vez mediante la interfaz de usuario de la aplicación de escritorio.

**_Aplicable a Windows® y macOS. ¿Cómo cambio de empresa?_**<br>Para cambiar de empresa, haga lo siguiente:

* En la aplicación de Adobe Dynamic Media Classic, seleccione la nueva empresa en la lista desplegable empresa.
* Cuando aparezca la ventana emergente, pulse **[!UICONTROL OK]** para cerrar la sesión y la aplicación.

  ![Para usar la nueva empresa, reinicie la aplicación](/help/using/assets/dmclassic-new-company1.png)

* Reinicie Adobe Dynamic Media Classic y, a continuación, inicie sesión como de costumbre para trabajar con la nueva empresa.

## Sugerencias y trucos

**_No puedo ver el panel Carro de medios en la página de aterrizaje de Adobe Dynamic Media Classic._**<br>En Adobe Dynamic Media Classic, pulse**[!UICONTROL Configuración > Configuración personal ]**. En la sección Explorador, asegúrese de que**[!UICONTROL Mostrar funciones de MediaPortal ]**está seleccionada (marcada). Tocar**[!UICONTROL Guardar > Cerrar ]**.

**_El estado de publicación (indicador verde) de un recurso no se refleja correctamente._**<br>En la interfaz de usuario del explorador, era necesario volver a iniciar sesión en la interfaz de usuario para ver el estado de publicación correcto de los recursos. En la aplicación de escritorio, Adobe ha introducido un**[!UICONTROL Actualizar ]**en la barra de herramientas, a la derecha de la**[!UICONTROL Seleccionar ninguno ]**botón. Pulse el botón**[!UICONTROL Actualizar ]**para ver el estado más reciente de todos los recursos de la página determinada. No es necesario volver a iniciar sesión, como con la interfaz de usuario del explorador.

![Icono Actualizar](/help/using/assets/refresh-icon1.png)
*Icono Actualizar*

**_No veo ajustes preestablecidos de conjunto por lotes funcionando en la aplicación de escritorio._**<br>Tocar**[!UICONTROL Cargar > Opciones del trabajo > Ajustes preestablecidos del conjunto de lotes ]**. Asegúrese de que las**[!UICONTROL Ajuste preestablecido del conjunto de lotes ]**está activada. Clic**[!UICONTROL Guardar y enviar la carga ]**.
