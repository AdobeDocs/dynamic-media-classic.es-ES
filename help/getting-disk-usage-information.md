---
title: Obtención de información sobre el uso del disco
seo-title: Obtención de información sobre el uso del disco
description: nulo
seo-description: Obtenga información sobre cómo obtener información sobre el uso del disco.
uuid: 01361693-53 d 0-4072-b 7 c 3-f 284631 d 28 cf
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6763546 d -83 c 4-42 dc -879 f -6 bbfc 8 b 56482
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

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

