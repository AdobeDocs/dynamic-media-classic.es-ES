---
title: Ajuste de publicación
description: La configuración de la configuración de publicación permite determinar cómo se envían los recursos de forma predeterminada desde los servidores de Adobe Dynamic Media Classic a los sitios web o las aplicaciones.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '2383'
ht-degree: 30%

---

# Ajuste de publicación {#publish-setup}

La configuración de la página Configuración de publicación determina cómo se envían los recursos de forma predeterminada desde los servidores de Adobe Dynamic Media Classic a los sitios web o las aplicaciones. Si no se especifica ninguna configuración, el servidor de Adobe Dynamic Media Classic envía un recurso según una configuración predeterminada en una página de instalación de publicación. Por ejemplo, una solicitud para enviar una imagen que no incluye un atributo de resolución genera una imagen con la configuración Resolución de objeto predeterminada en la página Servidor de imágenes.

Los administradores pueden cambiar la configuración predeterminada de las páginas Servidor de imágenes, Procesador de imágenes y Viñeta para establecer la configuración predeterminada de envío de recursos desde los servidores.

Para abrir las páginas de Configuración de publicación, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Configuración de publicación]**.

>[!NOTE]
>
>Las páginas Ajustes de publicación son para uso de programadores y desarrolladores de sitios Web experimentados. Adobe Dynamic Media Classic supone que los usuarios que cambian la configuración de estas páginas están familiarizados con Adobe Dynamic Media Classic, los estándares y convenciones del protocolo HTTP y la tecnología básica de imágenes.

## Image Server {#image-server}

La página Servidor de imágenes establece la configuración predeterminada para enviar imágenes desde los servidores de imágenes. La configuración está disponible en estas cinco categorías (consulte la página del servidor de imágenes para obtener descripciones detalladas de la configuración).

Cambie esta configuración solo con la ayuda de una persona de asistencia de Adobe Dynamic Media Classic.

* **[!UICONTROL Administración de catálogos]**: esta configuración determina cómo interactúan Adobe Dynamic Media Classic y el catálogo. A diferencia de la mayoría de los servidores web, las llamadas URL del servidor de imágenes de Dynamic Media se dirigen a un archivo de manifiesto o catálogo en lugar de a un archivo de imagen adecuado. El archivo de catálogo (que no debe confundirse con un catálogo electrónico) contiene una lista de todo el contenido publicado en el servidor de imágenes. También contiene la ruta a cada imagen. Si tiene un ID de Digimarc, introduzca su información de usuario en la sección Información de usuario de Digimarc.

* **[!UICONTROL Atributos de solicitud]**: esta configuración impone límites a las imágenes que se pueden entregar desde el servidor. Por ejemplo, el *límite máximo* de **[!UICONTROL tamaño de imagen de respuesta]** es de **[!UICONTROL ancho]** 5000 y **[!UICONTROL alto]** 5000.

* **[!UICONTROL Atributos de solicitud predeterminados]**: esta configuración pertenece al aspecto predeterminado de las imágenes.

* **[!UICONTROL Atributos de miniatura comunes]**: esta configuración se refiere al aspecto y la alineación predeterminados de las imágenes en miniatura.

* **[!UICONTROL Valores predeterminados de los campos de catálogo]**: esta configuración pertenece a la resolución y al tipo de miniatura predeterminado de las imágenes.

* **[!UICONTROL Atributos de administración de color]**: esta configuración determina qué perfiles de color ICC se utilizan.

* **[!UICONTROL Atributos de compatibilidad]**: esta configuración permite que los párrafos inicial y final de las capas de texto se traten como en la versión 3.6 para garantizar la compatibilidad con versiones anteriores.

* **[!UICONTROL Compatibilidad con localización]**: esta configuración le permite administrar varios atributos de configuración regional. También permite especificar una cadena de asignación de configuración regional, de forma que puede definir los idiomas que desee admitir para los distintos consejos de herramientas en los visores.

  Por ejemplo, si es una marca multinacional que vende en distintos países, puede asegurarse de que cada país tiene su propio visor con su propia configuración regional específica. Para llevar a cabo esta funcionalidad, puede especificar una cadena de asignación de configuración regional. A continuación, edite el texto de la información del objeto en el ajuste preestablecido de un visor. Solo tiene que añadir las cadenas de texto traducidas para el idioma que desee.

  >[!NOTE]
  > Para configurar las opciones de soporte de localización, [use Admin Console para crear un caso de soporte.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) En su caso de soporte técnico, solicite ayuda para la configuración.

  Para más información sobre la configuración de la **[!UICONTROL Asistencia para la localización]**, consulte [Consideraciones al configurar la localización de recursos](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Consideraciones al configurar la localización de recursos {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Si desea configurar opciones de soporte de localización en Adobe Dynamic Media Classic, como el campo Locale Map, [use Admin Console para crear un caso de soporte.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) En su caso de soporte técnico, solicite ayuda para la configuración.

Una forma habitual de utilizar Adobe Dynamic Media Classic es administrar las imágenes del producto en sitios web de e-Commerce. Las empresas internacionales se enfrentan a un reto importante, ya que los recursos para productos similares tienen un aspecto distinto según el país. Por lo general, las diferencias son para algunas partes de los medios generales. Abordar esas diferencias copiando todos los activos para cada uno de los países y sobrescribiendo sólo las diferencias es un esfuerzo tremendo y contradice la metáfora del activo primario único. Dichas diferencias en los recursos pueden ser numerosas, desde vídeos para cada país con diferentes pistas de audio hasta diferencias pequeñas pero importantes en el cable de alimentación que se utiliza con el producto. Adobe Dynamic Media Classic utiliza un mecanismo de búsqueda básico. Puede definir el orden de los sufijos de los recursos en que busca el servidor de imágenes, empezando por la configuración regional requerida.

#### Localización de los recursos

La configuración regional de un servicio de imágenes (IS) se identifica con el comando siguiente para IS/IR (procesamiento de imágenes):

`locale=`

Este comando acepta una cadena de ID de configuración regional (locId) que no distingue entre mayúsculas y minúsculas. El identificador de configuración regional suele ser una cadena de entre 2 y 6 caracteres compuesta por letras y &quot;`_`&quot;.

IS admite cadenas ASCII imprimibles arbitrarias. El comando `locale=` tiene un ámbito global, lo que significa que se aplica a toda la solicitud, incluidas todas las solicitudes IS e IR anidadas, las plantillas a las que se hace referencia y las capas de imagen. No se admiten varias configuraciones regionales por solicitud, como por ejemplo una configuración regional distinta para cada capa. Sin embargo, se pueden permitir omisiones explícitas en solicitudes anidadas.

Si no se especifica `locale=`, se pasa `attribute::DefaultLocale` a los motores de traducción. Se aplica una validación de entrada limitada al valor `locale=`. Se permiten valores `locale=` vacíos. Dado que `locale=` tiene un ámbito global, `attribute::DefaultLocale` lo proporciona el catálogo principal para toda la solicitud.

Algunos de los beneficios de usar `locale=` y `attribute::DefaultLocale` son los siguientes:

* Uso compartido de contenido para varias configuraciones regionales.
* Acceso a contenido de una configuración regional específica con identificadores genéricos.
* Flexibilidad en las convenciones de nombre y la administración del contenido de una configuración regional específica, tal como prefijo de configuración regional en vez de sufijo o contenido para una configuración regional concreta en un catálogo independiente.
* Compatibilidad con el acceso a versiones específicas de la configuración regional.
* Los objetos agregados, como los conjuntos de imágenes, a veces pueden contener referencias genéricas a contenido potencialmente específico de la configuración regional.
* Admite todo el contenido administrado por catálogos que necesitan localización, incluidas imágenes, conjuntos de imágenes, viñetas, materiales y registros de configuración del visualizador.
* Minimice los cambios de la base de datos de IPS y los mecanismos IS aparentes.
* Cuando se implementa RFC IS-63, se admite contenido estático como vídeos y máscaras.
* Se puede configurar la configuración regional predeterminada.

#### Escenarios de aplicación

| Aplicación | Situación |
| --- | --- |
| Localización del visor | Una vez implementados los catálogos de contenido estático, la localización se controla completamente con el parámetro locale=, anexado a todas las solicitudes realizadas a IS. Los registros de configuración, las apariencias, pantallas de bienvenida, etc., pueden tener o no variantes regionales. IS proporciona el contenido correcto sin que el visor necesite saber qué parte del contenido se ha localizado y cuáles son sus ID. |
| Imágenes y vídeo | Las compañías multinacionales suelen tener una mezcla de contenido genérico y regional. Con este mecanismo, una referencia a una imagen o un vídeo puede ser genérica, e IS muestra el contenido regional si está disponible. |
| Conjuntos de imágenes y conjuntos de medios | Todo el conjunto de imágenes puede ser diferente para algunas configuraciones regionales, como cuando un catálogo electrónico es diferente, con la traducción de un conjunto de imágenes genérico a uno específico de la configuración regional que gestiona el visor. Con mayor frecuencia, los ID individuales de un conjunto genérico pueden hacer referencia a contenido localizado. Por ejemplo, la mayoría de las fotos de un dispositivo pueden ser las mismas en todos los idiomas, excepto la foto del Panel de control de Campaign. IS traduce automáticamente los ID, por lo que no es necesario generar conjuntos de imágenes específicos de la configuración regional. |

#### Implementar la localización de recursos

Adobe Dynamic Media Classic y el servicio de imágenes tienen una interfaz que permite la localización de imágenes y contenido estático.

Sin localización, una URL del servidor de imágenes tendrá este aspecto:

`https://server/is/image/company/image`

Con la localización, una URL de Image Server agrega el parámetro `locale=` a la ruta de acceso, como se muestra a continuación:

`https://server/is/image/company/image?locale=de_DE`

Cuando el servidor de imágenes recibe la llamada http, el parámetro `locale=` se analiza a través del campo `localeMap` que se encuentra en el grupo **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Configuración de publicación]** > **[!UICONTROL Servidor de imágenes]** > **[!UICONTROL Compatibilidad con localización]**.

El campo de asignación de configuración regional contiene una lista de entradas separadas por barras verticales (|).

Cada entrada consta de una lista de valores separados por comas. El primer valor es el valor de búsqueda que se pasa a través del parámetro `locale=`. Los valores restantes son valores de sufijo/reemplazo que luego se prueban hasta que uno resulte en una imagen existente.

La aplicación de un sufijo o un valor de sustitución depende del ajuste de la configuración regional global en el grupo **[!UICONTROL Ajustes]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes de publicación]** > **[!UICONTROL Servidor de imágenes]** > **[!UICONTROL Asistencia para la localización]** .

