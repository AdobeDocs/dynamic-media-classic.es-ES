---
title: Publicar archivos
description: '"Aprenda a publicar sus recursos en los servidores de imágenes de Dynamic Media. Puede publicar recursos una vez o hacer que Adobe Dynamic Media Classic publique los recursos de forma recurrente. Después de publicarse, tiene los recursos disponibles para su entrega. Puede copiar las llamadas de URL desde Adobe Dynamic Media Classic y añadirlas a su sitio web o aplicación".'
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 45%

---

# Publicar archivos{#publishing-files}

Los recursos se publican en Dynamic Media Image Servers. Puede publicar recursos una vez o hacer que Adobe Dynamic Media Classic publique los recursos de forma recurrente. Después de publicarse, tiene los recursos disponibles para su entrega. Puede copiar las llamadas de URL desde Adobe Dynamic Media Classic y añadirlas a su sitio web o aplicación.

Adobe Dynamic Media Classic ahora admite el envío de todas las imágenes y vídeos a través de HTTP/2. Es decir, hay disponible una URL publicada o código incrustado para la imagen o el vídeo que se va a integrar con cualquier aplicación que acepte un recurso alojado. Ese recurso publicado se entrega mediante el protocolo HTTP/2. Este método de entrega mejora la forma en que los navegadores y servidores se comunican, lo que permite una mejor respuesta y tiempos de carga de todos los recursos de Adobe Dynamic Media Classic. Consulte [Preguntas frecuentes sobre la entrega de contenido HTTP2](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Publicar tras la carga {#publish-after-uploading}

Los recursos están en un estado publicado o no. De forma predeterminada, todos los recursos que cargue en Adobe Dynamic Media Classic se marcarán automáticamente para su publicación.

Para obtener más información, consulte la [PDF de avisos de publicación instantánea](/help/assets/rendering-instant-publish-notification.pdf).

Para marcar recursos para la publicación, siga estas técnicas:

* **[!UICONTROL Publicar tras la carga]** : en la página Cargar, cerca de la parte inferior, seleccione **[!UICONTROL Publicar tras la carga]**. El valor predeterminado es un estado seleccionado.

* **[!UICONTROL Publicar tras la carga]** - En el cuadro de diálogo Opciones de trabajo, seleccione **[!UICONTROL Publicar tras la carga]**. El valor predeterminado es un estado seleccionado.

Algunos recursos &quot;secundarios&quot; se marcan para la publicación de forma automática al marcarse para publicación los recursos principales. En esta tabla se muestran los recursos que se marcan para la publicación de forma automática.

| Elemento principal (grupo) | Elementos secundarios (miembros) |
| --- | --- |
| Conjuntos de imágenes | Imágenes del conjunto. |
| Conjuntos de muestras | Muestras del conjunto. |
| Conjuntos de giros | Imágenes del conjunto. |
| Plantillas | Archivos de plantilla, páginas e imágenes. |

Las imágenes derivadas también se marcan para la publicación de forma automática cuando se están publicando las imágenes principales. Las imágenes derivadas son imágenes que se han ajustado con las opciones de edición de imágenes. Puede ver estas imágenes derivadas en Vista de detalles en Creación y derivados.

## Creación de un trabajo de publicación {#creating-a-publish-job}

Cree un trabajo de publicación para publicar los recursos que ha cargado en los servidores de Adobe Dynamic Media Classic, pero aún no desea publicarlos automáticamente. Puede realizar un trabajo de publicación único o programar trabajos para que se repitan con regularidad. Adobe Dynamic Media Classic ofrece opciones de publicación avanzadas para la publicación en servidores específicos y opciones para volver a publicar recursos que ya se han publicado.

**Para crear un trabajo de publicación:**

1. En la barra de navegación global, seleccione **[!UICONTROL Publish]**.
1. En el cuadro de diálogo Publicar, seleccione si desea crear un trabajo de publicación de una sola vez o recurrente.

   Consulte [Creación de un trabajo de publicación único](publishing-files.md#creating_a_one_time_publish_job) y [Creación de un trabajo de publicación recurrente](publishing-files.md#creating_a_recurring_publish_job).

1. Introduzca un nombre de trabajo.
1. Si lo desea, acceda a las opciones avanzadas y elija entre estas opciones. 

   Consulte [Opciones avanzadas de publicación](publishing-files.md#advanced_publish_options).

1. Seleccionar **[!UICONTROL Enviar publicación]**.

Adobe Dynamic Media Classic realiza un seguimiento de los trabajos de publicación en la página Trabajos. Puede revisar los trabajos de publicación en esta página.

>[!NOTE]
>
>Los recursos que vuelve a publicar (los ha publicado anteriormente) no aparecen inmediatamente en el sitio web debido al mecanismo de almacenamiento en caché web en la red de entrega de contenido (CDN). Consulte [Segunda publicación de recursos y retrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Creación de un trabajo de publicación único {#creating-a-one-time-publish-job}

Cree un trabajo de publicación único seleccionando la variable **[!UICONTROL Único]** en la página Publicar.

Si desea que el trabajo de publicación se produzca más adelante, en la página Publicar, seleccione **[!UICONTROL Único]**, luego seleccione **[!UICONTROL Programar para más tarde]** menú desplegable. Utilice el control deslizante Calendario y Hora para seleccionar un día y una hora para ejecutar el trabajo de publicación.

### Creación de un trabajo de publicación recurrente {#creating-a-recurring-publish-job}

Cree un trabajo de publicación recurrente seleccionando **[!UICONTROL Recurrente]** en la página Publicar.

A continuación, elija una opción Repetir de **[!UICONTROL Diario]**, **[!UICONTROL Semanalmente]**, **[!UICONTROL Mensual]**, o **[!UICONTROL Personalizado]** A continuación, especifique cuándo desea que se repita el trabajo de publicación. Adobe Dynamic Media Classic presenta las herramientas de calendario para programar el trabajo de publicación recurrente. Puede seleccionar **[!UICONTROL Personalizado]** y escriba una regla en el campo de texto Regla para describir un intervalo de trabajo personalizado.

Consulte [Crear un intervalo de tiempo de trabajo de carga o publicación personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Los trabajos de publicación (y carga) recurrentes aparecen en la página Trabajos. Si desea editar o eliminar un trabajo programado vaya a la ficha Programados en la página Trabajos.

### Opciones avanzadas de publicación {#advanced-publish-options}

Puede acceder a las opciones avanzadas desde la página Publicar y especificar estas opciones para controlar un trabajo de publicación:

* **[!UICONTROL Publicar en]** : Para publicar recursos solo en un servidor específico, elija un tipo de servidor.

* **[!UICONTROL Publish]** : De forma predeterminada, Adobe Dynamic Media Classic publica solo los recursos que son nuevos y no se han publicado antes (opción Nuevo desde la última publicación ). Sin embargo, puede seleccionar **[!UICONTROL Publicación completa]** para publicar también recursos que se han actualizado o cambiado desde la última vez que se publicaron. Seleccionar **[!UICONTROL Completa con datos de búsqueda]** si publica un catálogo electrónico y desea que los lectores puedan buscarlo por palabra clave.

* **[!UICONTROL Ejecutar trabajo como]** - Elija un nombre de usuario de la lista. Desde la página Trabajos, puede ordenar los trabajos por nombre de usuario. Si elige un nombre, asociará el trabajo de publicación con un usuario.

**[!UICONTROL Notificación HTTP]** : introduzca una URL para almacenar en déclencheur los trabajos de publicación posteriores.

Consulte [Uso de un trabajo de carga o publicación como déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Cancelar un trabajo de publicación {#canceling-a-publish-job}

Puede cancelar un trabajo de publicación en curso. Además, si es administrador, puede cancelar un trabajo de publicación en curso desde la página Trabajos de la empresa.

Para cancelar un trabajo de publicación, vaya a la página Trabajos y seleccione **[!UICONTROL Cancelar]**. En la ficha Programados de la página Trabajos, puede pausar o reanudar un trabajo mediante la casilla de verificación de la columna Activo.

>[!NOTE]
>
>Al cancelar un trabajo de publicación, su estado se cambia a &quot;deteniendo&quot; hasta que el trabajo se pueda detener de forma segura. Si el trabajo de publicación está obteniendo datos de la base de datos, puede que tarde un tiempo en detenerse.

## Publicar recursos manualmente {#manually-publishing-assets}

Puede publicar recursos individuales manualmente en lugar de crear un trabajo de publicación. Cuando publica conjuntos, como un conjunto de imágenes o un conjunto de vídeos adaptable, se publican el conjunto (o “elemento principal”) y todos los miembros (o “elementos secundarios”) dentro de dicho conjunto.

Los recursos sin publicar se indican en la interfaz de usuario mediante un icono redondo gris con una barra diagonal (estado sin publicar) a la izquierda del nombre del recurso. Tras publicar un recurso, el icono cambia a verde y tiene una marca de comprobación blanca en el centro (estado publicado).

**Para publicar recursos manualmente:**

1. Realice una de las siguientes acciones:

   * En la vista de cuadrícula, la vista de lista o la vista de detalles, utilice los métodos tradicionales de selección de archivos para seleccionar uno o más recursos sin publicar.

      En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Publish]**.

   * En la vista de cuadrícula, vista de lista o vista de detalles, seleccione el icono gris redondeado con una barra diagonal a la izquierda del nombre del recurso.

## Cancelar la publicación manual de recursos {#manually-unpublishing-assets}

Puede cancelar la publicación de los recursos individuales manualmente. Al cancelar la publicación de conjuntos, como un conjunto de muestras o un catálogo electrónico, el conjunto (o “elemento principal”) pasa a un estado no publicado. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Los recursos publicados aparecen en la interfaz de usuario con un icono verde redondeado con una marca de comprobación blanca en el centro (estado publicado) a la izquierda del nombre del recurso. Una vez cancelada la publicación de un recurso, el icono se vuelve gris con una barra diagonal (estado sin publicar),

**Para cancelar la publicación de recursos manualmente:**

1. Realice una de las siguientes acciones:

   * En la vista de cuadrícula, vista de lista o vista de detalles, seleccione uno o varios recursos publicados.

      En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Cancelar publicación]**.

   * En la vista de cuadrícula, vista de lista o vista de detalles, seleccione el icono de marca de verificación redonda y verde a la izquierda del nombre del recurso.

## Obtener el historial de publicación de un recurso {#getting-an-asset-s-publish-history}

La última fecha de publicación de un recurso se muestra en Vista de detalles en la parte superior del panel. Para obtener más detalles acerca del historial de publicación, abra el panel Historial y servidores publicados en la Vista de detalles. En este panel, podrá ver cuándo se publicó el recurso y los servidores en los que se publicó.

## Segunda publicación de recursos y retrasos de CDN {#republished-assets-and-cdn-delays}

Los recursos de Adobe Dynamic Media Classic se distribuyen en la red de entrega de contenido (CDN). CDN es un sistema de servidores de ordenador conectados entre sí que cooperan con transparencia para entregar contenido, especialmente de medios de gran tamaño, a los usuarios finales. En el sistema CDN, el contenido web se almacena en memorias caché web que se encuentran en Internet (red de cachés de Edge). El contenido web se entrega desde las cachés web a los usuarios finales para realizar envíos más rápidos.

La primera vez que alguien descarga una página web, los recursos se envían a un servidor web de almacenamiento en caché de CDN. Se almacenan en este servidor para que la próxima vez que alguien que se encuentre en la misma zona acceda a la página web, se pueda agilizar la entrega del mismo contenido almacenado en la caché. El contenido se entrega con mayor rapidez porque se encuentra más cerca del usuario final. CDN agiliza la visualización de páginas web. Disminuye la necesidad de banda ancha del servidor central porque el contenido se entrega desde la red de borde de almacenamiento en caché, y no desde un servidor central en cada caso.

El contenido de Adobe Dynamic Media Classic recién publicado está disponible inmediatamente para el usuario final y rellena rápidamente la red de caché de Edge. Pero el nuevo contenido que se vuelve a publicar (las imágenes que tienen el mismo nombre que otras imágenes publicadas en un servidor de imágenes) no se actualiza en CDN hasta pasadas diez horas. En lugar de ver este contenido, los usuarios ven el de la memoria caché web de la red CDN. Por este motivo, los recursos que ha vuelto a publicar Adobe Dynamic Media Classic no aparecen a los usuarios finales durante diez horas.

Si desea que los recursos de imagen que se vuelven a publicar estén disponibles antes de ese plazo, puede vaciar las cachés web de CDN. Al vaciar estas memorias se eliminará el contenido antiguo de las cachés web de CDN y será sustituido por los recursos que se han publicado recientemente.

Para vaciar la caché, en la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Invalidar CDN]**. Se eliminan todos los archivos seleccionados de la caché. Si no hay ningún recurso para publicar o no es administrador de empresa, la opción Quitar de CDN no se encuentra disponible.

>[!MORELIKETHIS]
>
>* [Comprobar archivos de trabajo](checking-job-files.md)
>* [Editar, eliminar, pausar y reanudar trabajos recurrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

