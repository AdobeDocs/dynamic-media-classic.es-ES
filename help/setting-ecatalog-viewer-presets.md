---
title: Configuración de ajustes preestablecidos del visor de catálogos electrónicos
seo-title: Configuración de ajustes preestablecidos del visor de catálogos electrónicos
description: nulo
seo-description: Descubra cómo configurar ajustes preestablecidos de visor de catálogos electrónicos.
uuid: aca 66 bc 5-8491-4 d 81-9 a 06-1 d 3531860 a 14
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6 c 123 f 85-3 bc 4-4392-a 7 fb -55618127 c 65 e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Configuración de ajustes preestablecidos del visor de catálogos electrónicos{#setting-up-ecatalog-viewer-presets}

Los ajustes preestablecidos de visor de catálogos electrónicos determinan el estilo, el comportamiento y el aspecto de los visores de catálogos electrónicos. Dynamic Media Classic proporciona ajustes preestablecidos de visor de catálogos electrónicos y también puede crear sus propios ajustes preestablecidos de visor de catálogos electrónicos si es administrador.

Para crear un nuevo ajuste preestablecido, puede empezar desde cero o con un ajuste preestablecido de visor de catálogos electrónicos de Dynamic Media Classic y guardarlo con un nuevo nombre. Puede crear sus propios ajustes preestablecidos de visor para presentar el material impreso en los colores de la empresa y establecer el tono.

Los ajustes preestablecidos del visor de catálogos electrónicos proporcionan muchas opciones de configuración para pasar de página, acercar o alejar la imagen, realizar búsquedas y elegir “apariencias”. El aspecto de estos controles y del propiamente dicho depende de la selección de ajustes preestablecidos de visor de catálogos electrónicos.

Siga estos pasos para crear un ajuste preestablecido de visor de catálogos electrónicos (debe ser un administrador):

1. Haga clic en **Ajustes** &gt; **Ajustes preestablecidos de visor**.
1. En la pantalla Ajustes preestablecidos de visor, cree un ajuste preestablecido de visor de catálogos electrónicos desde cero o a partir de un ajuste preestablecido de visor de catálogos electrónicos existente:

   **Creación de un ajuste preestablecido de visor de catálogos electrónicos** Haga clic en Agregar. In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **Add**.

   **Edición de un ajuste preestablecido de visor de catálogos electrónicos** Seleccione un ajuste preestablecido de visor de catálogos electrónicos y haga clic en Editar. Click **Save As** after you finish creating the preset.

1. En la pantalla Configurar visor, introduzca un nombre para el ajuste preestablecido de visor de catálogos electrónicos.
1. En la pantalla de Configurar visor, establezca las opciones que desee.

   Haga clic en el icono de información  situado junto a la opción para ver su descripción.

   La pantalla Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. (Opcional) En Configuración de panel de información, la opción URL de servidor de información puede incluir los siguientes distintivos especiales, que el visor sustituye:

   | Distintivo | Se sustituye por | Notas |
   |--- |--- |--- |
   | `$1$` | valor rollover_key | The item identifier from the `<area>` element of the map. |
   | `$2$` | frame | El número de secuencia del cuadro que se muestra actualmente en el conjunto de imágenes. |
   | `$3$` | imageroot | El primer elemento de ruta del primer elemento especificado en el comando de imagen (normalmente el ID del catálogo de imágenes de la entrada del catálogo en la que se especifica el conjunto de imágenes). |

1. (Opcional) En Configuración de panel de información, en el cuadro Plantilla de respuesta, escriba el texto que desea que aparezca si Dynamic Media Classic encuentra un error al recuperar la información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de catálogo electrónico, pero ningún identificador rollover, aparecerá este mensaje para el usuario.

>[!NOTE]
>
>para usar esta plantilla de respuesta en lugar de la plantilla definida en el catálogo electrónico, añada “fmt=1” al final de la URL del servidor de información. Por ejemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Haga clic en **Guardar**.
1. Haga clic en Predeterminado si desea que el ajuste preestablecido del visor de catálogos electrónicos creado se utilice para mostrar los catálogos electrónicos de su página web.

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)