>[!NOTE]
>
>La configuración regional global solo es posible cuando se establece a través de la API, no dentro de la interfaz de Adobe Dynamic Media Classic.

**Ejemplo de sufijo:**

| URL | ID de localeMap | Resultado | Notas |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Observe que no se ha definido GlobalLocale. El parámetro de configuración regional de_DE se compara con la primera entrada en `localeMap`. El primer valor _DE correspondiente se añade como sufijo al recurso image_DE y se intenta encontrarlo en el servidor de imágenes. Si se encuentra en el servidor, se devuelve. De lo contrario, se utiliza el segundo valor &quot;&quot; como sufijo, lo que hace que se devuelva la propia imagen. |

**Ejemplo de reemplazo:**

| URL | ID de `GlobalLocale` y `localeMap` | Resultado | Notas |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | En el ejemplo de reemplazo anterior, GlobalLocale se establece en main. El parámetro de configuración regional de_DE se compara con la primera entrada en `localeMap`. La subcadena GlobalLocale se encuentra y se reemplaza por el primer valor correspondiente `de` en `localeMap`: `image-de-01`. Si se encuentra en el servidor de imágenes, se devuelve. Si no es así, se reemplaza el segundo valor, dando como resultado `image-main-01`. |

Si no se define ninguna configuración regional en la URL, el servidor de imágenes toma el valor de DefaultLocale, si se ha definido, y lo aplica a la URL.

Si se proporciona un parámetro de configuración regional desconocido o vacío con `locale=`, se busca en el `localeMap` el valor vacío &quot;comenzando por&quot;. Es importante tener una configuración regional predeterminada aplicada a configuraciones regionales desconocidas.

#### Acerca de defaultImage

El servidor de imágenes prueba las opciones de la configuración regional solicitada, una tras otra. Si no se encuentra ninguna coincidencia, las opciones de configuración regional se aplican a defaultImage y se devuelve la versión coincidente. Por lo tanto, cada configuración regional debe incluir una opción para la imagen sin localización o las versiones de imagen predeterminadas localizadas están disponibles en Adobe Dynamic Media Classic.

#### Escenarios para encontrar el localeMap

Supongamos que desee admitir las siguientes configuraciones regionales:

`en, en_us, en_uk, de, de_at, de_de, fr`

Estas configuraciones regionales se asignan a los sufijos `_E` (inglés), `_G` (alemán) y `_F` (francés). Para todos los ejemplos, el identificador de imagen de entrada genérico es `myImg`.

##### Comportamiento estándar para encontrar el localeMap

Los ID de configuración regional se asignan a los sufijos correspondientes. Si no se encuentra ningún ID de configuración regional en el catálogo, se prueba un ID genérico. Observe los valores de locSuffix vacíos que se asignan al ID genérico.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID de salida que se buscará |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Todos los demás | : |

##### Búsqueda del localeMap cuando se desconoce la configuración regional

