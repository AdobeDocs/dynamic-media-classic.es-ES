---
title: Visualización, adición y exportación de metadatos
description: Obtenga información sobre cómo ver, agregar y exportar metadatos en Adobe Dynamic Media Classic.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 46%

---

# Visualización, adición y exportación de metadatos{#viewing-adding-and-exporting-metadata}

Puede almacenar información específica de los archivos con los que trabaja en Adobe Dynamic Media Classic; esta información se denomina *metadatos*. Puede utilizar los metadatos en Adobe Dynamic Media Classic para organizar, buscar, filtrar y ordenar los recursos.

Los metadatos aparecen en la Vista de detalles junto con información generada por Adobe Dynamic Media Classic, como la fecha de creación del archivo, la fecha de publicación y las palabras clave. Para ver los metadatos, abra el recurso en la Vista de detalles y, a continuación, seleccione el panel Metadatos. Puede introducir y editar metadatos en la vista de detalles.

Algunos metadatos están incrustados directamente en un archivo. Si un archivo contiene estos metadatos, Adobe Dynamic Media Classic los carga automáticamente con el archivo. Puede incrustar metadatos en recursos de origen en Adobe Photoshop, InDesign, Illustrator y otras aplicaciones; Adobe Dynamic Media Classic reconoce estos metadatos. También puede agregar metadatos a archivos individuales en el panel Metadatos en la Vista de detalles. Para mantener la coherencia entre los recursos, los administradores de empresa pueden crear plantillas de metadatos que proporcionen los campos de metadatos que se pueden rellenar.

