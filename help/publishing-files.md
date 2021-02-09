---
title: 'Publicar archivos '
description: Los recursos se publican en los servidores de imágenes de Dynamic Media. Puede publicar recursos una sola vez o organizar que Dynamic Media Classic publique los recursos de forma periódica. Después de publicarse, tiene los recursos disponibles para su entrega. Puede copiar las llamadas mediante URL desde Dynamic Media Classic y agregarlas a su sitio Web o aplicación.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 75%

---


# Publicar archivos {#publishing-files}

Los recursos se publican en los servidores de imágenes de Dynamic Media. Puede publicar recursos una sola vez o organizar que Dynamic Media Classic publique los recursos de forma periódica. Después de publicarse, tiene los recursos disponibles para su entrega. Puede copiar las llamadas mediante URL desde Dynamic Media Classic y agregarlas a su sitio Web o aplicación.

Dynamic Media Classic ahora admite el envío de todas las imágenes y vídeos a través de HTTP/2. Es decir, una URL publicada o código incrustado para la imagen o el vídeo está disponible para integrarse con cualquier aplicación que acepte un recurso alojado. Ese recurso publicado se entrega a través del protocolo HTTP/2. Este método de envío mejora la forma en que se comunican los exploradores y los servidores, lo que permite una mejor respuesta y tiempos de carga de todos los recursos de Dynamic Media Classic. Consulte [Preguntas más frecuentes sobre el Envío HTTP2](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Publicar tras la carga {#publish-after-uploading}

Los recursos están en un estado publicado o no. De forma predeterminada, los recursos que cargue en Dynamic Media Classic se marcan automáticamente para su publicación.

Para obtener más información, consulte el [aviso de publicación instantánea PDF](/help/assets/rendering-instant-publish-notification.pdf).

Para marcar recursos para la publicación, siga estas técnicas:

* **Publicar tras la**
cargaEn la página de carga, cerca de la parte inferior, seleccione Publicar tras la carga. El valor predeterminado es un estado seleccionado.

* **Publicar tras la**
cargaEn el cuadro de diálogo Opciones de trabajo, seleccione Publicar tras la carga. El valor predeterminado es un estado seleccionado.

Algunos recursos &quot;secundarios&quot; se marcan para la publicación de forma automática al marcarse para publicación los recursos principales. En esta tabla se muestran los recursos que se marcan para la publicación de forma automática.

| Elemento principal (grupo) | Elementos secundarios (miembros) |
|--- |--- |
| Conjuntos de imágenes | Imágenes del conjunto. |
| Conjuntos de muestras | Muestras del conjunto. |
| Conjuntos de giros | Imágenes del conjunto. |
| Plantillas | Archivos de plantilla, páginas e imágenes. |

Las imágenes derivadas también se marcan para la publicación de forma automática cuando se están publicando las imágenes principales. Las imágenes derivadas son imágenes que se han ajustado con las opciones de edición de imágenes. Puede ver estas imágenes derivadas en la vista de detalles si selecciona Creación y derivados.

## Creación de un trabajo de publicación  {#creating-a-publish-job}

Cree un trabajo de publicación para publicar los recursos que ha cargado en los servidores de Dynamic Media Classic pero que aún no ha publicado automáticamente. Puede llevar a cabo un trabajo de publicación único o programar trabajos para que se repitan de forma regular. Dynamic Media Classic oferta opciones de publicación avanzadas para publicar en servidores específicos y opciones para volver a publicar recursos que ya se han publicado.

**Para crear un trabajo de publicación**

1. En la barra de navegación global, haga clic en **Publicar**.
1. En el cuadro de diálogo Publicar, seleccione si desea crear un trabajo de publicación de una sola vez o recurrente.

   Consulte [Creación de un trabajo de publicación único](publishing-files.md#creating_a_one_time_publish_job) y [Creación de un trabajo de publicación recurrente](publishing-files.md#creating_a_recurring_publish_job).

1. Introduzca un nombre de trabajo.
1. Si lo desea, acceda a las opciones avanzadas y elija entre estas opciones. 

   Consulte [Opciones avanzadas de publicación](publishing-files.md#advanced_publish_options).

1. Haga clic en **Enviar publ.**.

Dynamic Media Classic realiza un seguimiento de los trabajos de publicación en la página Trabajos. Puede revisar los trabajos de publicación en esta página.

>[!NOTE]
>
>los recursos que se vuelven a publicar (ya publicados con anterioridad) no aparecen de inmediato en la página Web debido al mecanismo Web de almacenamiento en caché de la red de entrega de contenido (CDN), Consulte [Segunda publicación de recursos y retrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Creación de un trabajo de publicación único {#creating-a-one-time-publish-job}

Para crear un trabajo de publicación único seleccione la opción Una vez en la página Publicar.

Si desea iniciar el trabajo de publicación más tarde, seleccione el menú Cuándo y elija Programar para más tarde. A continuación utilice el control deslizante de calendario y hora para seleccionar el día y la hora en que desea ejecutar el trabajo de publicación.

### Creación de un trabajo de publicación recurrente  {#creating-a-recurring-publish-job}

Para crear un trabajo de publicación recurrente seleccione la opción Recurrente en la página Publicar.

A continuación, elija una opción de repetición (A diario, Cada semana, Cada mes o Personalizar) según la frecuencia con que desee que se realice el trabajo. Dynamic Media Classic presenta herramientas de calendario para programar el trabajo de publicación recurrente. Puede elegir la opción Personalizar e introducir una regla en el cuadro Regla para describir un intervalo de trabajos personalizado. 

Consulte [Creación de un intervalo personalizado para un trabajo de carga o publicación](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Los trabajos de publicación (y carga) recurrentes aparecen en la página Trabajos. Si desea editar o eliminar un trabajo programado vaya a la ficha Programados en la página Trabajos.

### Opciones de publicación avanzadas {#advanced-publish-options}

Puede acceder a las opciones avanzadas desde la página Publicar y especificar estas opciones para controlar un trabajo de publicación:

* **Publicar**
paraElija un tipo de servidor para publicar recursos solo en un servidor específico, no en todos los servidores.

* ****
PublicarDe forma predeterminada, Dynamic Media Classic solo publica recursos nuevos que no se hayan publicado anteriormente (la opción Nuevo desde la última publicación). Sin embargo, puede elegir Publicación completa y publicar los recursos que se hayan actualizado o cambiado desde su última publicación. Elija Completa con datos de búsqueda si va a publicar un catálogo electrónico y desea que los lectores puedan realizar búsquedas por palabra clave.

* **Ejecutar trabajo**
comoElija un nombre de usuario en la lista. Desde la página Trabajos, puede ordenar los trabajos por nombre de usuario. Si elige un nombre, asociará el trabajo de publicación con un usuario.

**Notificación HTTPIntroduzca una dirección URL para el déclencheur de los trabajos de publicación posteriores.**


(Consulte [Uso de un trabajo de carga o publicación como desencadenador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)).

## Cancelación de un trabajo de publicación  {#canceling-a-publish-job}

Puede cancelar los trabajos de publicación que están en curso. Además, si es administrador, puede cancelar un trabajo de publicación en curso desde la página Trabajos de la empresa.

Para cancelar un trabajo de publicación, vaya a la página Trabajos y haga clic en Cancelar. En la ficha Programados de la página Trabajos, puede pausar o reanudar un trabajo mediante la casilla de verificación de la columna Activo.

>[!NOTE]
>
>Al cancelar un trabajo de publicación, su estado se cambia a &quot;deteniendo&quot; hasta que el trabajo se pueda detener de forma segura. Si el trabajo de publicación está obteniendo datos de la base de datos, puede que tarde un tiempo en detenerse.

## Publicación manual de recursos  {#manually-publishing-assets}

Puede publicar recursos individuales manualmente en lugar de crear un trabajo de publicación. Cuando publica conjuntos, como un conjunto de imágenes o un conjunto de vídeos adaptable, se publican el conjunto (o “elemento principal”) y todos los miembros (o “elementos secundarios”) dentro de dicho conjunto.

Los recursos sin publicar se indican en la interfaz de usuario con un icono gris redondeado con una barra diagonal (estado sin publicar) a la izquierda del nombre del recurso. Tras publicar un recurso, el icono cambia a verde y tiene una marca de comprobación blanca en el centro (estado publicado).

**Para publicar recursos manualmente**

1. Realice una de las siguientes acciones:

   * En la vista de cuadrícula, la vista de lista o la vista de detalles, utilice los métodos tradicionales de selección de archivos para seleccionar uno o más recursos sin publicar.

      En la barra de navegación global, haga clic en **Archivo > Publicar**.

   * En la vista de cuadrícula, la vista de lista o la vista de detalles, haga clic en el icono gris redondeado con una barra diagonal a la izquierda del nombre del recurso.

## Cancelación manual de la publicación de recursos  {#manually-unpublishing-assets}

Puede cancelar la publicación de los recursos individuales manualmente. Al cancelar la publicación de conjuntos, como un conjunto de muestras o un catálogo electrónico, el conjunto (o “elemento principal”) pasa a un estado no publicado. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Los recursos publicados aparecen en la interfaz de usuario con un icono verde redondeado con una marca de comprobación blanca en el centro (estado publicado) a la izquierda del nombre del recurso. Después de cancelar la publicación de un recurso, el icono se vuelve gris con una barra diagonal (estado sin publicar).

**Para cancelar la publicación de recursos manualmente**

1. Realice una de las siguientes acciones:

   * En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios recursos publicados.

      En la barra de navegación global, haga clic en **Archivo > **Cancelar la publicación**.

   * En la vista de cuadrícula, la vista de lista o la vista de detalles, haga clic en el icono verde redondeado a la izquierda del nombre del recurso.

## Obtención del historial de publicación de un recurso  {#getting-an-asset-s-publish-history}

La última fecha de publicación de los recursos se muestra en la vista de detalles, en la parte superior del panel. Puede obtener más detalles sobre el historial de publicación si abre el panel Historial y servidores publicados en la vista de detalles. En este panel, podrá ver cuándo se publicó el recurso y los servidores en los que se publicó.

## Segunda publicación de recursos y retrasos de CDN {#republished-assets-and-cdn-delays}

Los recursos de Dynamic Media Classic se distribuyen en la red de envío de contenido (CDN). CDN es un sistema de servidores de ordenador conectados entre sí que cooperan con transparencia para entregar contenido, especialmente de medios de gran tamaño, a los usuarios finales. En el sistema CDN, el contenido web se almacena en memorias caché web que se encuentran en Internet (red de cachés de Edge). El contenido web se distribuye a los usuarios finales desde estas memorias caché web para agilizar la distribución.

La primera vez que alguien descarga una página web, los recursos se envían a un servidor web de almacenamiento en caché de CDN. Se almacenan en este servidor para que la próxima vez que alguien que se encuentre en la misma zona acceda a la página web, se pueda agilizar la entrega del mismo contenido almacenado en la caché. El contenido se entrega con mayor rapidez porque se encuentra más cerca del usuario final. CDN agiliza la visualización de páginas web. Disminuye la necesidad de banda ancha del servidor central porque el contenido se entrega desde la red de borde de almacenamiento en caché, y no desde un servidor central en cada caso.

El contenido de Dynamic Media Classic recientemente publicado está disponible inmediatamente para el usuario final y rellena rápidamente la red de Edge Cache. Pero el nuevo contenido que se vuelve a publicar (las imágenes que tienen el mismo nombre que otras imágenes publicadas en un servidor de imágenes) no se actualiza en CDN hasta pasadas diez horas. En lugar de ver este contenido, los usuarios ven el de la memoria caché web de la red CDN. Por este motivo, es posible que los usuarios finales no vean los recursos republicados de Dynamic Media Classic durante diez horas.

Si desea que los recursos de imagen que se vuelven a publicar estén disponibles antes de ese plazo, puede vaciar las cachés web de CDN. Al vaciar estas memorias se eliminará el contenido antiguo de las cachés web de CDN y será sustituido por los recursos que se han publicado recientemente.

Para vaciar la caché, haga clic en Archivo > Inutilizar en CDN. Se eliminan todos los archivos seleccionados de la caché. Si no hay ningún recurso para publicar o no es administrador de empresa, la opción Quitar de CDN no se encuentra disponible.

>[!MORELIKETHIS]
>
>* [Comprobación de archivos de trabajo](checking-job-files.md)
>* [Edición, eliminación, pausa y reanudación de trabajos recurrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

