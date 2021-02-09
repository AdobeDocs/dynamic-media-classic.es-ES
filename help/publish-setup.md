---
title: Ajuste de publicación
description: La configuración de la pantalla Ajustes de publicación determina cómo se envían los recursos de forma predeterminada de los servidores de Dynamic Media Classic a los sitios web o las aplicaciones.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '2418'
ht-degree: 64%

---


# Ajuste de publicación {#publish-setup}

La configuración de la pantalla Ajustes de publicación determina cómo se envían los recursos de forma predeterminada de los servidores de Dynamic Media Classic a los sitios web o las aplicaciones. Si no se especifica ninguna configuración, el servidor de Dynamic Media Classic envía un recurso de acuerdo con la configuración predeterminada de la pantalla Ajustes de publicación. Por ejemplo, si se solicita una imagen que no incluye un atributo de resolución se enviará una imagen con la configuración de Resolución de objeto predeterminada que se encuentra en la pantalla del servidor de imágenes.

Los administradores pueden cambiar la configuración predeterminada de las pantallas Servidor de imágenes, Procesador de imágenes y Viñeta para establecer la configuración predeterminada a la hora de enviar recursos desde los servidores.

Para abrir las pantallas de Ajuste de publicación, haga clic en **Ajustes** > **Ajustes de aplicación** > **Ajustes de publicación**.

>[!NOTE]
>
>las pantallas de Ajuste de publicación están reservadas a los desarrolladores y programadores web experimentados. Dynamic Media Classic supone que los usuarios que cambian la configuración en estas pantallas están familiarizados con Dynamic Media Classic, las normas y convenciones del protocolo HTTP y la tecnología básica de imágenes.

## Servidor de imágenes {#image-server}

La pantalla del servidor de imágenes establece la configuración predeterminada a la hora de enviar imágenes desde los servidores de imágenes. Las opciones de configuración se dividen en estas cinco categorías (consulte la pantalla del servidor de imágenes para ver una descripción detallada de las opciones).

Cambie esta configuración solo con la ayuda de una persona de asistencia técnica de Dynamic Media Classic.

**Administración** de catálogosEsta configuración determina cómo interactúan Dynamic Media Classic y el catálogo. A diferencia de la mayoría de los servidores web, las llamadas mediante URL al servidor de imágenes de Dynamic Media se dirigen a un archivo de catálogo o manifiesto en lugar de a un archivo de imagen en sí. El archivo de catálogo (que no debe confundirse con un catálogo electrónico) contiene una lista del contenido que se ha publicado en el servidor de imágenes además de la ruta de cada imagen. Si tiene un ID de Digimarc, introduzca su información de usuario en la sección Información de usuario de Digimarc.

**Atributos** de solicitudEsta configuración impone límites a las imágenes que se pueden enviar desde el servidor. Por ejemplo, *máximo* **[!UICONTROL Límite de tamaño de imagen de respuesta]** es **[!UICONTROL Ancho]** 5000 y **[!UICONTROL Altura]** 5000.

**Atributos de solicitud predeterminadosEsta configuración se refiere al aspecto predeterminado de las imágenes.** 

**Atributos comunes de** miniaturaEsta configuración se refiere al aspecto y la alineación predeterminados de las imágenes en miniatura.

**Valores predeterminados para** los campos del catálogoEsta configuración se refiere a la resolución y al tipo de miniatura predeterminada de las imágenes.

**Atributos de administración de colorEsta configuración determina qué perfiles de color ICC se utilizan.** 

**Atributos de compatibilidadEsta configuración permite que los párrafos al inicio y al final de las capas de texto se traten como en la versión 3.6 para lograr compatibilidad con versiones anteriores.** 

**Compatibilidad con** localizacionesEsta configuración le permite administrar varios atributos de configuración regional. También permite especificar una cadena de asignación de configuración regional, de forma que puede definir los idiomas que desee admitir para los distintos consejos de herramientas en los visores.

Por ejemplo, si es una marca multinacional que vende en distintos países, puede asegurarse de que cada país tiene su propio visor con su propia configuración regional específica. Para llevar a cabo esta funcionalidad, puede especificar una cadena de asignación de configuración regional. A continuación, puede editar el texto de información sobre herramientas en un ajuste preestablecido del visor, agregando las cadenas de texto traducidas del visor para el idioma que desee.

>[!NOTE]
> Para configurar las opciones de Soporte de Localización, [utilice el Admin Console para crear un caso de soporte.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) En su caso de asistencia, solicite ayuda para configurar la asistencia.