Para obtener más información sobre los metadatos incrustados, consulte [Extensible Metadata Platform](https://www.adobe.com/products/xmp.html).

## Visualización de metadatos {#view-metadata}

Para ver los metadatos de un recurso, ábralo en Vista de detalles y pulse el panel Metadatos. Para seleccionar un conjunto de campos de metadatos, elija una opción en el menú Vista de metadatos. Adobe Dynamic Media Classic ofrece estas vistas de metadatos:

* **Vista compacta** - Una lista básica de valores.

* **IPTC** - Valores definidos por el Consejo Internacional de Prensa y Telecomunicaciones.

* **XMP** : valores definidos por el programa de metadatos ampliables.

Los administradores pueden crear vistas de metadatos. Estas vistas también aparecen en el menú Vistas de metadatos.

Consulte [Vistas de metadatos](application-setup.md#metadata_views) para obtener información sobre la creación de vistas de metadatos.

## Introducción manual de metadatos para un recurso {#manually-enter-metadata-for-an-asset}

1. Abra el recurso en la Vista de detalles.
1. Abra el panel Metadatos y realice una de estas acciones o ambas:

   * Elija una vista de metadatos para determinar qué campos de metadatos aparecen en el panel.
   * Elija un valor preestablecido y, a continuación, seleccione **[!UICONTROL Aplicar]** para rellenar campos de metadatos con valores preestablecidos. Los administradores de empresas son los encargados de crear estos valores de ajustes preestablecidos.

1. Introduzca los valores en el panel Metadatos.

>[!NOTE]
>
>Para editar los metadatos de varios recursos a la vez, seleccione los recursos y vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Editar información]**. Los cambios que se hagan en la ventana Editar información se aplicarán a todos los recursos seleccionados.

## Adición o edición de palabras clave {#add-or-edit-keywords}

Además de los metadatos, puede utilizar palabras clave para ayudar a buscar y administrar sus recursos.

Si ha añadido palabras clave a otros archivos durante esta sesión o si ha eliminado palabras clave de la lista, aparecerán en la tabla Sugerencias de palabras clave.

1. Abra el archivo en la vista de detalles.
1. Seleccionar **[!UICONTROL Palabras clave]**.
1. Para agregar palabras clave, realice lo siguiente:

   * Escriba una palabra clave en el cuadro de texto y seleccione **[!UICONTROL Añadir]**.
   * Seleccione una palabra clave en la **[!UICONTROL Sugerencias de palabras clave]** tabla.

1. Para quitar una palabra clave, selecciónela y seleccione **[!UICONTROL Eliminar]**. Pasará a incluirse en la tabla Sugerencias de palabras clave.

>[!NOTE]
>
>Puede añadir palabras clave a los archivos a medida que los carga en Adobe Dynamic Media Classic. En el cuadro de diálogo Cargar opciones del trabajo, elija **[!UICONTROL Metadatos adicionales]** e introduzca palabras clave.
>Consulte [Opciones de carga](uploading-files.md#upload_options).

## Importación de metadatos {#import-metadata}

En lugar de introducir los metadatos manualmente de uno en uno, puede importar los metadatos para varios recursos diferentes desde un archivo delimitado por tabuladores o XML. Introducir los metadatos en un archivo delimitado por tabuladores o XML e importar este archivo requiere menos tiempo que si se introducen estos metadatos en recursos individuales. En la primera fila del archivo delimitado por tabuladores, introduzca el ID y los nombres de los campos para los que desea grabar los metadatos. En cada fila posterior, introduzca un nombre de ID de recurso seguido de los valores de los metadatos. Los campos que no se incluyen en el archivo XML o delimitado por tabuladores no se modificarán. Para importar metadatos desde un archivo XML, asegúrese de que cumple con el archivo DTD.

>[!NOTE]
>
>Puede crear una plantilla para introducir metadatos de modo que se puedan importar correctamente a Adobe Dynamic Media Classic. Una vez creada la plantilla, puede utilizarla para introducir los metadatos.
>Consulte [Creación de una plantilla para la introducción y carga de metadatos](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Puede encontrar más información sobre las propiedades estandarizadas en [Centro para desarrolladores de Adobe XMP](https://www.adobe.com/devnet/xmp.html).

1. En el panel Examinar, seleccione las imágenes a las que quiera agregar metadatos a partir del archivo delimitado por tabuladores o XML.
1. Ir a **[!UICONTROL Archivo]** > **[!UICONTROL Importar metadatos]**.
1. En el **[!UICONTROL Cargar metadatos]** , seleccione **[!UICONTROL Examinar]**.
1. En el cuadro de diálogo **[!UICONTROL Seleccionar archivos para cargar]**, seleccione el archivo XML o delimitado por tabuladores que contenga los metadatos.
1. Introduzca un nombre de trabajo.
1. Seleccionar **[!UICONTROL Cargar]**.

### Identificación de diferentes tipos de metadatos en la importación

Tenga en cuenta lo siguiente al identificar diferentes tipos de metadatos para su importación:

* Los campos definidos por el usuario se identifican con su nombre tal como se crean en **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Campos definidos por el usuario]**. Utilice la función de Generar archivo para obtener una lista de todos los campos personalizables definidos con el formato correcto de importación.
* Las propiedades de metadatos XMP deben tener el prefijo XMP correspondiente antes que el nombre (propiedad- ). Dos puntos separan el prefijo y el nombre. XMP El prefijo de la dirección se puede encontrar en **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Esquema de metadatos]** editor. Los nombres técnicos se pueden encontrar en la documentación del esquema de XMP correspondiente. XMP Los nombres de las propiedades de no aparecen en la función Generar archivo.
* Las propiedades del esquema de metadatos deben tener el prefijo correspondiente antes del nombre (propiedad- ). Dos puntos separan el prefijo y el nombre. El prefijo y los nombres de propiedad se definen en el editor de esquemas de metadatos. Los nombres de las propiedades del esquema de metadatos no aparecen en la función Generar archivo.

XMP XMP Por ejemplo: la propiedad de la palabra clave en el código de la palabra clave es el esquema de la palabra clave &quot;Dublin Core&quot; con el prefijo de la palabra clave, que es el esquema de la palabra clave &quot;Dublin Core&quot;. `dc` y `subject` XMP es el nombre técnico de la. XMP El prefijo y el nombre de la técnica se combinan en la variable `dc:subject` nombre completo de la propiedad. En el formato de importación de metadatos XML, `dc.subject` debe ser el nombre de la propiedad. En el formato de importación delimitado por tabuladores, debe ser el encabezado de columna.

### Importación de palabras clave

Las palabras clave se pueden importar como listas separadas por comas. Si aparece una coma en cualquiera de los valores individuales, debe señalarse con una barra invertida (\). Una barra invertida literal es la barra invertida doble habitual (\\).

Por ejemplo, un archivo de importación de metadatos que contenga el valor `Hello\, World!,back\\slash,foo` para `dc:subject` XMP establece tres palabras clave del recurso: `Hello, World!,` `back\slash,` y `foo`.

### Importación de archivos XMP de metadatos de esquemas de metadatos y XMP

La importación de XML solo acepta XML válido. XMP XMP Al importar campos de esquema de metadatos o de recursos, el prefijo del área de nombres se agrega y se comporta aquí como un área de nombres de la. Este área de nombres debe declararse. Por ejemplo, en la etiqueta de nivel superior.

Por ejemplo:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### XMP Importar archivos delimitados por tabuladores de metadatos y esquemas de metadatos

El prefijo debe agregarse en el encabezado de la columna correspondiente del campo de importación.

## Importación de metadatos (mediante FTP) {#import-metadata-via-ftp}

Puede importar metadatos de varios archivos introduciéndolos en un archivo XML o delimitado por tabuladores y seleccionando **[!UICONTROL Procesar archivos de metadatos]** en la página Opciones del trabajo de carga (pestaña A través de FTP).

Asegúrese de que los datos del archivo XML o delimitado por tabuladores tienen el formato correcto. En la primera fila, introduzca el campo de ID seguido de los nombres de los campos de metadatos que desea modificar. En cada fila posterior, introduzca un nombre de ID de recurso seguido de los valores de los metadatos. Los campos que no se incluyen en el archivo XML o delimitado por tabuladores no se modificarán.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]**. Para importar los metadatos, en la página Cargar, seleccione **[!UICONTROL A través de FTP]** pestaña, luego seleccione **[!UICONTROL Opciones de trabajo]**. En el cuadro de diálogo Opciones del trabajo de carga, seleccione **[!UICONTROL Trabajo]**, luego seleccione **[!UICONTROL Procesar archivos de metadatos]** casilla de verificación.

## Cambio de nombre de ID por lotes con metadatos {#batch-rename-ids-using-metadata}

Mediante los metadatos importados de un archivo delimitado por tabuladores o un archivo XML, puede cambiar el nombre de los Adobe Dynamic Media Classic ID. Los metadatos importados solo se aplican a las imágenes que se especifican en el archivo de metadatos. No importa si las imágenes están seleccionadas en el panel Examinar.

Para cambiar el nombre del Adobe Dynamic Media Classic ID de una imagen, agregue una columna denominada *newipsid* al archivo delimitado por tabulaciones o agregue un campo llamado `new_vc_objectname` a los datos XML.

Por ejemplo:

|  | newipsid |
| --- | --- |
| pruebachaqueta_1 | Prueba_chaqueta_1 |
| pruebachaqueta_azul | Prueba_chaqueta_2 |

El registro de trabajo del trabajo de metadatos muestra qué ID se cambiaron de nombre correctamente y cuáles no.

## Creación de una plantilla para la introducción y carga de metadatos {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic ofrece un comando para crear una plantilla para grabar metadatos. El uso de la plantilla garantiza que los metadatos se introduzcan en el formato correcto para que se puedan cargar correctamente en Adobe Dynamic Media Classic. Para crear una plantilla para utilizarla en la grabación e importación de metadatos a Adobe Dynamic Media Classic, siga estos pasos:

1. Seleccione los recursos de imagen con los campos de metadatos que desee para la plantilla.
1. Ir a **[!UICONTROL Archivo]** > **[!UICONTROL Importar metadatos]**.
1. Para el **[!UICONTROL Tipo de propiedades de recurso]**, seleccione **[!UICONTROL Imagen]**.
1. Desde el **[!UICONTROL Generar archivo]** lista desplegable, elija **[!UICONTROL Plantilla delimitada por tabuladores]**, **[!UICONTROL Metadatos XML de recursos]**, o **[!UICONTROL DTD de XML]**.
1. Seleccionar **[!UICONTROL Generar]**.
1. Copie los datos en el cuadro de diálogo que aparece. Utilice estos datos para construir la plantilla.

## Trabajo con esquemas de metadatos {#working-with-metadata-schemas}

Un administrador de empresa puede ver una lista de todos los esquemas disponibles. En la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Metadatos]** > **[!UICONTROL Esquema de metadatos]**.

XMP Inicialmente, la lista de esquemas estándar globales como está oculta Para verlos, use la casilla de verificación de la parte inferior de la lista.

El administrador de la empresa puede crear un esquema personalizado o editar uno existente.

Puede utilizar el editor de esquemas de metadatos para realizar las siguientes acciones:

| Acción | Descripción |
| --- | --- |
| Agregar | Agrega una propiedad al esquema. Un cuadro de diálogo modal recopila la información: ID, etiqueta, estructura y tipo de datos. |
| Agregar valor de opción | Agrega una nueva opción seleccionable a una propiedad con estructura Opción abierta u Opción cerrada. Todos los valores de opción son del mismo tipo. Seleccione la propiedad en sí para habilitar el botón. |
| Editar | Permite editar la etiqueta de una propiedad o valor de opción. Solo se puede cambiar la etiqueta, ID, y la información de tipo es inmutable. |
| Mover hacia arriba/Mover hacia abajo | El orden en el esquema se refleja en la interfaz de usuario. Para cambiar el orden, seleccione una propiedad o un valor de opción, y muévalos con los botones. Actualmente no se admite arrastrar y soltar. |
| Eliminar | Elimina una propiedad o un valor de opción del esquema. XMP No elimina valores del bloque de la base de datos o del bloque de la base de datos de la. La propiedad ya no está disponible para las vistas de metadatos y se elimina de la vista de detalles del recurso. Si la propiedad se publicó en el servidor de metadatos, realice una publicación forzada para eliminar los datos del servidor de metadatos público. |

El sistema genera automáticamente un esquema personalizado para los campos definidos por el usuario con el prefijo `s7udf`. Son campos definidos por el usuario existentes y se editan en su propia sección de configuración.

