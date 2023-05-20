---
title: Comprobar archivos de trabajo
description: Obtenga información sobre cómo comprobar los archivos de trabajo en Adobe Dynamic Media Classic.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '1596'
ht-degree: 38%

---

# Comprobar archivos de trabajo{#checking-job-files}

Para monitorizar las cargas de archivos a Adobe Dynamic Media Classic y los archivos que publica en los servidores de Adobe Dynamic Media Classic, Adobe Dynamic Media Classic ofrece la página Trabajos. Desde este página, puede revisar los trabajos de carga y publicación, comprobar el estado de los trabajos y cancelar trabajos de publicación. También puede programar trabajos de carga y publicación.

Cuando carga recursos, aparece un icono que gira junto al menú Trabajos que indica que el trabajo está en curso y el número de archivos que se están procesando. Puede seleccionar el icono para ver más información sobre el trabajo activo.

>[!NOTE]
>
>También puede acceder a la lista con las publicaciones recientes desde la página Actividad reciente. Seleccionar **[!UICONTROL Reciente]** en la barra de navegación global.

## Acerca de la página Trabajos {#about-the-jobs-page}

Seleccionar **[!UICONTROL Trabajos]** en la barra de navegación global, para que se abra la página Trabajos. De forma predeterminada, la lista de trabajos empieza por los trabajos más recientes.

En la ficha Historial de la página Trabajos, los trabajos se clasifican según estas categorías:

* **[!UICONTROL Tipo de trabajo]** : Un icono indica el tipo de trabajo: Cargar y Publicar son los tipos de trabajo más comunes.

* **[!UICONTROL Nombre de trabajo]** - El nombre del trabajo. El nombre incluye la parte del nombre introducida por el usuario, así como la fecha y la hora.

* **[!UICONTROL Iniciado]** - Cuando comenzó el trabajo.

* **[!UICONTROL Total]** - El número de archivos transferidos.

* **[!UICONTROL W (advertencias)]** : el número de advertencias del trabajo (si las hay). Las advertencias indican los problemas sobre el trabajo que no afectan a la finalización del mismo. Normalmente, estas advertencias pueden omitirse porque se refieren a archivos ocultos. Por ejemplo, `.DS_store` Los archivos (Macintosh) y Thumbs.db (Windows®) contienen información sobre cómo mostrar archivos de imagen a los usuarios. Sin embargo, las entradas de advertencia relativas a estos archivos se pueden ignorar porque no pertenecen a cómo se utilizan estos archivos en Adobe Dynamic Media Classic. Si desea obtener información detallada sobre las advertencias, puede hacer doble clic en el nombre de trabajo.

* **[!UICONTROL E (errores)]** - Indica el número de errores en el trabajo (si los hay). Si desea obtener información detallada sobre los errores, puede hacer doble clic en el nombre de trabajo.

* **[!UICONTROL Duración]** - Cuánto tiempo se tardó en completar el trabajo.

* **[!UICONTROL Estado]** - Muestra el estado del trabajo.

* **[!UICONTROL Destino]** : para trabajos de carga, el nombre de la empresa y la carpeta en la que se cargaron los archivos. Esta categoría no se aplica a los trabajos de publicación.

* **[!UICONTROL Enviado por]** : lista de los usuarios que cargaron los recursos.

>[!NOTE]
>
>Puede cancelar los trabajos de publicación y carga en curso seleccionando la variable **[!UICONTROL Cancelar]** junto a la barra de progreso.

## Cambiar vistas en la página Trabajos {#changing-views-on-the-jobs-page}

Para ordenar trabajos o cambiar la vista de la ficha Historial en la página Trabajos, utilice estas técnicas:

* **[!UICONTROL Ordenando]** : seleccione un nombre de columna para ordenar la lista por una columna en particular. Para cambiar entre el orden ascendente o descendente, seleccione la flecha que aparece al lado del nombre de la columna.

* **[!UICONTROL Intervalo de fechas]** - Seleccione el **[!UICONTROL Intervalo de fechas]** y elija una opción para reducir la lista de trabajos a la fecha actual, la semana anterior o el mes anterior. Seleccionar **[!UICONTROL Intervalo de fechas personalizado]**, luego introduzca un intervalo de fechas específico.

* **[!UICONTROL Tipo de trabajo]** - Seleccione el **[!UICONTROL Tipo de trabajo]** y elija **[!UICONTROL Publish]** o **[!UICONTROL Cargar]** para reducir la lista a trabajos de publicación o carga. Seleccionar **[!UICONTROL Todo]** para ver ambos tipos de trabajos.

