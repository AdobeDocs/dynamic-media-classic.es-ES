---
title: Configurar ajustes preestablecidos del visor de catálogos electrónicos
description: Obtenga información sobre cómo configurar ajustes preestablecidos del visor de catálogos electrónicos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:57:04.669Z'
TQID: 'https://experienceleague.adobe.com/Ej7QeFT62FLz2hWS2w-ll2H9m2pkHXlMSJJDJTsgERg'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: dbe8354bb3a9240d20af51249b4b61e2544120bd
workflow-type: tm+mt
source-wordcount: 464
ht-degree: 12%

---

# Configurar ajustes preestablecidos del visor de catálogos electrónicos{#setting-up-ecatalog-viewer-presets}

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo, el comportamiento y el aspecto de los visores de catálogos electrónicos. Adobe Dynamic Media Classic incluye ajustes preestablecidos del visor de catálogos electrónicos, y puede crear ajustes preestablecidos personalizados si tiene acceso de administrador.

Para crear un ajuste preestablecido, puede crear un nuevo ajuste preestablecido o empezar con un ajuste preestablecido del visor de catálogos electrónicos proporcionado por Adobe Dynamic Media Classic y guardarlo con un nombre nuevo. Para presentar el material impreso en los colores de su empresa y definir el estilo, puede crear sus propios ajustes preestablecidos de visualizador de catálogos electrónicos.

Los ajustes preestablecidos del visualizador de catálogos electrónicos ofrecen muchas opciones para la navegación de páginas, el zoom, la búsqueda y la selección de &quot;temas&quot;. El aspecto de estos controles y el modo en que aparece el visor dependen de la elección de los ajustes preestablecidos del visor de catálogos electrónicos.

**Para configurar un ajuste preestablecido de visor de catálogo electrónico (debe tener acceso de administrador):**

1. En la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visor]**.
1. En la pantalla Ajustes preestablecidos del visor, cree un ajuste preestablecido del visor de catálogo electrónico creando uno nuevo o empezando desde uno existente:

   * **Crear un ajuste preestablecido de visor de catálogo electrónico**: seleccione **[!UICONTROL Agregar]**. En el cuadro de diálogo Agregar ajuste preestablecido de visor, elija una plataforma, elija Visor de catálogo electrónico y, a continuación, seleccione **[!UICONTROL Agregar]**.

   * **Editar un ajuste preestablecido de visor de catálogo electrónico**: seleccione un ajuste preestablecido de visor de catálogo electrónico y, a continuación, seleccione **[!UICONTROL Editar]**. Seleccione **[!UICONTROL Guardar como]** cuando termine de crear el ajuste preestablecido.

1. En la página `Configure Viewer`, escriba un nombre para el ajuste preestablecido del visor de catálogos electrónicos.
1. En la página `Configure Viewer`, defina las opciones que desee.

   Seleccione el icono **[!UICONTROL Info Tip]** junto a la opción si desea leer su descripción.

   La página Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. (Opcional) En la **[!UICONTROL Configuración del panel de información]**, la opción **[!UICONTROL URL del servidor de información]** puede incluir los siguientes tokens especiales que el visor sustituye.

   | Distintivo | Se sustituye por | Notas |
   | --- | --- | --- |
   | `$1$` | valor rollover_key | El identificador de elemento del elemento `<area>` del mapa. |
   | `$2$` | frame | El número de secuencia del cuadro que se muestra actualmente en el conjunto de imágenes. |
   | `$3$` | raíz de imagen | El primer elemento de ruta del primer elemento especificado en el comando de imagen (normalmente el ID del catálogo de imágenes de la entrada del catálogo en la que se especifica el conjunto de imágenes). |

1. (Opcional) En la **[!UICONTROL Configuración del panel de información]**, en el cuadro **[!UICONTROL Plantilla de respuesta]**, escriba el texto que desea que aparezca si Adobe Dynamic Media Classic encuentra un error al recuperar la información de un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y de catálogo electrónico pero no un identificador de rollover, aparecerá este mensaje.

>[!NOTE]
>
>Para utilizar esta plantilla de respuesta en lugar de la plantilla definida en el propio catálogo electrónico, agregue `fmt=1` al final de la dirección URL del servidor de información. Por ejemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Seleccione **[!UICONTROL Guardar]**.
1. Seleccione **[!UICONTROL Predeterminado]** para que el ajuste preestablecido del visor de catálogos electrónicos que ha creado se utilice para mostrar los catálogos electrónicos en su página web.

Para eliminar un ajuste preestablecido de visor de catálogo electrónico, selecciónelo en la pantalla Ajustes preestablecidos de visor y seleccione **[!UICONTROL Eliminar]**.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)
