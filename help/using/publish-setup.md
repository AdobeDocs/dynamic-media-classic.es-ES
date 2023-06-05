---
title: Ajuste de publicación
description: La configuración de Configuración de publicación permite determinar cómo se envían los recursos de forma predeterminada desde los servidores de Adobe Dynamic Media Classic a los sitios web o las aplicaciones.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '2405'
ht-degree: 43%

---

# Ajuste de publicación {#publish-setup}

La configuración de la página Configuración de publicación determina cómo se envían los recursos de forma predeterminada desde los servidores de Adobe Dynamic Media Classic a los sitios web o las aplicaciones. Si no se especifica ninguna configuración, el servidor de Adobe Dynamic Media Classic envía un recurso según una configuración predeterminada en una página de instalación de publicación. Por ejemplo, una solicitud para enviar una imagen que no incluye un atributo de resolución genera una imagen con la configuración Resolución de objeto predeterminada en la página Servidor de imágenes.

Los administradores pueden cambiar la configuración predeterminada de las páginas Servidor de imágenes, Procesador de imágenes y Viñeta para establecer la configuración predeterminada de envío de recursos desde los servidores.

Para abrir las páginas de Configuración de publicación, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes de publicación]**.

>[!NOTE]
>
>Las páginas Ajustes de publicación están destinadas a desarrolladores y programadores de sitios web experimentados. Adobe Dynamic Media Classic supone que los usuarios que cambian la configuración de estas páginas están familiarizados con Adobe Dynamic Media Classic, los estándares y convenciones del protocolo HTTP y la tecnología básica de imágenes.

## Image Server {#image-server}

La página Servidor de imágenes establece la configuración predeterminada para enviar imágenes desde servidores de imágenes. La configuración está disponible en estas cinco categorías (consulte la página del servidor de imágenes para obtener descripciones detalladas de la configuración).

Cambie esta configuración solo con la ayuda de una persona de asistencia de Adobe Dynamic Media Classic.

* **[!UICONTROL Administración de catálogos]** : esta configuración determina cómo interactúan Adobe Dynamic Media Classic y el catálogo. A diferencia de la mayoría de los servidores web, las llamadas URL del servidor de imágenes de Dynamic Media se dirigen a un archivo de manifiesto o catálogo en lugar de a un archivo de imagen adecuado. El archivo de catálogo (que no debe confundirse con un catálogo electrónico) contiene una lista del contenido que se ha publicado en el servidor de imágenes además de la ruta de cada imagen. Si tiene un ID de Digimarc, introduzca su información de usuario en la sección Información de usuario de Digimarc.

* **[!UICONTROL Atributos de solicitud]** : Esta configuración impone límites a las imágenes que se pueden enviar desde el servidor. Por ejemplo, la variable *maximum* **[!UICONTROL Límite de tamaño de imagen de respuesta]** es **[!UICONTROL Ancho]** 5000 y **[!UICONTROL Altura]** 5000.

* **[!UICONTROL Atributos de solicitud predeterminados]** : estos ajustes pertenecen al aspecto predeterminado de las imágenes.

* **[!UICONTROL Atributos de miniatura comunes]** : estos ajustes pertenecen al aspecto y la alineación predeterminados de las imágenes en miniatura.

* **[!UICONTROL Valores predeterminados de campos de catálogo]** : estos ajustes pertenecen a la resolución y al tipo de miniatura predeterminado de las imágenes.

* **[!UICONTROL Atributos de gestión de color]** : Esta configuración determina qué perfiles de color ICC se utilizan.

* **[!UICONTROL Atributos de compatibilidad]** : Esta configuración permite tratar los párrafos inicial y final de las capas de texto como si estuvieran en la versión 3.6 para garantizar la compatibilidad con versiones anteriores.

