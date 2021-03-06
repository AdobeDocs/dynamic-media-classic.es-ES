---
title: Perfiles ICC (International Color Consortium)
description: Obtenga información sobre los perfiles ICC en Adobe Dynamic Media Classic.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 54%

---

# Perfiles ICC{#icc-profiles}

Un perfil ICC (International Color Consortium) es un archivo que describe cómo se deben convertir los archivos de imagen de un espacio de color a otro. Los perfiles ICC le ayudan a obtener los colores correctos para las imágenes. Por ejemplo, para mostrar correctamente imágenes diseñadas para la impresión en un monitor de ordenador, puede elegir un perfil ICC. Este perfil convierte el espacio de color de la imagen y garantiza que los colores se muestren correctamente en línea.

En Adobe Dynamic Media Classic, puede elegir un perfil ICC para convertir imágenes a un espacio de color diferente al cargar las imágenes. Todos los perfiles ICC estándar de Photoshop están disponibles de forma predeterminada en Adobe Dynamic Media Classic. Para ver los nombres de los perfiles de color en la pantalla de carga, seleccione el menú Perfil de color. A continuación elija Personalizar De > A y elija un perfil ICC en los menús Convertir de y Convertir a.

Consulte [Opciones de edición de imágenes en upload](image-editing-options-upload.md#image-editing-options-at-upload).

Además de utilizar los perfiles ICC predeterminados, puede cargar otros perfiles ICC en Adobe Dynamic Media Classic y ponerlos a disposición para la conversión de espacio de color. Cambie a Vista detallada en el panel Examinar para investigar la clase de perfil, el tipo de espacio de color y el tipo PCS de un perfil ICC.

## Cargar perfiles ICC {#uploading-icc-profiles}

Cargue perfiles ICC utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar perfiles ICC en cualquier carpeta de Adobe de Dynamic Media Classic.

Consulte [Cargar los archivos](uploading-files.md#uploading_your_files).

## Examinar un perfil ICC {#examining-an-icc-profile}

Para examinar un perfil ICC, selecciónelo en el panel Examinar y muéstrelo en la Vista de detalles. Vista de detalles proporciona esta información sobre los perfiles ICC:

* **[!UICONTROL Clase de Perfil]** : ICC (International Color Consortium) define cada clase para cubrir un tipo de aplicación. Por ejemplo, los perfiles de entrada se aplican a los dispositivos como las cámaras digitales o los escáneres, mientras que los perfiles de salida se aplican a las impresoras.

* **[!UICONTROL Tipo de espacio de color]** : este número es el espacio de color de &quot;entrada&quot; del perfil, tal como lo define la ICC. El tipo de espacio de color especifica el número de componentes del espacio de color y la interpretación de esos componentes. Por ejemplo, RGB es un espacio de color con tres componentes: rojo, verde y azul. El tipo de espacio de color no precisa las características de color del espacio (por ejemplo, la cromaticidad de los colores primarios).

* **[!UICONTROL Tipo PCS]** : este tipo de PCS es el espacio de color de &quot;salida&quot; del perfil, su espacio de conexión de perfil. Por ejemplo, un perfil de color puede convertir RGB al PCS, el cual lo convierte en CMYK.

Para obtener un perfil de entrada, presentación y salida útil para el etiquetado de colores e imágenes, el tipo de PCS debe ser XYZ o Lab. Este perfil sería el espacio de color específico correspondiente que se define en la especificación de ICC.
