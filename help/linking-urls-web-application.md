---
title: Vinculación de direcciones URL al sitio web
description: Aprenda a vincular direcciones URL a la aplicación web.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 72%

---


# Vinculación de direcciones URL al sitio web{#linking-urls-to-your-web-application}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server a través de cadenas URL. Después de publicar una imagen, Dynamic Media Classic activa una cadena URL que hace referencia al ajuste preestablecido de imagen en los servidores de imágenes de Dynamic Media. Puede probar el funcionamiento de estas cadenas URL pegándolas en un explorador web.

Para colocar estas cadenas URL en sus páginas web y aplicaciones, cópielas desde Dynamic Media Classic. Para obtener una cadena URL generada con un ajuste preestablecido de imagen, abra la pantalla Vista previa o el panel Examinar (en vista de detalles).

## Obtención de una URL de ajuste preestablecido de imagen  {#obtaining-an-image-preset-url}

Puede obtener una cadena URL generada por un ajuste preestablecido de imagen en la Vista previa o en Vista de detalles. Una vez copiada, la URL queda disponible en el portapapeles para que pueda pegarla cuando lo necesite.

***Nota **: La URL no estará activa hasta que publique el recurso.*

### Obtención de una URL de ajuste preestablecido de imagen desde Vista previa {#obtaining-an-image-preset-url-from-preview}

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a las carpetas de recursos que contienen el recurso de imagen cuya vista previa desea obtener.
1. Realice una de las acciones siguientes:

   * Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de cuadrícula. En la ventana Recurso, seleccione un único recurso de imagen y, a continuación, haga clic en Vista previa > Lista de ajustes preestablecidos de imagen debajo de la imagen en miniatura.
   * Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de lista. En la ventana Recurso, seleccione un único recurso de imagen y, a continuación, haga clic en Vista previa > Lista de ajustes preestablecidos de imagen a la derecha de la imagen en miniatura.
   * Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de detalles. En la misma barra de herramientas, haga clic en Vista previa > Lista de ajustes preestablecidos de imagen.

1. (Opcional) En la ventana Lista de ajustes preestablecidos de imagen, en la lista desplegable inferior Codificación URL para la creación de copias URL, seleccione la codificación de URL que desee aplicar a la dirección URL del recurso de imagen cuando se copie.
1. En la ventana Lista de ajustes preestablecidos de imagen, en la parte superior derecha del panel de vista previa, haga clic en Copiar URL para el tipo de ajuste preestablecido seleccionado.
1. En la esquina inferior derecha de la ventana Lista de ajustes preestablecidos de imagen, haga clic en Cerrar para volver a la pantalla Recurso.

### Obtención de una URL de ajustes preestablecidos de imagen desde el panel Examinar  {#obtaining-an-image-preset-url-from-the-browse-panel}

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a las carpetas de recursos que contienen el recurso de imagen cuya vista previa desea obtener.
1. Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de cuadrícula. En la ventana Recurso, seleccione un único recurso de imagen.
1. Por encima de la ventana Recursos, en la parte derecha de la barra de herramientas, haga clic en Vista de detalles. 
1. Haga clic en Direcciones URL en el panel de la derecha para desplegar la lista de ajustes preestablecidos de imagen.
1. Haga clic en el vínculo Copiar URL junto al nombre del ajuste preestablecido cuya URL quiera copiar en el portapapeles.

## Acerca de las cadenas URL de ajustes preestablecidos de imagen  {#about-image-preset-url-strings}

Una llamada de URL para cambiar el tamaño de la imagen a los servidores de imágenes de Dynamic Media tiene la siguiente sintaxis básica:

*ruta*/*nombre de servidor de imágenes*/*nombre de cuenta*/*nombre de imagen*?*modificador1*&amp;*modificador2*&amp;...

En una URL del servidor de imágenes de Dynamic Media, las instrucciones para mostrar la imagen aparecen después del signo de interrogación (?). Por ejemplo, esta llamada mediante URL envía una imagen denominada “backpack” con una anchura de 250 píxeles:

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

Los nombres de ajuste preestablecido de imagen en direcciones URL se incluyen entre signos de dólar ($). Cuando un servidor de imágenes de Dynamic Media encuentra la parte de ajuste preestablecido de imagen de la URL (el `Large` en este caso), utilizando las instrucciones de tamaño y formato definidas por el ajuste preestablecido de imagen &quot;Grande&quot;.

## Adición de imágenes dinámicas a la página web {#adding-dynamic-images-to-your-web-page}

Para añadir imágenes dinámicas a la página web, la etiqueta `<IMG>` del código de la página web HTML se suele modificar utilizando la cadena URL de Dynamic Media Classic para realizar una solicitud a los servidores de imágenes de Dynamic Media. Esta cadena produce una imagen con las especificaciones de formato y tamaño definidas por el ajuste preestablecido de imagen.

Por ejemplo, en lugar de la típica llamada para abrir una imagen estática:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

ahora utilice la etiqueta `<IMG>`para reemplazar la referencia a una imagen estática por una llamada de ajuste preestablecido de imagen a la plataforma de Dynamic Media Classic. Ejemplo de llamada:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

En este ejemplo, Dynamic Media Image Server &quot;busca&quot; la definición de `$thumbnail$` y genera dinámicamente la imagen adecuada con las especificaciones de tamaño y formato definidas por el `thumbnail`Ajuste preestablecido de imagen. En una cadena URL, todos los elementos a excepción del nombre de archivo de imagen de producto (`backpack_trns` en este caso) suelen estar fijados para la plantilla de página. El único elemento que se inserta automáticamente en la plantilla desde el servidor comercial es el ID de IPS o nombre de la imagen.