Puede asignar configuraciones regionales desconocidas a ID específicos o genéricos. Por ejemplo, puede asignar configuraciones regionales desconocidas a los ID en inglés o, si no existen, a los ID genéricos.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID de salida que se buscará |
| --- | --- |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Todos los demás | myImg_E, myImg |

También puede tener un locSuffix dedicado, como U, solo para configuraciones regionales desconocidas y forzar a la imagen predeterminada si no existe `_U`, como en el siguiente ejemplo:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

O bien, puede asignarse directamente al ID genérico, como se muestra a continuación:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Búsqueda del localeMap mediante una búsqueda de varios niveles

Suele ser conveniente agrupar las configuraciones regionales, como Europa, Oriente Medio y Norteamérica, para tratar estándares regionales, como la exposición de la piel. Puede conseguir este efecto con una búsqueda con varios niveles.

Por ejemplo, supongamos que desea admitir colecciones para uso occidental y de Oriente Medio. Ambas colecciones se basan en la colección de imágenes genéricas y ambas añaden o modifican ciertas imágenes. Ambas colecciones se refinan aún más para configuraciones regionales específicas. Por ejemplo, `m1, m2` para dos variantes de Oriente Medio y `w1, w2,` y `w3` para tres configuraciones regionales occidentales, excepto que las imágenes se comparten para `w1` y `w3`. Las configuraciones regionales desconocidas solo se asignan a la colección genérica y no tienen acceso a las imágenes específicas de configuración regional. A continuación se muestra qué aspecto tendrá la asignación:

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

Utilizando el primer ejemplo como base, las imágenes de todos los idiomas podrían tener los sufijos `_1`, `_2` o `_3`. Las imágenes específicas de las configuraciones regionales en francés podrían tener los sufijos `_22` o `_23`. Y las imágenes específicas de las configuraciones regionales alemanas podrían tener los sufijos `_470` o `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID de salida que se buscará |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Todos los demás | myImg_1, myImg_2, myImg_3 |

##### Consideraciones importantes al implementar la compatibilidad con la localización

* La localización se limita a las llamadas de recursos basados en ID y no puede usarse en llamadas de recursos basados en rutas. Por consiguiente, al llamar a vídeos con configuraciones locales, debe llamarse como ID de empresa/recurso; no con la ruta completa del vídeo. No puede usar `RTMP` con la localización porque ese método es solo para llamadas de vídeo basadas en rutas de acceso.
* No puede utilizar conjuntos de medios mixtos que contengan un solo vídeo cuando localeMap está activo; si no, se producirá un error de la llamada al contenido. Para solucionar este problema, puede añadir un solo vídeo a un conjunto de vídeos adaptables. A continuación, añada el conjunto de vídeos adaptable a un conjunto de medios mixtos.
* Algunas solicitudes no se localizan, como las solicitudes de contenido de un conjunto de vídeos adaptable. Por lo tanto, si tiene intención de utilizar conjuntos de vídeos adaptables con la localización, coloque el conjunto de vídeos adaptable dentro de un conjunto de medios mixtos. A continuación, llame al conjunto a un visualizador de medios mixtos con el parámetro `locale=`.

## Procesador de imágenes {#image-renderer}

La página Procesador de imágenes establece la configuración predeterminada para enviar conjuntos de imágenes desde servidores de procesamiento de imágenes. La configuración está disponible en estas cinco categorías (consulte la página del servidor de imágenes para obtener descripciones detalladas de la configuración):

* **[!UICONTROL Administración de catálogos]**: esta configuración determina cómo interactúan Adobe Dynamic Media Classic y el archivo de catálogo. Las llamadas de URL del servidor de procesamiento de Adobe Dynamic Media Classic se realizan al catálogo, que a su vez llama a para enviar imágenes desde el servidor. Cambie esta configuración solo con la ayuda de una persona de asistencia de Adobe Dynamic Media Classic.

* **[!UICONTROL Atributos de sesión]**: esta configuración establece parámetros de error, la dirección URL de direcciones URL de imágenes relativas y si se permite la superposición de objetos.

* **[!UICONTROL Atributos de material predeterminados]**: esta configuración establece la resolución y el enfoque predeterminados para las imágenes.

* **[!UICONTROL Atributos de imagen de respuesta]**: esta configuración pertenece al aspecto predeterminado de las imágenes.

* **[!UICONTROL Atributos de administración de color]**: esta configuración pertenece a la configuración de color predeterminada de las imágenes.

## Viñeta {#vignette}

La página Viñeta ofrece opciones para establecer el aspecto predeterminado de las viñetas (consulte la página para obtener descripciones detalladas de las opciones).
