---
title: Administrar la carpeta Papelera
description: Obtenga información sobre cómo restaurar y eliminar permanentemente recursos en la carpeta Papelera de Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:15:24.015Z'
TQID: 'https://experienceleague.adobe.com/5XOu6T0n7zssUzXgQXushja4DJBSHs8-0-2h2Ao1L20'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
    internal-label: Dynamic Media Classic
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: cab998ae67e6e2d3df94f183437a38fef08c987b
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 23%
---
# Administrar la carpeta Papelera{#managing-the-trash-folder}

Los elementos que elimine de Adobe Dynamic Media Classic se moverán a la papelera. Estos elementos eliminados permanecen en esta carpeta durante un máximo de siete días hasta que se restauran o se eliminan de forma permanente. Puede examinar los elementos eliminados seleccionando el icono **[!UICONTROL Papelera]** en la parte inferior de la Biblioteca de recursos y viendo los elementos en la página Papelera.

>[!IMPORTANT]
>
>La carpeta Papelera no es compatible cuando Dynamic Media está integrado con Adobe Experience Manager. En estos entornos, los recursos que elimine se eliminarán permanentemente y no se moverán a la carpeta Papelera. <!-- CQDOC-23176 -->

Todos los usuarios pueden restaurar elementos desde la carpeta Papelera y colocarlos en la carpeta en que se encontraban antes de ser eliminados. Todos los usuarios pueden vaciar la carpeta Papelera y eliminar su contenido.

Al eliminar elementos de la papelera, se eliminan permanentemente los elementos de Adobe Dynamic Media Classic; los elementos eliminados de la papelera ya no se pueden restaurar. Si desea obtener información sobre la configuración de notificaciones destinadas a los administradores de la empresa cuando los recursos estén a punto de eliminarse automáticamente de la papelera, consulte [Configuración general de la aplicación](application-setup.md#general_settings).

>[!NOTE]
>
>Los Assets que se hayan movido a la papelera seguirán registrados en Adobe Dynamic Media Classic. Por ejemplo, supongamos que intenta cargar un archivo que tiene el mismo nombre que un archivo eliminado en la carpeta Papelera. Adobe Dynamic Media Classic trata el recurso que desea cargar como un recurso duplicado. En tal caso, se anexa un número a su nombre.

## Acerca de la carpeta Papelera {#about-the-trash-folder}

Si elimina un recurso en una carpeta, éste se colocará en la carpeta Papelera. Al eliminar un elemento y moverlo a la carpeta Papelera, ocurre lo siguiente:

* El elemento no se puede publicar. Incluso si el elemento se marcó para su publicación cuando lo eliminó, no se publica.
* El elemento permanece en la carpeta Papelera hasta que se restaure, pasen siete días o alguien elija el comando **[!UICONTROL Vaciar papelera]**. Después de siete días, una operación de eliminación automática elimina permanentemente el elemento.

## Restaurar recursos desde la carpeta Papelera {#restoring-assets-from-the-trash-folder}

No es necesario que la persona que eliminó un recurso lo restaure; cualquier persona puede restaurar recursos desde la carpeta Papelera. Los recursos restaurados se colocan en las carpetas de donde se eliminaron. Si estas carpetas ya no existen, Adobe Dynamic Media Classic las vuelve a crear y los recursos restaurados se colocan en las carpetas creadas de nuevo.

Para restaurar los recursos de la carpeta Papelera a las carpetas desde las que se eliminaron, haga lo siguiente:

1. En la parte inferior del panel Biblioteca de recursos, seleccione el icono **[!UICONTROL Papelera]** para abrir la carpeta Papelera.
1. Seleccione el recurso o los recursos que desea restaurar.
1. Haga clic en **[!UICONTROL Archivo]** > **[!UICONTROL Restaurar desde papelera]**.

## Eliminar permanentemente recursos de la carpeta Papelera {#permanently-deleting-assets-in-the-trash-folder}

Al eliminar recursos en la carpeta Papelera, éstos se eliminan de forma permanente. Los recursos se eliminan de forma automática de la carpeta Papelera después de siete días.

Puede eliminar permanentemente los recursos de la carpeta Papelera seleccionando el icono **[!UICONTROL Papelera]**. En la página Papelera, realice una de las acciones siguientes:

* **Eliminando recursos individuales**: puede eliminar recursos de forma permanente. Seleccione los recursos que desee y haga clic en **[!UICONTROL Archivo]** > **[!UICONTROL Vaciar la papelera]**.

* **Eliminando todos los recursos**: Haga clic en **[!UICONTROL Archivo]** > **[!UICONTROL Vaciar la papelera]**.

>[!MORELIKETHIS]
>
>* [Eliminar recursos](moving-renaming-deleting-assets.md#delete_assets)
