---
title: Perfiles ICC
seo-title: Perfiles ICC
description: nulo
seo-description: Obtenga información sobre perfiles ICC.
uuid: 708 ff 2 ad -9 a 47-4 e 3 e-b 643-5 b 19648 f 726 b
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 44 f 1 b 4 c 4-6 d 7 f -4 e 0 f -84 ce -11 d 26745 e 0 f 0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Perfiles ICC{#icc-profiles}

Un perfil ICC (International Color Consortium) es un archivo que describe cómo se deben convertir los archivos de imagen de un espacio de color a otro. Los perfiles ICC le ayudan a obtener los colores correctos para las imágenes. Por ejemplo, para mostrar correctamente imágenes diseñadas para la impresión en un monitor de ordenador, puede elegir un perfil ICC. Este perfil convierte el espacio de color de la imagen y garantiza que los colores se muestren correctamente en línea.

En Scene7 Publishing System, puede elegir un perfil ICC para convertir las imágenes a un espacio de color diferente al cargarlas. Todos los perfiles ICC estándar de Photoshop están disponibles de forma predeterminada en SPS. Para ver los nombres de los perfiles de color en la pantalla de carga, seleccione el menú Perfil de color. A continuación elija Personalizar De &gt; A y elija un perfil ICC en los menús Convertir de y Convertir a. Consulte [Opciones de edición de imágenes al cargarlas](image-editing-options-upload.md#image-editing-options-at-upload).

No solo puede utilizar los perfiles ICC predeterminados, también puede cargar otros perfiles ICC a SPS y hacer que estén disponibles para la conversión de espacios de color. Cambie a la vista de detalles en el panel Examinar para investigar la clase de perfil, el tipo de espacio de color y el tipo de PCS de un perfil ICC.

## Carga de perfiles ICC {#uploading-icc-profiles}

Cargue perfiles ICC utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar perfiles ICC en cualquier carpeta de SPS. Consulte [Carga de los archivos](uploading-files.md#uploading_your_files).

## Examen de un perfil ICC {#examining-an-icc-profile}

Para examinar un perfil ICC, selecciónelo en el panel Examinar y acceda a la vista de detalles. La vista de detalles le ofrece esta información sobre los perfiles ICC:

**Clase de perfil** El ICC (International Color Consortium) define cada clase para que ocupe un tipo de aplicación. Por ejemplo, los perfiles de entrada se aplican a los dispositivos como las cámaras digitales o los escáneres, mientras que los perfiles de salida se aplican a las impresoras.

**Tipo de espacio de color** Este número es el espacio de color "input" del perfil, tal como define el ICC. El tipo de espacio de color especifica el número de componentes del espacio de color y la interpretación de esos componentes. Por ejemplo, RGB es un espacio de color con tres componentes: rojo, verde y azul. El tipo de espacio de color no precisa las características de color del espacio (por ejemplo, la cromaticidad de los colores primarios).

**Tipo de PCS** Tipo Este tipo de PCS es el espacio de color "output" del perfil, su espacio de conexión de perfil. Por ejemplo, un perfil de color puede convertir RGB al PCS, el cual lo convierte en CMYK.

Para obtener un perfil de entrada, presentación y salida útil para el etiquetado de colores e imágenes, el tipo de PCS debe ser XYZ o Lab. Este perfil sería el espacio de color específico correspondiente que se define en la especificación de ICC.
