---
title: Vinculación de direcciones URL al sitio web
seo-title: Vinculación de direcciones URL al sitio web
description: nulo
seo-description: Descubra cómo vincular URL a la aplicación web.
uuid: 1179 bdd 3-9 b 39-47 f 9-945 d -1 c 1 ca 186 bf 96
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: 71299640-676 d -49 b 7-841 d -6118 f 31044 e 8
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Vinculación de direcciones URL al sitio web{#linking-urls-to-your-web-application}

Los sitios web y las aplicaciones acceden al contenido del servidor de imágenes de Dynamic Media a través de cadenas URL. Después de publicar una imagen, Dynamic Media Classic activa una cadena URL que hace referencia al ajuste preestablecido de imagen en los servidores de imágenes de Dynamic Media. Puede probar el funcionamiento de estas cadenas URL pegándolas en un explorador web.

Para colocar estas cadenas URL en las páginas web y aplicaciones, se deben copiar de Scene7 Publishing System. Para obtener una cadena URL generada con un ajuste preestablecido de imagen, abra la pantalla Vista previa o el panel Examinar (en vista de detalles).

## Obtención de una URL de ajuste preestablecido de imagen {#obtaining-an-image-preset-url}

Puede obtener una cadena URL generada por un ajuste preestablecido de imagen en la Vista previa o en Vista de detalles. Una vez copiada, la URL queda disponible en el portapapeles para que pueda pegarla cuando lo necesite.

***Nota**: La URL no se activa hasta que publique el recurso.*

### Obtención de una URL de ajuste preestablecido de imagen desde Vista previa {#obtaining-an-image-preset-url-from-preview}

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a las carpetas de recursos que contienen el recurso de imagen cuya vista previa desea obtener.
1. Realice una de las acciones siguientes:

   * Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de cuadrícula. En la ventana Recurso, seleccione un único recurso de imagen y, a continuación, haga clic en Vista previa &gt; Lista de ajustes preestablecidos de imagen debajo de la imagen en miniatura.
   * Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de lista. En la ventana Recurso, seleccione un único recurso de imagen y, a continuación, haga clic en Vista previa &gt; Lista de ajustes preestablecidos de imagen a la derecha de la imagen en miniatura.
   * Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de detalles. En la misma barra de herramientas, haga clic en Vista previa &gt; Lista de ajustes preestablecidos de imagen.

1. (Opcional) En la ventana Lista de ajustes preestablecidos de imagen, en la lista desplegable inferior Codificación URL para la creación de copias URL, seleccione la codificación de URL que desee aplicar a la dirección URL del recurso de imagen cuando se copie.
1. En la ventana Lista de ajustes preestablecidos de imagen, en la parte superior derecha del panel de vista previa, haga clic en Copiar URL para el tipo de ajuste preestablecido seleccionado.
1. En la esquina inferior derecha de la ventana Lista de ajustes preestablecidos de imagen, haga clic en Cerrar para volver a la pantalla Recurso.

### Obtención de una URL de ajustes preestablecidos de imagen desde el panel Examinar {#obtaining-an-image-preset-url-from-the-browse-panel}

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a las carpetas de recursos que contienen el recurso de imagen cuya vista previa desea obtener.
1. Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de cuadrícula. En la ventana Recurso, seleccione un único recurso de imagen.
1. Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de detalles. 
1. Haga clic en Direcciones URL en el panel de la derecha para desplegar la lista de ajustes preestablecidos de imagen.
1. Haga clic en el vínculo Copiar URL junto al nombre del ajuste preestablecido cuya URL quiera copiar en el portapapeles.

## Acerca de las cadenas URL de ajustes preestablecidos de imagen {#about-image-preset-url-strings}

Una llamada mediante URL para cambiar el tamaño de imagen a los servidores de imágenes de Dynamic Media tiene la siguiente sintaxis básica:

*ruta*/*nombre de servidor de imágenes*/*nombre de cuenta*/*nombre de imagen*?*modificador1*&amp;*modificador2*&amp;...

En una URL del servidor de imágenes de Dynamic Media, las instrucciones para que el servidor muestre la imagen aparecen después del signo de interrogación (?). Por ejemplo, esta llamada mediante URL envía una imagen denominada “backpack” con una anchura de 250 píxeles:

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

Los nombres de ajuste preestablecido de imagen en direcciones URL se incluyen entre signos de dólar ($). When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## Adición de imágenes dinámicas a la página web {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. Esta cadena produce una imagen con las especificaciones de formato y tamaño definidas por el ajuste preestablecido de imagen.

Por ejemplo, en lugar de la típica llamada para abrir una imagen estática:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

you now use the `<IMG>`tag to replace the reference to a static image with an Image Preset call to the Dynamic Media Classic platform. Ejemplo de llamada:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. En una cadena URL, todos los elementos a excepción del nombre de archivo de imagen de producto (`backpack_trns` en este caso) suelen estar fijados para la plantilla de página. El único elemento que se inserta automáticamente en la plantilla desde el servidor comercial es el ID de IPS o nombre de la imagen.
