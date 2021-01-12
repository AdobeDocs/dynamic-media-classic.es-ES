---
title: Uso compartido de cambios de recursos con iguales en tiempo real
seo-title: Uso compartido de cambios de recursos con iguales en tiempo real
description: nulo
seo-description: Descubra cómo compartir cambios de recursos con compañeros en tiempo real.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
translation-type: tm+mt
source-git-commit: 3a8283196c9c99a5709cf4995c426da7e4f6c83b
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 71%

---


# Uso compartido de cambios de recursos con iguales en tiempo real{#sharing-asset-changes-with-peers-in-real-time}

Con varias copias de Dynamic Media Classic ejecutándose en uno o más equipos de la misma compañía, las siguientes acciones de cualquier cliente de Dynamic Media Classic se actualizan en tiempo real con todos los clientes del mismo nivel:

* Edición de un recurso (generador, editor de imágenes, etc.)
* Cambio de nombre de un recurso
* Eliminación de un recurso
* Movimiento de un recurso
* Carga de uno o más recursos (tanto escritorio como FTP)
* Creación, eliminación o cambio de nombre de una carpeta

Después de realizar un cambio en el cliente de origen, todos los clientes del mismo nivel que iniciaron sesión en la misma compañía se actualizan con el cambio. Estos cambios no se notifican a los iguales a menos que estén editando el recurso cambiado en cualquiera de los generadores o editores de imágenes.

Al iniciar sesión, se le pedirá que permita o deniegue las actualizaciones de iguales. Puede especificar que se &quot;recuerde&quot; la selección para que solo se le pregunte una vez. Para borrar la opción elegida, elimine el sitio oportuno del panel Redes asistidas por pares de Configuración global.

Si está editando un recurso cambiado por un igual, se le pedirá que inserte el cambio en el generador o editor. Al elegir Sí, el generador o editor elimina los cambios realizados en el recurso e importa el recurso actualizado. Si elige No, no se cambia el recurso en el generador o editor sino que los cambios realizados se mantienen en la sesión.

Cuando guarde el recurso, se le notificará la existencia de una versión más reciente y se le preguntará si desea sobrescribir el recurso con sus cambios.
