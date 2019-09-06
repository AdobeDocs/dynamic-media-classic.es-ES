---
title: Gestión de la carpeta Papelera
seo-title: Gestión de la carpeta Papelera
description: nulo
seo-description: Descubra cómo gestionar la papelera.
uuid: 3992 a 5 b 8-1919-4924-b 07 d -7 fb 25565 effd
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: 553 c 95 fc -0 a 41-4 f 06-af 50-a 62 bc 1438149
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Gestión de la carpeta Papelera{#managing-the-trash-folder}

Los archivos que se eliminan de Scene7 Publishing System se mueven a la carpeta Papelera. Permanecen siete días en esta carpeta, hasta que se restauran o se eliminan de forma permanente. Puede examinar los elementos eliminados si selecciona el icono de la papelera  situado en la parte inferior de la biblioteca de recursos; se mostrarán los elementos que hay en la carpeta Papelera.

Todos los usuarios pueden restaurar elementos desde la carpeta Papelera y colocarlos en la carpeta en que se encontraban antes de ser eliminados. Todos los usuarios pueden vaciar la carpeta Papelera y eliminar su contenido.

Al eliminar elementos de la carpeta Papelera, éstos se eliminarán de forma permanente de Scene7 Publishing System; los elementos eliminados desde la carpeta Papelera no se podrán restaurar. Si desea obtener información sobre la configuración de notificaciones destinadas a los administradores de la empresa cuando los recursos estén a punto de eliminarse automáticamente de la papelera, consulte [Configuración general de la aplicación](application-setup.md#general_settings).

>[!NOTE]
>
>los recursos que se encuentran en la carpeta Papelera siguen registrados en Scene7 Publishing System. Si intenta cargar un archivo con el mismo nombre que un archivo eliminado en la carpeta Papelera, Dynamic Media Classic trata el recurso que desea cargar como recurso duplicado. Por tanto, se agregará un número al nombre.

## Acerca de la carpeta Papelera {#about-the-trash-folder}

Si elimina un recurso en una carpeta, éste se colocará en la carpeta Papelera. Al eliminar un elemento y moverlo a la carpeta Papelera, ocurre lo siguiente:

* Aunque el elemento se ha eliminado de las carpetas de Scene7 Publishing System, su ID no se podrá asignar a otro recurso mientras se encuentre en la carpeta Papelera. Si intenta cargar un recurso con el mismo nombre que un archivo en la carpeta Papelera, Dynamic Media Classic añadirá un numeral al nombre del recurso.
* El elemento no se puede publicar. Aunque el elemento estuviera marcado para la publicación al eliminarlo, no se publicará.
* El elemento permanece en la carpeta Papelera durante siete días, a menos que se restaure antes o alguien elija el comando para vaciar la papelera. Pasados siete días, se produce una operación de limpieza automática y el elemento se elimina de forma permanente.

## Restauración de recursos desde la carpeta Papelera {#restoring-assets-from-the-trash-folder}

La persona que eliminó el recurso no tiene por qué ser la misma que lo restaure; cualquier usuario puede restaurar recursos desde la carpeta Papelera. Los recursos restaurados se colocan en las carpetas de donde se eliminaron. Si estas carpetas ya no existen, Scene7 Publishing System vuelve a crearlas y los recursos restaurados se colocan en ellas.

Para restaurar recursos desde la carpeta Papelera y volver a colocarlos en las carpetas de las que se eliminaron, siga estos pasos:

1. Haga clic en el icono Papelera para abrir la carpeta Papelera.
1. Seleccione el recurso o los recursos que desea restaurar.
1. Elija Archivo &gt; Restaurar desde papelera.

## Eliminación permanente de recursos desde la carpeta Papelera {#permanently-deleting-assets-in-the-trash-folder}

Al eliminar recursos en la carpeta Papelera, éstos se eliminan de forma permanente. Los recursos se eliminan de forma automática de la carpeta Papelera después de siete días.

Si desea eliminar recursos de forma permanente desde la carpeta Papelera, seleccione el icono Papelera  para abrir esta carpeta. A continuación, elimine recursos individuales o elimine todos los recursos de la papelera:

**Eliminación de recursos individuales** Seleccione los recursos que desea eliminar de forma permanente y haga clic en Archivo &gt; Vacío de papelera.

**Al eliminar todos los recursos** , haga clic en Archivo &gt; Papelera vacía.

>[!MORELIKETHIS]
>
>* [Eliminación de recursos](moving-renaming-deleting-assets.md#delete_assets)

