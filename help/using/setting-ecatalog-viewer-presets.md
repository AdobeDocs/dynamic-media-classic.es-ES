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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# Configurar ajustes preestablecidos del visor de catálogos electrónicos{#setting-up-ecatalog-viewer-presets}

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo, el comportamiento y el aspecto de los visores de catálogos electrónicos. Adobe Dynamic Media Classic proporciona ajustes preestablecidos del visor de catálogos electrónicos, y también puede crear los suyos propios si es administrador.

Para crear un ajuste preestablecido, puede empezar desde cero o con un ajuste preestablecido del visor de catálogos electrónicos proporcionado por Adobe Dynamic Media Classic y guardarlo con un nuevo nombre. Puede crear sus propios ajustes preestablecidos de visor para presentar el material impreso en los colores de la empresa y establecer el tono.

Los ajustes preestablecidos del visor de catálogos electrónicos ofrecen muchas opciones para ir de página en página, ampliar, buscar y elegir &quot;aspectos&quot;. El aspecto de estos controles y el modo en que aparecerá el Visor dependen de la elección de los Ajustes preestablecidos del Visor de catálogos electrónicos.

Siga estos pasos para poder crear un ajuste preestablecido de visualizador de catálogos electrónicos (debe ser administrador):

1. En la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes preestablecidos de visor]**.
1. En la pantalla Ajustes preestablecidos de visor, cree un ajuste preestablecido de visor de catálogos electrónicos desde cero o a partir de un ajuste preestablecido de visor de catálogos electrónicos existente:

   * **Crear un ajuste preestablecido de visor de catálogos electrónicos**: Seleccionar **[!UICONTROL Añadir]**. En el cuadro de diálogo Agregar ajuste preestablecido de visor, elija una plataforma, elija Visor de catálogos electrónicos y, a continuación, seleccione **[!UICONTROL Añadir]**.

   * **Editar un ajuste preestablecido del visor de catálogos electrónicos**: seleccione un ajuste preestablecido del visor de catálogos electrónicos y, a continuación, seleccione **[!UICONTROL Editar]**. Seleccionar **[!UICONTROL Guardar como]** después de terminar de crear el ajuste preestablecido.

1. En el `Configure Viewer` , introduzca un nombre para el ajuste preestablecido del visor de catálogos electrónicos.
1. En el `Configure Viewer` , establezca las opciones que desee.

   seleccione el **[!UICONTROL Sugerencia de información]** junto a la opción si desea leer su descripción.

   La página Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. (Opcional) En el **[!UICONTROL Configuración del panel de información]**, el **[!UICONTROL URL de servidor de información]** Esta opción puede incluir los siguientes tokens especiales, que el visor sustituye:

   | Distintivo | Se sustituye por | Notas |
   | --- | --- | --- |
   | `$1$` | valor rollover_key | El identificador de elemento del `<area>` del mapa. |
   | `$2$` | frame | El número de secuencia del cuadro que se muestra actualmente en el conjunto de imágenes. |
   | `$3$` | raíz de imagen | El primer elemento de ruta del primer elemento especificado en el comando de imagen (normalmente el ID del catálogo de imágenes de la entrada del catálogo en la que se especifica el conjunto de imágenes). |

1. (Opcional) En el **[!UICONTROL Configuración del panel de información]**, en el **[!UICONTROL Plantilla de respuesta]** , escriba el texto que desea que aparezca si Adobe Dynamic Media Classic encuentra un error al recuperar la información de un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de catálogo electrónico, pero ningún identificador rollover, aparecerá este mensaje para el usuario.

>[!NOTE]
>
>Para utilizar esta plantilla de respuesta en lugar de la plantilla definida en el propio catálogo electrónico, añada `fmt=1` al final de la URL del servidor de información. Por ejemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Seleccionar **[!UICONTROL Guardar]**.
1. Seleccionar **[!UICONTROL Predeterminado]** de forma que el ajuste preestablecido del visor de catálogos electrónicos que ha creado sea el que se utiliza para mostrar los catálogos electrónicos en su página web.

Para eliminar un ajuste preestablecido del visor de catálogos electrónicos, selecciónelo en la pantalla Ajustes preestablecidos del visor y seleccione **[!UICONTROL Eliminar]**.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)
