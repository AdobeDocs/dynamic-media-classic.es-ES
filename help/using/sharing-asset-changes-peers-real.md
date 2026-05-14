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
autotag-review: '2026-05-13T20:12:54.992Z'
TQID: 'https://experienceleague.adobe.com/Yn5GsnQ4cM3Byk18iEB8Z4uGsTt9FjEZOBP17Yt-K8M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 281
ht-degree: 26%

---

# Comparta cambios de recursos con compañeros en tiempo real{#sharing-asset-changes-with-peers-in-real-time}

Supongamos que tiene varias copias de Adobe Dynamic Media Classic ejecutándose en equipos de la misma compañía. En este caso, las siguientes acciones de cualquier cliente de Dynamic Media Classic se actualizan en tiempo real con todos los clientes del mismo nivel:

* Editar un recurso (generador, editor de imágenes, etc.)
* Cambio de nombre de un recurso
* Eliminación de un recurso
* Movimiento de un recurso
* Carga de uno o más recursos (tanto escritorio como FTP)
* Creación, eliminación o cambio de nombre de una carpeta

Después de realizar un cambio en el cliente de origen, todos los clientes del mismo nivel conectados a la misma compañía se actualizan con el cambio. Estos cambios no se notifican a los iguales a menos que estén editando el recurso cambiado en cualquiera de los generadores o editores de imágenes.

Cuando inició sesión, se le pidió que permitiera o denegara las actualizaciones de iguales. Puede especificar que se &quot;recuerde&quot; la selección para que solo se le pregunte una vez. Para borrar la opción elegida, elimine el sitio oportuno del panel Redes asistidas por pares de Configuración global.

Si estaba editando un recurso modificado por un compañero, se le pedirá que introduzca el cambio en el generador o editor. Si elige **[!UICONTROL Sí]**, el generador o editor descartará los cambios realizados en el recurso e importará el recurso actualizado. Si elige **[!UICONTROL No]**, el recurso no cambiará en el generador o editor y cualquier cambio que haya realizado persistirá en esa sesión.

Cuando guardó el recurso, se le notificó que existe una versión más reciente y se le preguntó si desea sobrescribir el recurso con sus cambios.
