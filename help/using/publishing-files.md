---
title: Archivos Publish
description: Obtenga información sobre cómo publicar sus recursos en Dynamic Media Image Servers.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1674'
ht-degree: 21%

---

# Archivos Publish{#publishing-files}

Los recursos se publican en Dynamic Media Image Servers. Puede publicar recursos una vez o hacer que Adobe Dynamic Media Classic publique los recursos de forma recurrente. Después de publicarse, tiene los recursos disponibles para su entrega. Puede copiar las llamadas de URL desde Adobe Dynamic Media Classic y añadirlas a su sitio web o aplicación.

Adobe Dynamic Media Classic ahora admite el envío de todas las imágenes y vídeos a través de HTTP/2. Es decir, hay disponible una URL publicada o un código incrustado para la imagen o el vídeo que se va a integrar con cualquier aplicación que acepte un recurso alojado. Ese recurso publicado utiliza el protocolo HTTP/2 para entregarlo. Este método de entrega mejora la forma en que los navegadores y servidores se comunican, lo que permite una mejor respuesta y tiempos de carga de todos los recursos de Adobe Dynamic Media Classic. Consulte [Preguntas frecuentes sobre la entrega de contenido HTTP2](https://experienceleague.adobe.com/es/docs/experience-manager-65/content/assets/dynamic/http2).

## Publicar tras la carga {#publish-after-uploading}

Los recursos están en un estado publicado o no. De forma predeterminada, todos los recursos que cargue en Adobe Dynamic Media Classic se marcarán automáticamente para su publicación.

Para obtener más información, consulte [PDF de avisos instantáneos de Publish](/help/using/assets/rendering-instant-publish-notification.pdf).

Utilice estas técnicas para marcar recursos para su publicación:

* **[!UICONTROL Publish después de cargar]**: en la página Cargar, cerca de la parte inferior, selecciona **[!UICONTROL Publish después de cargar]**. El valor predeterminado es un estado seleccionado.

* **[!UICONTROL Publish después de cargar]**: en el cuadro de diálogo Opciones del trabajo, seleccione **[!UICONTROL Publish después de cargar]**. El valor predeterminado es un estado seleccionado.

Algunos recursos &quot;secundarios&quot; se marcan para la publicación de forma automática al marcarse para publicación los recursos principales. Esta tabla enumera los recursos secundarios marcados automáticamente para su publicación.

| Elemento principal (grupo) | Elementos secundarios (miembros) |
| --- | --- |
| Conjuntos de imágenes | Imágenes del conjunto. |
| Conjuntos de muestras | Muestras del conjunto. |
| Conjuntos de giros | Imágenes del conjunto. |
| Plantillas | Archivos de plantilla, páginas e imágenes. |

Las imágenes derivadas también se marcan automáticamente para su publicación cuando se publican sus imágenes principales. Las imágenes derivadas son imágenes que se han ajustado con las opciones de edición de imágenes. Puede ver estas imágenes derivadas en Vista de detalles en Creación y derivados.

## Creación de un trabajo de publicación {#creating-a-publish-job}

Cree un trabajo de publicación para publicar los recursos que ha cargado en los servidores de Adobe Dynamic Media Classic, pero no desea que se publiquen automáticamente todavía. Puede realizar un trabajo de publicación único o programar trabajos para que se repitan con regularidad. Adobe Dynamic Media Classic ofrece opciones de publicación avanzadas para la publicación en servidores específicos y opciones para volver a publicar recursos que ya se han publicado.

**Para crear un trabajo de publicación:**

1. En la barra de navegación global, seleccione **[!UICONTROL Publish]**.
1. En el cuadro de diálogo Publicación, elija si desea un trabajo de publicación único o recurrente.

   Consulte [Crear un trabajo de publicación único](publishing-files.md#creating_a_one_time_publish_job) y [Crear un trabajo de publicación recurrente](publishing-files.md#creating_a_recurring_publish_job).

1. Introduzca un nombre de trabajo.
1. Si lo desea, acceda a las opciones avanzadas y elija entre estas opciones. 

   Consulte [Opciones avanzadas de publicación](publishing-files.md#advanced_publish_options).

1. Seleccione **[!UICONTROL Enviar Publish]**.

Adobe Dynamic Media Classic realiza un seguimiento de los trabajos de publicación en la página Trabajos. Puede revisar los trabajos de publicación en esta página.

>[!NOTE]
>
>Assets que ha vuelto a publicar (ya los ha publicado anteriormente) no aparece inmediatamente en el sitio web debido al mecanismo de almacenamiento en caché web en la red de entrega de contenido (CDN). Consulte [Segunda publicación de recursos y retrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Creación de un trabajo de publicación único {#creating-a-one-time-publish-job}

Cree un trabajo de publicación único seleccionando la opción **[!UICONTROL Único]** en la página Publicación.

Si desea que el trabajo de publicación se realice más adelante, en la página Publicación, seleccione **[!UICONTROL Único]**. En la lista desplegable, seleccione **[!UICONTROL Programar para más tarde]**. Utilice el control deslizante Calendario y Hora para seleccionar un día y una hora para ejecutar el trabajo de publicación.

### Crear un trabajo de publicación recurrente {#creating-a-recurring-publish-job}

Cree un trabajo de publicación recurrente seleccionando **[!UICONTROL Recurrente]** en la página Publicación.

A continuación, elija una opción Repetir de **[!UICONTROL Diario]**, **[!UICONTROL Semanal]**, **[!UICONTROL Mensual]** o **[!UICONTROL Personalizado]**, y después especifique cuándo desea que se repita el trabajo de publicación. Adobe Dynamic Media Classic presenta las herramientas de calendario para programar el trabajo de publicación recurrente. Puede seleccionar la opción **[!UICONTROL Personalizado]** e introducir una regla en el campo de texto Regla para describir un intervalo de trabajo personalizado.

Consulte [Crear un intervalo de tiempo de trabajo de publicación o carga personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Los trabajos de publicación (y carga) recurrentes aparecen en la página Trabajos. Si desea editar o eliminar un trabajo programado vaya a la ficha Programados en la página Trabajos.

### Opciones avanzadas de publicación {#advanced-publish-options}

Puede mostrar las opciones Avanzadas en la página Publicación y elegir estas opciones para administrar un trabajo de publicación:

* **[!UICONTROL Publish To]**: para publicar recursos solamente en un servidor específico, elija un tipo de servidor.

* **[!UICONTROL Publish]**: de forma predeterminada, Adobe Dynamic Media Classic publica solo los recursos que son nuevos y no se han publicado antes (opción Nuevo desde el último Publish ). Sin embargo, puede seleccionar **[!UICONTROL Publish completo]** para que también pueda publicar recursos que se hayan actualizado o cambiado desde la última vez que se publicaron. Seleccione **[!UICONTROL Completo con datos de búsqueda]** si va a publicar un catálogo electrónico y desea que los lectores puedan buscarlo por palabra clave.

* **[!UICONTROL Ejecutar trabajo como]**: Elija un nombre de usuario en la lista. Desde la página Trabajos, puede ordenar los trabajos por nombre de usuario. Al elegir un nombre, asocia un trabajo de publicación con un usuario.

**[!UICONTROL Notificación HTTP]**: escriba una dirección URL para almacenar en déclencheur los trabajos de publicación posteriores.

Ver [Usar un trabajo de carga o publicación como déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Cancelar un trabajo de publicación {#canceling-a-publish-job}

Puede cancelar un trabajo de publicación en curso. Además, si es administrador, puede cancelar un trabajo de publicación en curso desde la página Trabajos de la empresa.

Para cancelar un trabajo de publicación, vaya a la página Trabajos y seleccione **[!UICONTROL Cancelar]**. En la ficha Programado de la página Trabajos, puede pausar o reanudar un trabajo si anula la selección o activa la casilla de verificación de la columna Activo del trabajo.

>[!NOTE]
>
>Después de cancelar un trabajo de publicación, su estado cambia a &quot;detener&quot; hasta que el trabajo llegue un punto en el que se pueda detener de forma segura. Detener un trabajo de publicación puede tardar algún tiempo si el trabajo está en proceso de obtener datos de la base de datos.

## Recursos de Publish manualmente {#manually-publishing-assets}

Puede publicar recursos individuales manualmente en lugar de crear un trabajo de publicación. Cuando publica conjuntos, como un conjunto de imágenes o un conjunto de vídeos adaptable, se publican el conjunto (o &quot;principal&quot;) y todos los miembros (o &quot;secundarios&quot;) de ese conjunto.

Los recursos sin publicar se indican en la interfaz de usuario mediante un icono redondo gris con una barra diagonal (estado sin publicar) a la izquierda del nombre del recurso. Tras publicar un recurso, el icono cambia a verde y tiene una marca de comprobación blanca en el centro (estado publicado).

**Para publicar recursos manualmente:**

1. Realice una de las siguientes acciones:

   * En la vista de cuadrícula, la vista de lista o la vista de detalles, utilice los métodos tradicionales de selección de archivos para seleccionar uno o más recursos sin publicar.

     En la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Publish]**.

   * En la vista de cuadrícula, vista de lista o vista de detalles, seleccione el icono gris redondeado con una barra diagonal a la izquierda del nombre del recurso.

## Cancelar la publicación de recursos manualmente {#manually-unpublishing-assets}

Puede cancelar la publicación de los recursos individuales manualmente. Al cancelar la publicación de conjuntos, como un conjunto de muestras o un catálogo electrónico, el conjunto (o &quot;principal&quot;) pasa a estar en estado de no publicación. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Los recursos publicados se indican en la interfaz de usuario mediante un icono redondo de color verde con una marca de verificación blanca en el centro (estado publicado), a la izquierda del nombre del recurso. Una vez cancelada la publicación de un recurso, el icono se vuelve gris con una barra diagonal (estado sin publicar),

**Para cancelar la publicación manual de recursos:**

1. Realice una de las siguientes acciones:

   * En la vista de cuadrícula, vista de lista o vista de detalles, seleccione uno o varios recursos publicados.

     En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Cancelar la publicación]**.

   * En la vista de cuadrícula, vista de lista o vista de detalles, seleccione el icono de marca de verificación redonda y verde a la izquierda del nombre del recurso.

## Obtener el historial de publicación de un recurso {#getting-an-asset-s-publish-history}

La última fecha de publicación de un recurso se muestra en Vista de detalles en la parte superior del panel. Para obtener más detalles acerca del historial de publicación, abra el panel Historial y servidores publicados en la Vista de detalles. En este panel, podrá ver cuándo se publicó el recurso y los servidores en los que se publicó.

## Segunda publicación de recursos y retrasos de CDN {#republished-assets-and-cdn-delays}

Los recursos de Adobe Dynamic Media Classic se distribuyen en la red de entrega de contenido (CDN). CDN es un sistema de servidores de ordenador conectados entre sí que cooperan con transparencia para entregar contenido, especialmente de medios de gran tamaño, a los usuarios finales. En el sistema CDN, el contenido web se almacena en cachés web a través de Internet (lo que se denomina red de caché perimetral). El contenido web se entrega desde las cachés web a los usuarios finales para realizar envíos más rápidos.

La primera vez que alguien descarga una página web, los recursos se envían a un servidor de caché web de CDN. Este servidor los almacena de modo que la próxima vez que alguien en la misma área acceda a la página web, el mismo contenido almacenado en caché se envíe más rápido. El contenido se entrega con mayor rapidez porque se encuentra más cerca del usuario final. CDN hace que las páginas web se muestren más rápido. Disminuye la necesidad de banda ancha del servidor central porque el contenido se entrega desde la red de borde de almacenamiento en caché, y no desde un servidor central en cada caso.

El contenido de Adobe Dynamic Media Classic recién publicado está disponible inmediatamente para el usuario final y rellena rápidamente la red de caché de Edge. Sin embargo, el contenido recién republicado, es decir, las imágenes que tienen los mismos nombres que las imágenes publicadas anteriormente en un servidor de imágenes, no se actualizan en CDN durante un máximo de diez horas. En su lugar, los usuarios finales ven lo que hay en una caché web en la red CDN. Por este motivo, los recursos que ha vuelto a publicar Adobe Dynamic Media Classic no aparecen a los usuarios finales durante diez horas.

Si desea que los recursos de imagen recién publicados estén disponibles antes del retraso de diez horas, puede vaciar las cachés web en CDN. Al vaciar estas cachés web, se elimina el contenido antiguo de las cachés web de la CDN y se sustituye por los recursos publicados más recientemente.

Para vaciar la caché, en la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Invalidar CDN]**. Se eliminan todos los archivos seleccionados de la caché. Si no hay ningún recurso para publicar o no es administrador de empresa, la opción Quitar de CDN no se encuentra disponible.

>[!MORELIKETHIS]
>
>* [Comprobar archivos de trabajo](checking-job-files.md)
>* [Editar, eliminar, pausar y reanudar trabajos recurrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
