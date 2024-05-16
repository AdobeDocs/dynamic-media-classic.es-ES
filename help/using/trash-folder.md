---
title: Administrar la carpeta Papelera
description: Obtenga información sobre cómo administrar la carpeta Papelera.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 28%

---

# Administrar la carpeta Papelera{#managing-the-trash-folder}

Los elementos que elimine de Adobe Dynamic Media Classic se moverán a la papelera. Estos elementos eliminados permanecen en esta carpeta durante siete días hasta que se restauran o se eliminan de forma permanente. Puede examinar los elementos eliminados seleccionando la **[!UICONTROL Papelera]** en la parte inferior de la biblioteca de recursos y viendo los elementos en la página de la carpeta Papelera.

Todos los usuarios pueden restaurar elementos desde la carpeta Papelera y colocarlos en la carpeta en que se encontraban antes de ser eliminados. Todos los usuarios pueden vaciar la carpeta Papelera y eliminar su contenido.

Al eliminar elementos de la papelera, se eliminan permanentemente los elementos de Adobe Dynamic Media Classic; los elementos eliminados de la papelera ya no se pueden restaurar. Si desea obtener información sobre la configuración de notificaciones destinadas a los administradores de la empresa cuando los recursos estén a punto de eliminarse automáticamente de la papelera, consulte [Configuración general de la aplicación](application-setup.md#general_settings).

>[!NOTE]
>
>Los recursos que se han movido a la papelera siguen registrados en Adobe Dynamic Media Classic. Por ejemplo, supongamos que intenta cargar un archivo que tiene el mismo nombre que un archivo eliminado en la carpeta Papelera. Adobe Dynamic Media Classic trata el recurso que desea cargar como un recurso duplicado. En este caso, se anexa un número a su nombre.

## Acerca de la carpeta Papelera {#about-the-trash-folder}

Si elimina un recurso en una carpeta, éste se colocará en la carpeta Papelera. Al eliminar un elemento y moverlo a la carpeta Papelera, ocurre lo siguiente:

* Aunque el elemento se elimine de la carpeta Adobe Dynamic Media Classic, su ID no se podrá asignar a otro recurso mientras permanezca en la carpeta Papelera. Si intenta cargar un recurso con el mismo nombre que un archivo en la carpeta Papelera, Adobe Dynamic Media Classic anexa un número al nombre del recurso.
* El elemento no se puede publicar. Aunque el elemento estuviera marcado para la publicación al eliminarlo, no se publicará.
* El elemento permanece en la carpeta Papelera hasta que se restaure, pasen siete días o alguien elija el **[!UICONTROL Vaciar la papelera]** comando. Pasados siete días, se produce una operación de limpieza automática y el elemento se elimina de forma permanente.

## Restaurar recursos desde la carpeta Papelera {#restoring-assets-from-the-trash-folder}

No es necesario que la persona que eliminó un recurso lo restaure; cualquier persona puede restaurar recursos desde la carpeta Papelera. Los recursos restaurados se colocan en las carpetas de donde se eliminaron. Si estas carpetas ya no existen, Adobe Dynamic Media Classic las vuelve a crear y los recursos restaurados se colocan en las carpetas creadas de nuevo.

Para restaurar los recursos de la carpeta Papelera a las carpetas desde las que se eliminaron, haga lo siguiente:

1. En la parte inferior del panel Biblioteca de recursos, seleccione la **[!UICONTROL Papelera]** para abrir la carpeta Papelera.
1. Seleccione el recurso o los recursos que desea restaurar.
1. Ir a **[!UICONTROL Archivo]** > **[!UICONTROL Restaurar desde papelera]**.

## Eliminación permanente de recursos desde la carpeta Papelera {#permanently-deleting-assets-in-the-trash-folder}

Al eliminar recursos en la carpeta Papelera, éstos se eliminan de forma permanente. Los recursos se eliminan de forma automática de la carpeta Papelera después de siete días.

Puede eliminar permanentemente los recursos de la carpeta Papelera seleccionando la **[!UICONTROL Papelera]** icono. En la página Papelera, realice una de las acciones siguientes:

* **Eliminación de recursos individuales**: puede eliminar recursos de forma permanente. Seleccione los recursos que desee y haga clic en **[!UICONTROL Archivo]** > **[!UICONTROL Vaciar de papelera]**.

* **Eliminando todos los recursos**: Vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Vaciar papelera]**.

>[!MORELIKETHIS]
>
>* [Eliminar recursos](moving-renaming-deleting-assets.md#delete_assets)
