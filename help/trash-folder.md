---
title: Gestión de la carpeta Papelera
description: Obtenga información sobre cómo administrar la carpeta Papelera.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Administración de recursos
role: Profesional empresarial
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 60%

---


# Gestión de la carpeta Papelera{#managing-the-trash-folder}

Los elementos que elimine de Dynamic Media Classic se moverán a la carpeta Papelera. Permanecen siete días en esta carpeta, hasta que se restauran o se eliminan de forma permanente. Puede examinar los elementos eliminados si selecciona el icono de la papelera  situado en la parte inferior de la biblioteca de recursos; se mostrarán los elementos que hay en la carpeta Papelera.

Todos los usuarios pueden restaurar elementos desde la carpeta Papelera y colocarlos en la carpeta en que se encontraban antes de ser eliminados. Todos los usuarios pueden vaciar la carpeta Papelera y eliminar su contenido.

Al eliminar elementos de la carpeta Papelera, se eliminan permanentemente los elementos de Dynamic Media Classic; los elementos eliminados de la carpeta Papelera ya no se pueden restaurar. Si desea obtener información sobre la configuración de notificaciones destinadas a los administradores de la empresa cuando los recursos estén a punto de eliminarse automáticamente de la papelera, consulte [Configuración general de la aplicación](application-setup.md#general_settings).

>[!NOTE]
>
>Los recursos que se han movido a la carpeta Papelera siguen registrados en Dynamic Media Classic. Si intenta cargar un archivo que tenga el mismo nombre que un archivo eliminado en la carpeta Papelera, Dynamic Media Classic trata el recurso que desea cargar como un recurso duplicado. Por tanto, se agregará un número al nombre.

## Acerca de la carpeta Papelera {#about-the-trash-folder}

Si elimina un recurso en una carpeta, éste se colocará en la carpeta Papelera. Al eliminar un elemento y moverlo a la carpeta Papelera, ocurre lo siguiente:

* Aunque el elemento se haya eliminado de las carpetas de Dynamic Media Classic, su ID no se puede asignar a otro recurso mientras permanezca en la carpeta Papelera. Si intenta cargar un recurso con el mismo nombre que un archivo en la carpeta Papelera, Dynamic Media Classic añade un número al nombre del recurso.
* El elemento no se puede publicar. Aunque el elemento estuviera marcado para la publicación al eliminarlo, no se publicará.
* El elemento permanece en la carpeta Papelera durante siete días, a menos que se restaure antes o alguien elija el comando para vaciar la papelera. Pasados siete días, se produce una operación de limpieza automática y el elemento se elimina de forma permanente.

## Restauración de recursos desde la carpeta Papelera  {#restoring-assets-from-the-trash-folder}

La persona que eliminó el recurso no tiene por qué ser la misma que lo restaure; cualquier usuario puede restaurar recursos desde la carpeta Papelera. Los recursos restaurados se colocan en las carpetas de donde se eliminaron. Si estas carpetas ya no existen, Dynamic Media Classic las vuelve a crear y los recursos restaurados se colocan en las carpetas creadas de nuevo.

Para restaurar recursos desde la carpeta Papelera y volver a colocarlos en las carpetas de las que se eliminaron, siga estos pasos:

1. Haga clic en el icono Papelera para abrir la carpeta Papelera.
1. Seleccione el recurso o los recursos que desea restaurar.
1. Elija Archivo > Restaurar desde papelera.

## Eliminación permanente de recursos desde la carpeta Papelera  {#permanently-deleting-assets-in-the-trash-folder}

Al eliminar recursos en la carpeta Papelera, éstos se eliminan de forma permanente. Los recursos se eliminan de forma automática de la carpeta Papelera después de siete días.

Si desea eliminar recursos de forma permanente desde la carpeta Papelera, seleccione el icono Papelera  para abrir esta carpeta. A continuación, elimine recursos individuales o elimine todos los recursos de la papelera:

* **Eliminación de** recursos individualesSeleccione los recursos que desea eliminar de forma permanente y haga clic en  **[!UICONTROL Archivo > Vacío de la papelera]**.

* **Eliminación de todos los** recursosHaga clic en  **[!UICONTROL Archivo > Papelera vacía]**.

>[!MORELIKETHIS]
>
>* [Eliminación de recursos](moving-renaming-deleting-assets.md#delete_assets)