>[!NOTE]
>
>Los cambios en el esquema nunca cambian los metadatos del recurso. Sin embargo, no son visibles para todas las funciones de Adobe Dynamic Media Classic y del servidor de metadatos, y no se puede acceder a ellos después de cambiarlos. Del mismo modo, si existen metadatos para un recurso, la creación del esquema coincidente permite utilizarlos en Adobe Dynamic Media Classic y en el servidor de metadatos.

El Editor de esquemas de metadatos ofrece una forma gráfica de agregar o editar un esquema de empresa personalizado dentro de Adobe Dynamic Media Classic. Un esquema se define por un prefijo, un espacio de nombre y una lista de propiedades.

* **[!UICONTROL Nombre]** - Nombre de interfaz de usuario para el esquema. Se utiliza para identificar las propiedades en las vistas de metadatos y la búsqueda avanzada. Similar a las secciones XMP como Basic, IPTC, PDF.

* **[!UICONTROL Prefijo]** : identificador técnico único del esquema. Limitado a las letras a-z y A-Z. El prefijo no está visible en la interfaz de usuario de Adobe Dynamic Media Classic XMP, pero se utiliza cuando los metadatos de un recurso se almacenan en el bloque de la base de datos y en el bloque de la base de datos de la aplicación. El prefijo se usa para identificar de forma exclusiva los campos de metadatos en las consultas de búsqueda de metadatos en el servidor de metadatos o durante la importación.

* **[!UICONTROL Área de nombres]** : Identificador único técnico para el esquema, normalmente una URL en el formulario `https://your.company.com/name/version/`. Consulte ejemplos en la lista de esquemas de estándares. El área de nombres no está visible en la interfaz de usuario de Adobe Dynamic Media Classic XMP, pero se utiliza para almacenar metadatos en el bloque de.

* **[!UICONTROL Descripción]** - Descripción en formato libre del esquema.

>[!NOTE]
>
>El prefijo y el espacio de nombre no se pueden editar. Para cambiar estas propiedades, deberá eliminar y volver a crear el esquema.

Las propiedades describen los metadatos que se pueden almacenar con este esquema en el bloque XMP. Una propiedad consta de lo siguiente:

| Propiedad | Descripción |
| --- | --- |
| ID | Identificador técnico para esta propiedad. El ID no es visible en la interfaz de usuario de Adobe Dynamic Media Classic XMP, pero se utiliza cuando los metadatos de un recurso se almacenan en el bloque de la base de datos y en el bloque de la base de datos de la base de datos. Este código se utiliza para crear consultas de búsqueda en el servidor de metadatos. El ID tiene algunas limitaciones, por ejemplo: <ul><li>No puede contener espacios</li><li>No &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>No puede contener un número como primer carácter</li><li>Lo mejor es utilizar una letra de a-z o A-Z como primer carácter</li></ul> <br>Una vez creado, el ID no se puede modificar. |
| Etiqueta | Nombre de interfaz de usuario para esta propiedad. |
| Estructura | Determina el tipo de la propiedad junto con el tipo de datos. La estructura puede ser uno de los siguientes valores:<ul><li>Tipo simple: solo el valor del tipo de datos.</li><li>Secuencia: una lista de valores del mismo tipo de datos.</li><li>Opción abierta: seleccione un elemento de la lista de valores predefinidos, o introduzca texto libre. El tipo de datos solo puede ser Cadena o Entero.</li><li>Opción cerrada: seleccione un elemento de la lista de valores predefinidos (una ventana emergente o un cuadro combinado).</li></ul> |
| Tipo de datos | Seleccione uno de estos tipos disponibles: <ul><li>Cadena</li><li>Entero</li><li>Flotante</li><li>Sí/No (booleano)</li><li>Fecha</li></ul> |

Si la propiedad tiene la estructura Opción abierta u Opción cerrada, debe proporcionar al menos un valor de opción. La Opción abierta se puede cambiar. La Opción cerrada no se puede cambiar. Todos los valores de opción tienen el tipo de datos de la propiedad.

| Propiedad | Descripción |
| --- | --- |
| ID | Identificador técnico para este valor. El ID no es visible en la interfaz de usuario de Adobe Dynamic Media Classic XMP, pero se utiliza cuando los metadatos de un recurso se almacenan en el bloque de la base de datos y en el bloque de la base de datos de la base de datos. Este ID se utiliza en las consultas de búsquedas del servidor de metadatos. El ID no puede contener espacios. Una vez creado, el ID no se puede modificar. |
| Etiqueta | Nombre de interfaz de usuario para este valor. |

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de visor](application-setup.md#viewer_presets)
>* [Ajustes preestablecidos de metadatos](application-setup.md#metadata_presets)