* **[!UICONTROL Compatibilidad con localización]***: esta configuración le permite administrar varios atributos de configuración regional. También permite especificar una cadena de asignación de configuración regional, de forma que puede definir los idiomas que desee admitir para los distintos consejos de herramientas en los visores.

   Por ejemplo, si es una marca multinacional que vende en distintos países, puede asegurarse de que cada país tiene su propio visor con su propia configuración regional específica. Para llevar a cabo esta funcionalidad, puede especificar una cadena de asignación de configuración regional. A continuación, edite el texto de información de objeto en el ajuste preestablecido de un visualizador añadiendo las cadenas de texto traducidas para el idioma que desee.

   >[!NOTE]
   > Para configurar las opciones de Compatibilidad con localización, [utilice el Admin Console para crear un caso de asistencia.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) En su caso de asistencia, solicite ayuda para la configuración.

   Para más información sobre la configuración de la **[!UICONTROL Asistencia para la localización]**, consulte [Consideraciones al configurar la localización de recursos](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Consideraciones al configurar la localización de recursos {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Si desea configurar las opciones de Compatibilidad con localización en Adobe Dynamic Media Classic, como el campo Mapa de configuración regional, [utilice el Admin Console para crear un caso de asistencia.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) En su caso de asistencia, solicite ayuda para la configuración.

Una forma habitual de utilizar Adobe Dynamic Media Classic es administrar las imágenes de los productos en los sitios web de comercio electrónico. Las empresas internacionales se enfrentan a un reto importante, ya que los recursos para productos similares tienen un aspecto distinto según el país. Por lo general, las diferencias son para algunas partes de los medios generales. Abordar esas diferencias copiando todos los activos para cada uno de los países y sobrescribiendo sólo las diferencias es un esfuerzo tremendo y contradice la metáfora del activo primario único. Dichas diferencias en los recursos pueden ser numerosas, desde vídeos para cada país con diferentes pistas de audio hasta diferencias pequeñas pero importantes en el cable de alimentación que se utiliza con el producto. Adobe Dynamic Media Classic utiliza un mecanismo de búsqueda básico. Puede definir el orden de los sufijos de los recursos en que busca el servidor de imágenes, empezando por la configuración regional requerida.

#### Búsqueda de recursos

La configuración regional de un servicio de imágenes (IS) se identifica con el comando siguiente para IS/IR (procesamiento de imágenes):

`locale=`

Este comando acepta una cadena de ID de configuración regional (locId) que no distingue entre mayúsculas y minúsculas. El ID de configuración regional suele ser una cadena de 2-6 caracteres compuesta por letras y “_”.

IS admite cadenas ASCII imprimibles arbitrarias. El `locale=` tiene un ámbito global, lo que significa que se aplica a toda la solicitud, incluidas todas las solicitudes IS e IR anidadas, las plantillas a las que se hace referencia y las capas de imagen. No se admiten varias configuraciones regionales por solicitud, como por ejemplo una configuración regional distinta para cada capa. Sin embargo, se pueden permitir omisiones explícitas en solicitudes anidadas.

If `locale=` no se ha especificado, `attribute::DefaultLocale` se pasa a los motores de traducción. La validación de entrada limitada se aplica al `locale=` valor. Empty `locale=` Los valores de están permitidos. Porque `locale=` tiene un ámbito global, `attribute::DefaultLocale` es proporcionada por el catálogo principal para toda la solicitud.

Algunas de las ventajas de utilizar `locale=` y `attribute::DefaultLocale` incluir lo siguiente:

* Uso compartido de contenido para varias configuraciones regionales.
* Acceso a contenido de una configuración regional específica con identificadores genéricos.
* Flexibilidad en las convenciones de nombre y la administración del contenido de una configuración regional específica, tal como prefijo de configuración regional en vez de sufijo o contenido para una configuración regional concreta en un catálogo independiente.
* Compatibilidad con el acceso a versiones específicas de la configuración regional.
* Los objetos agregados, como los conjuntos de imágenes, a veces pueden contener referencias genéricas a contenido potencialmente específico de la configuración regional.
* Admite todo el contenido gestionado por catálogos que necesiten localización, incluidas imágenes, conjuntos de imágenes, viñetas, materiales y registros de configuración del visualizador.
* Minimice los cambios de la base de datos de IPS y los mecanismos IS aparentes.
* Cuando se implementa RFC IS-63, se admite contenido estático como vídeos y máscaras.
* Se puede configurar la configuración regional predeterminada.

#### Situaciones de aplicación

| Aplicación | Situación |
| --- | --- |
| Localización del visor | Tras implementar los catálogos de contenido estático, el parámetro locale= añadido a todas las solicitudes a IS controla la localización completamente. Los registros de configuración, las apariencias, pantallas de bienvenida, etc., pueden tener o no variantes regionales. IS proporciona el contenido correcto sin que el visor necesite saber qué parte del contenido se ha localizado y cuáles son sus ID. |
| Imágenes y vídeo | Las compañías multinacionales suelen tener una mezcla de contenido genérico y regional. Con este mecanismo, una referencia a una imagen o un vídeo puede ser genérica, e IS muestra el contenido regional si está disponible. |
| Conjuntos de imágenes y conjuntos de medios | Todo el conjunto de imágenes puede ser diferente para algunas configuraciones regionales, como cuando un catálogo electrónico es diferente, con la traducción de un conjunto de imágenes genérico a uno específico de la configuración regional que gestiona el visor. Con mayor frecuencia, los ID individuales de un conjunto genérico pueden hacer referencia a contenido localizado. Por ejemplo, la mayoría de las fotos de un dispositivo pueden ser las mismas en todos los idiomas, excepto la foto del Panel de control de Campaign. IS traduce automáticamente los identificadores, por lo que no es necesario generar conjuntos de imágenes regionales. |

#### Implementar la localización de recursos

Adobe Dynamic Media Classic y el servicio de imágenes tienen una interfaz que permite localizar imágenes y contenido estático.

Sin localización, una URL del servidor de imágenes tendrá este aspecto:

`https://server/is/image/company/image`

Con la localización, una URL de Image Server agrega el `locale=` a la ruta, como en el siguiente ejemplo:

`https://server/is/image/company/image?locale=de_DE`

Cuando el servidor de imágenes recibe la llamada http, la variable `locale=` se analiza mediante el parámetro `localeMap` campo encontrado en **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes de publicación]** > **[!UICONTROL Servidor de imágenes]** > **[!UICONTROL Compatibilidad con localización]** grupo.

El campo de asignación de configuración regional contiene una lista de entradas separadas por barras verticales (|).

Cada entrada consta de una lista de valores separados por comas. El primer valor es el valor de búsqueda que pasa el `locale=` parámetro. Los valores restantes son valores de sufijo/reemplazo que luego se prueban hasta que uno resulte en una imagen existente.

La aplicación de un sufijo o un valor de sustitución depende del ajuste de la configuración regional global en el grupo **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes de publicación]** > **[!UICONTROL Servidor de imágenes]** > **[!UICONTROL Asistencia para la localización]** .

>[!NOTE]
>
>La configuración regional global solo es posible cuando se establece a través de la API, no dentro de la interfaz de Adobe Dynamic Media Classic.

**Ejemplo de sufijo:**

| URL | ID de localeMap | Resultado |
| --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Observe que no se ha definido GlobalLocale. El parámetro de configuración regional de_DE se compara con la primera entrada de `localeMap`. El primer valor correspondiente _DE se añade como sufijo al recurso image_DE y se intenta encontrarlo en el servidor de imágenes. Si se encuentra en el servidor, se devuelve. De lo contrario, se utiliza como sufijo el segundo valor “”, con lo que se devuelve la propia imagen. |

**Ejemplo de sustitución:**

| URL | `GlobalLocale` y `localeMap` ID | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | En el ejemplo de sustitución superior, GlobalLocale se define en main. El parámetro de configuración regional de_DE se compara con la primera entrada de `localeMap`. La subcadena GlobalLocale se encuentra y se reemplaza por el primer valor correspondiente `de` en el `localeMap`: `image-de-01`. Si se encuentra en el servidor de imágenes, se devuelve. De lo contrario, se sustituye el segundo valor, lo que resulta en `image-main-01`. |

Si no se define ninguna configuración regional en la URL, el servidor de imágenes toma el valor de DefaultLocale, si se ha definido, y lo aplica a la URL.

Si se proporciona un parámetro de configuración regional desconocido o vacío con `locale=`y, a continuación, el `localeMap` se analiza para buscar el valor vacío &quot;comenzando por&quot;. Es importante tener una configuración regional predeterminada aplicada a configuraciones regionales desconocidas.

#### Acerca de defaultImage

El servidor de imágenes prueba las opciones de la configuración regional solicitada, una tras otra. Si no se encuentra ninguna coincidencia, las opciones de configuración regional se aplican a defaultImage y se devuelve la versión coincidente. Por lo tanto, cada configuración regional debe incluir una opción para la imagen sin localización o las versiones de imagen predeterminadas localizadas están disponibles en Adobe Dynamic Media Classic.

#### Situaciones de búsqueda de localeMap

Supongamos que desee admitir las siguientes configuraciones regionales:

`en, en_us, en_uk, de, de_at, de_de, fr`

Estas configuraciones regionales se asignan a los sufijos `_E`, `_G`, y `_F`, para inglés, alemán y francés, respectivamente. En todos los ejemplos, el ID de imagen de entrada genérico es `myImg`.

##### Comportamiento estándar de búsqueda de localeMap

Los ID de configuración regional se asignan a los sufijos correspondientes. Si no se encuentra ningún ID de configuración regional en el catálogo, se prueba un ID genérico. Observe los valores vacíos de locSuffix que se asignan al ID genérico.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID de salida que se buscará |
| --- | --- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Todos los demás | - |

##### Búsqueda de localeMap cuando la configuración regional es desconocida

Puede asignar configuraciones regionales desconocidas a ID específicos o genéricos. Para el ejemplo, puede asignar configuraciones regionales desconocidas a los ID en inglés o, si no existen, a los ID genéricos.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID de salida que se buscará |
| --- | --- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Todos los demás | myImg_E,myImg |

