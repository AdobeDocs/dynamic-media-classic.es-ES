---
title: Carga de recursos de imagen o recursos de vector
seo-title: Carga de recursos de imagen o recursos de vector
description: nulo
seo-description: Obtenga información sobre cómo cargar un recurso de imagen o un recurso de vector.
uuid: d0e4a754-8a49-4b0f-b202-e9003bdb8f20
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: de21dca9-99fe-4183-b647-debfe112fda4
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 84%

---


# Carga de recursos de imagen o recursos de vector{#uploading-an-image-asset-or-a-vector-asset}

Para poder cargar un recurso de imagen, primero debe solicitar una clave secreta compartida. Esta clave permite recuperar un distintivo de carga. Este distintivo de carga se emplea para cargar recursos de imagen o vector.

## Solicitud de la clave secreta compartida  {#requesting-a-shared-secret-key}

Solicite una *clave secreta compartida* [mediante el Admin Console para crear un caso de soporte.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) En el caso de soporte, solicite una clave secreta compartida.

En el mensaje, proporcione el nombre de empresa que desee utilizar para cargar los recursos de imagen. Después de recibir la clave de Dynamic Media Classic, guárdela de forma local para usarla en el futuro.

## Recuperación del distintivo de carga {#retrieving-the-upload-token}

El *distintivo de carga* garantiza que nadie más use la misma clave secreta compartida para cargar recursos. Garantiza que la carga sea legítima y que proceda de una fuente de confianza.

El distintivo de carga es una cadena alfanumérica que solo se encuentra disponible durante un tiempo concreto. Use las siguientes URL (sustituyendo la clave secreta compartida por la suya) para recuperar el distintivo de carga.

* Imagen
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`En este ejemplo, la clave secreta compartida es  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vector
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`En este ejemplo, la clave secreta compartida es  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

De manera predeterminada, el distintivo de carga caduca en 5 minutos (300 segundos) después de recuperarlo. Si desea solicitar más tiempo, incluya en la URL `expires` seguido de la cantidad de tiempo necesaria en segundos. Por ejemplo, esta URL de imagen de ejemplo recupera un distintivo de carga válido durante 1.800 segundos:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

Éste es un ejemplo de respuesta correcta para imágenes:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Guarde el distintivo de carga en el equipo local para utilizarlo en las futuras solicitudes.

Se pueden usar los campos siguientes en la cadena de consulta URL para recuperar un distintivo de carga:

| Parámetro de URL | Obligatorio u opcional | Valor |
|--- |--- |--- |
| op | Obligatorio | get_uploadtoken |
| shared_secret | Obligatorio | Clave secreta compartida de la empresa que realiza la carga. |
| expires | Opcional | Número de segundos durante los que es válido el distintivo de carga. Si no se especifica, el valor predeterminado es 300 segundos. |

**URL de imagen de muestra:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**URL de vector de prueba:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Métodos HTTP permitidos:** GET y POST

Ya puede cargar un recurso de imagen.

