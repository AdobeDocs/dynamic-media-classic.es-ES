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
autotag-review: '2026-05-13T19:59:42.608Z'
TQID: 'https://experienceleague.adobe.com/eGKamqA47mITzfyTuHoFYLfWEXOP0jAl5XWDpihGjZA'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 528
ht-degree: 31%

---

# Perfiles ICC{#icc-profiles}

Un perfil ICC (International Color Consortium) es un archivo que describe cómo convertir correctamente archivos de imagen de un espacio de color a otro. Los perfiles ICC le ayudan a obtener los colores correctos para las imágenes. Por ejemplo, para mostrar correctamente imágenes diseñadas para imprimirse en un monitor de equipo, puede elegir un perfil ICC. Este perfil convierte el espacio de color de la imagen y garantiza que los colores se muestren correctamente en línea.

En Adobe Dynamic Media Classic, puede elegir un perfil ICC para convertir las imágenes a un espacio de color diferente al cargarlas. Todos los perfiles ICC estándar de Photoshop están disponibles de forma predeterminada en Adobe Dynamic Media Classic. Para ver los nombres de los perfiles de color en la pantalla de carga, seleccione el menú Perfil de color. A continuación elija Personalizar De > A y elija un perfil ICC en los menús Convertir de y Convertir a.

Ver [Opciones de edición de imágenes al cargar](image-editing-options-upload.md#image-editing-options-at-upload).

Además de utilizar los perfiles ICC predeterminados, puede cargar otros perfiles ICC en Adobe Dynamic Media Classic y ponerlos a disposición de la conversión del espacio de color. Cambie a Vista de detalles en el panel de exploración para investigar la clase de perfil, el tipo de espacio de color y el tipo PCS de un perfil ICC.

En resumen, los puntos clave para los perfiles ICC son los siguientes:

* Los perfiles ICC permiten una correcta conversión de color entre los diferentes espacios de color para los archivos de imagen.
* Adobe Dynamic Media Classic incorpora todos los perfiles ICC estándar de Photoshop para lograr conversiones de imagen sólidas.
* Los perfiles ICC personalizados añaden flexibilidad para satisfacer las necesidades avanzadas de conversión de espacio de color.
* Ver detalles como Clase de perfil y Tipo de PCS en la Vista de detalles le ayuda a gestionar la configuración de ICC.
* La carga de perfiles ICC es sencilla y garantiza el acceso a todas las carpetas en Dynamic Media Classic.


## Carga de perfiles ICC {#uploading-icc-profiles}

Cargue perfiles ICC utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar perfiles ICC en cualquier carpeta de Adobe Dynamic Media Classic.

Ver [Cargar los archivos](uploading-files.md#uploading_your_files).

## Examen de un perfil ICC {#examining-an-icc-profile}

Para examinar un perfil ICC, selecciónelo en el panel Examinar y muéstrelo en la Vista de detalles. La Vista de detalles proporciona esta información sobre los perfiles ICC:

* **[!UICONTROL Clase de perfil]**: el ICC define cada clase para cubrir un tipo de aplicación. Por ejemplo, los perfiles de entrada se aplican a dispositivos como cámaras digitales y escáneres. Los perfiles de salida se aplican a las impresoras.

* **[!UICONTROL Tipo de espacio de color]**: este número es el espacio de color de &quot;entrada&quot; del perfil, tal como lo define el ICC. El tipo de espacio de color especifica el número de componentes del espacio de color y la interpretación de esos componentes. Por ejemplo, RGB es un espacio de color con tres componentes: rojo, verde y azul. El tipo de espacio de color no precisa las características de color del espacio (por ejemplo, la cromaticidad de los colores primarios).

* **[!UICONTROL Tipo PCS]**: Este tipo PCS es el espacio de color de &quot;salida&quot; del perfil (su espacio de conexión de perfil). Por ejemplo, un perfil de color puede convertir RGB al PCS, el cual lo convierte en CMYK.

Para un perfil de entrada, visualización o salida útil para etiquetar colores o imágenes, el tipo de PCS es XYZ o Lab. Este perfil sería el espacio de color específico correspondiente que se define en la especificación de ICC.
