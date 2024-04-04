---
title: Comparta cambios de recursos con compañeros en tiempo real
description: Aprenda a compartir cambios de recursos con compañeros en tiempo real en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 26%

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

Cuando inició sesión, se le pidió que permitiera o denegara las actualizaciones de iguales. Puede especificar que se &quot;recuerde&quot; la selección para que solo se le pregunte una vez. Para borrar la opción elegida, elimine el sitio oportuno del panel Redes asistidas por pares de Configuración global.

Si estaba editando un recurso modificado por un elemento del mismo nivel, se le pedirá que introduzca el cambio en el generador o editor. Si elige **[!UICONTROL Sí]**, el generador o editor descarta los cambios realizados en el recurso e importa el recurso actualizado. Si elige **[!UICONTROL No]** Sin embargo, el recurso no se modifica en el generador o editor y cualquier cambio que haya realizado persistirá en esa sesión.

Cuando guardó el recurso, se le notificó que existe una versión más reciente y se le preguntó si desea sobrescribir el recurso con sus cambios.