Consulte [Carga de recursos de imagen](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Carga de recursos de imagen  {#uploading-an-image-asset}

Después de recuperar un distintivo de carga válido durante un tiempo determinado, ya se puede cargar un recurso de imagen. El recurso se carga como una publicación de varias partes o formularios mientras que el resto de los valores se envía en forma de cadena de consulta URL, tal como se muestra en este ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Los campos `upload_token` y `company_name` son obligatorios.

Consulte [Recuperación del distintivo de carga](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperación de la clave secreta compartida](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

También se pueden enviar otros valores opcionales en forma de cadenas de consulta URL, como en este ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

El parámetro `file_limit` especifica el límite de tamaño de archivo en bytes. El parámetro `file_exts` especifica las extensiones de nombre de archivo permitidas en la carga. Ambos valores son opcionales.

En la aplicación se definen límites globales tanto para el límite de tamaño de los archivos como para las extensiones de nombre de archivo permitidas. Todo lo incluido en la solicitud se acepta si es un subconjunto de los límites globales. Éstos son los límites globales:

| Límite global | Valor |
|--- |--- |
| Tamaño de archivo para todos los clientes | 20 MB |
| Formatos de archivo de imagen admitidos para la carga | BMP, GIF, JPG, PNG y PSD |

El siguiente formulario HTML permite al usuario cargar un recurso. En el formulario se pide al usuario que introduzca la información siguiente:

* Nombre de empresa.
* Distintivo de carga.
* Límite de tamaño de archivo.
* Lista de extensiones de nombre de archivo.
* Indica si se debe conservar o no el perfil de color y el nombre de archivo asociados al recurso.
* Indica si se utiliza o no el fondo de cobertura. Si activa Fondo de cobertura, defina la esquina, la tolerancia y el método de relleno. Consulte Fondo de cobertura en [Opciones de edición de imágenes al cargar](image-editing-options-upload.md#image-editing-options-at-upload).
* Nombre del archivo que se debe cargar

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

Puede vista del código fuente HTML asociado con el formulario anterior haciendo clic en el siguiente vínculo:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

En Firefox, haga clic con el botón secundario en la ventana del explorador y, a continuación, haga clic en **Origen de página de Vista**. El código muestra la cadena de consulta URL y el método POST oportunos que se ejecutan cuando el usuario hace clic en **Enviar**.

Para ver la respuesta en XML en Internet Explorer, haga clic en **Ver > Código fuente**. Para vista de respuestas XML en Firefox, haga clic en **Herramientas > Desarrollador web > Origen de página**. Se recomienda utilizar Firefox para ver las respuestas en XML.

A continuación se muestra una respuesta de carga correcta de ejemplo:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>El recurso cargado (JPG, GIF, etc.) se convierte al formato PTIFF y la respuesta envía un vínculo directo a ese recurso PTIFF.

El recurso es igual que cualquier otro recurso de servicio de imágenes, es decir, se le pueden aplicar consultas de procesamiento. Por ejemplo, la URL siguiente solicita un recurso ajustado con la anchura y la altura especificadas.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Envíe el recurso para la carga como una publicación de varias partes o formularios y el resto de los valores en forma de cadena de consulta URL. Se pueden usar los campos siguientes en la cadena de consulta URL para cargar un recurso:

| Parámetro de URL | Obligatorio u opcional | Valor |
|--- |--- |--- |
| op | Obligatorio | cargar |
| upload_token | Obligatorio | Distintivo de carga para la clave secreta compartida asociada a la empresa. |
| company_name | Obligatorio | Nombre de la empresa que realiza la carga. |
| file_limit | Opcional | Límite de tamaño de archivo, en bytes, del recurso. |
| file_exts | Opcional | Lista de extensiones admitidas para el archivo de recurso de imagen. |
| preserve_colorprofile | Opcional | Conserva el perfil de color incrustado al convertir el archivo cargado a formato PTIFF. Los valores posibles son true y false. El valor predeterminado es false. |
| preserve_filename | Opcional | Conserva el nombre de archivo del recurso cargado. Los valores posibles son true y false. El valor predeterminado es false. |

>[!NOTE]
>
>Es obligatorio enviar el recurso que se desea cargar como el único campo en las solicitudes POST de varias partes.

**URL de ejemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST

### Obtención de los metadatos de los recursos de imagen  {#getting-asset-metadata-for-images}

Se puede usar `image_info` para recuperar los metadatos de cualquier recurso cargado, tal como se muestra en el siguiente ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Éste es un ejemplo de respuesta correcta:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Se pueden usar los campos siguientes en la cadena de consulta URL para solicitar información de un recurso:

| Parámetro de URL | Obligatorio u opcional | Valor |
|--- |--- |--- |
| op | Obligatorio | image_info |
| shared_secret | Obligatorio | Clave secreta compartida de la empresa. |
| image_name | Obligatorio | Nombre de la imagen. |

**URL de ejemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Método HTTP permitido:**

GET y POST

## Carga de recursos de vector  {#uploading-a-vector-asset}

Después de recuperar un distintivo de carga válido durante un tiempo determinado, ya se puede cargar un recurso de vector. El recurso se carga como una publicación de varias partes o formularios mientras que el resto de los valores se envía en forma de cadena de consulta URL, tal como se muestra en este ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

Los campos `upload_token` y `company_name` son obligatorios.

Consulte [Recuperación del distintivo de carga](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperación de la clave secreta compartida](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

También se pueden enviar otros valores opcionales en forma de cadenas de consulta URL, como en este ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

El parámetro `file_limit` especifica el límite de tamaño de archivo en bytes. El parámetro `file_exts` especifica las extensiones de nombre de archivo permitidas en la carga. Ambos valores son opcionales.

En la aplicación se definen límites globales tanto para el límite de tamaño de los archivos como para las extensiones de nombre de archivo permitidas. Todo lo incluido en la solicitud se acepta si es un subconjunto de los límites globales. Éstos son los límites globales:

| Límite global | Valor |
|--- |--- |
| Tamaño de archivo para todos los clientes | 20 MB |
| Formatos de archivo de vector admitidos para la carga | AI, EPS, PDF (solo cuando el archivo PDF se haya abierto y guardado en Adobe Illustrator CS6) |

El siguiente formulario HTML permite al usuario cargar un recurso. En el formulario se pide al usuario que introduzca la información siguiente:

* Nombre de empresa.
* Distintivo de carga.
* Límite de tamaño de archivo.
* Lista de extensiones de nombre de archivo.
* Indica si se debe conservar o no el perfil de color y el nombre de archivo asociados al recurso.
* Indica si se utiliza o no el fondo de cobertura. Si activa Fondo de cobertura, defina la esquina, la tolerancia y el método de relleno. Consulte Fondo de cobertura en [Opciones de edición de imágenes al cargar](image-editing-options-upload.md#image-editing-options-at-upload).
* Nombre del archivo que se debe cargar

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

Al hacer clic con el botón derecho en la ventana del explorador y, luego, hacer clic en **Ver código fuente**, aparece el siguiente código, que corresponde al formulario mostrado en la ilustración. El código muestra la cadena de consulta URL y el método POST oportunos que se ejecutan cuando el usuario hace clic en **Enviar**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Para ver la respuesta en XML en Internet Explorer, haga clic en **Ver** > **Código fuente**. Para ver la respuesta en XML en Firefox, haga clic en **Ver** > **Código fuente de la página**. Se recomienda utilizar Firefox para ver las respuestas en XML.

A continuación se muestra una respuesta de carga correcta de ejemplo:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>El recurso cargado (AI, EPS, PDF, etc.) se convierte al formato FXG y la respuesta envía un vínculo directo a ese recurso FXG.

El recurso es igual que cualquier otro recurso de impresión virtual, es decir, se le pueden aplicar consultas de procesamiento. Por ejemplo, la siguiente URL convierte un recurso FXG en una imagen PNG de 500 x 500.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Envíe el recurso para la carga como una publicación de varias partes o formularios y el resto de los valores en forma de cadena de consulta URL. Se pueden usar los campos siguientes en la cadena de consulta URL para cargar un recurso:

| Parámetro de URL | Obligatorio u opcional | Valor |
|--- |--- |--- |
| op | Obligatorio | cargar |
| upload_token | Obligatorio | Distintivo de carga para la clave secreta compartida asociada a la empresa. |
| compañía_nombre | Obligatorio | Nombre de la empresa que realiza la carga. |
| file_limit | Opcional | Límite de tamaño de archivo, en bytes, del recurso. |
| file_exts | Opcional | Lista de extensiones admitidas para el archivo de recurso. |

>[!NOTE]
>
>Es obligatorio enviar el recurso que se desea cargar como el único campo en las solicitudes POST de varias partes.

**URL de ejemplo:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST
