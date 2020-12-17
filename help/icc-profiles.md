---
title: Perfiles ICC
seo-title: Perfiles ICC
description: nulo
seo-description: Obtenga información sobre los perfiles ICC.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 71%

---


# Perfiles ICC{#icc-profiles}

Un perfil ICC (International Color Consortium) es un archivo que describe cómo se deben convertir los archivos de imagen de un espacio de color a otro. Los perfiles ICC le ayudan a obtener los colores correctos para las imágenes. Por ejemplo, para mostrar correctamente imágenes diseñadas para la impresión en un monitor de ordenador, puede elegir un perfil ICC. Este perfil convierte el espacio de color de la imagen y garantiza que los colores se muestren correctamente en línea.

En Dynamic Media Classic, puede elegir un perfil ICC para convertir imágenes a un espacio de color diferente al cargar las imágenes. Todos los perfiles ICC estándar de Photoshop están disponibles de forma predeterminada en Dynamic Media Classic. Para ver los nombres de los perfiles de color en la pantalla de carga, seleccione el menú Perfil de color. A continuación elija Personalizar De > A y elija un perfil ICC en los menús Convertir de y Convertir a. Consulte [Opciones de edición de imágenes al cargarlas](image-editing-options-upload.md#image-editing-options-at-upload).

Además de utilizar los perfiles ICC predeterminados, puede cargar otros perfiles ICC a Dynamic Media Classic y hacerlos disponibles para la conversión de espacio de color. Cambie a la vista de detalles en el panel Examinar para investigar la clase de perfil, el tipo de espacio de color y el tipo de PCS de un perfil ICC.

## Carga de perfiles ICC  {#uploading-icc-profiles}

Cargue perfiles ICC utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar perfiles ICC en cualquier carpeta de Dynamic Media Classic. Consulte [Carga de los archivos](uploading-files.md#uploading_your_files).

## Examen de un perfil ICC  {#examining-an-icc-profile}

Para examinar un perfil ICC, selecciónelo en el panel Examinar y acceda a la vista de detalles. La vista de detalles le ofrece esta información sobre los perfiles ICC:

**Clase** de perfilEl ICC (International Color Consortium) define cada clase para cubrir un tipo de aplicación. Por ejemplo, los perfiles de entrada se aplican a los dispositivos como las cámaras digitales o los escáneres, mientras que los perfiles de salida se aplican a las impresoras.

**Tipo de** espacio de colorEste número es el espacio de color de &quot;entrada&quot; del perfil, tal como lo define el ICC. El tipo de espacio de color especifica el número de componentes del espacio de color y la interpretación de esos componentes. Por ejemplo, RGB es un espacio de color con tres componentes: rojo, verde y azul. El tipo de espacio de color no precisa las características de color del espacio (por ejemplo, la cromaticidad de los colores primarios).

**Tipo** de PCSEste tipo de PCS es el espacio de color de &quot;salida&quot; del perfil, es decir, su espacio de conexión de perfil. Por ejemplo, un perfil de color puede convertir RGB al PCS, el cual lo convierte en CMYK.

Para obtener un perfil de entrada, presentación y salida útil para el etiquetado de colores e imágenes, el tipo de PCS debe ser XYZ o Lab. Este perfil sería el espacio de color específico correspondiente que se define en la especificación de ICC.