Para más información sobre la configuración de la **Asistencia para la localización**, consulte [Consideraciones al configurar la localización de recursos](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Consideraciones al configurar la localización de recursos {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Si desea configurar las opciones de Soporte de Localización en Dynamic Media Classic, como el campo Asignación de configuración regional, [utilice el Admin Console para crear un caso de soporte.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) En su caso de asistencia, solicite ayuda para configurar la asistencia.

Una forma común de utilizar Dynamic Media Classic es administrar las imágenes de los productos en los sitios web de comercio electrónico. Las empresas internacionales se enfrentan a un reto importante, ya que los recursos para productos similares tienen un aspecto distinto según el país. Normalmente, las diferencias constituyen una pequeña parte de todo el medio. Copiar todos los recursos para cada uno de los países y sobrescribir solo las diferencias es un enorme esfuerzo y contradice el principio de un solo recurso maestro. Dichas diferencias en los recursos pueden ser numerosas, desde vídeos para cada país con diferentes pistas de audio hasta diferencias pequeñas pero importantes en el cable de alimentación que se utiliza con el producto. Dynamic Media Classic utiliza un mecanismo de búsqueda básico. Puede definir el orden de los sufijos de los recursos en que busca el servidor de imágenes, empezando por la configuración regional requerida.

**Búsqueda de recursos**

La configuración regional de un servicio de imágenes (IS) se identifica con el comando siguiente para IS/IR (procesamiento de imágenes):

`locale=`

Este comando acepta una cadena de ID de configuración regional (locId) que no distingue entre mayúsculas y minúsculas. El ID de configuración regional suele ser una cadena de 2-6 caracteres compuesta por letras y “_”.

IS admite cadenas ASCII arbitrarias imprimibles.El comando `locale=` tiene un ámbito global, lo que significa que se aplica a toda la solicitud, incluidas todas las solicitudes IS e IR anidadas, las plantillas a las que se hace referencia y las capas de imagen. No se admiten varias configuraciones regionales por solicitud, como por ejemplo una configuración regional distinta para cada capa. Sin embargo, se pueden permitir omisiones explícitas en solicitudes anidadas.

Si no se especifica `locale=`, `attribute::DefaultLocale` se pasa a los motores de traducción. La validación de entrada limitada se aplica al valor `locale=`. Se permiten valores `locale=` vacíos. Dado que `locale=` tiene un ámbito global, `attribute::DefaultLocale` lo proporciona el catálogo principal para toda la solicitud.

Algunos de los beneficios de utilizar `locale=` y `attribute::DefaultLocale` incluyen lo siguiente:

* Uso compartido de contenido para varias configuraciones regionales.
* Acceso a contenido de una configuración regional específica con identificadores genéricos.
* Flexibilidad en las convenciones de nombre y la administración del contenido de una configuración regional específica, tal como prefijo de configuración regional en vez de sufijo o contenido para una configuración regional concreta en un catálogo independiente.
* Acceso directo a versiones de una configuración regional específica.
* Los objetos agregados, como conjuntos de imágenes, puede contener referencias genéricas a contenido potencialmente específico para una configuración regional.
* Admite todo el contenido administrado por los catálogos que deban localizarse, incluyendo imágenes, conjuntos de imágenes, ilustraciones, materiales y registros de configuración del visor.
* Minimice los cambios de la base de datos de IPS y los mecanismos IS aparentes.
* Se añadirá compatibilidad con contenido estático como vídeos y apariencias cuando se implemente RFC IS-63.
* Se puede configurar la configuración regional predeterminada.

**Situaciones de aplicación**

| Aplicación | Situación |
|--- |--- |
| Localización de un visor | Tras implementar los catálogos de contenido estático, el parámetro locale= añadido a todas las solicitudes a IS controla la localización completamente. Los registros de configuración, las apariencias, pantallas de bienvenida, etc., pueden tener o no variantes regionales. IS proporciona el contenido correcto sin que el visor necesite saber qué parte del contenido se ha localizado y cuáles son sus ID. |
| Imágenes y vídeo | Las compañías multinacionales suelen tener una mezcla de contenido genérico y regional. Con este mecanismo, una referencia a una imagen o un vídeo puede ser genérica, e IS muestra el contenido regional si está disponible. |
| Conjuntos de imágenes y conjuntos de medios | El conjunto de imágenes completo puede ser diferente para algunas configuraciones regionales (por ejemplo, cuando un catálogo electrónico es completamente diferente) con la traducción de un conjunto de imágenes genérico a uno específico de una configuración regional gestionado por el visor.Más comúnmente, los ID individuales de un conjunto genérico pueden referirse a contenido localizado. Por ejemplo, la mayoría de las fotografías de un dispositivo pueden ser iguales en todos los idiomas, excepto la fotografía del panel de control. IS traduce automáticamente los identificadores, por lo que no es necesario generar conjuntos de imágenes regionales. |

**Implementación de la localización de recursos**

Dynamic Media Classic y el servicio de imágenes tienen una interfaz que permite la localización de imágenes y contenido estático.

Sin localización, una URL del servidor de imágenes tendrá este aspecto:

`https://server/is/image/company/image`

Con la localización, una URL del servidor de imágenes agrega el parámetro `locale=` a la ruta, como se muestra a continuación:

`https://server/is/image/company/image?locale=de_DE`

Cuando el servidor de imágenes recibe la llamada http, el parámetro `locale=` se analiza a través del campo localeMap que se encuentra en el grupo **Ajustes** > **Ajustes de aplicación** > **Ajustes de publicación** > **Servidor de imágenes** > **Soporte de Localización&lt;a 10/>.**

El campo de asignación de configuración regional contiene una lista de entradas separadas por barras verticales (|).

Cada entrada consta de una lista de valores separados por comas. El primer valor es el valor de búsqueda que pasa el parámetro `locale=`. Los valores restantes son sufijos o valores de sustitución que se prueban posteriormente hasta que uno resulta en una imagen existente.

La aplicación de un sufijo o un valor de sustitución depende del ajuste de la configuración regional global en el grupo **Ajustes** > **Ajustes de aplicación** > **Ajustes de publicación** > **Servidor de imágenes** > **Asistencia para la localización** .

>[!NOTE]
>
>Actualmente, la configuración regional global solo es posible cuando se establece mediante la API, no en la interfaz de Dynamic Media Classic.

**Ejemplo de sufijo**

| URL | ID de localeMap | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Observe que no se ha definido GlobalLocale. El parámetro de configuración regional de_DE se compara con la primera entrada de localeMap. El primer valor correspondiente _DE se añade como sufijo al recurso image_DE y se intenta encontrarlo en el servidor de imágenes. Si se encuentra en el servidor, se devuelve. De lo contrario, se utiliza como sufijo el segundo valor “”, con lo que se devuelve la propia imagen. |

**Ejemplo de sustitución**

| URL | ID de GlobalLocale y de localeMap | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | En el ejemplo de sustitución superior, GlobalLocale se define en main. El parámetro de configuración regional de_DE se compara con la primera entrada de localeMap. Se busca la subcadena GlobalLocale y se sustituye por el primer valor correspondiente de localeMap: image-de-01. Si se encuentra en el servidor de imágenes, se devuelve. De lo contrario, se sustituye el segundo valor, lo que resulta en image-main-01. |

Si no se define ninguna configuración regional en la URL, el servidor de imágenes toma el valor de DefaultLocale, si se ha definido, y lo aplica a la URL.

Si se proporciona un parámetro de configuración regional desconocido o vacío con `locale=`, se busca en localeMap el valor vacío &quot;comenzando con&quot;. Es importante configurar esta opción para tener una configuración regional predeterminada para configuraciones regionales desconocidas.

**Acerca de defaultImage**

El servidor de imágenes prueba las opciones de la configuración regional solicitada, una tras otra. Si no coincide ninguna, se aplican las opciones de configuración regional a defaultImage y se devuelve la versión coincidente. Por lo tanto, cada configuración regional debe incluir una opción para la imagen sin localización o las versiones de defaultImage localizadas deben estar disponibles en Dynamic Media Classic.

**Situaciones de búsqueda de localeMap**

Supongamos que desee admitir las siguientes configuraciones regionales:

`en, en_us, en_uk, de, de_at, de_de, fr`

Estas configuraciones regionales se asignan a los sufijos `_E`, `_G` y `_F` para inglés, alemán y francés, respectivamente. En todos los ejemplos, el ID de imagen de entrada genérico es `myImg`.

*Comportamiento estándar de búsqueda de localeMap*

Los ID de configuración regional se asignan a los sufijos correspondientes. Si no se encuentra ningún ID de configuración regional en el catálogo, se prueba un ID genérico. Observe los valores vacíos de locSuffix que se asignan al ID genérico.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID de salida que se buscará |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Todos los demás | - |

*Búsqueda de localeMap cuando la configuración regional es desconocida*

Puede asignar configuraciones regionales desconocidas a ID específicos o genéricos. Para este ejemplo, puede asignar configuraciones regionales desconocidas a ID ingleses o, si no existen, a los ID genéricos.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID de salida que se buscará |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Todos los demás | myImg_E,myImg |

También puede tener un locSuffix dedicado, como U, solo para configuraciones regionales desconocidas y forzar la imagen predeterminada si no existe ningún `_U`, como se muestra a continuación:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

O bien, puede asignarse directamente al ID genérico, como se muestra a continuación:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Búsqueda de localeMap mediante una búsqueda con varios niveles*

Suele ser conveniente agrupar las configuraciones regionales, como Europa, Oriente Medio y Norteamérica, para tratar estándares regionales, como la exposición de la piel. Puede conseguir este efecto con una búsqueda con varios niveles.

Para este ejemplo, supongamos que desee admitir colecciones para su aplicación en Occidente y Oriente. Ambas colecciones se basan en la colección de imágenes genéricas y ambas añaden o modifican ciertas imágenes. Ambas colecciones se refinan posteriormente para configuraciones regionales específicas, como `m1, m2` para dos variantes del medio oriente y `w1, w2,` y `w3` para tres configuraciones regionales occidentales, con la diferencia de que las imágenes se comparten para `w1` y `w3`. Las configuraciones regionales desconocidas solo se asignan a la colección genérica y no tienen acceso a las imágenes específicas de configuración regional. A continuación se muestra qué aspecto tendrá la asignación:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | ID de salida que se buscará |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Todos los demás | mylmg |

*Búsqueda de localeMap en ID específicos*

Algunas convenciones de nombre no admiten ID de imágenes genéricos. Los ID genéricos de la solicitud deben asignarse a un ID específico del catálogo. Sin embargo, puede haber casos en los que no se conoce el ID específico exacto.

Utilizando el primer ejemplo como base, las imágenes para todos los idiomas pueden tener los sufijos `_1`, `_2` o `_3`. Las imágenes que son específicas de las configuraciones regionales francesas pueden tener los sufijos `_22` o `_23`. Y las imágenes que son específicas de las configuraciones regionales alemanas pueden tener los sufijos `_470` o `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID de salida que se buscará |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Todos los demás | myImg_1, myImg_2, myImg_3 |

**Consideraciones importantes al implementar la asistencia para la localización**

* La localización se limita a las llamadas de recursos basados en ID y no puede usarse en llamadas de recursos basados en rutas. Por consiguiente, al llamar a vídeos con configuraciones locales, debe llamarse como ID de empresa/recurso; no con la ruta completa del vídeo. Esto significa que no puede utilizar RTMP con la localización porque este método solo se utiliza con llamadas de vídeo basadas en ruta.
* No puede utilizar conjuntos de medios mixtos que contengan un solo vídeo cuando localeMap está activo; si no, se producirá un error de la llamada al contenido. Para solucionar este problema, puede añadir un solo vídeo a un conjunto de vídeos adaptable. A continuación, añada el conjunto de vídeos adaptable a un conjunto de medios mixtos.
* Algunas solicitudes no se localizan, como las solicitudes de contenido de un conjunto de vídeos adaptable. Por tanto, si desea utilizar conjuntos de vídeos adaptables con la localización, debe poner el conjunto de vídeos adaptable dentro de un conjunto de medios mixtos. A continuación, llame al conjunto en un visor de medios mixtos con el parámetro `locale=`.

## Procesador de imágenes {#image-renderer}

La pantalla del procesador de imágenes establece la configuración predeterminada a la hora de enviar conjuntos de imágenes desde los servidores de procesamiento de imágenes. Las opciones de configuración se dividen en estas cinco categorías (consulte la pantalla del servidor de imágenes para ver una descripción detallada de las opciones):

**Administración** de catálogosEsta configuración determina cómo interactúan Dynamic Media Classic y el archivo de catálogo. Las llamadas mediante URL al servidor de procesamiento de Dynamic Media Classic se realizan en el catálogo, que a su vez llama para enviar imágenes desde el servidor. Cambie esta configuración solo con la ayuda de una persona de asistencia técnica de Dynamic Media Classic.

**Atributos de** sesiónEsta configuración establece parámetros de error, la dirección URL de las URL de imagen relativas y si se permite la superposición de objetos.

**Atributos de material predeterminadosEsta configuración establece la resolución predeterminada y la configuración de enfoque de las imágenes.** 

**Atributos de** imagen de respuestaEsta configuración se refiere al aspecto predeterminado de las imágenes.

**Atributos de administración de colorEsta configuración se refiere a la configuración de color predeterminada de las imágenes.** 

## Viñeta {#vignette}

En la pantalla Viñeta se puede establecer la apariencia predeterminada de las viñetas (consulte la pantalla para ver una descripción detallada de las opciones).
