---
title: Vinculación de una plantilla a una página web
description: Obtenga información sobre cómo vincular una plantilla a una página web en Adobe Dynamic Media Classic.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 40%

---

# Vinculación de una plantilla a una página web{#linking-a-template-to-a-web-page}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server mediante cadenas URL. Después de publicar una plantilla, Adobe Dynamic Media Classic activa una cadena URL que hace referencia a la plantilla en los servidores de imágenes de Dynamic Media. Puede pegar esta URL en un explorador web para probar su funcionamiento.

Para colocar cadenas de URL en las páginas web y aplicaciones, cópielas desde Adobe Dynamic Media Classic. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen, vaya a la pantalla Vista previa o al panel Examinar (en la Vista de detalles). A continuación, seleccione un ajuste preestablecido de imagen y seleccione el botón Copiar URL.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Obtención de una URL de plantilla {#obtaining-a-template-url}

Puede obtener una cadena URL de plantilla generada por un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla. Una vez copiada la URL, ésta queda disponible en el portapapeles para que pueda pegarla cuando lo necesite. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen desde la página Vista previa de plantilla, haga lo siguiente:

1. Seleccione la sustitución de la plantilla **[!UICONTROL Previsualizar]** o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Previsualizar]**.
1. En los menús de Ajuste preestablecido, elija el Ajuste preestablecido de imagen que desee aplicar para enviar la imagen de plantilla. La página Vista previa muestra el aspecto de la plantilla cuando se envía desde el servidor.
1. Seleccionar **[!UICONTROL Copiar URL]** para poder copiar la URL en el Portapapeles.

## Agregación de direcciones URL de plantilla  a la página Web {#adding-template-urls-to-your-web-page}

Para añadir una plantilla a la página web, consulte con el equipo de desarrollo de la página web para modificar `<IMG>` en el código de la página web del HTML. Utilice la cadena URL de Adobe Dynamic Media Classic para realizar una solicitud a los servidores de imágenes de Dynamic Media. El motor comercial o el código de página web dinámico inserta la imagen de plantilla con el tamaño y el formato definidos por el ajuste preestablecido elegido para la plantilla.

>[!MORELIKETHIS]
>
>* [Añadir imágenes dinámicas a la página web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
