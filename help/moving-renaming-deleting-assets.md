---
title: Mover, cambiar el nombre y eliminar recursos
description: Obtenga información sobre cómo mover, cambiar el nombre y eliminar recursos en Adobe Dynamic Media Classic.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 37%

---

# Mover, cambiar el nombre y eliminar recursos{#moving-renaming-and-deleting-assets}

Puede mover y eliminar recursos, así como cambiarles el nombre, desde el panel Examinar. Además, puede eliminar varios recursos de forma simultánea con un archivo de texto.

## Desplazamiento de recursos {#move-assets}

En el panel Examinar, puede mover recursos a carpetas diferentes.

1. Seleccione los recursos en el panel Examinar y realice una de las siguientes acciones:

   * Busque la carpeta a la que desea mover los recursos en la biblioteca de recursos y arrastre los recursos a esta carpeta.
   * Vaya a **[!UICONTROL File]** > **[!UICONTROL Move]**, seleccione una carpeta en la ventana Mover recursos y seleccione **[!UICONTROL Mover]**.

## Cambio de nombre de un recurso {#rename-assets}

1. Seleccione el recurso en el panel Examinar y realice una de las siguientes acciones:

   * Seleccione el nombre, escriba un nuevo nombre y pulse **[!UICONTROL Enter]** o seleccione fuera del nombre.
   * Vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Cambiar nombre]**. Se resaltará el nombre del archivo. Introduzca un nuevo nombre y pulse **[!UICONTROL Enter]**.

Asegúrese de no introducir el nombre de un recurso de Dynamic Media Classic de Adobe existente.

## Eliminación de recursos {#delete-assets}

Puede eliminar los recursos seleccionados en el panel Examinar y eliminar carpetas enteras. Los recursos y carpetas eliminados se mueven a la carpeta Papelera, donde permanecerán durante 7 días antes de ser eliminados de forma permanente.

Al eliminar un recurso, todos los derivados de dicho recurso se eliminarán con él. Por ejemplo, si elimina una imagen para la cual ha creado destinos de zoom, se eliminarán tanto la imagen como los destinos de zoom.

>[!NOTE]
>
>los destinos de zoom, los atributos de imagen y las entradas del historial se eliminarán permanentemente al eliminar los recursos a partir de los que se originaron. No se mueven junto con el recurso a la carpeta Papelera, por lo que no se pueden restaurar desde la papelera.

1. Realice una de las siguientes acciones:

   * Para eliminar uno o varios recursos, seleccione los recursos en el panel Examinar y pulse **[!UICONTROL Eliminar]** o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]**.
   * Para eliminar una carpeta, seleccione la carpeta en la biblioteca de recursos y seleccione **[!UICONTROL Quitar carpeta]**.

      Al eliminar una carpeta, se eliminan la carpeta, todos los recursos de la carpeta y todos los recursos de las subcarpetas.

>[!NOTE]
>
>Adobe Dynamic Media Classic recomienda sobrescribir los archivos de recursos en lugar de eliminarlos si el motivo para eliminarlos es reemplazarlos por otro con el mismo nombre.

## Eliminación de varios recursos con un archivo de texto {#delete-multiple-assets-with-a-text-file}

Para eliminar muchos recursos a la vez en toda la biblioteca de recursos, puede enumerarlos en un archivo de texto y enviarlos a Adobe Dynamic Media Classic.

Cree la lista de ID de Dynamic Media Classic de Adobe y guárdela como un archivo de texto (.txt). Cada ID de Dynamic Media Classic de Adobe debe estar en su propia línea (seguido de un retorno duro).

Después de crear la lista, siga estos pasos para eliminar los recursos:

1. Vaya a **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**.
1. En el cuadro de diálogo Eliminar lista de recursos, busque o escriba la ruta al archivo de texto con la lista de recursos que desee eliminar.
1. Seleccione **[!UICONTROL Delete]**.

Cuando elimine recursos con un archivo de texto, si algún ID de Dynamic Media Classic de Adobe no está en la lista, se mostrará el mensaje &quot;No se pueden validar estas entradas en la lista:&quot; y la lista de entradas. Sin embargo, Adobe Dynamic Media Classic no genera un error en la página Trabajo.

>[!MORELIKETHIS]
>
>* [Seleccionar recursos en el panel Examinar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparar los recursos y las carpetas para su carga](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restaurar recursos desde la carpeta Papelera](trash-folder.md#restoring_assets_from_the_trash_folder)

