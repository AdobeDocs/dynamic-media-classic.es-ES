---
title: Visualización, adición y exportación de metadatos
seo-title: Visualización, adición y exportación de metadatos
description: nulo
seo-description: Obtenga información sobre cómo ver, agregar y exportar metadatos.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: referencia
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Visualización, adición y exportación de metadatos{#viewing-adding-and-exporting-metadata}

Puede almacenar información específica sobre los archivos con que trabaja en Scene7 Publishing System; esta información recibe el nombre de *metadatos*. Puede utilizar los metadatos en Dynamic Media Classic para organizar, buscar, filtrar y ordenar los recursos.

Los metadatos aparecen en la vista de detalles junto con la información generada por Dynamic Media Classic, como la fecha de creación del archivo, la fecha de publicación y las palabras clave. Para ver los metadatos, abra el recurso en la vista de detalles y seleccione el panel Metadatos. Puede introducir y editar metadatos en la vista de detalles.

Algunos metadatos están incrustados directamente en un archivo. Si un archivo contiene estos metadatos, Dynamic Media Classic los carga automáticamente con el archivo. Puede incrustar metadatos en recursos de origen en Adobe Photoshop, InDesign, Illustrator y otras aplicaciones; Dynamic Media Classic reconoce estos metadatos. También puede añadir metadatos a archivos individuales en el panel de metadatos, en la vista de detalles. Para mantener la coherencia entre los recursos, los administradores de empresa pueden crear plantillas de metadatos que proporcionen los campos de metadatos que se pueden rellenar.

For more information about embedded metadata, see [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Visualización de metadatos {#view-metadata}

Para ver los metadatos de un recurso, abra el recurso en la vista de detalles y seleccione el panel Metadatos. A continuación, seleccione una opción en el menú Vista de metadatos para seleccionar un conjunto de campos de metadatos. Dynamic Media Classic ofrece estas vistas de metadatos:

* **Vista compacta** Una lista básica de valores.

* **IPTC** Values según la definición del Consejo Internacional de Telecomunicaciones de Prensa.

* **Valores XMP** definidos por la plataforma de metadatos extensible.

Los administradores pueden crear vistas de metadatos. Estas vistas también aparecen en el menú Vistas de metadatos. Para obtener más información acerca de la creación de vistas de metadatos, consulte [Vistas de metadatos](application-setup.md#metadata_views).

## Introducción manual de metadatos para un recurso {#manually-enter-metadata-for-an-asset}

1. Abra el recurso en la vista de detalles.
1. Abra el panel Metadatos y realice una de estas acciones o ambas:

   * Elija una vista de metadatos para determinar qué campos de metadatos aparecen en el panel.
   * Elija un valor de ajuste preestablecido y haga clic en Aplicar para rellenar los campos de metadatos con valores de ajustes preestablecidos. Los administradores de empresas son los encargados de crear estos valores de ajustes preestablecidos.

1. Introduzca los valores en el panel Metadatos.

>[!NOTE]
>
>Para editar los metadatos de varios recursos a la vez, seleccione los recursos y haga clic en Archivo &gt; Editar información. Los cambios que se hagan en la ventana Editar información se aplicarán a todos los recursos seleccionados.

## Adición o edición de palabras clave {#add-or-edit-keywords}

Además de los metadatos, las palabras clave también le pueden servir para buscar y gestionar sus recursos.

Si durante la sesión ha agregado palabras clave para otros archivos, o si las ha eliminado de su lista, aparecerán todas en la tabla Sugerencias de palabras clave.

1. Abra el archivo en la vista de detalles.
1. Haga clic en Palabras clave.
1. Para agregar palabras clave, realice lo siguiente:

   * Escriba una palabra clave en el cuadro de texto y haga clic en Agregar.
   * En la tabla Sugerencias de palabras clave, haga clic en una palabra clave.

1. Para eliminar una palabra clave, selecciónela y haga clic en Eliminar. Pasará a incluirse en la tabla Sugerencias de palabras clave.

>[!NOTE]
Puede agregar palabras clave a los archivos al cargarlos en Dynamic Media Classic. En el cuadro de diálogo Opciones de trabajo de carga, seleccione Metadatos adicionales e introduzca palabras clave. Consulte [Opciones de carga](uploading-files.md#upload_options).

## Importación de metadatos {#import-metadata}

En lugar de introducir los metadatos manualmente de uno en uno, puede importar los metadatos para varios recursos diferentes desde un archivo delimitado por tabuladores o XML. Introducir los metadatos en un archivo delimitado por tabuladores o XML e importar este archivo requiere menos tiempo que si se introducen estos metadatos en recursos individuales. En la primera fila del archivo delimitado por tabuladores, introduzca el ID y los nombres de los campos para los que desea grabar los metadatos. En cada fila posterior, introduzca un nombre de ID de recurso seguido de los valores de los metadatos. Los campos que no se incluyen en el archivo XML o delimitado por tabuladores no se modificarán. Para importar metadatos desde un archivo XML, asegúrese de que cumple con el archivo DTD.

>[!NOTE]
Puede crear una plantilla para introducir los metadatos de modo que puedan importarse correctamente en Scene7 Publishing System. Una vez creada la plantilla, puede utilizarla para introducir los metadatos. Consulte [Creación de una plantilla para la introducción y carga de metadatos](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Puede obtener más información sobre las propiedades estandarizadas en: https://www.adobe.com/devnet/xmp.html

1. En el panel Examinar, seleccione las imágenes a las que quiera agregar metadatos a partir del archivo delimitado por tabuladores o XML.
1. Haga clic en **Archivo** &gt; **Importar metadatos**.
1. En el cuadro de diálogo **Cargar metadatos**, haga clic en **Examinar**.
1. En el cuadro de diálogo **Seleccionar archivos para cargar**, seleccione el archivo XML o delimitado por tabuladores que contenga los metadatos.
1. Introduzca un nombre de trabajo.
1. Haga clic en **Cargar**.

**Identificación de los distintos tipos de metadatos en la importación**

Tenga en cuenta lo siguiente al identificar diferentes tipos de metadatos para su importación:

* Los campos personalizables se identifican por su nombre según se crearon en Ajustes &gt; Ajustes de aplicación &gt; Metadatos &gt; Campos personalizables. Utilice la función de Generar archivo para obtener una lista de todos los campos personalizables definidos con el formato correcto de importación.
* Las propiedades de metadatos XMP deben tener el prefijo XMP correspondiente antes que el nombre (propiedad- ). Dos puntos separan el prefijo y el nombre. El prefijo XMP se puede encontrar en Ajustes &gt; Ajustes de aplicación &gt; Metadatos &gt; Editor de esquemas de metadatos. Los nombres técnicos se pueden encontrar en la documentación del esquema de XMP correspondiente. Tenga en cuenta que los nombres de propiedades XMP no aparecen en la función Generar archivo.
* Las propiedades del esquema de metadatos deben tener el prefijo correspondiente antes del nombre (propiedad- ). Dos puntos separan el prefijo y el nombre. El prefijo y los nombres de propiedad se definen en el editor de esquemas de metadatos. Tenga en cuenta que los nombres de propiedades de los esquemas de metadatos no aparecen en la función Generar archivo.

Por ejemplo: la propiedad XMP para las palabras clave es el esquema de XMP "Dublin Core" con el prefijo "dc" y "subject" es el nombre técnico de XMP. El prefijo y nombre XMP técnico se combinan en el nombre de propiedad completo "dc:subject". En el formato importación de metadatos XML, "dc.subject" debe ser el nombre de la propiedad. En el formato de importación delimitado por tabuladores, ése debe ser el encabezado de columna.

**Importación de palabras clave**

Las palabras clave se pueden importar como listas separadas por comas. Si una coma aparece en cualquiera de los valores individuales, necesita una barra invertida (\) como carácter de escape. Una barra invertida literal es la barra invertida doble habitual (\\).

Por ejemplo, un archivo de importación de metadatos que contenga el valor "Hello\, World!,barra\\invertida,foo" para "dc:subject" presenta tres palabras clave XMP en el recurso: "Hello, World!" "barra\invertida" y "foo".

**Importación de archivos XMP de metadatos de esquemas de metadatos y XMP**

La importación de XML solo acepta XML válido. Al importar los campos de esquemas de metadatos o XMP, se agrega el prefijo de espacio de nombre y se comporta como un espacio de nombre XMP. Este espacio de nombre se debe declarar, por ejemplo, en la etiqueta de nivel superior.

Por ejemplo:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importación de archivos delimitados por tabuladores de metadatos de esquemas de metadatos y XMP**

El prefijo debe agregarse en el encabezado de la columna correspondiente del campo de importación.

## Importación de metadatos (mediante FTP) {#import-metadata-via-ftp}

Para importar metadatos para varios archivos, introduzca los metadatos en un archivo XML o delimitado por tabuladores y seleccione la opción Procesar archivos de metadatos en la pantalla de carga mediante FTP.

Asegúrese de que los datos del archivo XML o delimitado por tabuladores tienen el formato correcto. En la primera fila, introduzca el campo de ID seguido de los nombres de los campos de metadatos que desea modificar. En cada fila posterior, introduzca un nombre de ID de recurso seguido de los valores de los metadatos. Los campos que no se incluyen en el archivo XML o delimitado por tabuladores no se modificarán.

Haga clic en el botón Cargar en la barra de navegación global y, en la pantalla Trabajos, elija la ficha Por medio de FTP para importar los metadatos. A continuación, haga clic en Opciones de trabajo. En el cuadro de diálogo Opciones de trabajo de carga, elija Procesar archivos de metadatos.

## Cambio de nombre de ID por lotes con metadatos {#batch-rename-ids-using-metadata}

Puede cambiar el nombre de los ID de Scene7 Publishing System con metadatos importados de un archivo delimitado por tabuladores o un archivo XML. Los metadatos importados solo se aplican a las imágenes que se especifican en el archivo de metadatos. No importa si las imágenes están seleccionadas en el panel Examinar.

To rename an image’s Scene7 Publishing System ID, add a column labeled *newipsid* to the tab-delimited file, or add a field called* new_vc_objectname* to the XML data.

Por ejemplo:

| ipsid | newipsid |
|--- |--- |
| pruebachaqueta_1 | Prueba_chaqueta_1 |
| pruebachaqueta_azul | Prueba_chaqueta_2 |


El registro de trabajos para el trabajo de metadatos muestra qué ID se han cambiado correctamente y cuáles no.

## Creación de una plantilla para la introducción y carga de metadatos {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic ofrece un comando para crear una plantilla para grabar metadatos. El uso de esta plantilla garantiza que los metadatos se introducen con el formato correcto de modo que puedan cargarse correctamente a Scene7 Publishing System. Siga estos pasos para crear una plantilla y utilizarla en la grabación e importación de metadatos a Scene7 Publishing System:

1. Seleccione recursos de imagen con los campos de metadatos que desee incluir en la plantilla.
1. Elija Archivo &gt; Importar metadatos.
1. Seleccione Imagen para el tipo de propiedades de recurso.
1. En el menú de generación de archivos, seleccione Plantilla delimitada por tabuladores, Metadatos XML de recursos o DTD de XML.
1. Haga clic en Generar.
1. Copie los datos en el cuadro de diálogo que aparece. Utilice estos datos para construir la plantilla.

## Trabajo con esquemas de metadatos {#working-with-metadata-schemas}

Un administrador de empresa puede ver una lista de todos los esquemas disponibles. Abra Ajustes de aplicación &gt; Metadatos &gt; Esquema de metadatos.

Inicialmente, en la lista, los esquemas de estándares globales como XMP se encuentran ocultos. Para verlos, use la casilla de verificación de la parte inferior de la lista.

Los administradores de empresa pueden crear un nuevo esquema personalizado o editar un esquema personalizado existente.

Puede utilizar el editor de esquemas de metadatos para realizar las siguientes acciones:

| Acción | Descripción |
|--- |--- |
| Agregar | Añade una nueva propiedad al esquema. Un cuadro de diálogo modal recopila la siguiente información: ID, etiqueta, estructura y tipo de datos. |
| Agregar valor de opción | Agrega una nueva opción seleccionable a una propiedad con estructura Opción abierta u Opción cerrada. Todos los valores de opción son del mismo tipo. Debe seleccionar la propiedad para activar el botón. |
| Editar | Permite editar la etiqueta de una propiedad o valor de opción. Solo se puede cambiar la etiqueta, ID, y la información de tipo es inmutable. |
| Mover hacia arriba/Mover hacia abajo | El orden en el esquema se refleja en la interfaz de usuario. Para cambiar el orden, seleccione una propiedad o un valor de opción, y muévalos con los botones. La función de arrastrar y soltar no se admite en este momento. |
| Eliminar | Elimina una propiedad o un valor de opción del esquema. No elimina los valores del bloque XMP ni la base de datos. La propiedad ya no está disponible para vistas de metadatos y se elimina de la vista de detalles del recurso. Si la propiedad se ha publicado en el servidor de metadatos, fuerce la publicación para eliminar los datos del servidor de metadatos público. |

El sistema genera automáticamente un esquema personalizado para los campos definidos por el usuario con el prefijo "s7udf". Éstos son los campos definidos por el usuario existentes y se editan en su propia sección de ajustes.

>[!NOTE]
Los cambios en el esquema nunca cambian los metadatos del recurso. Sin embargo, no son visibles para todas las funciones del servidor de metadatos SPS y no se puede acceder a ellos una vez que se han cambiado. Del mismo modo, si existen metadatos para un recurso, la creación del esquema de coincidencia permite que los metadatos se puedan usar en SPS y en el servidor de metadatos.

El editor de esquemas de metadatos permite para agregar o editar de forma gráfica un esquema personalizado de la empresa en SPS. Un esquema se define por un prefijo, un espacio de nombre y una lista de propiedades.

* Nombre

   Nombre de interfaz de usuario para el esquema. Se utiliza para identificar las propiedades en las vistas de metadatos y la búsqueda avanzada. Similar a las secciones XMP como Basic, IPTC, PDF.

* Prefijo

   Identificador técnico exclusivo para el esquema. Limitado a las letras a-z y A-Z. El prefijo no se encuentra visible en la interfaz de usuario de SPS, pero se utiliza cuando los metadatos de un recurso se almacenan en el bloque XMP y nuestra base de datos. El prefijo se usa para identificar de forma exclusiva los campos de metadatos en las consultas de búsqueda de metadatos en el servidor de metadatos o durante la importación.

* Espacio de nombre

   Identificador técnico único para el esquema, generalmente una dirección URL en el formulario `https://your.company.com/name/version/`. Consulte ejemplos en la lista de esquemas de estándares. El espacio de nombre no es visible en la interfaz de usuario de SPS, pero se utiliza para almacenar los metadatos en el bloque XMP.

* Descripción

   Descripción de formato libre del esquema.

>[!NOTE]
El prefijo y el espacio de nombre no se pueden editar. Para cambiar estas propiedades, deberá eliminar y volver a crear el esquema.

Las propiedades describen los metadatos que se pueden almacenar con este esquema en el bloque XMP. Una propiedad consta de lo siguiente:

| Propiedad | Descripción |
|--- |--- |
| ID | Identificador técnico para esta propiedad. El ID no es visible en la interfaz de usuario de SPS, pero se usa, cuando los metadatos de un recurso se almacenan en el bloque XMP y nuestra base de datos. Este código se utiliza para crear consultas de búsqueda en el servidor de metadatos. El ID tiene algunas limitaciones, por ejemplo: <ul><li>No puede contener espacios</li><li>No ".", ":", "$"</li><li>No puede contener un número como primer carácter</li><li>Lo mejor es utilizar una letra de a-z o A-Z como primer carácter</li></ul> <br>Una vez creado, el ID no se puede modificar. |
| Etiqueta | Nombre de interfaz de usuario para esta propiedad. |
| Estructura | Determina el tipo de la propiedad junto con el tipo de datos. La estructura puede ser uno de los siguientes valores:<ul><li>Tipo simple: solo el valor del tipo de datos.</li><li>Secuencia: una lista de valores del mismo tipo de datos.</li><li>Opción abierta: seleccione un elemento de la lista de valores predefinidos, o introduzca texto libre. El tipo de datos solo puede ser Cadena o Entero.</li><li>Opción cerrada: seleccione un elemento de la lista de valores predefinidos (una ventana emergente o un cuadro combinado).</li></ul> |
| Tipo de datos | Seleccione uno de estos tipos disponibles: <ul><li>Cadena</li><li>Entero</li><li>Flotante</li><li>Sí/No (booleano)</li><li>Fecha</li></ul> |


Si la propiedad tiene la estructura Opción abierta u Opción cerrada, debe proporcionar al menos un valor de opción. La Opción abierta se puede cambiar. La Opción cerrada no se puede cambiar. Todos los valores de opción tienen el tipo de datos de la propiedad.

| Propiedad | Descripción |
|--- |--- |
| ID | Identificador técnico para este valor. El ID no es visible en la interfaz de usuario de SPS, pero se utiliza cuando los metadatos de un recurso se almacenan en el bloque XMP y la base de datos. Este ID se utiliza en las consultas de búsquedas del servidor de metadatos. El ID no puede contener espacios. Una vez creado, el ID no se puede modificar. |
| Etiqueta | Nombre de interfaz de usuario para este valor. |

>[!MORELIKETHIS]
* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)
* [Ajustes preestablecidos de metadatos](application-setup.md#metadata_presets)

