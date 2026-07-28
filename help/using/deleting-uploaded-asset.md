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
autotag-review: '2026-05-13T19:44:43.552Z'
TQID: 'https://experienceleague.adobe.com/EVwriRMQMB9aO3j-cZeaFeZE3wVtbQmQZA67ioyUniI'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 7f6a75dae63b295e7df72b3b8b0935a2406c3d32
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 32%

---

# Eliminar un recurso cargado{#deleting-an-uploaded-asset}

Puede usar el parámetro `delete` en este formato para eliminar un recurso:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

A continuación se muestra un ejemplo de respuesta después de haber eliminado un recurso de imagen:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
>A partir del 1 de mayo de 2023, los recursos UGC en Dynamic Media estarán disponibles para su uso hasta 60 días después de la fecha de carga. Después de 60 días, los recursos se eliminan.

>[!NOTE]
>
>La compatibilidad con recursos de imagen vectorial UGC nuevos o existentes en Adobe Dynamic Media Classic finalizó el 30 de septiembre de 2021.

**URL de imagen de muestra:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- 
**Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` 
-->