* **[!UICONTROL Mostrar]** - Vaya a **[!UICONTROL Mostrar]** > **[!UICONTROL Mis trabajos]** o **[!UICONTROL Mostrar]** > **[!UICONTROL Todas las tareas]** para reducir la lista a los trabajos que ha pedido o a los trabajos que han pedido los miembros de su compañía.

## Ver, copiar o imprimir un informe de Detalles del trabajo {#viewing-copying-or-printing-a-job-details-report}

Haga doble clic en el nombre de un informe en la página Trabajos para que se abra la página Detalles del trabajo. Esta página ofrece un informe resumido acerca de los archivos del trabajo. Seleccionar **[!UICONTROL Ver detalles]** para poder ver el Adobe Dynamic Media Classic ID, la ruta de destino y la información de estado de una entrada. Si ha cargado un archivo PostScript o de PDF que requiera fuentes que no estén disponibles en Adobe Dynamic Media Classic, el informe indicará las fuentes que faltan.

Puede copiar esta información en el portapapeles.

1. Haga doble clic en el nombre de un informe en la página Trabajos.
1. En la página Detalles del trabajo, seleccione **[!UICONTROL Ver detalles]** para obtener un informe detallado sobre una entrada.
1. Seleccionar **[!UICONTROL Copiar al portapapeles]**.

## Gestión de trabajos recurrentes de carga y publicación {#handling-recurring-upload-and-publish-jobs}

Los trabajos recurrentes de carga y publicación que se crean en las páginas de carga y publicación se muestran en la ficha Programados de la página Trabajos. Desde esta ficha, puede editar y eliminar los trabajos recurrentes.

Seleccione el botón Trabajos en la barra de navegación global y, en la página Trabajos, seleccione la opción **[!UICONTROL Programado]** para poder editar y eliminar trabajos recurrentes.

>[!NOTE]
>
>Puede filtrar la lista de trabajos en **[!UICONTROL Programado]** pestaña con el **[!UICONTROL Tipo de trabajo]** y **[!UICONTROL Mostrar]** menús. Seleccione un tipo de trabajo para poder reducir la lista y publicar trabajos de un tipo específico. Seleccione una **[!UICONTROL Mostrar]** si desea mostrar los trabajos que ha creado o los creados por todos los miembros de su empresa.

### Editar, eliminar, pausar y reanudar trabajos recurrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Seleccione un trabajo recurrente en la página Trabajos y siga estas instrucciones si desea editarlo o eliminarlo:

* **Editar un trabajo recurrente** - Seleccione el **[!UICONTROL Editar]** y escriba la información de programación en el cuadro de diálogo Editar trabajo programado. Si desea que el trabajo se repita en un intervalo de su elección, vaya a **[!UICONTROL Repetir]** > **[!UICONTROL Personalizado]**.

