---
title: Vinculación de URL en la aplicación web
description: Obtenga información sobre cómo vincular direcciones URL a su aplicación web desde Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 26%

---

# Vinculación de URL en la aplicación web{#linking-urls-to-your-web-application}

Sus sitios web y aplicaciones acceden al contenido de Dynamic Media Image Server mediante cadenas URL. Después de publicar una imagen, Adobe Dynamic Media Classic activa una cadena URL que hace referencia al ajuste preestablecido de imagen en los servidores de imágenes de Dynamic Media. Puede pegar estas direcciones URL en un explorador web para probarlas.

Para colocar estas cadenas de URL en las páginas web y aplicaciones, cópielas desde Adobe Dynamic Media Classic. Para obtener una cadena URL generada con un ajuste preestablecido de imagen, vaya a la pantalla Vista previa o al panel Examinar (en la Vista de detalles).

## Obtener una URL de ajuste preestablecido de imagen {#obtaining-an-image-preset-url}

Puede obtener una cadena URL generada por un ajuste preestablecido de imagen en la Vista previa o en Vista de detalles. Una vez copiada, la URL queda disponible en el portapapeles para que pueda pegarla cuando lo necesite.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

### Obtener una URL de ajuste preestablecido de imagen de la vista previa {#obtaining-an-image-preset-url-from-preview}

1. En el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el recurso de imagen que desea previsualizar.
1. Realice una de las acciones siguientes:

   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de cuadrícula]**. En la ventana Recurso, seleccione un único recurso de imagen y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista de ajustes preestablecidos de imagen]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de lista]**. En la ventana Recurso, seleccione un único recurso de imagen y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista de ajustes preestablecidos de imagen]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista de ajustes preestablecidos de imagen]**.

1. (Opcional) En la Lista de ajustes preestablecidos de imagen, en la lista desplegable Codificación URL para la creación de copias URL, seleccione la Codificación URL que se aplicará a la URL del recurso de imagen cuando se copie.
1. En la ventana Lista de ajustes preestablecidos de imagen, en el área superior derecha del panel de vista previa, seleccione **[!UICONTROL Copiar URL]** para el tipo de ajuste preestablecido seleccionado.
1. En la esquina inferior derecha de la ventana Lista de ajustes preestablecidos de imagen, seleccione **[!UICONTROL Cerrar]** para volver a la pantalla Recursos.

### Obtenga una URL de ajuste preestablecido de imagen del panel Examinar {#obtaining-an-image-preset-url-from-the-browse-panel}

1. En el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el recurso de imagen que desea previsualizar.
1. Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de cuadrícula]**. En la ventana Recurso, seleccione un único recurso de imagen.
1. Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de detalles]**.
1. Seleccionar **[!UICONTROL URL]** en el panel situado en la parte derecha de la pantalla para poder desplegar la lista de ajustes preestablecidos de imagen.
1. Seleccionar **[!UICONTROL Copiar URL]** junto al nombre del ajuste preestablecido de imagen con la dirección URL que desea copiar en el portapapeles.

## Acerca de las cadenas URL de ajustes preestablecidos de imagen {#about-image-preset-url-strings}

Una llamada URL para el ajuste de tamaño de imagen en servidores de imágenes de Dynamic Media tiene la siguiente sintaxis básica:

*ruta*/*nombre de servidor de imágenes*/*nombre de cuenta*/*nombre de imagen*?*modificador1*&amp;*modificador2*&amp;...

En la URL de un servidor de imágenes de Dynamic Media, las instrucciones para mostrar la imagen al servidor aparecen después del signo de interrogación (?). Por ejemplo, esta llamada URL ofrece una imagen denominada &quot;mochila&quot; con una anchura de 250 píxeles:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Una URL de ajuste preestablecido de imagen contiene todas las instrucciones de modificador para presentar la imagen con las especificaciones de formato y tamaño correctas. Si no hay un ajuste preestablecido de imagen, observará que todas las instrucciones de modificador aparecen tras el signo de interrogación (?) en esta cadena URL:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

Pero en una cadena URL generada con un ajuste preestablecido de imagen, el nombre del ajuste aparece en lugar de las instrucciones definidas por el ajuste preestablecido. Por ejemplo, para la URL larga ilustrada arriba, la cadena URL es:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Los nombres de ajuste preestablecido de imagen en direcciones URL se incluyen entre signos de dólar ($). Cuando un servidor de imágenes de Dynamic Media encuentra la parte de ajuste preestablecido de imagen de la URL (la variable `Large` en este caso), utilizando las instrucciones de tamaño y formato definidas por el ajuste preestablecido de imagen &quot;Grande&quot;.

## Agregar imágenes dinámicas a la página Web {#adding-dynamic-images-to-your-web-page}

Al agregar imágenes dinámicas a la página web, se `<IMG>` El código de la página del HTML suele modificarse con la cadena URL de Adobe Dynamic Media Classic para realizar una solicitud a los servidores de imágenes de Dynamic Media. Esta cadena produce una imagen con las especificaciones de formato y tamaño definidas por el ajuste preestablecido de imagen.

Por ejemplo, en lugar de la típica llamada para abrir una imagen estática:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Ahora puede usar la variable `<IMG>`para reemplazar la referencia a una imagen estática con una llamada de ajuste preestablecido de imagen a la plataforma de Adobe Dynamic Media Classic. Ejemplo de llamada:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

En este ejemplo, un servidor de imágenes de Dynamic Media busca la definición de `$thumbnail$` y genera dinámicamente la imagen adecuada con las especificaciones de tamaño y formato definidas por el `thumbnail`Ajuste preestablecido de imagen. En una cadena URL, todos los elementos excepto el nombre de archivo de la imagen del producto ( `backpack_trns` en este caso) suelen estar cableadas para la plantilla de página. El único elemento que se inserta automáticamente en la plantilla desde el servidor comercial es el ID de IPS o nombre de la imagen.
