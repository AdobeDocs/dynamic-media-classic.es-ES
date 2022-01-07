---
title: 'Aplicación de escritorio de Adobe Dynamic Media Classic: ya disponible'
description: Obtenga más información sobre la aplicación de escritorio de Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: df41d69e2fa6e9db806d8ffbb06edc42b70d1011
workflow-type: tm+mt
source-wordcount: '1940'
ht-degree: 1%

---

# Ya disponible: aplicación de escritorio de Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Los usuarios de Adobe Dynamic Media Classic ahora tienen acceso a una nueva experiencia de aplicación de escritorio que ya no depende de la tecnología de Flash de Adobe del navegador.

Esta nueva aplicación ya está disponible para Windows® y macOS.

>[!IMPORTANT]
>
>Adobe recomienda instalar la nueva aplicación de escritorio de Adobe Dynamic Media Classic antes del 1 de octubre de 2020. Al hacerlo, se asegurará de que la transición sea fluida antes de que el Flash Player del Adobe quede obsoleto el 31 de diciembre de 2020. Después de esta fecha, no podrá iniciar sesión en la versión del navegador de la interfaz de usuario de Adobe Dynamic Media Classic, etiquetada como Adobe Dynamic Media Classic en el producto.

Consulte las preguntas frecuentes para la sección [Ya está disponible la nueva experiencia de inicio de sesión en Adobe Dynamic Media Classic.](/help/new-ui-2020.md)

## Requisitos del sistema para la aplicación de escritorio de Adobe Dynamic Media Classic {#system-requirements-dmc-app}

La aplicación de escritorio de Adobe Dynamic Media Classic es compatible con los siguientes sistemas operativos:

* macOS 10.10 o posterior.
* Windows® 7 o posterior.

>[!NOTE]
>
>La notificación de actualización en la aplicación de escritorio de Adobe Dynamic Media Classic no se genera para *menor* versiones. Los clientes que se benefician de las correcciones en una versión menor pueden actualizarse.

## Correcciones en la última versión (20.22.1) {#release-jan2022}

* 

   <!-- CQ-4333853 :  -->Image editing **[!UICONTROL Save]** buttons were non-functional.
* 

   <!-- CQ-4334638 :  -->In the Set editors, the **[!UICONTROL Close]**, **[!UICONTROL Save]**, and **[!UICONTROL Save As]** buttons become disabled after scrolling assets in the **[!UICONTROL Add Assets]** panel.
* 

   <!-- CQ-4335992 :  -->**[!UICONTROL Play]** button in Video Detail view did not work.
* 

   <!-- CQ-4336687 :  -->Could not enter `d` and `e` in **[!UICONTROL Username]** and **[!UICONTROL Password]** fields when running macOS Monterey.
* 

   <!-- CQ-4334197 :  -->Moved the remaining analytics APIs to version 2.0.

## Correcciones en la versión (20.21.3) {#release-sept2021}

