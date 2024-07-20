---
title: Configuración de informes de Adobe Analytics
description: Obtenga información sobre cómo configurar informes de Adobe Analytics en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 18%

---

# Configuración de informes de Adobe Analytics{#configuring-adobe-analytics-reports}

Para indicar a Adobe Analytics qué información desea incluir en los informes de Adobe Analytics, vaya a la pantalla Configuración de Adobe Analytics. Siguiendo los informes de configuración, esta pantalla enumera, para cada evento de visualizador del que desee obtener información, una variable de Adobe Analytics y una variable de Adobe Dynamic Media Classic correspondientes. Estas combinaciones de eventos de visualizador, variables de Adobe Analytics y variables de Adobe Dynamic Media Classic determinan qué información se registra en los informes.

Además de asociar eventos de visor con variables, la pantalla Configuración de Adobe Analytics ofrece herramientas para activar, editar y eliminar eventos de visor.

>[!NOTE]
>
>Siempre que cambie la configuración de los informes de Adobe Analytics en Adobe Analytics, vuelva a iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic, vuelva a guardar la configuración de Adobe Analytics y, a continuación, vuelva a publicar.

Ver [Iniciar sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Ver [información de configuración de Publish](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Asignar variables de Adobe Analytics a eventos y variables de visualizador de Adobe Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilice la pantalla Configuración de Adobe Analytics para asociar eventos de visor con variables de Adobe Analytics y de Adobe Dynamic Media Classic. Para cada evento de visor, elija una variable de Adobe Analytics y una variable de Adobe Dynamic Media Classic. Para obtener instrucciones acerca de cómo abrir la pantalla Configuración de Adobe Analytics, consulte [Iniciar sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Para asignar variables de Adobe Analytics a eventos y variables de visualizador de Adobe Dynamic Media Classic:**

1. Después de iniciar sesión en Adobe Analytics desde Dynamic Media Classic y seleccionar un grupo de informes, en la página Configuración de Adobe Analytics, en la columna de la tabla derecha, active un evento de visor seleccionando **[!UICONTROL Habilitar]**.
1. En la columna Variables, muestre el selector de pares de variables seleccionando el botón de flecha para el evento de visor deseado.

   Consulte [Eventos de visor](configuring-analytics-reports.md#viewer_events).

1. Añada una variable de Adobe Dynamic Media Classic.

   Ver [variables de Adobe Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Añada una variable de Adobe Analytics.
1. (Opcional) Para agregar otro par de variables, seleccione **[!UICONTROL Agregar]**.
1. Seleccione **[!UICONTROL Guardar]**.

   Después de seleccionar **[!UICONTROL Guardar]**, el evento del visor, su variable de Adobe Analytics y su variable de Adobe Dynamic Media Classic se enumeran en la pantalla Configuración de Adobe Analytics.

1. En la esquina inferior derecha, seleccione **[!UICONTROL Cerrar]**.
1. Vaya a **[!UICONTROL Publish]** > **[!UICONTROL Enviar Publish]** para ejecutar una publicación del servicio de imágenes.

   La publicación es necesaria para que la información contenida en los visores esté disponible en los servidores de Adobe Dynamic Media Classic.

### Eventos de visor {#viewer-events}

Los eventos de visor describen las acciones que los usuarios realizan con los visores de Dynamic Media Classic. Cuando un usuario inicia una acción (por ejemplo, seleccionar una miniatura o iniciar o detener un vídeo), el visor &quot;difunde&quot; un evento a la página web. Los datos asociados con ese evento también se insertan.

En la tabla siguiente se describen los eventos de visor que se pueden agregar a la pantalla Configuración de Adobe Analytics.

| Evento de visor | Compatibilidad y visores de plataforma de visor HTML5 | Descripción |
| --- | --- | --- |
| LOAD | **X** (catálogo electrónico, flotante, conjunto de giros, vídeo, zoom) | Cuando un usuario inicia un visor |
| PAGE | **X** (catálogo electrónico) | En los catálogos electrónicos, cuando un usuario cambia de página; en los visores de zoom segmentados, cuando selecciona otro destino o muestra de color. |
| SWAP | **X** (catálogo electrónico, flotante, conjunto de giros, vídeo, zoom) | Cuando un usuario selecciona una miniatura diferente para ver una imagen diferente. |
| ITEM | **X** (catálogo electrónico) | En visores compatibles con mapas de imagen en las que se hayan definido rollovers, cuando un usuario desliza el puntero sobre un mapa de imagen para leer el texto rollover. |
| HREF | **X** (catálogo electrónico) | En los visores compatibles con mapas de imagen, cuando un usuario selecciona una dirección URL en un mapa de imagen. |
| TARGET | | En visores de zoom de destino, cuando un usuario selecciona un destino de zoom para ampliar a parte de una imagen. |
| SEARCH | | En los catálogos electrónicos, cuando un usuario realiza la búsqueda de una palabra. |
| PLAY | **X** (vídeo) | En los visores de vídeo, cuando un usuario selecciona Reproducir para comenzar a reproducir un vídeo.<br><br>**Nota:** Si usa informes de vídeo basados en Adobe Analytics Heartbeat, no es necesario que asigne ninguna variable a este evento de visor al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con los visores de vídeo y medios mixtos predeterminados de Adobe Dynamic Media Classic HTML5. El reproductor de vídeo genera datos de seguimiento para verlos en los informes de vídeo de Adobe Analytics. Consulte [Habilitar informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSE | **X** (vídeo) | En los visores de vídeo, cuando un usuario selecciona **[!UICONTROL Pausa]** para inmovilizar un vídeo.<br><br>**Nota:** Si usa informes de vídeo basados en Adobe Analytics Heartbeat, no es necesario que asigne ninguna variable a este evento de visor al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con los visores de vídeo y medios mixtos predeterminados de Adobe Dynamic Media Classic HTML5. El reproductor de vídeo genera datos de seguimiento para verlos en los informes de vídeo de Adobe Analytics. Consulte [Habilitar informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| STOP | **X** (vídeo) | En los visores de vídeo, cuando un usuario selecciona **[!UICONTROL Detener]** para detener la reproducción de un vídeo.<br><br>**Nota:** Si usa informes de vídeo basados en Adobe Analytics Heartbeat, no es necesario que asigne ninguna variable a este evento de visor al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con los visores de vídeo y medios mixtos predeterminados de Adobe Dynamic Media Classic HTML5. El reproductor de vídeo genera datos de seguimiento para verlos en los informes de vídeo de Adobe Analytics. Consulte [Habilitar informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| MILESTONE | **X** (vídeo) | En los visores de vídeo, los eventos de hito se generan cuando el usuario ha visto el 0, el 25, el 50, el 75 o el 100% del vídeo.<br><br>**Nota:** Si usa informes de vídeo basados en Adobe Analytics Heartbeat, no es necesario que asigne ninguna variable a este evento de visor al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con los visores de vídeo y medios mixtos predeterminados de Adobe Dynamic Media Classic HTML5. El reproductor de vídeo genera datos de seguimiento para verlos en los informes de vídeo de Adobe Analytics. Consulte [Habilitar informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| SWATCH | **X** (flotante, zoom) | Este evento de visor está asignado al evento de visor de PÁGINAS en Adobe Dynamic Media Classic. |
| ZOOM | **X** (catálogo electrónico, conjunto de giros, zoom) | No rastreado por Adobe Analytics. |
| PAN | **X** (catálogo electrónico, conjunto de giros, zoom) | No rastreado por Adobe Analytics. |
| SPIN | **X** (conjunto de giros) | No rastreado por Adobe Analytics. |

### Variables de Adobe Dynamic Media Classic {#scene-variables}

Para cada evento de visor en la pantalla Configuración de Adobe Analytics, elige una variable de Adobe Analytics y una *variable de Adobe Dynamic Media Classic*. Las variables de Adobe Dynamic Media Classic representan datos que se pueden obtener para un informe. Por ejemplo, la variable `searchTerm` enumera las palabras clave utilizadas en las búsquedas en catálogo electrónico.

En la tabla siguiente se describen las variables de Adobe Dynamic Media Classic:

| variable de Adobe Dynamic Media Classic | Descripción |
| --- | --- |
| asset | Archivo de ruta de vídeo o ID de recurso de Adobe Dynamic Media Classic. |
| viewerId | Número arbitrario asignado a cada tipo de visor distinto. |
| pageLabel | En los catálogos electrónicos, página que muestra un visor. |
| label | El valor de la etiqueta (una cadena). |
| frame | La referencia de página o página en un conjunto de imágenes. |
| rollover_keyRaw | El valor HREF completo, no cualquier parte procesada de él. |
| rollover_keyProc | ID de un elemento al que se hace referencia en un mapa de imagen (válido para href y eventos de elemento). |
| searchTerm | Término que se utiliza en la búsqueda en los catálogos electrónicos. |
| timeStamp | Reproducir, detener y pausar seleccionados en los visores de vídeo. |
| progress | Porcentaje de un evento de hito que se ha finalizado. |
| targetId | El valor de ID (un número). |

## Activación, edición y eliminación de eventos de visor {#activating-editing-and-deleting-viewer-events}

En la pantalla de configuración de Adobe Analytics puede activar, editar y eliminar eventos de visor:

* **Activar**: selecciona **[!UICONTROL Activar]** para activar o **[!UICONTROL Desactivar]** para desactivar un evento de visor seleccionado.

* **Editar**: selecciona un evento de visor y el botón gris de **[!UICONTROL Ver/Editar]** variables. En las listas desplegables Variable de Adobe Dynamic Media Classic y Variable de Adobe Analytics, elija una variable diferente en cada lista respectiva. Para obtener más información, consulte [Asignación de variables de Adobe Analytics a eventos y variables de visualizador de Adobe Dynamic Media Classic](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Eliminar**: seleccione un evento de visor y haga clic en el botón gris de **[!UICONTROL Ver/Editar]** variables. Seleccione **[!UICONTROL Eliminar]**.
