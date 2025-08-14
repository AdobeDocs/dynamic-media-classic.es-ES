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
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 17%

---

# Vinculación de una plantilla a una página web{#linking-a-template-to-a-web-page}

Sus sitios web y aplicaciones acceden al contenido del servidor de imágenes de Dynamic Media mediante cadenas URL. Después de publicar una plantilla, Adobe Dynamic Media Classic activa una cadena URL que hace referencia a la plantilla en los servidores de imágenes de Dynamic Media. Puede pegar esta dirección URL en un explorador web para probarla.

Para colocar cadenas de URL en las páginas web y aplicaciones, cópielas desde Adobe Dynamic Media Classic. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen, vaya a la pantalla Vista previa o al panel Examinar (en la Vista de detalles). A continuación, seleccione un ajuste preestablecido de imagen y seleccione el botón Copiar URL.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Obtención de una URL de plantilla {#obtaining-a-template-url}

Puede obtener una cadena URL de plantilla generada por un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla. Una vez copiada la URL, ésta queda disponible en el portapapeles para que pueda pegarla cuando lo necesite. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen desde la página Vista previa de plantilla, haga lo siguiente:

1. Seleccione el botón de rollover **[!UICONTROL Vista previa]** de la plantilla o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Vista previa]**.
1. En los menús del ajuste preestablecido, seleccione el ajuste preestablecido de imagen con el que desea enviar la imagen de plantilla. La página Vista previa muestra el aspecto de la plantilla cuando se envía desde el servidor.
1. Seleccione **[!UICONTROL Copiar URL]** para poder copiar la URL en el Portapapeles.

## Añadir URL de plantilla a la página web {#adding-template-urls-to-your-web-page}

Para agregar una plantilla a su página web, consulte con el equipo de desarrollo de páginas web para modificar la etiqueta `<IMG>` en el código de la página web de HTML. Utilice la cadena URL de Adobe Dynamic Media Classic para realizar una solicitud a los servidores de imágenes de Dynamic Media. El motor de comercio o el código de página Web dinámica insertan la imagen de la plantilla con el tamaño y con la especificación de formato definida por el ajuste preestablecido de imagen que elija para la plantilla.

>[!MORELIKETHIS]
>
>* [Agregar imágenes dinámicas a su página web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
