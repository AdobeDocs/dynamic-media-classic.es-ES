---
title: Mover, cambiar el nombre y eliminar recursos
description: Obtenga información sobre cómo mover, cambiar el nombre y eliminar recursos en Adobe Dynamic Media Classic.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# Mover, cambiar el nombre y eliminar recursos{#moving-renaming-and-deleting-assets}

Puede mover y eliminar recursos, así como cambiarles el nombre, desde el panel Examinar. Además, puede eliminar varios recursos de forma simultánea con un archivo de texto.

## Desplazamiento de recursos {#move-assets}

En el panel Examinar, puede mover recursos a carpetas diferentes.

**Para mover recursos:**

1. Seleccione los recursos en el panel Examinar y realice una de las siguientes acciones:

   * Muestre la carpeta a la que desea mover los recursos en la Biblioteca de recursos y arrastre los recursos a la carpeta.
   * Ir a **[!UICONTROL Archivo]** > **[!UICONTROL Mover]**, seleccione una carpeta en la ventana Mover recursos y seleccione **[!UICONTROL Mover]**.

## Cambio de nombre de un recurso {#rename-assets}

1. Seleccione el recurso en el panel Examinar y realice una de las siguientes acciones:

   * Seleccione el nombre, escriba un nombre nuevo y pulse **[!UICONTROL Entrar]** o seleccione fuera del nombre.
   * Ir a **[!UICONTROL Archivo]** > **[!UICONTROL Cambiar nombre]**. Se resaltará el nombre del archivo. Introduzca un nombre nuevo y pulse **[!UICONTROL Entrar]**. Asegúrese de no introducir el nombre de un recurso de Adobe Dynamic Media Classic existente.

## Eliminación de recursos {#delete-assets}

Puede eliminar los recursos seleccionados en el panel de exploración y eliminar carpetas completas. Los recursos y carpetas eliminados se mueven a la carpeta Papelera, donde permanecerán durante 7 días antes de ser eliminados de forma permanente.

Al eliminar un recurso, todos los derivados de dicho recurso se eliminarán con él. Por ejemplo, si elimina una imagen para la cual ha creado destinos de zoom, se eliminarán tanto la imagen como los destinos de zoom.

los destinos de zoom, los atributos de imagen y las entradas del historial se eliminarán permanentemente al eliminar los recursos a partir de los que se originaron. No se mueven junto con el recurso a la carpeta Papelera, por lo que no se pueden restaurar desde la papelera.

>[!IMPORTANT]
>
>La eliminación en lote es una operación intensiva. Asegúrese de ejecutar las eliminaciones masivas secuencialmente en lugar de como operaciones de eliminación simultáneas y pesadas. Adobe recomienda limitar las operaciones de eliminación a 5000 o menos eliminaciones de recursos por hora. Cualquier número que sea bueno a 5000 por hora puede causar una limitación de la velocidad.

**Para eliminar recursos:**

1. Realice una de las siguientes acciones:

   * Para eliminar uno o varios recursos, selecciónelos en el panel Examinar y presione **[!UICONTROL Eliminar]** o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]**.
   * Para eliminar una carpeta, selecciónela en la Biblioteca de recursos y seleccione **[!UICONTROL Quitar carpeta]**.

      Al eliminar una carpeta, se elimina la carpeta, todos sus recursos y todos los de sus subcarpetas.

Adobe Dynamic Media Classic recomienda sobrescribir los archivos de recursos en lugar de eliminarlos si el motivo para eliminar un archivo de recursos es reemplazarlo por otro con el mismo nombre.

## Eliminación de varios recursos con un archivo de texto {#delete-multiple-assets-with-a-text-file}

Para eliminar muchos recursos a la vez en la biblioteca de recursos, puede enumerar los recursos que desea eliminar en un archivo de texto y enviar la lista a Adobe Dynamic Media Classic.

Cree la lista de Adobe Dynamic Media Classic ID y guárdela como un archivo de texto (.txt). Cada ID de Adobe Dynamic Media Classic debe estar en su propia línea (seguida de una devolución fuerte).

Después de crear la lista, siga estos pasos para eliminar los recursos:

1. Ir a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar lista de recursos]**.
1. En el cuadro de diálogo Eliminar lista de recursos, examine o escriba la ruta de acceso al archivo de texto con la lista de recursos que desea eliminar.
1. Seleccionar **[!UICONTROL Eliminar]**.

Cuando se eliminan recursos con un archivo de texto, si algún Adobe Dynamic Media Classic ID no está en la lista, se muestra el mensaje &quot;No se pueden validar estas entradas en la lista:&quot;. También se muestra la lista de entradas. Sin embargo, Adobe Dynamic Media Classic no genera un error en la página Trabajo.

>[!MORELIKETHIS]
>
>* [Seleccionar recursos en el panel Examinar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparación de recursos y carpetas para su carga](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restaurar recursos desde la carpeta Papelera](trash-folder.md#restoring_assets_from_the_trash_folder)

