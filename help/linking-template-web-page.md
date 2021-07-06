---
title: Vinculación de una plantilla a una página web
description: Aprenda a vincular una plantilla a una página web.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 50%

---

# Vinculación de una plantilla a una página web{#linking-a-template-to-a-web-page}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server mediante cadenas URL. Después de publicar una plantilla, Dynamic Media Classic activa una cadena URL que hace referencia a la plantilla en los servidores de imágenes de Dynamic Media. Puede pegar esta URL en un explorador web para probar su funcionamiento.

Para colocar cadenas URL en sus páginas web y aplicaciones, cópielas desde Dynamic Media Classic. Para obtener una URL de plantilla generada con un ajuste preestablecido de imagen, abra la pantalla Vista previa o el panel Examinar (en vista de detalles). A continuación, seleccione un ajuste preestablecido de imagen y seleccione el botón Copiar URL.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Obtención de una URL de plantilla {#obtaining-a-template-url}

Puede obtener una cadena URL de plantilla generada por un ajuste preestablecido de imagen en la pantalla Vista previa de plantilla. Una vez copiada la URL, ésta queda disponible en el portapapeles para que pueda pegarla cuando lo necesite. Para obtener una cadena URL de plantilla generada con un ajuste preestablecido de imagen desde la página Vista previa de plantilla, haga lo siguiente:

1. Haga clic en el botón **[!UICONTROL Preview]** de sustitución de la plantilla o seleccione **[!UICONTROL File]** > **[!UICONTROL Preview]**.
1. En los menús de Ajuste preestablecido, elija el Ajuste preestablecido de imagen que desee aplicar para enviar la imagen de plantilla. La página Vista previa muestra el aspecto de la plantilla cuando se envía desde el servidor.
1. Haga clic en **[!UICONTROL Copiar URL]** para copiar la URL en el portapapeles.

## Adición de direcciones URL de plantilla a la página web {#adding-template-urls-to-your-web-page}

Para agregar una plantilla a la página web, consulte con el equipo de desarrollo de la página web para modificar la etiqueta `<IMG>` en el código de la página web HTML. Utilice la cadena URL de Dynamic Media Classic para realizar una solicitud a los servidores de imágenes de Dynamic Media. El motor comercial o el código de página web dinámico inserta la imagen de plantilla con el tamaño y el formato definidos por el ajuste preestablecido elegido para la plantilla.

>[!MORELIKETHIS]
>
>* [Adición de imágenes dinámicas a la página web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

