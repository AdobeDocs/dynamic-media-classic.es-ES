---
title: Configuración de ajustes preestablecidos del visor de catálogos electrónicos
description: Obtenga información sobre cómo configurar los ajustes preestablecidos de visor de catálogos electrónicos.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 66%

---


# Configuración de ajustes preestablecidos del visor de catálogos electrónicos{#setting-up-ecatalog-viewer-presets}

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo, el comportamiento y el aspecto de los visores de catálogos electrónicos. Dynamic Media Classic proporciona ajustes preestablecidos de visor de catálogos electrónicos y también puede crear sus propios ajustes preestablecidos de visor de catálogos electrónicos si es administrador.

Para crear un nuevo ajuste preestablecido, puede realizar inicios desde cero o inicios con un ajuste preestablecido de visor de catálogos electrónicos proporcionado por Dynamic Media Classic y guardarlo con un nuevo nombre. Puede crear sus propios ajustes preestablecidos de visor para presentar el material impreso en los colores de la empresa y establecer el tono.

Los ajustes preestablecidos del visor de catálogos electrónicos proporcionan muchas opciones de configuración para pasar de página, acercar o alejar la imagen, realizar búsquedas y elegir “apariencias”. El aspecto de estos controles y del propiamente dicho depende de la selección de ajustes preestablecidos de visor de catálogos electrónicos.

Siga estos pasos para crear un ajuste preestablecido de visor de catálogos electrónicos (debe ser un administrador):

1. Haga clic en **Ajustes** > **Ajustes preestablecidos de visor**.
1. En la pantalla Ajustes preestablecidos de visor, cree un ajuste preestablecido de visor de catálogos electrónicos desde cero o a partir de un ajuste preestablecido de visor de catálogos electrónicos existente:

   * **Creación de un**
ajuste preestablecido de visor de catálogos electrónicos Haga clic en Añadir. En el cuadro de diálogo Añadir ajuste preestablecido de visor, elija una plataforma, seleccione Visor de catálogos electrónicos y, a continuación, haga clic en 
**Agregar**.

   * **Edición de un**
ajuste preestablecido de visor de catálogos electrónicosSeleccione un ajuste preestablecido de visor de catálogos electrónicos y, a continuación, haga clic en Editar. Haga clic 
**Guarde** cuando haya terminado de crear el ajuste preestablecido.

1. En la pantalla Configurar visor, introduzca un nombre para el ajuste preestablecido de visor de catálogos electrónicos.
1. En la pantalla de Configurar visor, establezca las opciones que desee.

   Haga clic en el icono de información  situado junto a la opción para ver su descripción.

   La pantalla Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. (Opcional) En Configuración de panel de información, la opción URL de servidor de información puede incluir los siguientes distintivos especiales, que el visor sustituye:

   | Distintivo | Se sustituye por | Notas |
   |--- |--- |--- |
   | `$1$` | valor rollover_key | El identificador de elemento del elemento `<area>` del mapa. |
   | `$2$` | frame | El número de secuencia del cuadro que se muestra actualmente en el conjunto de imágenes. |
   | `$3$` | imageroot | El primer elemento de ruta del primer elemento especificado en el comando de imagen (normalmente el ID del catálogo de imágenes de la entrada del catálogo en la que se especifica el conjunto de imágenes). |

1. (Opcional) En Configuración del panel de información, en el cuadro Plantilla de respuesta, escriba el texto que desea que aparezca si Dynamic Media Classic encuentra un error al recuperar la información de un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de catálogo electrónico, pero ningún identificador rollover, aparecerá este mensaje para el usuario.

>[!NOTE]
>
>para usar esta plantilla de respuesta en lugar de la plantilla definida en el catálogo electrónico, añada “fmt=1” al final de la URL del servidor de información. Por ejemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Haga clic en **Guardar**.
1. Haga clic en Predeterminado si desea que el ajuste preestablecido del visor de catálogos electrónicos creado se utilice para mostrar los catálogos electrónicos de su página web.

Para eliminar un ajuste preestablecido de visor de catálogos electrónicos, selecciónelo en la pantalla Ajustes preestablecidos de visor y haga clic en **Eliminar**.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)

