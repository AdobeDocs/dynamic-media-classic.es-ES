---
title: Configuración de ajustes preestablecidos del visor de catálogos electrónicos
description: Aprenda a configurar los ajustes preestablecidos del visualizador de catálogos electrónicos.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 42%

---

# Configuración de ajustes preestablecidos del visor de catálogos electrónicos{#setting-up-ecatalog-viewer-presets}

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo, el comportamiento y el aspecto de los visores de catálogos electrónicos. Adobe Dynamic Media Classic proporciona ajustes preestablecidos de visor de catálogos electrónicos y también puede crear sus propios ajustes preestablecidos de visor de catálogos electrónicos si es un administrador.

Para crear un ajuste preestablecido, puede empezar desde cero o con un ajuste preestablecido de visor de catálogos electrónicos proporcionado por Dynamic Media Classic de Adobe y guardarlo con un nuevo nombre. Puede crear sus propios ajustes preestablecidos de visor para presentar el material impreso en los colores de la empresa y establecer el tono.

Los ajustes preestablecidos del visor de catálogos electrónicos proporcionan muchas opciones de configuración para pasar de página, acercar o alejar la imagen, realizar búsquedas y elegir “apariencias”. El aspecto de estos controles y el aspecto del visor depende de la elección de los ajustes preestablecidos del visor de catálogos electrónicos.

Siga estos pasos para crear un ajuste preestablecido de visualizador de catálogos electrónicos (debe ser administrador):

1. En la barra de navegación global, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visor]**.
1. En la pantalla Ajustes preestablecidos de visor, cree un ajuste preestablecido de visor de catálogos electrónicos desde cero o a partir de un ajuste preestablecido de visor de catálogos electrónicos existente:

   * **Creación de un ajuste preestablecido de visualizador de catálogos electrónicos** : haga clic en  **[!UICONTROL Agregar]**. En el cuadro de diálogo Agregar ajuste preestablecido de visualizador, seleccione una plataforma, elija Visualizador de catálogos electrónicos y haga clic en **[!UICONTROL Agregar]**.

   * **Edición de un ajuste preestablecido de visualizador de catálogos electrónicos** : seleccione un ajuste preestablecido de visualizador de catálogos electrónicos y haga clic en Editar. Haga clic en **[!UICONTROL Guardar como]** después de terminar de crear el ajuste preestablecido.

1. En la pantalla Configurar visor, introduzca un nombre para el ajuste preestablecido de visor de catálogos electrónicos.
1. En la pantalla de Configurar visor, establezca las opciones que desee.

   Haga clic en el icono **[!UICONTROL Info Tip]** situado junto a la opción si desea leer su descripción.

   La página Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. (Opcional) En la **[!UICONTROL Configuración del panel de información]**, la **[!UICONTROL URL del servidor de información]** puede incluir los siguientes tokens especiales, que el visor sustituye:

   | Distintivo | Se sustituye por | Notas |
   |--- |--- |--- |
   | `$1$` | valor rollover_key | Identificador de elemento del elemento `<area>` del mapa. |
   | `$2$` | frame | El número de secuencia del cuadro que se muestra actualmente en el conjunto de imágenes. |
   | `$3$` | imageroot | El primer elemento de ruta del primer elemento especificado en el comando de imagen (normalmente el ID del catálogo de imágenes de la entrada del catálogo en la que se especifica el conjunto de imágenes). |

1. (Opcional) En **[!UICONTROL Configuración del panel de información]**, en el cuadro **[!UICONTROL Plantilla de respuesta]**, escriba el texto que desee que aparezca si Adobe Dynamic Media Classic encuentra un error al recuperar información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de catálogo electrónico, pero ningún identificador rollover, aparecerá este mensaje para el usuario.

>[!NOTE]
>
>Para utilizar esta plantilla de respuesta en lugar de la plantilla definida en el propio catálogo electrónico, agregue `fmt=1` al final de la URL del servidor de información. Por ejemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Haga clic en **Guardar**.
1. Haga clic en Predeterminado si desea que el ajuste preestablecido del visor de catálogos electrónicos creado se utilice para mostrar los catálogos electrónicos de su página web.

Para eliminar un ajuste preestablecido de visualizador de catálogos electrónicos, selecciónelo en la pantalla Ajustes preestablecidos de visualizador y haga clic en **[!UICONTROL Eliminar]**.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)

