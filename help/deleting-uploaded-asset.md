---
title: Eliminación de recursos cargados
seo-title: Eliminación de recursos cargados
description: nulo
seo-description: Obtenga información sobre cómo eliminar un recurso cargado.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '99'
ht-degree: 88%

---


# Eliminación de recursos cargados{#deleting-an-uploaded-asset}

Se puede usar el parámetro `delete` con este formato para eliminar un recurso:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

A continuación se muestra un ejemplo de respuesta después de haber eliminado un recurso de imagen:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Se pueden usar los campos siguientes en la cadena de consulta URL para eliminar un recurso:

| Parámetro de URL | Obligatorio u opcional | Valor |
|--- |--- |--- |
| op | Obligatorio | eliminar |
| shared_secret | Obligatorio | Clave secreta compartida de la empresa. |
| <ul><li>Para imágenes:image_name</li><li>Para el vector:fxg_name</li></ul> | Obligatorio | Nombre del recurso que se debe eliminar. |

**URL de imagen de muestra:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**URL de vector de prueba:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
