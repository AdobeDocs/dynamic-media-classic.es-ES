---
title: Uso compartido de cambios de recursos con iguales en tiempo real
seo-title: Uso compartido de cambios de recursos con iguales en tiempo real
description: nulo
seo-description: Aprenda a compartir cambios de recursos con compañeros en tiempo real.
uuid: 13 fa 4 f 6 e -66 bf -4682-96 a 9-0 e 7040706 f 53
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: ca 7 c 8 a 7 f -76 f 4-4 a 25-8 c 36-617 a 029 e 55 be
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Uso compartido de cambios de recursos con iguales en tiempo real{#sharing-asset-changes-with-peers-in-real-time}

Con varias copias de Dynamic Media Classic ejecutadas en uno o más equipos de la misma empresa, las siguientes acciones de cualquier cliente de Dynamic Media Classic se actualizan en tiempo real con todos los clientes de iguales:

* Edición de un recurso (generador, editor de imágenes, etc.)
* Cambio de nombre de un recurso
* Eliminación de un recurso
* Movimiento de un recurso
* Carga de uno o más recursos (tanto escritorio como FTP)
* Creación, eliminación o cambio de nombre de una carpeta

Una vez que se realiza un cambio en el cliente de origen, se actualizan con dicho cambio todos los clientes de iguales de la misma empresa. Estos cambios no se notifican a los iguales a menos que estén editando el recurso cambiado en cualquiera de los generadores o editores de imágenes.

Al iniciar la sesión, Flash Player pregunta si desea permitir o rechazar las actualizaciones de iguales. Puede especificar que se "recuerde" la selección para que solo se le pregunte una vez. Para borrar la opción elegida, elimine el sitio oportuno del panel Redes asistidas por pares de Configuración global.

Si está editando un recurso cambiado por un igual, se le pedirá que inserte el cambio en el generador o editor. Al elegir Sí, el generador o editor elimina los cambios realizados en el recurso e importa el recurso actualizado. Si elige No, no se cambia el recurso en el generador o editor sino que los cambios realizados se mantienen en la sesión.

Cuando guarde el recurso, se le notificará la existencia de una versión más reciente y se le preguntará si desea sobrescribir el recurso con sus cambios.
