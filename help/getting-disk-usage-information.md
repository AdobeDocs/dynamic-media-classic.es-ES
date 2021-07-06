---
title: Obtención de información sobre el uso del disco
description: Aprenda a obtener información sobre el uso del disco.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '88'
ht-degree: 88%

---

# Obtención de información sobre el uso del disco {#getting-disk-usage-information}

El parámetro `disk_info` se puede usar para recuperar información sobre el uso del espacio en disco de la empresa, tal como se muestra en este ejemplo:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Éste es un ejemplo de respuesta:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Se pueden usar los campos siguientes en la cadena de consulta URL para obtener información sobre el uso del disco:

| Parámetro de URL | Obligatorio u opcional | Valor |
|--- |--- |--- |
| op | Obligatorio | disk_info |
| shared_secret | Obligatorio | Clave secreta compartida de la empresa |

El siguiente ejemplo de código obtiene información del disco de la empresa 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
