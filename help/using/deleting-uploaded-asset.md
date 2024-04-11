---
title: Eliminar un recurso de imagen rasterizada cargado
description: Obtenga información sobre cómo eliminar un recurso cargado en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 33%

---

# Eliminar un recurso cargado{#deleting-an-uploaded-asset}

Puede usar el complemento `delete` en este formato para eliminar un recurso:

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
| --- | --- | --- |
| `op` | Obligatorio | eliminar |
| `shared_secret` | Obligatorio | La clave que es un secreto compartido para la compañía. |
| `image_name` | Obligatorio | Nombre del recurso que se va a eliminar. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>A partir del 1 de mayo de 2023, los recursos UGC de Dynamic Media estarán disponibles para su uso durante un máximo de 60 días a partir de la fecha de carga. Después de 60 días, los recursos se eliminarán.

>[!NOTE]
>
>La compatibilidad con recursos de imagen vectorial UGC nuevos o existentes en Adobe Dynamic Media Classic finalizó el 30 de septiembre de 2021.

**URL de imagen de muestra:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
