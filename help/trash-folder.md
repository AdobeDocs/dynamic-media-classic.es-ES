---
title: Administrar la carpeta Papelera
description: Obtenga información sobre cómo administrar la carpeta Papelera.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 33%

---

# Administrar la carpeta Papelera{#managing-the-trash-folder}

Los elementos que elimine de Adobe Dynamic Media Classic se moverán a la carpeta Papelera. Los archivos eliminados permanecen en esta carpeta durante siete días hasta que se restauran o se eliminan de forma permanente. Para examinar los elementos eliminados, haga clic en el icono **[!UICONTROL Papelera]** en la parte inferior de la biblioteca de recursos y vea los elementos en la página de la carpeta Papelera.

Todos los usuarios pueden restaurar elementos desde la carpeta Papelera y colocarlos en la carpeta en que se encontraban antes de ser eliminados. Todos los usuarios pueden vaciar la carpeta Papelera y eliminar su contenido.

Al eliminar elementos de la carpeta Papelera, se eliminan permanentemente los elementos de Adobe Dynamic Media Classic; los elementos eliminados de la carpeta Papelera ya no se pueden restaurar. Si desea obtener información sobre la configuración de notificaciones destinadas a los administradores de la empresa cuando los recursos estén a punto de eliminarse automáticamente de la papelera, consulte [Configuración general de la aplicación](application-setup.md#general_settings).

>[!NOTE]
>
>Los recursos que se han movido a la carpeta Papelera siguen registrados en Adobe Dynamic Media Classic. Si intenta cargar un archivo que tenga el mismo nombre que un archivo eliminado en la carpeta Papelera, Adobe Dynamic Media Classic trata el recurso que desea cargar como un recurso duplicado. Por tanto, se agregará un número al nombre.

## Acerca de la carpeta Papelera {#about-the-trash-folder}

Si elimina un recurso en una carpeta, éste se colocará en la carpeta Papelera. Al eliminar un elemento y moverlo a la carpeta Papelera, ocurre lo siguiente:

* Aunque el elemento se haya eliminado de las carpetas de Dynamic Media Classic de Adobe, su ID no se puede asignar a otro recurso mientras permanezca en la carpeta Papelera. Si intenta cargar un recurso con el mismo nombre que un archivo en la carpeta Papelera, Adobe Dynamic Media Classic añade un número al nombre del recurso.
* El elemento no se puede publicar. Aunque el elemento estuviera marcado para la publicación al eliminarlo, no se publicará.
* El elemento permanece en la carpeta Papelera hasta que se restaura, pasan siete días o alguien elige el comando **[!UICONTROL Vacíe la papelera]**. Pasados siete días, se produce una operación de limpieza automática y el elemento se elimina de forma permanente.

## Restaurar recursos desde la carpeta Papelera {#restoring-assets-from-the-trash-folder}

No es necesario que la persona que ha eliminado un activo lo restaure; cualquier usuario puede restaurar recursos desde la carpeta Papelera. Los recursos restaurados se colocan en las carpetas de donde se eliminaron. Si estas carpetas ya no existen, Adobe Dynamic Media Classic las vuelve a crear y los recursos restaurados se colocan en las carpetas creadas de nuevo.

Para restaurar recursos de la carpeta Papelera a las carpetas de las que se eliminaron, haga lo siguiente:

1. En la parte inferior del panel Biblioteca de recursos, seleccione el icono **[!UICONTROL Papelera]** para abrir la carpeta Papelera.
1. Seleccione el recurso o los recursos que desea restaurar.
1. Vaya a **[!UICONTROL File]** > **[!UICONTROL Restore from trash]**.

## Eliminación permanente de recursos desde la carpeta Papelera {#permanently-deleting-assets-in-the-trash-folder}

Al eliminar recursos en la carpeta Papelera, éstos se eliminan de forma permanente. Los recursos se eliminan de forma automática de la carpeta Papelera después de siete días.

Para eliminar permanentemente los recursos de la carpeta Papelera, seleccione el icono **[!UICONTROL Papelera]**. En la página Carpeta Papelera , realice una de las acciones siguientes:

* **Eliminación de recursos individuales** : seleccione los recursos que desea eliminar de forma permanente y, a continuación, vaya a  **[!UICONTROL Archivo]**  >  **[!UICONTROL Vacío en la papelera]**.

* **Eliminación de todos los recursos** : vaya a  **[!UICONTROL Archivo]**  >  **[!UICONTROL Basura vacía]**.

>[!MORELIKETHIS]
>
>* [Eliminación de recursos](moving-renaming-deleting-assets.md#delete_assets)