También puede tener un locSuffix dedicado, como U, solo para configuraciones regionales desconocidas y forzar a la imagen predeterminada si no `_U` existe, como en el siguiente ejemplo:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

O bien, puede asignarse directamente al ID genérico, como se muestra a continuación:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Búsqueda del localeMap mediante una búsqueda de varios niveles

Suele ser conveniente agrupar las configuraciones regionales, como Europa, Oriente Medio y Norteamérica, para tratar estándares regionales, como la exposición de la piel. Puede conseguir este efecto con una búsqueda con varios niveles.

Para este ejemplo, supongamos que desee admitir colecciones para su aplicación en Occidente y Oriente. Ambas colecciones se basan en la colección de imágenes genéricas y ambas añaden o modifican ciertas imágenes. Ambas colecciones se refinan aún más para configuraciones regionales específicas, como `m1, m2` para dos variantes de Oriente Medio, y `w1, w2,` y `w3` para tres configuraciones regionales occidentales, excepto que las imágenes se comparten para `w1` y `w3`. Las configuraciones regionales desconocidas solo se asignan a la colección genérica y no tienen acceso a las imágenes específicas de configuración regional. A continuación se muestra qué aspecto tendrá la asignación:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | ID de salida que se buscará |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Todos los demás | mylmg |

##### Busque el localeMap buscando ID específicos

Algunas convenciones de nomenclatura de imágenes no admiten ID de imagen genéricos. Los ID genéricos de la solicitud deben asignarse a un ID específico del catálogo. Sin embargo, hay casos en los que se desconoce el ID específico exacto.

Utilizando el primer ejemplo como base, las imágenes de todos los idiomas podrían tener los sufijos `_1`, `_2`, o `_3`. Las imágenes específicas de las configuraciones regionales en francés pueden tener los sufijos `_22` o `_23` sufijo. Y las imágenes específicas de las configuraciones regionales alemanas podrían tener los sufijos `_470` o `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID de salida que se buscará |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Todos los demás | myImg_1, myImg_2, myImg_3 |

##### Consideraciones importantes al implementar la asistencia para la localización

* La localización se limita a las llamadas de recursos basados en ID y no puede usarse en llamadas de recursos basados en rutas. Por consiguiente, al llamar a vídeos con configuraciones locales, debe llamarse como ID de empresa/recurso; no con la ruta completa del vídeo. No se puede utilizar rtmp con la localización porque ese método es sólo para videollamadas basadas en rutas.
* No puede utilizar conjuntos de medios mixtos que contengan un solo vídeo cuando localeMap está activo; si no, se producirá un error de la llamada al contenido. Para solucionar este problema, puede añadir un solo vídeo a un conjunto de vídeos adaptables. A continuación, añada el conjunto de vídeos adaptable a un conjunto de medios mixtos.
* Algunas solicitudes no se localizan, como las solicitudes de contenido de un conjunto de vídeos adaptable. Por lo tanto, si tiene intención de utilizar conjuntos de vídeos adaptables con la localización, coloque el conjunto de vídeos adaptable dentro de un conjunto de medios mixtos. A continuación, llame al conjunto a un visualizador de medios mixtos con el `locale=` parámetro.

## Procesador de imágenes {#image-renderer}

La página Procesador de imágenes establece la configuración predeterminada para enviar conjuntos de imágenes desde servidores de procesamiento de imágenes. La configuración está disponible en estas cinco categorías (consulte la página del servidor de imágenes para obtener descripciones detalladas de la configuración):

* **[!UICONTROL Administración de catálogos]** : Esta configuración determina cómo interactúan Adobe Dynamic Media Classic y el archivo de catálogo. Las llamadas de URL del servidor de procesamiento de Adobe Dynamic Media Classic se realizan al catálogo, que a su vez llama a para enviar imágenes desde el servidor. Cambie esta configuración solo con la ayuda de una persona de asistencia de Adobe Dynamic Media Classic.

* **[!UICONTROL Atributos de sesión]** : Esta configuración establece parámetros de error, la dirección URL de direcciones URL de imágenes relativas y si se permite la superposición de objetos.

* **[!UICONTROL Atributos de material predeterminados]** : Esta configuración establece la resolución y los ajustes de enfoque predeterminados para las imágenes.

* **[!UICONTROL Atributos de imagen de respuesta]** : estos ajustes pertenecen al aspecto predeterminado de las imágenes.

* **[!UICONTROL Atributos de gestión de color]** - Estos ajustes pertenecen a los ajustes de color predeterminados de las imágenes.

## Viñeta {#vignette}

La página Viñeta ofrece opciones para establecer el aspecto predeterminado de las viñetas (consulte la página para obtener descripciones detalladas de las opciones).
