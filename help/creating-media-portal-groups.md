---
title: Crear y administrar grupos de Media Portal
description: Obtenga información sobre cómo crear y administrar grupos de Media Portal en Dynamic Media Classic.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 57%

---

# Crear y administrar grupos de Media Portal{#creating-and-managing-media-portal-groups}

Los *grupos* están pensados para ayudarle a administrar los usuarios de Media Portal. Para poder acceder a un recurso, un usuario debe ser miembro de al menos un grupo que tenga permiso de acceso a dicho recurso. Cuando se agrega un usuario, se le asigna a un grupo o más. Al hacerlo, se le otorga acceso al usuario a las carpetas que se han asignado al grupo. También puede elegir a qué ajustes preestablecidos de imagen podrá acceder un grupo determinado.

## Usar grupos para restringir el acceso a carpetas, recursos y ajustes preestablecidos de imagen {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Para otorgar permiso a diferentes niveles, cree grupos. Por cada grupo, puede asignar permisos de lectura, escritura y eliminación de las diferentes carpetas y recursos de las carpetas. Asimismo, puede decidir a qué ajustes preestablecidos de imagen podrá acceder el grupo. A continuación, asigne usuarios a los grupos. Un usuario puede ser miembro de varios grupos. El concepto de grupo le permite disponer de flexibilidad para asignar acceso a conjuntos limitados del contenido total.

Si no concede específicamente a un grupo permiso para un recurso o carpeta, ese recurso o carpeta hereda los permisos que asignó a su carpeta principal (la carpeta situada encima de él en la jerarquía de carpetas). Conceda permisos a la carpeta principal para asegurarse de que todas las carpetas secundarias tienen los mismos derechos que la principal.

>[!NOTE]
>
>Un usuario puede ser miembro de varios grupos. Cuando un usuario pertenece a dos grupos con permisos de acceso diferentes a una carpeta, el usuario recibe el permiso mayor. 

## Adición de un grupo {#adding-a-group}

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de Media Portal]** > **[!UICONTROL Grupos]**.
1. Seleccione **[!UICONTROL Add]**.
1. En el cuadro de diálogo Agregar grupo, escriba un nombre para el grupo en el cuadro Nombre del grupo y, a continuación, seleccione **[!UICONTROL Agregar grupo]**.
1. Si lo desea, puede seleccionar las casillas de verificación que hay junto a los nombres de los usuarios para agregar usuarios al grupo nuevo.
1. Si desea especificar permisos de acceso ahora, seleccione la pestaña **[!UICONTROL Permisos de acceso a recursos]** y, a continuación, especifique las opciones que desee.

   Consulte [Establecimiento de permisos de acceso a recursos para un grupo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Si desea elegir qué ajustes preestablecidos de imagen están disponibles para el grupo, seleccione la pestaña **[!UICONTROL Permisos de acceso a ajustes preestablecidos de imagen]** y seleccione los ajustes preestablecidos de imagen que el grupo puede utilizar.

   Consulte [Elección de permisos de acceso a ajustes preestablecidos de imagen para un grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Seleccione **[!UICONTROL Cerrar]**.

## Establecimiento de permisos de acceso a recursos para un grupo {#establishing-asset-access-permissions-for-a-group}

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de Media Portal]** > **[!UICONTROL Grupos]**.
1. En la página de lista de grupos, realice una de las siguientes acciones:

   * Para agregar un grupo y especificar permisos, seleccione **[!UICONTROL Agregar]**. En el cuadro de diálogo Agregar grupo, escriba un nombre para el grupo, seleccione **[!UICONTROL Agregar grupo]** y agregue usuarios al grupo.
   * Para editar los permisos de un grupo, seleccione el grupo y, a continuación, seleccione **[!UICONTROL Editar]**.

1. En el cuadro de diálogo Agregar grupo o Editar grupo, seleccione la pestaña **[!UICONTROL Permisos de acceso a recursos]**. En la parte derecha de la ficha aparecen cuadros para conceder los permisos de lectura, escritura y eliminación de capetas y recursos. Puede expandir y contraer las carpetas y subcarpetas del panel izquierdo.
1. Para asignar derechos a carpetas o recursos individuales, seleccione la carpeta en el panel izquierdo. El contenido de la carpeta aparece en el panel derecho. Para asignar derechos al grupo, seleccione los cuadros de los archivos o carpetas correspondientes en el panel derecho.

   Esta tabla relaciona diferentes tareas con los permisos de lectura, escritura y eliminación.

   | Tarea | Leer | Escribir | Eliminar |
   | --- | --- | --- | --- |
   | Examinar carpetas y archivos | X |  |  |
   | Editar archivos (recortar, enfocar, ajustar)  |  | X |  |
   | Cambiar nombres de archivo |  | X |  |
   | Mover archivos a otras carpetas |  | X |  |
   | Cambiar el nombre de los archivos |  | X |  |
   | Eliminar archivos |  |  | X |

1. Seleccione **[!UICONTROL Cerrar]**.

>[!NOTE]
>
>los derechos de acceso se establecen cuando se selecciona un cuadro. Cuando asigna derechos a una carpeta, sus subcarpetas y todos los archivos que están dentro reciben los mismos derechos que la carpeta principal. No obstante, puede especificar derechos diferentes para subcarpetas y archivos de recursos independientes.

## Elección de permisos de acceso a ajustes preestablecidos de imagen para un grupo {#choosing-image-preset-access-permissions-for-a-group}

Elija los permisos de acceso a ajustes preestablecidos de imagen para un grupo si desea especificar los ajustes preestablecidos de imagen disponibles para los miembros de un grupo cuando se exportan recursos con Media Portal.

Consulte también [Especificar las opciones de exportación disponibles para los usuarios de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**Para elegir los permisos de acceso de ajustes preestablecidos de imagen para un grupo:**

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de Media Portal]** > **[!UICONTROL Grupos]**.
1. En la página de lista de grupos, realice una de las siguientes acciones:

   * Para agregar un grupo y especificar qué ajustes preestablecidos de imagen están disponibles, seleccione **[!UICONTROL Agregar]**. En el cuadro de diálogo Agregar grupo, escriba un nombre para el grupo, seleccione **[!UICONTROL Agregar grupo]** y agregue usuarios al grupo.
   * Para editar las opciones de ajustes preestablecidos de imagen de un grupo, seleccione el grupo y, a continuación, seleccione **[!UICONTROL Editar]**.

1. En el cuadro de diálogo Agregar grupo o Editar grupo, seleccione la pestaña **[!UICONTROL Permisos de acceso a ajustes preestablecidos de imagen]**.
1. Para especificar qué ajustes preestablecidos están disponibles para los usuarios de Media Portal cuando exportan recursos, seleccione o anule la selección de Ajustes preestablecidos de imagen.
1. Seleccione **[!UICONTROL Cerrar]**.

## Edición y eliminación de grupos {#edit-and-delete-groups}

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de Media Portal]** > **[!UICONTROL Grupos]**.
1. En la página de lista de grupos, seleccione un grupo y edítelo o elimínelo.

   **Editar un grupo** : seleccione  **[!UICONTROL Editar]** y, a continuación, elija opciones en el cuadro de diálogo Editar grupo.

   **Eliminar un grupo** : seleccione  **[!UICONTROL Eliminar]**.
