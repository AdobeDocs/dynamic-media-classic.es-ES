---
title: Configuración de informes de Adobe Analytics
seo-title: Configuración de informes de Adobe Analytics
description: nulo
seo-description: Obtenga información sobre cómo configurar los informes de Adobe Analytics.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 51%

---


# Configuración de informes de Adobe Analytics{#configuring-adobe-analytics-reports}

Para indicar a Adobe Analytics la información que desea incluir en los informes de Adobe Analytics, vaya a la pantalla de configuración de Adobe Analytics. Después de configurar los informes, esta pantalla lista, para cada evento de visor sobre el que desee obtener información, una variable Adobe Analytics y una variable de Dynamic Media Classic correspondientes. Estas combinaciones de eventos de visor, variables de Adobe Analytics y variables de Dynamic Media Classic determinan la información que se debe informar.

Además de asociar eventos de visor con variables, la pantalla de configuración de Adobe Analytics ofrece herramientas para activar, editar y eliminar eventos de visor.

>[!NOTE]
>
>Siempre que cambie la configuración de los informes de Adobe Analytics en Adobe Analytics, asegúrese de volver a iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic, vuelva a guardar la configuración de Adobe Analytics y, a continuación, vuelva a publicar.

Consulte [Inicio de sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consulte [Publicación de la información de configuración](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Asignación de variables de Adobe Analytics a eventos y variables del visor de Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilice la pantalla de configuración de Adobe Analytics para asociar eventos de visor con variables de Adobe Analytics y variables de Dynamic Media Classic. Para cada evento de visor, elija una variable de Adobe Analytics y una variable de Dynamic Media Classic. Si precisa instrucciones para acceder a la pantalla de configuración de Adobe Analytics, consulte [Inicio de sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Asignación de variables de Adobe Analytics a eventos y variables del visor de Dynamic Media Classic**

1. After you log in to Adobe Analytics from within Dynamic Media Classic and select a report suite, on the Adobe Analytics Configuration page, in the far right column of the table, activate a viewer event by clicking **Enable**.
1. En la columna Variables, muestre el selector de pares de variables haciendo clic en el botón de flecha del evento de visor deseado.

   Consulte [Eventos de visor](configuring-analytics-reports.md#viewer_events).

1. Añada una variable de Dynamic Media Classic.

   Consulte Variables [de Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Añada una variable de Adobe Analytics.
1. (Opcional) Para añadir otro par de variables, haga clic en **Agregar**.
1. Haga clic en **Guardar**.

   Después de hacer clic en Guardar, el evento del visor, su variable de Adobe Analytics y su variable de Dynamic Media Classic se muestran en la pantalla de configuración de Adobe Analytics.

1. En la esquina inferior derecha, haga clic en **Cerrar**.
1. Haga clic en **Publicar** > **Enviar publ.** para ejecutar una publicación para servicio de imágenes.

   La publicación es necesaria para que la información contenida en los visores esté disponible en los servidores de Dynamic Media Classic.

### Eventos de visor {#viewer-events}

Los eventos de visor describen las acciones que los usuarios realizan con los visores de Dynamic Media Classic. Cuando un usuario inicia una acción, como hacer clic en una miniatura o iniciar o detener un vídeo, el visor “difunde” un evento en la página Web, junto con los datos asociados con dicho evento.

La tabla siguiente describe los eventos de visor que puede añadir a la pantalla de configuración de Adobe Analytics.

| Evento de visor | Compatibilidad y visores de plataforma de visor HTML5 | Descripción |
|--- |--- |--- |
| LOAD | **X** (catálogo electrónico, flotante, conjunto de giros, vídeo, zoom) | Cuando un usuario inicia el visor. |
| PAGE | **X** (catálogo electrónico) | En los catálogos electrónicos, cuando un usuario da la vuelta a una página; en visores con destino de zoom, cuando un usuario hace clic en un destino o una muestra de color diferentes. |
| SWAP | **X** (catálogo electrónico, flotante, conjunto de giros, vídeo, zoom) | Cuando un usuario hace clic en otra miniatura para ver una imagen diferente. |
| ITEM | **X** (catálogo electrónico) | En visores compatibles con mapas de imagen en las que se hayan definido rollovers, cuando un usuario desliza el puntero sobre un mapa de imagen para leer el texto rollover. |
| HREF | **X** (catálogo electrónico) | En visores que admiten mapas de imagen, cuando un usuario hace clic en una URL de un mapa de imagen. |
| TARGET |  | En visores con destino de zoom, cuando un usuario hace clic en un destino de zoom para ampliar parte de una imagen. |
| SEARCH |  | En los catálogos electrónicos, cuando un usuario realiza la búsqueda de una palabra. |
| PLAY | **X** (vídeo) | En los visores de vídeo, cuando un usuario hace clic en Reproducir para iniciar la reproducción de un vídeo.<br><br>**Nota:** Si utiliza el sistema de informes de vídeo basado en Adobe Analytics Heartbeat, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 incorporados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE | **X** (vídeo) | En los visores de vídeo, cuando un usuario hace clic en Pausa para interrumpir la reproducción de un vídeo.<br><br>**Nota:** Si utiliza el sistema de informes de vídeo basado en Adobe Analytics Heartbeat, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 incorporados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| STOP | **X** (vídeo) | En los visores de vídeo, cuando un usuario hace clic en Detener para parar la reproducción de un vídeo.<br><br>**Nota:** Si utiliza el sistema de informes de vídeo basado en Adobe Analytics Heartbeat, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 incorporados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Vídeo) | En los visores de vídeo, los eventos de hito se generan cuando el usuario ha visto el 0, el 25, el 50, el 75 o el 100% del vídeo.<br><br>**Nota:** Si utiliza el sistema de informes de vídeo basado en Adobe Analytics Heartbeat, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 incorporados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| SWATCH | X (flotante, zoom) | Este evento de visor está asignado al evento de visor PAGE en Dynamic Media Classic. |
| ZOOM | **X** (catálogo electrónico, conjunto de giros, zoom) | No rastreado por Adobe Analytics.<br> |
| PAN | **X** (catálogo electrónico, conjunto de giros, zoom) | No rastreado por Adobe Analytics.<br> |
| SPIN | **X** (conjunto de giros) | No rastreado por Adobe Analytics.<br> |


### Variables de Dynamic Media Classic {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose a Adobe Analytics variable and a *Dynamic Media Classic variable*. Las variables de Dynamic Media Classic representan datos que se pueden obtener para un informe. Por ejemplo, la variable `searchTerm` enumera las palabras clave utilizadas en las búsquedas de los catálogos electrónicos.

En la tabla siguiente se describen las variables de Dynamic Media Classic.

| Variable de Dynamic Media Classic | Descripción |
|--- |:--- |
| asset | Archivo de ruta de vídeo o ID de recurso de Dynamic Media Classic. |
| viewerId | Número arbitrario asignado a cada tipo de visor distinto. |
| pageLabel | En los catálogos electrónicos, página que muestra un visor. |
| label | El valor de la etiqueta (una cadena). |
| frame | La página o referencia de página de un conjunto de imágenes. |
| rollover_keyRaw | El valor HREF completo y no únicamente una parte procesada del mismo. |
| rollover_keyProc | ID de un elemento al que se hace referencia en un mapa de imagen (válido para href y eventos de elemento). |
| searchTerm | Término que se utiliza en la búsqueda en los catálogos electrónicos. |
| timeStamp | Opciones de reproducción, detención y pausa en los visores de vídeo. |
| progress | Porcentaje de un evento de hito que se ha finalizado. |
| targetId | El valor del identificador (un número). |

## Activación, edición y eliminación de eventos de visor {#activating-editing-and-deleting-viewer-events}

En la pantalla de configuración de Adobe Analytics puede activar, editar y eliminar eventos de visor:

* **Activación** Haga clic en **[!UICONTROL Habilitar]** para activar o **[!UICONTROL Desactivar]** para desactivar un evento de visor seleccionado.

* **Edición** Seleccione un evento de visor y haga clic en el botón gris **[!UICONTROL Vista/Editar]** variables. En las listas desplegables Variable de Dynamic Media Classic y Variable de Adobe Analytics, elija una variable diferente de cada lista respectiva. Para obtener más información, consulte Asignación de variables de Adobe Analytics a eventos y variables de visor de Dynamic Media Classic.

* **Eliminación** Seleccione un evento de visor y haga clic en el botón gris **[!UICONTROL Vista/Editar]** variables. Haga clic en **[!UICONTROL Eliminar]**.
