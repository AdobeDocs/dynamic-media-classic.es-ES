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
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# Configurar ajustes preestablecidos del visor de catálogos electrónicos{#setting-up-ecatalog-viewer-presets}

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo, el comportamiento y el aspecto de los visores de catálogos electrónicos. Adobe Dynamic Media Classic proporciona ajustes preestablecidos del visor de catálogos electrónicos, y también puede crear los suyos propios si es administrador.

Para crear un ajuste preestablecido, puede empezar desde cero o con un ajuste preestablecido del visor de catálogos electrónicos proporcionado por Adobe Dynamic Media Classic y guardarlo con un nuevo nombre. Puede crear sus propios ajustes preestablecidos de visor para presentar el material impreso en los colores de la empresa y establecer el tono.

Los ajustes preestablecidos del visor de catálogos electrónicos ofrecen muchas opciones para ir de página en página, ampliar, buscar y elegir &quot;aspectos&quot;. El aspecto de estos controles y el modo en que aparecerá el Visor dependen de la elección de los Ajustes preestablecidos del Visor de catálogos electrónicos.

Siga estos pasos para poder crear un ajuste preestablecido de visualizador de catálogos electrónicos (debe ser administrador):

1. En la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visor]**.
1. En la pantalla Ajustes preestablecidos de visor, cree un ajuste preestablecido de visor de catálogos electrónicos desde cero o a partir de un ajuste preestablecido de visor de catálogos electrónicos existente:

   * **Crear un ajuste preestablecido de visor de catálogo electrónico**: seleccione **[!UICONTROL Agregar]**. En el cuadro de diálogo Agregar ajuste preestablecido de visor, elija una plataforma, elija Visor de catálogo electrónico y, a continuación, seleccione **[!UICONTROL Agregar]**.

   * **Editar un ajuste preestablecido de visor de catálogo electrónico**: seleccione un ajuste preestablecido de visor de catálogo electrónico y, a continuación, seleccione **[!UICONTROL Editar]**. Seleccione **[!UICONTROL Guardar como]** cuando termine de crear el ajuste preestablecido.

1. En la página `Configure Viewer`, escriba un nombre para el ajuste preestablecido del visor de catálogos electrónicos.
1. En la página `Configure Viewer`, defina las opciones que desee.

   seleccione el icono **[!UICONTROL Sugerencia de información]** junto a la opción si desea leer su descripción.

   La página Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. (Opcional) En la **[!UICONTROL Configuración del panel de información]**, la opción **[!UICONTROL URL del servidor de información]** puede incluir los siguientes tokens especiales, que el visor sustituye:

   | Distintivo | Se sustituye por | Notas |
   | --- | --- | --- |
   | `$1$` | valor rollover_key | El identificador de elemento del elemento `<area>` del mapa. |
   | `$2$` | frame | El número de secuencia del cuadro que se muestra actualmente en el conjunto de imágenes. |
   | `$3$` | raíz de imagen | El primer elemento de ruta del primer elemento especificado en el comando de imagen (normalmente el ID del catálogo de imágenes de la entrada del catálogo en la que se especifica el conjunto de imágenes). |

1. (Opcional) En **[!UICONTROL Configuración del panel de información]**, en el cuadro **[!UICONTROL Plantilla de respuesta]**, escriba el texto que desea que aparezca si Adobe Dynamic Media Classic encuentra un error al recuperar información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de catálogo electrónico, pero ningún identificador rollover, aparecerá este mensaje para el usuario.

>[!NOTE]
>
>Para utilizar esta plantilla de respuesta en lugar de la plantilla definida en el propio catálogo electrónico, agregue `fmt=1` al final de la dirección URL del servidor de información. Por ejemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Seleccione **[!UICONTROL Guardar]**.
1. Seleccione **[!UICONTROL Predeterminado]** para que el ajuste preestablecido del visor de catálogos electrónicos que ha creado sea el que se utilice para mostrar los catálogos electrónicos en su página web.

Para eliminar un ajuste preestablecido de visor de catálogo electrónico, selecciónelo en la pantalla Ajustes preestablecidos de visor y seleccione **[!UICONTROL Eliminar]**.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)
