---
title: Comparta cambios de recursos con compañeros en tiempo real
description: Aprenda a compartir cambios de recursos con compañeros en tiempo real en Adobe Dynamic Media Classic.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 44%

---

# Comparta cambios de recursos con compañeros en tiempo real{#sharing-asset-changes-with-peers-in-real-time}

Con varias copias de Adobe Dynamic Media Classic ejecutándose en varios equipos de la misma empresa, las siguientes acciones de cualquier cliente de Adobe Dynamic Media Classic se actualizan en tiempo real con todos los clientes del mismo nivel:

* Editar un recurso (generador, editor de imágenes, etc.)
* Cambio de nombre de un recurso
* Eliminación de un recurso
* Movimiento de un recurso
* Carga de uno o más recursos (tanto escritorio como FTP)
* Creación, eliminación o cambio de nombre de una carpeta

Después de realizar un cambio en el cliente de origen, todos los clientes del mismo nivel conectados a la misma compañía se actualizan con el cambio. Estos cambios no se notifican a los iguales a menos que estén editando el recurso cambiado en cualquiera de los generadores o editores de imágenes.

Al iniciar sesión, se le pedirá que permita o deniegue las actualizaciones de igual a igual. Puede especificar que se &quot;recuerde&quot; la selección para que solo se le pregunte una vez. Para borrar la opción elegida, elimine el sitio oportuno del panel Redes asistidas por pares de Configuración global.

Si está editando un recurso cambiado por un igual, se le pedirá que inserte el cambio en el generador o editor. Si elige **[!UICONTROL Sí]**, el generador o editor descarta los cambios realizados en el recurso e importa el recurso actualizado. Si elige **[!UICONTROL No]** Sin embargo, el recurso no se modifica en el generador o editor y cualquier cambio que haya realizado persistirá en esa sesión.

Cuando guarde el recurso, se le notificará la existencia de una versión más reciente y se le preguntará si desea sobrescribir el recurso con sus cambios.
