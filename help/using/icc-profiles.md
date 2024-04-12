---
title: Perfiles ICC (International Color Consortium)
description: Obtenga información acerca de los perfiles ICC en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 50%

---

# Perfiles ICC{#icc-profiles}

Un perfil ICC (International Color Consortium) es un archivo que describe cómo se deben convertir los archivos de imagen de un espacio de color a otro. Los perfiles ICC le ayudan a obtener los colores correctos para las imágenes. Por ejemplo, para mostrar correctamente imágenes diseñadas para la impresión en un monitor de ordenador, puede elegir un perfil ICC. Este perfil convierte el espacio de color de la imagen y garantiza que los colores se muestren correctamente en línea.

En Adobe Dynamic Media Classic, puede elegir un perfil ICC para convertir las imágenes a un espacio de color diferente al cargarlas. Todos los perfiles ICC estándar de Photoshop están disponibles de forma predeterminada en Adobe Dynamic Media Classic. Para ver los nombres de los perfiles de color en la pantalla de carga, seleccione el menú Perfil de color. A continuación, elija Personalizado desde > Hasta y elija un nombre de perfil ICC en los menús Convertido desde y Convertido a.

Consulte [Opciones de edición de imágenes al cargar](image-editing-options-upload.md#image-editing-options-at-upload).

Además de utilizar los perfiles ICC predeterminados, puede cargar otros perfiles ICC en Adobe Dynamic Media Classic y ponerlos a disposición de la conversión del espacio de color. Cambie a la Vista de detalles en el panel de exploración para investigar la clase de perfil, el tipo de espacio de color y el tipo PCS de un perfil ICC.

## Carga de perfiles ICC {#uploading-icc-profiles}

Cargue perfiles ICC utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar perfiles ICC en cualquier carpeta de Adobe Dynamic Media Classic.

Consulte [Cargar los archivos](uploading-files.md#uploading_your_files).

## Examen de un perfil ICC {#examining-an-icc-profile}

Para examinar un perfil ICC, selecciónelo en el panel de exploración y muéstrelo en la vista de detalles. La Vista de detalles proporciona esta información sobre los perfiles ICC:

* **[!UICONTROL Clase de perfil]** - El ICC (International Color Consortium) define cada clase para cubrir un tipo de aplicación. Por ejemplo, los perfiles de entrada se aplican a los dispositivos como las cámaras digitales o los escáneres, mientras que los perfiles de salida se aplican a las impresoras.

* **[!UICONTROL Tipo de espacio de color]** - Este número es el espacio de color de &quot;entrada&quot; del perfil, tal como lo define el ICC. El tipo de espacio de color especifica el número de componentes del espacio de color y la interpretación de esos componentes. Por ejemplo, RGB es un espacio de color con tres componentes: rojo, verde y azul. El tipo de espacio de color no precisa las características de color del espacio (por ejemplo, la cromaticidad de los colores primarios).

* **[!UICONTROL Tipo de PCS]** - Este tipo de PCS es el espacio de color de &quot;salida&quot; del perfil: su espacio de conexión de perfil. Por ejemplo, un perfil de color puede convertir RGB al PCS, el cual lo convierte en CMYK.

Para obtener un perfil de entrada, presentación y salida útil para el etiquetado de colores e imágenes, el tipo de PCS debe ser XYZ o Lab. Este perfil sería el espacio de color específico correspondiente que se define en la especificación de ICC.
