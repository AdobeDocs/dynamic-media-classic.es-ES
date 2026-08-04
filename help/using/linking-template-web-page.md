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
autotag-review: '2026-05-13T19:52:27.080Z'
TQID: 'https://experienceleague.adobe.com/c1Un6UFrYZh-tqwPp98shMiTUEEMhkEn1vmxEl2rVq0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f55e82148ae9d11c54dda28351743b02c1fb58a4
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 12%

---

# Vinculación de una plantilla a una página web{#linking-a-template-to-a-web-page}

Sus sitios web y aplicaciones acceden al contenido de Dynamic Media Image Server mediante cadenas de URL. Después de publicar una plantilla, Adobe Dynamic Media Classic activa una cadena URL que hace referencia a la plantilla en los servidores de imágenes de Dynamic Media. Puede pegar esta dirección URL en un explorador web para probarla.

Para colocar cadenas de URL en las páginas web y aplicaciones, cópielas desde Adobe Dynamic Media Classic. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen, vaya a la pantalla Vista previa o al panel Examinar (en la Vista de detalles). A continuación, seleccione un ajuste preestablecido de imagen y seleccione el botón Copiar URL.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Obtención de una URL de plantilla {#obtaining-a-template-url}

Puede obtener una cadena URL de plantilla generada por un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla. Después de copiar la dirección URL, se guarda en el Portapapeles para poder pegarla según sea necesario. Para obtener una cadena de URL de plantilla generada con un ajuste preestablecido de imagen desde la página Vista previa de plantilla, haga lo siguiente:

1. Seleccione el botón **[!UICONTROL Vista previa]** de la plantilla o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Vista previa]**.
1. En los menús del ajuste preestablecido, seleccione el ajuste preestablecido de imagen con el que desea enviar la plantilla. La página Vista previa muestra la plantilla tal como se envía desde el servidor.
1. Seleccione **[!UICONTROL Copiar URL]** para poder copiar la URL en el Portapapeles.

## Añadir URL de plantilla a la página web {#adding-template-urls-to-your-web-page}

Para agregar una plantilla a su página web, consulte con el equipo de desarrollo de páginas web para modificar la etiqueta `<IMG>` en el código de la página web de HTML. Utilice la cadena URL de Adobe Dynamic Media Classic para enviar una solicitud a los servidores de imágenes de Dynamic Media. El motor de comercio o el código de página web dinámica insertan la imagen de plantilla con el tamaño y con las especificaciones de formato definidas por el ajuste preestablecido de imagen que haya elegido para la plantilla.

>[!MORELIKETHIS]
>
>* [Agregar imágenes dinámicas a su página web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
