---
title: Comprobación de archivos de trabajo
description: Obtenga información sobre cómo comprobar los archivos de trabajo.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Administración de recursos
role: Profesional empresarial
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1605'
ht-degree: 71%

---


# Comprobación de archivos de trabajo{#checking-job-files}

Para supervisar las cargas de archivos a Dynamic Media Classic y los archivos que publica en los servidores de Dynamic Media Classic, Dynamic Media Classic ofrece la página Trabajos . Desde este página, puede revisar los trabajos de carga y publicación, comprobar el estado de los trabajos y cancelar trabajos de publicación. También puede programar trabajos de carga y publicación.

Cuando carga recursos, aparece un icono que gira junto al menú Trabajos que indica que el trabajo está en curso y el número de archivos que se están procesando. Puede hacer clic en el icono para obtener más información sobre el trabajo activo.

>[!NOTE]
>
>También puede acceder a la lista con las publicaciones recientes desde la página Actividad reciente. Haga clic en Reciente en la barra de navegación global para abrir esta página.

## Acerca de la página Trabajos  {#about-the-jobs-page}

Seleccione el botón Trabajos en la barra de navegación global para abrir la página Trabajos. De forma predeterminada, la lista de trabajos empieza por los trabajos más recientes.

En la ficha Historial de la página Trabajos, los trabajos se clasifican según estas categorías:

**Tipo de** trabajoUn icono indica el tipo de trabajo: Cargar y publicar son los tipos de trabajo más comunes.

**Nombre** del trabajoEl nombre del trabajo. El nombre está formado por la parte introducida por el usuario y el sello de fecha y hora.

**** ComenzadoCuando se inició el trabajo.

**** Total: el número de archivos transferidos.

**W (advertencias)** El número de advertencias en el trabajo (si las hay). Las advertencias indican los problemas sobre el trabajo que no afectan a la finalización del mismo. Normalmente, estas advertencias pueden omitirse porque se refieren a archivos ocultos. Por ejemplo, los archivos .DS_store (Macintosh) y Thumbs.db (Windows) contienen información sobre la manera en que los usuarios finales ven los archivos de imagen. Sin embargo, las entradas de advertencia relativas a estos archivos se pueden ignorar porque no se refieren a cómo se utilizan estos archivos en Dynamic Media Classic. Si desea obtener información detallada sobre las advertencias, puede hacer doble clic en el nombre de trabajo.

**E (errores)** Muestra el número de errores en el trabajo (si los hay). Si desea obtener información detallada sobre los errores, puede hacer doble clic en el nombre de trabajo.

**** DuraciónEl tiempo que se tardó en completar el trabajo.

**** StatusMuestra el estado del trabajo.

**** DestinoPara los trabajos de carga, el nombre de la empresa y la carpeta a la que se cargaron los archivos. Esta categoría no se aplica a los trabajos de publicación.

**Enviado** porListas que cargaron los recursos.

***Nota **: Para cancelar los trabajos de publicación y carga en curso, haga clic en el botón Cancelar situado junto a la barra de progreso.*

## Cambio de vistas en la página Trabajos {#changing-views-on-the-jobs-page}

Para ordenar trabajos o cambiar la vista de la ficha Historial en la página Trabajos, utilice estas técnicas:

**** SortingSeleccione un nombre de columna para ordenar la lista por una columna concreta. Para cambiar entre el orden ascendente o descendente, seleccione la flecha que aparece al lado del nombre de la columna.

**Intervalo de** fechasSeleccione el menú Intervalo de fechas y elija una opción para reducir la lista de trabajos a la fecha actual, a la semana anterior o al mes anterior. Elija Intervalo de fechas personalizado para introducir un intervalo de fechas específico.

**Tipo de** trabajoSeleccione el menú Tipo de trabajo y elija Publicar o Cargar para reducir la lista para publicar trabajos o cargar trabajos. Elija Todo para ver ambos tipos de trabajo.

**** MostrarSeleccione Mostrar > Mis trabajos o Mostrar > Todos los trabajos para reducir la lista a los trabajos que haya pedido o a los que hayan pedido los empleados de la empresa.

## Ver, copiar o imprimir un informe de Detalles del trabajo {#viewing-copying-or-printing-a-job-details-report}

