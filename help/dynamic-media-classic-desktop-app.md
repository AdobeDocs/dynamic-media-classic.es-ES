---
title: 'Aplicación de escritorio de Adobe Dynamic Media Classic: ahora disponible'
seo-title: 'Aplicación de escritorio de Adobe Dynamic Media Classic: ahora disponible'
description: nulo
seo-description: Obtenga más información sobre la aplicación de escritorio Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 88f73056803a34ef2748b19eafbe7d50933b4d6a
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---


# Ya disponible: Aplicación de escritorio de Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Los usuarios de Dynamic Media Classic ahora tienen acceso a una nueva experiencia de aplicación de escritorio que ya no depende de la tecnología Adobe Flash en el navegador.

Esta nueva aplicación ya está disponible para Windows y MacOS.

>[!IMPORTANT]
>
>Le recomendamos que instale la nueva aplicación de escritorio Adobe Dynamic Media Classic antes del 1 de octubre de 2020. Al hacerlo, se asegurará de que dispone de una transición suave antes de que Adobe Flash Player quede obsoleto el 31 de diciembre de 2020. En esa fecha, ya no podrá iniciar sesión en la versión del navegador de la interfaz de usuario de Adobe Dynamic Media Classic, etiquetada como Scene7 Publishing System en el producto.

Consulte las preguntas más frecuentes sobre la experiencia de inicio de sesión de [nuevo Dynamic Media Classic ahora disponible.](/help/new-ui-2020.md)

## Requisitos del sistema para la aplicación de escritorio de Adobe Dynamic Media Classic {#system-requirements-dmc-app}

La aplicación de escritorio Adobe Dynamic Media Classic es compatible con los siguientes sistemas operativos:
* macOS X 10.10 o posterior.
* Windows 7 o posterior.

## Descargar e instalar la aplicación de escritorio de Adobe Dynamic Media Classic {#installation-dmc-app}

1. Desinstale cualquier versión anterior de la aplicación de escritorio de Dynamic Media Classic en el sistema.

1. Descargue el instalador más reciente para la aplicación de escritorio Adobe Dynamic Media Classic.

   * [macOS (.dmg) - Descargar.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.exe): descarga.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Realice una de las siguientes acciones en función del instalador que descargó.

   * **Para macOS** : en el cuadro de diálogo **[!UICONTROL Arrastrar y soltar para instalar]** , arrastre **[!UICONTROL Adobe Dynamic Media Classic]** y suéltelo en **[!UICONTROL Aplicaciones]**.

      ![Arrastre y suelte la instalación en macOS](/help/assets/dragondrop-install1.png)

   * En la carpeta **[!UICONTROL Aplicaciones]** , toque el icono de Adobe Dynamic Media Classic.
   * En el cuadro de diálogo, toque **[!UICONTROL Abrir]** para abrir la aplicación de escritorio de Adobe Dynamic Media Classic.

      ![Abrir aplicación descargada](/help/assets/open-dmclassicapp1.png)

   * **Para Windows** : ejecute el archivo binario del instalador y siga las instrucciones que aparecen en pantalla para instalar la aplicación de escritorio.

1. Al abrir la aplicación, se muestra la nueva página de inicio de sesión de Adobe Dynamic Media Classic:

   ![Inicio de sesión de Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Utilice las mismas credenciales que las credenciales del explorador para iniciar sesión en Adobe Dynamic Media Classic.

   Para que el **[!UICONTROL servidor]** lo utilice, consulte la siguiente asignación para el entorno de producción:

   | URL del explorador | Nombre del servidor de aplicaciones de escritorio |
   |---|---|
   | https://s7sps1.scene7.com/ | Producción de NA (Norteamérica) |
   | https://s7sps3.scene7.com/ | Producción EMEA (Europa, Oriente Medio y África) |
   | https://s7sps5.scene7.com/ | Producción de APAC (Asia-Pacífico) |

1. Al publicar la interfaz de usuario de inicio de sesión, verá la experiencia familiar de la interfaz de usuario del explorador. Puede llevar su actividad diaria como de costumbre ahora en la interfaz de usuario de la aplicación de escritorio.

## Vídeo explicativo sobre el uso de la aplicación Dynamic Media Classic Desktop

Vea un [vídeo explicativo sobre el uso de Dynamic Media Classic Desktop App](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) (Duración: 2 minutos y 36 segundos).

## Limitaciones conocidas en Dynamic Media Classic

**_Solo se aplica a Windows: ¿Existe alguna limitación en el número de archivos que se pueden cargar a través de la interfaz de usuario de la aplicación de escritorio?_**<br> Sí, se puede cargar un máximo de 150 archivos a la vez mediante la interfaz de usuario de la aplicación de escritorio.

**_Se aplica a Windows y macOS: ¿Cómo cambio entre compañías?_**<br> Para cambiar entre compañías, haga lo siguiente:
* En la aplicación Dynamic Media Classic, seleccione la nueva compañía en la lista desplegable compañía.
* Cuando aparezca la ventana emergente, toque **[!UICONTROL Aceptar]** para cerrar sesión y cerrar la aplicación.

   ![Reinicie la aplicación para utilizar la nueva compañía](/help/assets/dmclassic-new-company1.png)
* Reinicie Dynamic Media Classic e inicie sesión como de costumbre para trabajar con la nueva compañía.

## Sugerencias y trucos

**_No puedo ver el panel Carro multimedia en la página de aterrizaje de Dynamic Media Classic._**<br> En Dynamic Media Classic, toque **[!UICONTROL Ajustes > Ajustes]** personales. En la sección Explorador, asegúrese de que la opción **[!UICONTROL Mostrar funciones]** de Media Portal está seleccionada (activada). Toque **[!UICONTROL Guardar > Cerrar]**.

**_El estado de publicación (indicador verde) de un recurso no se refleja correctamente._**<br> En la interfaz de usuario del explorador, se requería volver a iniciar sesión en la interfaz de usuario para ver el estado de publicación correcto de los recursos. En la aplicación de escritorio, hemos introducido un icono **[!UICONTROL Actualizar]** en la barra de herramientas, a la derecha del botón **[!UICONTROL Seleccionar ninguno]** . Toque el icono **[!UICONTROL Actualizar]** para ver el estado más reciente de todos los recursos de una página determinada. No es necesario volver a iniciar sesión como en la interfaz de usuario del explorador.

![Icono](/help/assets/refresh-icon1.png)Actualizar icono *Actualizar*

**_No veo que los ajustes preestablecidos de conjunto de lotes funcionen en la aplicación de escritorio._**<br> Toque **[!UICONTROL Cargar > Opciones de trabajo > Valores preestablecidos]** de conjunto por lotes. Asegúrese de que el ajuste preestablecido **[!UICONTROL de conjunto de]** lotes correspondiente está activado. Haga clic en **[!UICONTROL Guardar y enviar carga]**.