* Miniaturas rotas de los recursos que se ven después de un período de inactividad en la aplicación de escritorio.
* La aplicación de escritorio deja de responder, normalmente después de las operaciones Set.
* El modo de ocultación y bloqueo de solicitud se habilita automáticamente en **[!UICONTROL Probar servicio de imágenes]**.

   Consulte [Probar el servicio Secure Testing](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Se ha actualizado el mecanismo de autenticación con Adobe Analytics. Relevante para nuevas integraciones o si algunas variables de Analytics deben actualizarse desde la aplicación de escritorio de Dynamic Media Classic.

   Consulte [Iniciar sesión en Adobe Analytics](/help/log-analytics.md) para ver los pasos actualizados.

## Correcciones en la versión 20.21.2 {#minor-release}

* Limitación conocida en 20.21.1: el **[!UICONTROL Servidor]** la lista desplegable de la pantalla de inicio de sesión estaba vacía.
* En **[!UICONTROL Cargar opciones de trabajo]**, Valor predeterminado de nomenclatura de capas en **[!UICONTROL Opciones de Photoshop]**, ahora **[!UICONTROL Photoshop y nombre de capa]**. Las capas en el archivo PSD se cargan como imágenes independientes.
   * El valor predeterminado anterior de **[!UICONTROL Nombre de la capa]**, las imágenes reciben el nombre del nombre o número de capa de su archivo PSD. El número de capa se utilizó si los nombres de capa en el archivo PSD eran nombres de capa predeterminados de Photoshop.
   * El nuevo valor predeterminado de **[!UICONTROL Photoshop y nombre de capa]**, nombra las imágenes después del archivo de PSD seguido del nombre o número de capa. El número de capa se utiliza si los nombres de capa en el archivo PSD son nombres de capa predeterminados de Photoshop.
   * Dado que las imágenes de capa en Adobe Dynamic Media Classic ahora tienen nombres únicos, no se van a producir actualizaciones en el PSD o las plantillas existentes (que comparten nombres de capa en los archivos de PSD originales).
* Miniaturas de recursos rotas.

## Correcciones en la versión 20.21.1 {#latest-fixes-desktop-app}

* Problemas de inicio de sesión debido al tiempo de espera que dan como resultado el siguiente mensaje: *Este usuario puede asignarse al grupo o grupos sin permiso. Póngase en contacto con su administrador.*
* Los ajustes preestablecidos de visor se duplican con cada intento de contraseña incorrecto.
* La aplicación de escritorio deja de responder debido a muchos recursos en la carpeta raíz. (Fijo en Windows®; trabajando como desee en macOS).

## Correcciones en la versión 20.20.2 {#previous-version-fixes-desktop-app}

* No hay limitación en el número de archivos que puede cargar a través de la interfaz de usuario de la aplicación de escritorio tanto para macOS como para Windows®.
* No es necesario cerrar sesión en la aplicación de escritorio para cambiar entre empresas.
* Ctrl+V para pegar ahora funciona en Windows®.
* En el futuro, cuando se publique una nueva versión de la aplicación de escritorio, se notificará a los usuarios desde la propia aplicación de escritorio.

## Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en macOS o Windows® {#installation-dmc-app}

Véase también:

* [Descargue y silencie instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac](#install-silent-mac-dmc-app)
* [Descargue e instale silenciosamente la última aplicación de escritorio de Adobe Dynamic Media Classic en Windows®](#install-silent-windows-dmc-app)

1. Desinstale cualquier versión anterior de la aplicación de escritorio de Adobe Dynamic Media Classic en su sistema.

1. Descargue el último instalador de la aplicación de escritorio de Adobe Dynamic Media Classic.

   * La versión más reciente (20.22.1) está disponible en:

      * [macOS (.DMG): Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows (.EXE): descarga](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * La versión anterior (20.21.3) está disponible en:

      * [macOS (.DMG): Descargar](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)
      * [Windows® (.EXE) - Descargar](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Realice una de las siguientes acciones en función del instalador que descargó.

   * **macOS** -En el **[!UICONTROL Arrastre y suelte para instalar]** cuadro de diálogo, arrastrar **[!UICONTROL Adobe Dynamic Media Classic]** y suéltelo **[!UICONTROL Aplicaciones]**.

      ![Arrastre y suelte la instalación en macOS](/help/assets/dragondrop-install1.png)

   * En el **[!UICONTROL Aplicaciones]** , pulse el icono Adobe Dynamic Media Classic .
   * En el cuadro de diálogo, pulse **[!UICONTROL Apertura]** para abrir la aplicación de escritorio de Adobe Dynamic Media Classic.

      ![Abrir aplicación descargada](/help/assets/open-dmclassicapp1.png)

   * **Windows** - Ejecute el archivo binario del instalador y siga las instrucciones que aparecen en la pantalla para instalar la aplicación de escritorio.

1. Cuando abre la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Inicio de sesión en Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para la variable **[!UICONTROL Servidor]** para usar, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (América del Norte) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción APAC (Asia-Pacífico) | https://s7sps5.scene7.com/ |

1. Tras iniciar sesión, observe la experiencia familiar de la interfaz de usuario del explorador. Puede continuar su actividad diaria de Adobe Dynamic Media Classic como de costumbre en la aplicación de escritorio.

## Descargar y *silencioso* instale la última aplicación de escritorio de Adobe Dynamic Media Classic en macOS {#install-silent-mac-dmc-app}

Véase también:

* [Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac o Windows®](#installation-dmc-app)
* [Descargue e instale silenciosamente la última aplicación de escritorio de Adobe Dynamic Media Classic en Windows®](#install-silent-windows-dmc-app)

Para descargar y *silencioso* instale la última versión de la aplicación de escritorio de Adobe Dynamic Media Classic en macOS:

1. Desinstale cualquier versión anterior de la aplicación de escritorio de Adobe Dynamic Media Classic en su sistema.

1. Descargue el último instalador de la aplicación de escritorio de Adobe Dynamic Media Classic para macOS.

   * [macOS (.DMG): Descargar](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)

1. Monte la imagen de disco descargada (.DMG) en una ubicación de punto de montaje mediante el siguiente comando:

   `hdiutil attach adobe-dynamic-media-classic-20.22.1.dmg -mountpoint <mount_point_path>`

1. Copie el archivo .APP a **[!UICONTROL Aplicaciones]** mediante el siguiente comando:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Cuando abre la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Inicio de sesión en Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para la variable **[!UICONTROL Servidor]** para usar, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (América del Norte) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción APAC (Asia-Pacífico) | https://s7sps5.scene7.com/ |

## Descargar y *silencioso* instalar la aplicación de escritorio Adobe Dynamic Media Classic más reciente en Windows® {#install-silent-windows-dmc-app}

El comando que utiliza es para una instalación silenciosa básica de MSI. Sin embargo, el instalador de la aplicación de escritorio de Adobe Dynamic Media Classic es un instalador de InstallScript MSI creado con InstallShield. Cuando ejecuta el instalador en modo de registro, cualquier interacción del usuario se registra en un archivo de respuesta. A continuación, este archivo de respuesta se utiliza para una instalación silenciosa, tal como se describe en [Ejecución de instalaciones en modo silencioso.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Véase también:

* [Descargue e instale la última aplicación de escritorio de Adobe Dynamic Media Classic en Mac o Windows®](#installation-dmc-app)
* [Descargue y silencie instale la última aplicación de escritorio de Adobe Dynamic Media Classic en macOS](#install-silent-mac-dmc-app)

Para descargar y *silencioso* instale la última versión de la aplicación de escritorio de Adobe Dynamic Media Classic en Windows®:

1. Desinstale cualquier versión anterior de la aplicación de escritorio de Adobe Dynamic Media Classic en su sistema.

1. Descargue el último instalador de la aplicación de escritorio de Adobe Dynamic Media Classic.

   * [Windows® (.EXE) - Descargar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Ejecute el instalador en modo de registro mediante el siguiente comando:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. En la ventana del instalador de la GUI, siga los pasos para instalar de modo que las interacciones/entradas, como la ubicación de instalación, se registren en `Setup.iss` archivo.

1. Copie el `Setup.iss` y `adobe-dynamic-media-classic-20.22.1.exe` a otro equipo.

1. Ejecute el siguiente comando para una instalación silenciosa:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Los detalles sobre los parámetros de la línea de comandos están disponibles en [Parámetros de línea de comandos de Setup.exe y Update.exe.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Cuando abre la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Inicio de sesión en Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para iniciar sesión en la aplicación de escritorio de Adobe Dynamic Media Classic, utilice las mismas credenciales que utilizó para iniciar sesión en Adobe Dynamic Media Classic en el explorador.

   Para la variable **[!UICONTROL Servidor]** para usar, consulte la siguiente asignación para el entorno de producción:

   | Servidores | URL del explorador |
   | --- | --- |
   | Producción de NA (América del Norte) | https://s7sps1.scene7.com/ |
   | Producción de EMEA (Europa, Oriente Medio y África) | https://s7sps3.scene7.com/ |
   | Producción APAC (Asia-Pacífico) | https://s7sps5.scene7.com/ |

## Tutorial de vídeo sobre el uso de la aplicación de escritorio de Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Ver un [videotutorial sobre el uso de Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Longitud: 2 minutos y 36 segundos).

## Borrado de la caché de imágenes y la caché de recursos del equipo mediante la aplicación de escritorio {#clear-cache}

1. En la aplicación de escritorio de Adobe Dynamic Media Classic, cerca de la esquina superior derecha, pulse **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**.
1. En el **[!UICONTROL Configuración personal]** en el **[!UICONTROL Escritorio]** , realice una de las acciones siguientes:
   * Para quitar todos los archivos de imagen en caché de Dynamic Media de Adobe del equipo, pulse **[!UICONTROL Borrar caché de imágenes]** y, a continuación, toque **[!UICONTROL OK]**.
   * Para quitar todos los archivos de recursos en caché de Dynamic Media de Adobe del equipo, pulse **[!UICONTROL Borrar caché de recursos]** y, a continuación, toque **[!UICONTROL OK]**.
1. En la esquina inferior derecha de la página, pulse **[!UICONTROL Cerrar]**.

### Borrado manual de la caché de imágenes y la caché de recursos

Además de borrar la imagen y la caché de recursos mediante la aplicación de escritorio, puede borrar manualmente la caché directamente desde el sistema de archivos.

1. En función del sistema operativo, vaya a lo siguiente:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitación conocida en Adobe Dynamic Media Classic 20.21.1

* La variable **[!UICONTROL Servidor]** La lista desplegable está vacía después de actualizar a la aplicación de escritorio de Adobe Dynamic Media Classic 20.21.1: Situación: Instale e inicie sesión en Adobe Dynamic Media Classic 20.20.1 o 20.20.2 y, a continuación, cierre la aplicación. A continuación, actualice a Adobe Dynamic Media Classic 20.21.1. Cuando intente iniciar sesión, el **[!UICONTROL Servidor]** lista desplegable en la **[!UICONTROL Iniciar sesión en su cuenta]** El cuadro de diálogo está vacío. Para solucionar este problema, debe [borrar manualmente la caché](#clear-cache) (consulte los pasos anteriores).

## Limitaciones conocidas en Adobe Dynamic Media Classic 20.20.1 (corregidas en 20.20.2)

**_Solo se aplica a Windows®. ¿Existe alguna limitación en el número de archivos que se pueden cargar a través de la interfaz de usuario de la aplicación de escritorio?_**<br>Sí, se puede cargar un máximo de 150 archivos a la vez mediante la interfaz de usuario de la aplicación de escritorio.

**_Se aplica a Windows® y macOS. ¿Cómo puedo cambiar entre empresas?_**<br>Para cambiar entre empresas, haga lo siguiente:

* En la aplicación de Adobe Dynamic Media Classic, seleccione la nueva empresa en la lista desplegable de la empresa.
* Cuando aparezca la ventana emergente, pulse **[!UICONTROL OK]** para cerrar la sesión y cerrar la aplicación.

   ![Para usar la nueva empresa, reinicie la aplicación](/help/assets/dmclassic-new-company1.png)

* Reinicie Adobe Dynamic Media Classic y luego inicie sesión como de costumbre para trabajar con la nueva empresa.

## Sugerencias y trucos

**_No puedo ver el panel Carro de medios en la página de aterrizaje de Adobe Dynamic Media Classic._**<br>En Adobe Dynamic Media Classic, pulse**[!UICONTROL Configuración > Configuración personal ]**. En la sección Explorador , asegúrese de que**[!UICONTROL Mostrar funciones de MediaPortal ]**está seleccionada (marcada). Toque**[!UICONTROL Guardar > Cerrar ]**.

**_El estado de publicación (indicador verde) de un recurso no se refleja correctamente._**<br>En la interfaz de usuario del explorador, era necesario volver a iniciar sesión en la interfaz de usuario para ver el estado de publicación correcto de los recursos. En la aplicación de escritorio, Adobe ha introducido un**[!UICONTROL Actualizar ]**en la barra de herramientas, a la derecha del**[!UICONTROL Seleccionar Ninguno ]**botón. Toque .**[!UICONTROL Actualizar ]**para ver el estado más reciente de todos los recursos de una página determinada. No es necesario volver a iniciar sesión como con la interfaz de usuario del explorador.

![Actualizar icono](/help/assets/refresh-icon1.png)
*Actualizar icono*

**_No veo ajustes preestablecidos de conjuntos de lotes que funcionen en la aplicación de escritorio._**<br>Toque**[!UICONTROL Cargar > Opciones de trabajo > Ajustes preestablecidos de conjunto de lotes ]**. Asegúrese de que**[!UICONTROL Ajuste preestablecido de conjunto de lotes ]**está activada. Haga clic en**[!UICONTROL Cargar Guardar y enviar ]**.