En la página Trabajos, haga doble clic en el nombre de un informe para abrir la página con los detalles del trabajo. Esta página ofrece un informe resumido acerca de los archivos del trabajo. Haga clic en Ver detalle para ver el Dynamic Media ID de una entrada, la ruta de destino y la información de estado. Si ha cargado un archivo PDF o PostScript que requiere fuentes que no están disponibles en Dynamic Media Classic, el informe enumera las fuentes que faltan.

Puede copiar esta información en el portapapeles.

1. En la página Trabajos, haga doble clic en el nombre de un informe para abrir la página con los detalles del trabajo. 
1. Haga clic en Ver detalles para obtener un informe detallado sobre una entrada.
1. Haga clic en Copiar en el portapapeles.

## Gestión de trabajos recurrentes de carga y publicación {#handling-recurring-upload-and-publish-jobs}

Los trabajos recurrentes de carga y publicación que se crean en las páginas de carga y publicación se muestran en la ficha Programados de la página Trabajos. Desde esta ficha, puede editar y eliminar los trabajos recurrentes.

Seleccione el botón Trabajos en la barra de navegación global y, una vez en la página Trabajos, seleccione la ficha Programados para editar o eliminar los trabajos recurrentes.

>[!NOTE]
>
>La lista de trabajos de esta ficha puede filtrarse con los menús Tipo de trabajo y Mostrar. Elija un tipo de trabajo para reducir la lista a trabajos de publicación de un tipo específico. Elija la opción Mostrar para mostrar los trabajos creados por usted o los trabajos creados por todos los empleados de su empresa.

### Edición, eliminación, pausa y reanudación de trabajos recurrentes  {#editing-deleting-pausing-and-resuming-recurring-jobs}

Seleccione un trabajo recurrente en la página Trabajos y siga estas instrucciones para editarlo o eliminarlo:

**Edición de un** trabajo recurrenteSeleccione el botón Editar e introduzca la información de programación en el cuadro de diálogo Editar Trabajo Programado. Si desea que el trabajo se repita según un intervalo personalizado, elija Repetir > Personalizar. 

