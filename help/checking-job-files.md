---
title: Comprobación de archivos de trabajo
seo-title: Comprobación de archivos de trabajo
description: nulo
seo-description: Descubra cómo comprobar los archivos de trabajo.
uuid: 8241 a 894-3014-4 a 5 c -96 ef -71 f 3 aaa 3716 a
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/upload_ and_ publish_ assets
discoiquuid: d 53 ae 5 dd -8 daf -4 d 87-b 9 a 6-3039 bad 30538
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Comprobación de archivos de trabajo{#checking-job-files}

Para controlar la carga de archivos a Scene 7 Publishing System y los archivos publicados en servidores de Dynamic Media Classic, SPS ofrece la página Trabajos. Desde este página, puede revisar los trabajos de carga y publicación, comprobar el estado de los trabajos y cancelar trabajos de publicación. También puede programar trabajos de carga y publicación.

Cuando carga recursos, aparece un icono que gira junto al menú Trabajos que indica que el trabajo está en curso y el número de archivos que se están procesando. Puede hacer clic en el icono para obtener más información sobre el trabajo activo.

>[!NOTE]
>
>También puede acceder a la lista con las publicaciones recientes desde la página Actividad reciente. Haga clic en Reciente en la barra de navegación global para abrir esta página.

## Acerca de la página Trabajos {#about-the-jobs-page}

Seleccione el botón Trabajos en la barra de navegación global para abrir la página Trabajos. De forma predeterminada, la lista de trabajos empieza por los trabajos más recientes.

En la ficha Historial de la página Trabajos, los trabajos se clasifican según estas categorías:

**Tipo de trabajo** Un icono indica el tipo de trabajo: La carga y la publicación son los tipos de trabajo más comunes.

**Nombre** de trabajo El nombre del trabajo. El nombre está formado por la parte introducida por el usuario y el sello de fecha y hora.

**Se inició** cuando comenzó el trabajo.

**Total** El número de archivos transferidos.

**W (advertencias)** El número de advertencias del trabajo (en caso de existir alguna). Las advertencias indican los problemas sobre el trabajo que no afectan a la finalización del mismo. Normalmente, estas advertencias pueden omitirse porque se refieren a archivos ocultos. Por ejemplo, los archivos .DS_store (Macintosh) y Thumbs.db (Windows) contienen información sobre la manera en que los usuarios finales ven los archivos de imagen. Sin embargo, las entradas de advertencia relacionadas con estos archivos se pueden ignorar porque no están relacionadas con la forma en que se utilizan estos archivos en Dynamic Media Classic. Si desea obtener información detallada sobre las advertencias, puede hacer doble clic en el nombre de trabajo.

**E (errores)** Enumera el número de errores del trabajo (en caso de existir alguno). Si desea obtener información detallada sobre los errores, puede hacer doble clic en el nombre de trabajo.

**Duración** durante cuánto tiempo se llevó a cabo el trabajo.

**Estado** Muestra el estado del trabajo.

**Destino** de los trabajos de carga, el nombre de la empresa y la carpeta a la que se cargaron los archivos. Esta categoría no se aplica a los trabajos de publicación.

**Enviado por** listas que cargaron los recursos.

***Nota**: Puede cancelar los trabajos de publicación y carga en curso haciendo clic en el botón Cancelar situado junto a la barra de progreso.*

## Cambio de vistas en la página Trabajos {#changing-views-on-the-jobs-page}

Para ordenar trabajos o cambiar la vista de la ficha Historial en la página Trabajos, utilice estas técnicas:

**Clasificación** Seleccione un nombre de columna para ordenar la lista según una columna en particular. Para cambiar entre el orden ascendente o descendente, seleccione la flecha que aparece al lado del nombre de la columna.

**Intervalo** de fechas Seleccione el menú Intervalo de fechas y elija una opción para reducir la lista de trabajos a la fecha actual, a la semana anterior o al mes anterior. Elija Intervalo de fechas personalizado para introducir un intervalo de fechas específico.

**Tipo de trabajo** Seleccione el menú Tipo de trabajo y elija Publicar o Cargar para reducir la lista a trabajos de publicación o cargar trabajos. Elija Todo para ver ambos tipos de trabajo.

**Mostrar** elija Mostrar &gt; Mis trabajos o Mostrar &gt; Todos los trabajos para reducir la lista a los trabajos que ha pedido o a los trabajos que han pedido las personas de su empresa.

## Visualización, copia o impresión de un informe con los detalles del trabajo {#viewing-copying-or-printing-a-job-details-report}

En la página Trabajos, haga doble clic en el nombre de un informe para abrir la página con los detalles del trabajo. Esta página ofrece un informe resumido acerca de los archivos del trabajo. Haga clic en Ver detalles para ver el ID de SPS, ruta de destino e información de estado de una entrada. Si ha cargado un archivo PDF o PostScript que requiere fuentes que no están disponibles en SPS, las fuentes que faltan se mostrarán en el informe.

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

### Edición, eliminación, pausa y reanudación de trabajos recurrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Seleccione un trabajo recurrente en la página Trabajos y siga estas instrucciones para editarlo o eliminarlo:

**Edición de un trabajo recurrente** Seleccione el botón Editar e introduzca la información de programación en el cuadro de diálogo Editar trabajo programado. Si desea que el trabajo se repita según un intervalo personalizado, elija Repetir &gt; Personalizar. 

Consulte [Creación de un intervalo personalizado para un trabajo de carga o publicación](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Eliminación de un trabajo recurrente** Seleccione el botón Eliminar.

**Pausar (y reanudar) un trabajo recurrente** en la columna Activo, anule la selección de una casilla de verificación para pausar un trabajo; seleccione una casilla de verificación para reanudar un trabajo en pausa.

### Creación de un intervalo personalizado para un trabajo de carga o publicación {#creating-a-custom-upload-or-publish-job-time-interval}

Si desea crear un intervalo personalizado para un trabajo de carga (por medio de FTP) o publicación, elija Repetir &gt; Personalizar en la página de carga o publicación. A continuación introduzca números y comodines en el cuadro Regla para describir el intervalo de repetición de los trabajos de carga o publicación.

La sintaxis con que se describen los intervalos para los trabajos de carga y publicación en el cuadro Regla es la siguiente:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

For example, `0 15 10 * * ?` schedules a job at 10:15.00 every day.

En las tablas y la lista siguientes se explica cómo se describe un intervalo en el cuadro Regla.

En esta tabla se muestran los períodos temporales, los valores permitidos y los comodines que se admiten:

| Períodos temporales | Valores permitidos | Comentarios | Comodines admitidos |
|--- |--- |--- |--- |
| Segundos | 0-59 |  | , - * / |
| Minutos | 0-59 |  | , - * / |
| Horas | 0-23 | Tenga en cuenta que se utiliza un reloj de 24 horas. | , - * / |
| Día del mes | 1-31 | No puede especificar un valor numérico tanto para "día del mes" como para "día de la semana". Uno de estos campos debe usar el símbolo ?, que actúa como comodín. | , - * / ? L C |
| Mes | 1-12 o Ene, Feb, Mar, Abr, May, Jun, Jul, Ago, Sep, Oct, Nov, Dic., Dic., Dic., Dic., | Los valores distinguen entre mayúsculas y minúsculas. | , - * / |
| Día de la semana | lun, mar, mié, jue, vie, sáb, dom | Los valores distinguen entre mayúsculas y minúsculas. No puede especificar un valor numérico tanto para "día del mes" como para "día de la semana". Uno de estos campos debe usar el símbolo ?, que actúa como comodín. | , - * / ? L C # |
| Año (opcional) | Vacío o 1970-2099 |  | , - * / |


En esta tabla se muestran los caracteres comodín que se admiten en el cuadro Regla y cómo se utilizan estos caracteres:

| Carácter comodín | Nombre | Qué describe |
|--- |--- |--- |
| * | Asterisco | Todos los valores (por ejemplo, "cada minuto"). |
| ? | Signo de interrogación | Ningún valor específico (por ejemplo, "cualquier minuto dentro de la hora especificada"). |
| , | Coma | Valores adicionales (por ejemplo, "lunes y miércoles"). |
| - | Guión | Intervalo de valores (por ejemplo, "de lunes a viernes"). |
| / | Barra diagonal | Períodos (por ejemplo, "cada 15 minutos"). |
| L | L mayúscula | Último "día del mes" o "día de la semana" (solo disponible para estos campos). Por ejemplo, si el mes es enero y se escribe el valor L en el campo "día del mes" el trabajo se programa para el 31 de enero.En el campo "día de la semana", puede introducir este carácter si desea programar el trabajo para que se ejecute los sábados. Puede utilizarlo con un número (por ejemplo, 6 L) para especificar el último viernes del mes. No especifique L con los comodines coma o guión. |
| # | Almohadilla | Número del día de la semana dentro del mes (solo disponible para el campo "día de la semana").Por ejemplo, si introduce 5#3 en el campo "día de la semana" el trabajo se ejecutará en tercer viernes del mes. El 5 representa el "viernes" (el quinto día de la semana) y el 3 equivale a la tercera vez que se da en el mes. |
| C | # C mayúscula | Primer "día del mes" o "día de la semana" en el calendario (solo disponible para estos campos). Por ejemplo: si se especifica un valor de 1 C para el "día del mes", se programará el primer día del calendario que se produce el día o después del quinto. Para el campo "día de la semana", especifique 1 C programando el primer día del calendario que se produzca a los lunes o después del lunes. |

En esta lista se pueden ver ejemplos de cómo se describen los intervalos de tiempo en el cuadro Regla:

* 0 0 12 * * ?: a mediodía todos los días
* 0 15 10 ? * *: a las 10:15 todos los días
* 0 0/5 14 * * ?: cada 5 minutos entre las 14:00 y las 14:55 todos los días
* 0 0/5 14,18 * * ?: cada 5 minutos entre las 14:00 y las 14:55 todos los días y cada 5 minutos entre las 18:00 y las 18:55 todos los días
* 0 10,44 14 ? 3: los miércoles a las 14:10 y a las 14:44 y todos los miércoles de marzo
* 0 15 10 ? *: Lunes a viernes a las 10:15 todos los días de la semana
* 0 15 10 20 * ?: a las 10:15 el día 20 de cada mes
* 0 15 10 L * ?: a las 10:15 el último día de cada mes
* 0 15 10 ? * 6L: a las 10:15 el último sábado de cada mes
* 0 15 10 * * 5#3: a las 10:15 el tercer viernes de cada mes

## Uso de un trabajo de carga o publicación como desencadenador {#using-an-upload-or-publish-job-as-a-trigger}

Al cargar recursos por medio de FTP o al ejecutar un trabajo de publicación, se programa un trabajo posterior que se iniciará en cuanto finalice la carga. (Si hay otros trabajos programados para ese mismo momento, el trabajo que programe aquí se colocará detrás de ellos). El nuevo trabajo envía una notificación a la dirección especificada para activar el código de esa ubicación. Este trabajo de carga que sigue recibe el mismo nombre que el trabajo de carga actual, pero se le añade el prefijo _Pub.

Para hacer que un trabajo de carga o publicación desencadene otro trabajo, seleccione Avanzada en la página de carga o publicación. A continuación, introduzca la URL en el campo de texto Notificación http.