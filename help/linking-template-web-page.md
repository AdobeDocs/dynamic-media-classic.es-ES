---
title: Vinculación de una plantilla a una página web
seo-title: Vinculación de una plantilla a una página web
description: nulo
seo-description: Descubra cómo vincular una plantilla a una página web.
uuid: f 111 ef 06-4 afc -454 c -86 ce -5 d 640236 d 40 b
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template_ basics
discoiquuid: 989 dba 07-448 a -45 b 1-b 157-af 50 abb 5359 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Vinculación de una plantilla a una página web{#linking-a-template-to-a-web-page}

Los sitios web y las aplicaciones acceden al contenido del servidor de imágenes de Dynamic Media a través de cadenas URL. Después de publicar una plantilla, Dynamic Media Classic activa una cadena URL que hace referencia a la plantilla en los servidores de imágenes de Dynamic Media. Puede pegar esta URL en un explorador web para probar su funcionamiento.

Para colocar cadenas URL en las páginas web y aplicaciones, se deben copiar de Scene7 Publishing System. Para obtener una URL de plantilla generada con un ajuste preestablecido de imagen, abra la pantalla Vista previa o el panel Examinar (en vista de detalles). A continuación, seleccione un ajuste preestablecido de imagen y seleccione el botón Copiar URL.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Obtención de una URL de plantilla {#obtaining-a-template-url}

Puede obtener una cadena URL de plantilla generada por un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla. Una vez copiada la URL, ésta queda disponible en el portapapeles para que pueda pegarla cuando lo necesite. Siga estos pasos para obtener una cadena URL de plantilla generada con un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla:

1. Haga clic en el botón de rollover de vista previa de la plantilla o elija Archivo &gt; Vista previa. Se abre la pantalla Vista previa.
1. En los menús de Ajuste preestablecido, elija el Ajuste preestablecido de imagen que desee aplicar para enviar la imagen de plantilla. La pantalla Vista previa muestra el aspecto que tendrá la plantilla procedente del servidor.
1. Haga clic en el botón Copiar URL para copiar la URL en el portapapeles.

## Adición de direcciones URL de plantilla a la página web {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. El motor comercial o el código de página web dinámico inserta la imagen de plantilla con el tamaño y el formato definidos por el ajuste preestablecido elegido para la plantilla.

>[!MORELIKETHIS]
>
>* [Adición de imágenes dinámicas a la página web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