Consulte [Creación de un intervalo personalizado para un trabajo de carga o publicación](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Eliminación de un** trabajo recurrenteSeleccione el botón Eliminar.

**Pausar (y reanudar) un** trabajo recurrenteEn la columna Activo, anule la selección de una casilla de verificación para pausar un trabajo; seleccione una casilla de verificación para reanudar un trabajo que se haya pausado.

### Creación de un intervalo personalizado para un trabajo de carga o publicación {#creating-a-custom-upload-or-publish-job-time-interval}

Si desea crear un intervalo personalizado para un trabajo de carga (por medio de FTP) o publicación, elija Repetir > Personalizar en la página de carga o publicación. A continuación introduzca números y comodines en el cuadro Regla para describir el intervalo de repetición de los trabajos de carga o publicación.

La sintaxis con que se describen los intervalos para los trabajos de carga y publicación en el cuadro Regla es la siguiente:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Por ejemplo, `0 15 10 * * ?` programa un trabajo a las 10:15.00 todos los días.

En las tablas y la lista siguientes se explica cómo se describe un intervalo en el cuadro Regla.

En esta tabla se muestran los períodos temporales, los valores permitidos y los comodines que se admiten:

| Períodos temporales | Valores permitidos | Comentarios | Comodines admitidos |
|--- |--- |--- |--- |
| Segundos | 0-59 |  | , - * / |
| Minutos | 0-59 |  | , - * / |
| Horas | 0-23 | Tenga en cuenta que se utiliza un reloj de 24 horas. | , - * / |
| Día del mes | 1-31 | No puede especificar un valor numérico tanto para &quot;día del mes&quot; como para &quot;día de la semana&quot;. Uno de estos campos debe usar el símbolo ?, que actúa como comodín. | , - * / ? L C |
| Mes | 1-12 o Ene, Feb, Mar, Abr, Mayo, Jun, Julio, Ago, Sep, Sep, Oct, Nov, Dic | Los valores distinguen entre mayúsculas y minúsculas. | , - * / |
| Día de la semana | lun, mar, mié, jue, vie, sáb, dom | Los valores distinguen entre mayúsculas y minúsculas. No puede especificar un valor numérico tanto para &quot;día del mes&quot; como para &quot;día de la semana&quot;. Uno de estos campos debe usar el símbolo ?, que actúa como comodín. | , - * / ? L C # |
| Año (opcional) | Vacío o 1970-2099 |  | , - * / |


En esta tabla se muestran los caracteres comodín que se admiten en el cuadro Regla y cómo se utilizan estos caracteres:

| Carácter comodín | Nombre | Qué describe |
|--- |--- |--- |
| * | Asterisco | Todos los valores (por ejemplo, &quot;cada minuto&quot;). |
| ? | Signo de interrogación | Ningún valor específico (por ejemplo, &quot;cualquier minuto dentro de la hora especificada&quot;). |
| , | Coma | Valores adicionales (por ejemplo, &quot;lunes y miércoles&quot;). |
| - | Guión | Intervalo de valores (por ejemplo, &quot;de lunes a viernes&quot;). |
| / | Barra diagonal | Períodos (por ejemplo, &quot;cada 15 minutos&quot;). |
| L | L mayúscula | Último &quot;día del mes&quot; o &quot;día de la semana&quot; (solo disponible para estos campos). Por ejemplo, si el mes es enero y se escribe el valor L en el campo &quot;día del mes&quot; el trabajo se programa para el 31 de enero.En el campo &quot;día de la semana&quot;, puede introducir este carácter si desea programar el trabajo para que se ejecute los sábados. Puede usarlo con un número (por ejemplo, 6L) para especificar el último viernes del mes. No especifique L con los caracteres comodín de coma o guión. |
| # | Almohadilla | Número del día de la semana dentro del mes (solo disponible para el campo &quot;día de la semana&quot;).Por ejemplo, si introduce 5#3 en el campo &quot;día de la semana&quot; el trabajo se ejecutará en tercer viernes del mes. El 5 representa el &quot;viernes&quot; (el quinto día de la semana) y el 3 equivale a la tercera vez que se da en el mes. |
| C | # C mayúscula | Primer &quot;día del mes&quot; o &quot;día de la semana&quot; en el calendario (solo disponible para estos campos). Por ejemplo, si se especifica un valor de 1C para &quot;día del mes&quot;, se programará el primer día del calendario que se produzca en el quinto día o después de él. Para el campo &quot;día de la semana&quot;, si se especifica 1C, se programará el primer día del calendario que se produzca el domingo o después de él |

En esta lista se pueden ver ejemplos de cómo se describen los intervalos de tiempo en el cuadro Regla:

* 0 0 12 * * ?: a mediodía todos los días
* 0 15 10 ? * *: a las 10:15 todos los días
* 0 0/5 14 * * ?: cada 5 minutos entre las 14:00 y las 14:55 todos los días
* 0 0/5 14,18 * * ?: cada 5 minutos entre las 14:00 y las 14:55 todos los días y cada 5 minutos entre las 18:00 y las 18:55 todos los días
* 0 10,44 14 ? 3: los miércoles a las 14:10 y a las 14:44 y todos los miércoles de marzo
* 0 15 10 ? *: Lunes a viernes a las 10:15 todos los días entre semana
* 0 15 10 20 * ?: a las 10:15 el día 20 de cada mes
* 0 15 10 L * ?: a las 10:15 el último día de cada mes
* 0 15 10 ? * 6L: a las 10:15 el último sábado de cada mes
* 0 15 10 * * 5#3: a las 10:15 el tercer viernes de cada mes

## Uso de un trabajo de carga o publicación como desencadenador  {#using-an-upload-or-publish-job-as-a-trigger}

Al cargar recursos por medio de FTP o al ejecutar un trabajo de publicación, se programa un trabajo posterior que se iniciará en cuanto finalice la carga. (Si hay otros trabajos programados para ese mismo momento, el trabajo que programe aquí se colocará detrás de ellos). El nuevo trabajo envía una notificación a la dirección especificada para activar el código de esa ubicación. Este trabajo de carga que sigue recibe el mismo nombre que el trabajo de carga actual, pero se le añade el prefijo _Pub.

Para hacer que un trabajo de carga o publicación desencadene otro trabajo, seleccione Avanzada en la página de carga o publicación. A continuación, introduzca la URL en el campo de texto Notificación http.
