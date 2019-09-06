---
title: Desplazamiento, cambio de nombre y eliminación de recursos
seo-title: Desplazamiento, cambio de nombre y eliminación de recursos
description: nulo
seo-description: Obtenga información sobre cómo mover, renombrar y eliminar recursos.
uuid: deff 6521-0 ad 0-4 db 9-b 4 e 0-e 3211 ff 97740
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: 1 c 9 e 29 f 0-3083-4 d 22-a 439-2 a 01 faf 59683
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Desplazamiento, cambio de nombre y eliminación de recursos{#moving-renaming-and-deleting-assets}

Puede mover y eliminar recursos, así como cambiarles el nombre, desde el panel Examinar. Además, puede eliminar varios recursos de forma simultánea con un archivo de texto.

## Desplazamiento de recursos {#move-assets}

En el panel Examinar, puede mover recursos a carpetas diferentes.

1. Seleccione los recursos en el panel Examinar y realice una de las siguientes acciones:

   * Busque la carpeta a la que desea mover los recursos en la biblioteca de recursos y arrastre los recursos a esta carpeta.
   * Elija Archivo &gt; Mover, seleccione una carpeta en la ventana Mover recursos y seleccione Mover.

## Cambio de nombre de un recurso {#rename-assets}

Para cambiar el nombre de un recurso:

1. Seleccione el recurso en el panel Examinar y realice una de las siguientes acciones:

   * Seleccione el nombre, escriba un nombre nuevo y pulse Intro o haga clic fuera del nombre.
   * Elija Archivo &gt; Cambiar nombre. Se resaltará el nombre del archivo. Introduzca un nuevo nombre y pulse Intro.

Asegúrese de que el nombre introducido no corresponde al de ningún recurso de Scene7 Publishing System existente.

## Eliminación de recursos {#delete-assets}

Puede eliminar los recursos que seleccione desde el panel Examinar, así como carpetas enteras. Los recursos y carpetas eliminados se mueven a la carpeta Papelera, donde permanecerán durante 7 días antes de ser eliminados de forma permanente.

Al eliminar un recurso, todos los derivados de dicho recurso se eliminarán con él. Por ejemplo, si elimina una imagen para la cual ha creado destinos de zoom, se eliminarán tanto la imagen como los destinos de zoom.

>[!NOTE]
>
>los destinos de zoom, los atributos de imagen y las entradas del historial se eliminarán permanentemente al eliminar los recursos a partir de los que se originaron. No se mueven junto con el recurso a la carpeta Papelera, por lo que no se pueden restaurar desde la papelera.

1. Realice una de las siguientes acciones:

   * Para eliminar uno o más recursos, selecciónelos en el panel Examinar y pulse Suprimir o seleccione Archivo &gt; Eliminar.
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      Al eliminar una carpeta se eliminarán la carpeta, los recursos que contenga y los recursos que haya en las subcarpetas.

>[!NOTE]
>
>Dynamic Media Classic recomienda sobrescribir los archivos de recursos en lugar de eliminarlos si el motivo para eliminar un archivo de recurso es reemplazarlo por otro con el mismo nombre.

## Eliminación de varios recursos con un archivo de texto {#delete-multiple-assets-with-a-text-file}

Para eliminar varios recursos a la vez en la biblioteca de recursos, puede enumerar los recursos que desea eliminar en un archivo de texto y enviar la lista a Dynamic Media Classic.

Cree una lista con los ID de Scene7 Publishing System y guárdela como un archivo de texto (.txt). Cada ID de Scene7 Publishing System debe estar en una línea diferente (seguido de un salto de línea).

Después de crear la lista, siga estos pasos para eliminar los recursos:

1. Seleccione Archivo &gt; Lista de recursos para eliminar.
1. En el cuadro de diálogo Lista de recursos para eliminar, busque el archivo de texto (o escriba la ruta) con la lista de recursos que desea eliminar.
1. Haga clic en el botón Eliminar.

Al eliminar recursos con un archivo de texto, si algún ID de Scene 7 Publishing System no se encuentra en la lista, aparece un mensaje que le permite saber que Dynamic Media Classic es «No se pueden validar estas entradas en la lista: " junto con la lista de entradas. Sin embargo, Dynamic Media Classic no generará un error en la pantalla Trabajo.

>[!MORELIKETHIS]
>
>* [Selección de recursos en el panel Examinar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparación de los recursos y las carpetas para la carga](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restauración de recursos desde la carpeta Papelera](trash-folder.md#restoring_assets_from_the_trash_folder)

