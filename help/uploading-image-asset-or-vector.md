---
title: Cargar un recurso de imagen de trama
description: Obtenga información sobre cómo cargar un recurso de imagen de trama en Adobe Dynamic Media Classic
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: f92109182283f3bf046604b1b6910180f858d73e
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 69%

---

# Cargar un recurso de imagen de trama {#uploading-an-image-asset-or-a-vector-asset}

Para poder cargar un recurso de imagen, primero debe solicitar una clave secreta compartida. Esta clave permite recuperar un distintivo de carga. A continuación, utilice el token de carga para cargar recursos de imagen de trama.

>[!IMPORTANT]
>
>La compatibilidad con los recursos vectoriales UGC nuevos o existentes en Adobe Dynamic Media Classic finalizó el 30 de septiembre de 2021.

## Solicitar una clave secreta compartida {#requesting-a-shared-secret-key}

Solicite una *clave secreta compartida* [utilizando el Admin Console para crear un caso de soporte.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) En su caso de asistencia, solicite una clave secreta compartida.

En el mensaje, proporcione el nombre de empresa que desee utilizar para cargar los recursos de imagen. Cuando reciba la clave de Adobe Dynamic Media Classic, guárdela localmente para usarlo más adelante.

## Recuperar el token de carga {#retrieving-the-upload-token}

El *distintivo de carga* garantiza que nadie más use la misma clave secreta compartida para cargar recursos. Garantiza que la carga sea legítima y que proceda de una fuente de confianza.

El distintivo de carga es una cadena alfanumérica que solo se encuentra disponible durante un tiempo concreto. Utilice las siguientes direcciones URL, sustituyendo la clave secreta compartida, para poder recuperar el token de carga.

* Imagen rasterizada
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`En este ejemplo, la clave secreta compartida es  `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

De manera predeterminada, el distintivo de carga caduca en 5 minutos (300 segundos) después de recuperarlo. Si desea solicitar más tiempo, incluya en la URL `expires` seguido de la cantidad de tiempo necesaria en segundos. Por ejemplo, esta URL de imagen de ejemplo recupera un distintivo de carga válido durante 1.800 segundos:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

La respuesta correcta para las imágenes es similar a la siguiente:

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
| --- | --- | --- |
| op | Obligatorio | get_uploadtoken |
| shared_secret | Obligatorio | Clave secreta compartida de la empresa que realiza la carga. |
| expires | Opcional | Número de segundos durante los que es válido el distintivo de carga. Si no se especifica, el valor predeterminado es 300 segundos. |

**URL de imagen de trama de ejemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**Métodos HTTP permitidos:**
`GET` y  `POST`

Ya puede cargar un recurso de imagen.

Consulte [Cargar un recurso de imagen](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Cargar un recurso de imagen de trama {#uploading-an-image-asset}

Después de recuperar un distintivo de carga válido durante un tiempo determinado, ya se puede cargar un recurso de imagen. El recurso se carga como una publicación de varias partes o formularios mientras que el resto de los valores se envía en forma de cadena de consulta URL, tal como se muestra en este ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Los campos `upload_token` y `company_name` son obligatorios.

Consulte [Recuperar el token de carga](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Consulte [Recuperar una clave secreta compartida](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

También se pueden enviar otros valores opcionales en forma de cadenas de consulta URL, como en este ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

El parámetro `file_limit` especifica el límite de tamaño de archivo en bytes. El parámetro `file_exts` especifica las extensiones de nombre de archivo permitidas en la carga. Ambos valores son opcionales.

En la aplicación se definen límites globales tanto para el límite de tamaño de los archivos como para las extensiones de nombre de archivo permitidas. Todo lo incluido en la solicitud se acepta si es un subconjunto de los límites globales. Éstos son los límites globales:

| Límite global | Valor |
| --- | --- |
| Tamaño de archivo para todos los clientes | 20 MB |
| Formatos de archivo de imagen admitidos para la carga | BMP, GIF, JPG, PNG y PSD, TIFF |

El siguiente formulario HTML permite al usuario cargar un recurso. En el formulario se pide al usuario que introduzca la información siguiente:

* Nombre de empresa.
* Distintivo de carga.
* Límite de tamaño de archivo.
* Lista de extensiones de nombre de archivo.
* Si se desea conservar el perfil de color y el nombre de archivo asociados al recurso.
* Si se utiliza el fondo de Knockout. Si activa Fondo de Knockout, defina la Esquina, Tolerancia y Método de Relleno.
Consulte Contexto de Knockout en [Opciones de ajuste de imágenes en upload](image-editing-options-upload.md#image-editing-options-at-upload).
* Nombre del archivo que se debe cargar.

Puede ver el código fuente HTML asociado con el formulario anterior seleccionando [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

En Firefox, haga clic con el botón derecho en la ventana del explorador y, a continuación, seleccione **[!UICONTROL Ver origen de página]**. El código muestra la cadena de consulta URL y el método POST oportunos que se ejecutan cuando el usuario hace clic en **[!UICONTROL Enviar]**.

Para ver la respuesta XML en Internet Explorer, vaya a **[!UICONTROL View]** > **[!UICONTROL Source]**. Para ver la respuesta XML en Firefox, vaya a **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Web Developer Tools]**. Se recomienda utilizar Firefox para ver las respuestas en XML.

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
| --- | --- | --- |
| `op` | Obligatorio | cargar |
| `upload_token` | Obligatorio | Distintivo de carga para la clave secreta compartida asociada a la empresa. |
| `company_name` | Obligatorio | Nombre de la empresa que realiza la carga. |
| `file_limit` | Opcional | Límite de tamaño de archivo, en bytes, del recurso. |
| `file_exts` | Opcional | Lista de extensiones admitidas para el archivo de recurso de imagen. |
| `preserve_colorprofile` | Opcional | Conserva el perfil de color incrustado al convertir el archivo cargado a formato PTIFF. Los valores posibles son true y false. El valor predeterminado es false. |
| `preserve_filename` | Opcional | Conserva el nombre de archivo del recurso cargado. Los valores posibles son true y false. El valor predeterminado es false. |

>[!NOTE]
>
>Es obligatorio enviar el recurso que se desea cargar como el único campo en las solicitudes POST de varias partes.

**URL de ejemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Método HTTP permitido:**

POST

### Obtener metadatos de recursos para imágenes {#getting-asset-metadata-for-images}

Se puede usar `image_info` para recuperar los metadatos de cualquier recurso cargado, tal como se muestra en el siguiente ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Un ejemplo de respuesta correcta es similar al siguiente:

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
| --- | --- | --- |
| `op` | Obligatorio | image_info |
| `shared_secret` | Obligatorio | Clave secreta compartida de la empresa. |
| `image_name` | Obligatorio | Nombre de la imagen. |

**URL de ejemplo:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Método HTTP permitido:**

GET y POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->