---
title: Mover, cambiar el nombre y eliminar recursos
description: Obtenga información sobre cómo mover, cambiar el nombre y eliminar recursos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 17%

---

# Mover, cambiar el nombre y eliminar recursos{#moving-renaming-and-deleting-assets}

Puede mover, cambiar el nombre y eliminar recursos desde el panel Examinar. Además, puede eliminar varios recursos de forma simultánea con un archivo de texto.

## Desplazamiento de recursos {#move-assets}

Puede mover recursos a diferentes carpetas en el panel Examinar.

**Para mover recursos:**

1. Seleccione el recurso o los recursos en el panel Examinar y realice una de las siguientes acciones:

   * Muestre la carpeta a la que desea mover los recursos en la Biblioteca de recursos y arrastre los recursos a la carpeta.
   * Vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Mover]**, seleccione una carpeta en la ventana Mover Assets y seleccione **[!UICONTROL Mover]**.

## Cambio de nombre de un recurso {#rename-assets}

1. Seleccione el recurso en el panel Examinar y realice una de las siguientes acciones:

   * Seleccione el nombre, escriba un nombre nuevo y presione **[!UICONTROL Intro]** o seleccione un nombre distinto.
   * Vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Cambiar nombre]**. Se resaltará el nombre del archivo. Escriba un nombre nuevo y presione **[!UICONTROL Entrar]**. Asegúrese de no introducir el nombre de un recurso de Adobe Dynamic Media Classic existente.

## Eliminación de recursos {#delete-assets}

Puede eliminar los recursos seleccionados en el panel Examinar y eliminar carpetas completas. Los recursos y carpetas eliminados se mueven a la carpeta Papelera, donde permanecerán durante 7 días antes de ser eliminados de forma permanente.

Al eliminar un recurso, también se eliminan todos los recursos derivados de él. Por ejemplo, al eliminar una imagen para la que ha creado Destinos de zoom, se eliminan los Destinos de zoom junto con la imagen.

los destinos de zoom, los atributos de imagen y las entradas del historial se eliminarán permanentemente al eliminar los recursos a partir de los que se originaron. No se mueven junto con el recurso a la carpeta Papelera, por lo que no se pueden restaurar desde la papelera.

>[!IMPORTANT]
>
>La eliminación en lote es una operación intensiva. Asegúrese de ejecutar las eliminaciones masivas secuencialmente en lugar de como operaciones de eliminación simultáneas y pesadas. Adobe recomienda limitar las operaciones de eliminación a 5000 o menos eliminaciones de recursos por hora. Cualquier número mayor de 5000 por hora puede limitar la velocidad.

**Para eliminar recursos:**

1. Realice una de las siguientes acciones:

   * Para eliminar uno o más recursos, selecciónelos en el panel Examinar y presione **[!UICONTROL Eliminar]** o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]**.
   * Para eliminar una carpeta, selecciónela en la Biblioteca de recursos y seleccione **[!UICONTROL Quitar carpeta]**.

     Al eliminar una carpeta, se elimina la carpeta, todos sus recursos y todos los de sus subcarpetas.

Adobe Dynamic Media Classic recomienda sobrescribir los archivos de recursos en lugar de eliminarlos si el motivo para eliminar un archivo de recursos es reemplazarlo por otro con el mismo nombre.

## Eliminación de varios recursos con un archivo de texto {#delete-multiple-assets-with-a-text-file}

Para eliminar muchos recursos a la vez en la biblioteca de recursos, puede enumerar los recursos que desea eliminar en un archivo de texto y enviar la lista a Adobe Dynamic Media Classic.

Cree la lista de Adobe Dynamic Media Classic ID y guárdela como un archivo de texto (.txt). Cada ID de Adobe Dynamic Media Classic debe estar en su propia línea (seguida de una devolución fuerte).

Después de crear la lista, siga estos pasos para eliminar los recursos:

1. Vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar lista de recursos]**.
1. En el cuadro de diálogo **[!UICONTROL Lista de recursos eliminados]**, escriba la ruta de acceso al archivo de texto con la lista de recursos que desea eliminar.
1. Seleccione **[!UICONTROL Eliminar]**.

Cuando se eliminan recursos con un archivo de texto, si algún Adobe Dynamic Media Classic ID no está en la lista, se muestra el mensaje &quot;No se pueden validar estas entradas en la lista:&quot;. También se muestra la lista de entradas. Sin embargo, Adobe Dynamic Media Classic no genera un error en la página Trabajo.

>[!MORELIKETHIS]
>
>* [Seleccionar recursos en el panel Examinar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Prepare sus recursos y carpetas para la carga](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restaurar recursos desde la carpeta Papelera](trash-folder.md#restoring_assets_from_the_trash_folder)