Consulte [Crear un intervalo de tiempo de trabajo de carga o publicación personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Eliminación de un trabajo recurrente** - Seleccione el **[!UICONTROL Eliminar]** botón.

* **Pausa (y reanudación) de un trabajo recurrente** : en la columna Activo, anule la selección de una casilla de verificación para pausar un trabajo; seleccione una casilla de verificación para reanudar un trabajo que se haya pausado.

### Crear un intervalo de tiempo de trabajo de carga o publicación personalizado {#creating-a-custom-upload-or-publish-job-time-interval}

Para crear un intervalo de tiempo personalizado para una carga (a través de FTP) o un trabajo de publicación, en la página Cargar o Publicar, vaya a **[!UICONTROL Repetir]** > **[!UICONTROL Personalizado]**. A continuación, introduzca números y caracteres comodín en el cuadro Regla que describa un intervalo de tiempo para que los trabajos de carga o publicación se repitan.

La sintaxis con que se describen los intervalos para los trabajos de carga y publicación en el cuadro Regla es la siguiente:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Por ejemplo, `0 15 10 * * ?` programa un trabajo a las 10:15 todos los días.

En las tablas y la lista siguientes se explica cómo se describe un intervalo en el cuadro Regla.

En esta tabla se muestran los períodos temporales, los valores permitidos y los comodines que se admiten:

| Períodos temporales | Valores permitidos | Comentarios | Comodines admitidos |
|--- |--- |--- |--- |
| Segundos | 0-59 |  | `, - * /` |
| Minutos | 0-59 |  | `, - * /` |
| Horas | 0-23 | Tenga en cuenta que se utiliza un reloj de 24 horas. | `, - * /` |
| Día del mes | 1-31 | No puede especificar un valor numérico tanto para &quot;día del mes&quot; como para &quot;día de la semana&quot;. Uno de estos campos debe utilizar un `?` carácter comodín. | `, - * / ? L C` |
| Mes | 1-12 o enero, febrero, marzo, abril, mayo, junio, julio, agosto, septiembre, septiembre, octubre, noviembre, diciembre | Los valores distinguen entre mayúsculas y minúsculas. | `, - * /` |
| Día de la semana | lun, mar, mié, jue, vie, sáb, dom | Los valores distinguen entre mayúsculas y minúsculas. No puede especificar un valor numérico tanto para &quot;día del mes&quot; como para &quot;día de la semana&quot;. Uno de estos campos debe utilizar un `?` carácter comodín. | `, - * / ? L C #` |
| Año (opcional) | Vacío o 1970-2099 |  | `, - * /` |


En esta tabla se muestran los caracteres comodín que se admiten en el cuadro Regla y cómo se utilizan estos caracteres:

| Carácter comodín | Nombre | Qué describe |
|--- |--- |--- |
| `*` | Asterisco | Todos los valores (por ejemplo, &quot;cada minuto&quot;). |
| `?` | Signo de interrogación | Ningún valor específico (por ejemplo, &quot;cualquier minuto dentro de la hora especificada&quot;). |
| `,` | Coma | Otros valores (por ejemplo, &quot;lunes y miércoles&quot;). |
| `-` | Guión | Intervalo de valores (por ejemplo, &quot;de lunes a viernes&quot;). |
| `/` | Barra diagonal | Períodos (por ejemplo, &quot;cada 15 minutos&quot;). |
| `L` | L mayúscula | Último &quot;día del mes&quot; o &quot;día de la semana&quot; (solo disponible para estos campos). Por ejemplo, si el mes es enero y se escribe el valor L en el campo &quot;día del mes&quot; el trabajo se programa para el 31 de enero. En el campo &quot;día de la semana&quot;, puede introducir este carácter si desea programar el trabajo para que se ejecute los sábados. Puede utilizarlo con un número (por ejemplo, `6L`) para especificar el último viernes del mes. No especificar `L` con los comodines de coma o guión. |
| `#` | Almohadilla | Número del día de la semana dentro del mes (solo disponible para el campo &quot;día de la semana&quot;). Por ejemplo, `6#3` en el campo &quot;día de la semana&quot; especifica el tercer viernes del mes. El `6` indica &quot;viernes&quot; (el sexto día de la semana) y `3` indica la tercera incidencia en el mes. |
| `C` | # C mayúscula | Primer &quot;día del mes&quot; o &quot;día de la semana&quot; en el calendario (solo disponible para estos campos). Por ejemplo, si se especifica un valor de `1C` para las programaciones de &quot;día del mes&quot;, el primer día del calendario que se produce en el quinto día o después de este. Para el campo &quot;día de la semana&quot;, especificando `1C` programa el primer día del calendario que se produzca el domingo o después |

En esta lista se pueden ver ejemplos de cómo se describen los intervalos de tiempo en el cuadro Regla:

* `0 0 12 * * ?` : a mediodía todos los días
* `0 15 10 ? * *` : a las 10:15 todos los días
* `0 0/5 14 * * ?`: cada 5 minutos entre las 14:00 y las 14:55 todos los días
* `0 0/5 14,18 * * ?` : cada 5 minutos entre las 14:00 y las 14:55 todos los días y cada 5 minutos entre las 18:00 y las 18:55 todos los días
* `0 10,44 14 ? 3` : los miércoles a las 14:10 y a las 14:44 y todos los miércoles de marzo
* `0 15 10 ? *` : Lunes a viernes a las 10:15 todos los días laborables
* `0 15 10 20 * ?` : a las 10:15 el día 20 de cada mes
* `0 15 10 L * ?` : a las 10:15 el último día de cada mes
* `0 15 10 ? * 6L` : a las 10:15 el último sábado de cada mes
* `0 15 10 * * 6#3` : A las 10:15 am del tercer viernes de cada mes

## Uso de un trabajo de carga o publicación como déclencheur {#using-an-upload-or-publish-job-as-a-trigger}

Al cargar recursos a través de FTP o ejecutar un trabajo de publicación, puede programar un trabajo posterior para que comience cuando se complete la carga. (Si hay otros trabajos programados para empezar, el trabajo que programa aquí se pone en cola detrás de ellos). El nuevo trabajo envía una notificación a la dirección especificada para que se pueda activar el código en esa ubicación. Este trabajo de carga que sigue recibe el mismo nombre que el trabajo de carga actual, pero se le añade el prefijo _Pub.

Para convertir un trabajo de carga o publicación en otro déclencheur, seleccione **[!UICONTROL Avanzadas]** en la página Cargar o publicar. A continuación, introduzca la URL en el campo de texto Notificación http.
