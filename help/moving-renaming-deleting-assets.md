---
title: Desplazamiento, cambio de nombre y eliminación de recursos
seo-title: Desplazamiento, cambio de nombre y eliminación de recursos
description: nulo
seo-description: Obtenga información sobre cómo mover, cambiar el nombre y eliminar recursos.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 66%

---


# Desplazamiento, cambio de nombre y eliminación de recursos{#moving-renaming-and-deleting-assets}

Puede mover y eliminar recursos, así como cambiarles el nombre, desde el panel Examinar. Además, puede eliminar varios recursos de forma simultánea con un archivo de texto.

## Desplazamiento de recursos {#move-assets}

En el panel Examinar, puede mover recursos a carpetas diferentes.

1. Seleccione los recursos en el panel Examinar y realice una de las siguientes acciones:

   * Busque la carpeta a la que desea mover los recursos en la biblioteca de recursos y arrastre los recursos a esta carpeta.
   * Elija Archivo > Mover, seleccione una carpeta en la ventana Mover recursos y seleccione Mover.

## Cambio de nombre de un recurso {#rename-assets}

Para cambiar el nombre de un recurso:

1. Seleccione el recurso en el panel Examinar y realice una de las siguientes acciones:

   * Seleccione el nombre, escriba un nombre nuevo y pulse Intro o haga clic fuera del nombre.
   * Elija Archivo > Cambiar nombre. Se resaltará el nombre del archivo. Introduzca un nuevo nombre y pulse Intro.

Asegúrese de no introducir el nombre de un recurso de Dynamic Media Classic existente.

## Eliminación de recursos {#delete-assets}

Puede eliminar los recursos que seleccione desde el panel Examinar, así como carpetas enteras. Los recursos y carpetas eliminados se mueven a la carpeta Papelera, donde permanecerán durante 7 días antes de ser eliminados de forma permanente.

Al eliminar un recurso, todos los derivados de dicho recurso se eliminarán con él. Por ejemplo, si elimina una imagen para la cual ha creado destinos de zoom, se eliminarán tanto la imagen como los destinos de zoom.

>[!NOTE]
>
>los destinos de zoom, los atributos de imagen y las entradas del historial se eliminarán permanentemente al eliminar los recursos a partir de los que se originaron. No se mueven junto con el recurso a la carpeta Papelera, por lo que no se pueden restaurar desde la papelera.

1. Realice una de las siguientes acciones:

   * Para eliminar uno o más recursos, selecciónelos en el panel Examinar y pulse Suprimir o seleccione Archivo > Eliminar.
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      Al eliminar una carpeta se eliminarán la carpeta, los recursos que contenga y los recursos que haya en las subcarpetas.

>[!NOTE]
>
>Dynamic Media Classic recomienda sobrescribir los archivos de recursos en lugar de eliminarlos si el motivo para eliminarlos es reemplazarlos por otro con el mismo nombre.

## Eliminación de varios recursos con un archivo de texto {#delete-multiple-assets-with-a-text-file}

Para eliminar varios recursos a la vez en toda la biblioteca de recursos, puede realizar la lista de los recursos que desee eliminar en un archivo de texto y enviar la lista a Dynamic Media Classic.

Cree la lista de Dynamic Media Classic ID y guárdela como archivo de texto (.txt). Cada ID de Dynamic Media Classic debe estar en su propia línea (seguido de un salto de línea).

Después de crear la lista, siga estos pasos para eliminar los recursos:

1. Seleccione Archivo > Lista de recursos para eliminar.
1. En el cuadro de diálogo Lista de recursos para eliminar, busque el archivo de texto (o escriba la ruta) con la lista de recursos que desea eliminar.
1. Haga clic en el botón Eliminar.

Al eliminar recursos con un archivo de texto, si no hay ningún ID de Dynamic Media Classic en la lista, se muestra un mensaje que le permite saber que Dynamic Media Classic es &quot;No se pueden validar estas entradas en la lista:&quot; junto con la lista de entradas. Sin embargo, Dynamic Media Classic no generará un error en la pantalla Trabajo.

>[!MORELIKETHIS]
>
>* [Selección de recursos en el panel Examinar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparación de los recursos y las carpetas para la carga](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restauración de recursos desde la carpeta Papelera](trash-folder.md#restoring_assets_from_the_trash_folder)

