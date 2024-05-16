---
title: Vinculación de una plantilla a una página web
description: Obtenga información sobre cómo vincular una plantilla a una página web en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 17%

---

# Vinculación de una plantilla a una página web{#linking-a-template-to-a-web-page}

Sus sitios web y aplicaciones acceden al contenido de Dynamic Media Image Server mediante cadenas URL. Después de publicar una plantilla, Adobe Dynamic Media Classic activa una cadena URL que hace referencia a la plantilla en los servidores de imágenes de Dynamic Media. Puede pegar esta dirección URL en un explorador web para probarla.

Para colocar cadenas de URL en las páginas web y aplicaciones, cópielas desde Adobe Dynamic Media Classic. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen, vaya a la pantalla Vista previa o al panel Examinar (en la Vista de detalles). A continuación, seleccione un ajuste preestablecido de imagen y seleccione el botón Copiar URL.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Obtención de una URL de plantilla {#obtaining-a-template-url}

Puede obtener una cadena URL de plantilla generada por un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla. Una vez copiada la URL, ésta queda disponible en el portapapeles para que pueda pegarla cuando lo necesite. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen desde la página Vista previa de plantilla, haga lo siguiente:

1. Seleccione la sustitución de la plantilla **[!UICONTROL Previsualizar]** o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Previsualizar]**.
1. En los menús del ajuste preestablecido, seleccione el ajuste preestablecido de imagen con el que desea enviar la imagen de plantilla. La página Vista previa muestra el aspecto de la plantilla cuando se envía desde el servidor.
1. Seleccionar **[!UICONTROL Copiar URL]** para poder copiar la URL en el Portapapeles.

## Añadir URL de plantilla a la página web {#adding-template-urls-to-your-web-page}

Para agregar una plantilla a la página Web, consulte con el equipo de desarrollo de páginas Web para modificar la plantilla `<IMG>` en el código de la página web del HTML. Utilice la cadena URL de Adobe Dynamic Media Classic para realizar una solicitud a los servidores de imágenes de Dynamic Media. El motor de comercio o el código de página Web dinámica insertan la imagen de la plantilla con el tamaño y con la especificación de formato definida por el ajuste preestablecido de imagen que elija para la plantilla.

>[!MORELIKETHIS]
>
>* [Agregar imágenes dinámicas a la página Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
