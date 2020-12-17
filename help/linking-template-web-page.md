---
title: Vinculación de una plantilla a una página web
seo-title: Vinculación de una plantilla a una página web
description: nulo
seo-description: Obtenga información sobre cómo vincular una plantilla a una página web.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 70%

---


# Vinculación de una plantilla a una página web{#linking-a-template-to-a-web-page}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server a través de cadenas URL. Después de publicar una plantilla, Dynamic Media Classic activa una cadena URL que hace referencia a la plantilla en los servidores de imágenes de Dynamic Media. Puede pegar esta URL en un explorador web para probar su funcionamiento.

Para colocar cadenas URL en las páginas web y las aplicaciones, cópielas desde Dynamic Media Classic. Para obtener una URL de plantilla generada con un ajuste preestablecido de imagen, abra la pantalla Vista previa o el panel Examinar (en vista de detalles). A continuación, seleccione un ajuste preestablecido de imagen y seleccione el botón Copiar URL.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Obtención de una URL de plantilla  {#obtaining-a-template-url}

Puede obtener una cadena URL de plantilla generada por un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla. Una vez copiada la URL, ésta queda disponible en el portapapeles para que pueda pegarla cuando lo necesite. Siga estos pasos para obtener una cadena URL de plantilla generada con un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla:

1. Haga clic en el botón de rollover de vista previa de la plantilla o elija Archivo > Vista previa. Se abre la pantalla Vista previa.
1. En los menús de Ajuste preestablecido, elija el Ajuste preestablecido de imagen que desee aplicar para enviar la imagen de plantilla. La pantalla Vista previa muestra el aspecto que tendrá la plantilla procedente del servidor.
1. Haga clic en el botón Copiar URL para copiar la URL en el portapapeles.

## Adición de direcciones URL de plantilla a la página web  {#adding-template-urls-to-your-web-page}

Para agregar una plantilla a la página web, consulte con el equipo de desarrollo de la página web para modificar la etiqueta `<IMG>` en el código de la página web HTML mediante la cadena URL de Dynamic Media Classic para realizar una solicitud a los servidores de imágenes de Dynamic Media. El motor comercial o el código de página web dinámico inserta la imagen de plantilla con el tamaño y el formato definidos por el ajuste preestablecido elegido para la plantilla.

>[!MORELIKETHIS]
>
>* [Adición de imágenes dinámicas a la página web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

