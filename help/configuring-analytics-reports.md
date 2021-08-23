---
title: Configurar informes de Adobe Analytics
description: Obtenga información sobre cómo configurar informes de Adobe Analytics en Dynamic Media Classic.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 31%

---

# Configurar informes de Adobe Analytics{#configuring-adobe-analytics-reports}

Para indicar a Adobe Analytics la información que desea incluir en los informes de Adobe Analytics, vaya a la pantalla de configuración de Adobe Analytics. Después de configurar los informes, esta pantalla muestra, para cada evento de visor del que desee obtener información, una variable de Adobe Analytics y una variable de Dynamic Media Classic correspondientes. Estas combinaciones de variables de visor (variable Adobe Analytics) y variables de Dynamic Media Classic determinan qué información se incluye en los informes.

Además de asociar eventos de visor con variables, la pantalla Configuración de Adobe Analytics ofrece herramientas para activar, editar y eliminar eventos de visor.

>[!NOTE]
>
>Siempre que cambie la configuración de los informes de Adobe Analytics en Adobe Analytics, asegúrese de volver a iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic, volver a guardar la configuración de Adobe Analytics y, a continuación, volver a publicar.

Consulte [Inicio de sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consulte [Publicar información de configuración](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Asignación de variables de Adobe Analytics a eventos y variables de visores de Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilice la pantalla Configuración de Adobe Analytics para asociar eventos de visor con variables de Adobe Analytics y variables de Dynamic Media Classic. Para cada evento de visor, elija una variable de Adobe Analytics y una variable de Dynamic Media Classic. Si precisa instrucciones para acceder a la pantalla de configuración de Adobe Analytics, consulte [Inicio de sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Para asignar variables de Adobe Analytics a eventos y variables del visor de Dynamic Media Classic**

1. Después de iniciar sesión en Adobe Analytics desde Dynamic Media Classic y seleccionar un grupo de informes, en la página Configuración de Adobe Analytics , en la columna de la tabla derecha, active un evento de visor seleccionando **[!UICONTROL Habilitar]**.
1. En la columna Variables , muestre el selector de pares de variables seleccionando el botón de flecha para el Evento de visualizador deseado.

   Consulte [Eventos de visor](configuring-analytics-reports.md#viewer_events).

1. Agregue una variable de Dynamic Media Classic.

   Consulte [Variables de Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Añada una variable de Adobe Analytics.
1. (Opcional) Para agregar otro par de variables, seleccione **[!UICONTROL Agregar]**.
1. Seleccione **[!UICONTROL Guardar]**.

   Después de seleccionar **[!UICONTROL Guardar]**, el evento del visor, su variable de Adobe Analytics y la variable de Dynamic Media Classic se muestran en la pantalla Configuración de Adobe Analytics .

1. En la esquina inferior derecha, seleccione **[!UICONTROL Cerrar]**.
1. Seleccione **[!UICONTROL Publicar]** > **[!UICONTROL Enviar publicación]** para ejecutar una publicación de servicio de imágenes.

   La publicación es necesaria para que la información contenida en los visores esté disponible en los servidores de Dynamic Media Classic.

### Eventos de visor {#viewer-events}

Los eventos del visor describen las acciones que los usuarios realizan con los visores de Dynamic Media Classic. Cuando un usuario inicia una acción determinada, como seleccionar una miniatura o iniciar o detener un vídeo, el visor &quot;transmite&quot; un evento a la página web, junto con los datos asociados con ese evento.

La tabla siguiente describe los eventos de visor que puede añadir a la pantalla de configuración de Adobe Analytics.

| Evento de visor | Compatibilidad y visores de plataforma de visor HTML5 | Descripción |
|--- |--- |--- |
| LOAD | **X** (catálogo electrónico, flotante, conjunto de giros, vídeo, zoom) | Cuando un usuario inicia un visor |
| PAGE | **X** (catálogo electrónico) | En los catálogos electrónicos, cuando un usuario da vuelta una página; en los visores de zoom orientados, cuando un usuario selecciona un destino o una muestra de color diferente |
| SWAP | **X** (catálogo electrónico, flotante, conjunto de giros, vídeo, zoom) | Cuando un usuario selecciona una miniatura diferente para ver una imagen diferente |
| ITEM | **X** (catálogo electrónico) | En visores compatibles con mapas de imagen en las que se hayan definido rollovers, cuando un usuario desliza el puntero sobre un mapa de imagen para leer el texto rollover |
| HREF | **X** (catálogo electrónico) | En los visores compatibles con los mapas de imagen, cuando un usuario selecciona una URL en un mapa de imagen |
| TARGET |  | En los visualizadores de zoom orientados, cuando un usuario selecciona un destino de zoom para hacer zoom en una parte de una imagen. |
| SEARCH |  | En los catálogos electrónicos, cuando un usuario realiza la búsqueda de una palabra. |
| PLAY | **X** (vídeo) | En los visualizadores de vídeo, cuando un usuario selecciona Reproducir para comenzar a reproducir un vídeo.<br><br>**Nota:** Si utiliza la creación de informes de vídeo basada en latidos de Adobe Analytics, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 predeterminados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. Consulte [Habilitar los informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSE | **X** (vídeo) | En los visualizadores de vídeo, cuando un usuario selecciona **[!UICONTROL Pausar]** para congelar un vídeo.<br><br>**Nota:** Si utiliza la creación de informes de vídeo basada en latidos de Adobe Analytics, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 predeterminados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. Consulte [Habilitar los informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| STOP | **X** (vídeo) | En los visualizadores de vídeo, cuando un usuario selecciona **[!UICONTROL Stop]** para detener la reproducción de un vídeo.<br><br>**Nota:** Si utiliza la creación de informes de vídeo basada en latidos de Adobe Analytics, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 predeterminados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. Consulte [Habilitar los informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Vídeo) | En los visores de vídeo, los eventos de hito se generan cuando el usuario ha visto el 0, el 25, el 50, el 75 o el 100% del vídeo.<br><br>**Nota:** Si utiliza la creación de informes de vídeo basada en latidos de Adobe Analytics, no es necesario asignar ninguna variable a este evento de visor al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y de vídeo HTML5 predeterminados de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics. Consulte [Habilitar los informes de vídeo de Adobe Analytics](enabling-analytics-video-reports.md). |
| SWATCH | X (flotante, zoom) | Este evento de visor está asignado al evento de visor de PÁGINA en Dynamic Media Classic. |
| ZOOM | **X** (catálogo electrónico, conjunto de giros, zoom) | No rastreado por Adobe Analytics.<br> |
| PAN | **X** (catálogo electrónico, conjunto de giros, zoom) | No rastreado por Adobe Analytics.<br> |
| SPIN | **X** (conjunto de giros) | No rastreado por Adobe Analytics.<br> |


### Variables de Dynamic Media Classic {#scene-variables}

Para cada evento de visor en la pantalla Configuración de Adobe Analytics, seleccione una variable de Adobe Analytics y una *variable de Dynamic Media Classic*. Las variables de Dynamic Media Classic representan datos que se pueden obtener para un informe. Por ejemplo, la variable `searchTerm` enumera las palabras clave utilizadas en las búsquedas de los catálogos electrónicos.

La tabla siguiente describe las variables de Dynamic Media Classic:

| Variable de Dynamic Media Classic | Descripción |
|--- |:--- |
| asset | ID de recurso o archivo de ruta de vídeo de Dynamic Media Classic. |
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

## Activar, editar y eliminar eventos de visor {#activating-editing-and-deleting-viewer-events}

En la pantalla de configuración de Adobe Analytics puede activar, editar y eliminar eventos de visor:

* ****
ActivarSeleccione  **** Habilitar para activar o  **** Desactivar un evento de visor seleccionado.

* ****
EditarSeleccione un evento de visor y seleccione el botón gris  **[!UICONTROL Ver/]** Editar variables. En las listas desplegables Variable de Dynamic Media Classic y Variable de Adobe Analytics , elija una variable diferente de cada lista respectiva. Para obtener más información, consulte Asignación de variables de Adobe Analytics a eventos y variables de visor de Dynamic Media Classic .

* ****
EliminarSeleccione un evento de visor y seleccione el botón gris  **[!UICONTROL Ver/]** Editar variables. Seleccione **[!UICONTROL Delete]**.
