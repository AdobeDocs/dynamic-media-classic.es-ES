---
title: '" Inicio rápido: Publicación de plantilla "'
seo-title: '" Inicio rápido: Publicación de plantilla "'
description: nulo
seo-description: Una introducción e Inicio rápido a la publicación de plantillas para ayudarle a empezar a utilizarlo rápidamente.
uuid: 101 b 6211-2421-4565-8635-944315 a 5 c 512
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/template-publishing
discoiquuid: 03671 fc 1-ce 3 b -4 fae-ad 1 f -53 c 99 abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

Adobe Dynamic Media Classic Web-to-Print le permite crear contenido profesional para imprimir que sus clientes, clientes y personal podrán personalizar fácilmente. Podrá mantener la identidad de su marca y empresa durante todo el proceso de publicación. Los usuarios finales podrán personalizar el contenido de impresión para el que usted les autorice. Por ejemplo, podrá ofrecer productos personalizados como papeles, tarjetas de negocio, cheques, pósters, tarjetas de felicitación, etiquetas, regalos, ropa, calendarios, o álbumes de recortes y fotográficos. Las empresas podrán mantener una identidad de marca común en sus creaciones y personalizarla según la región, franquicia, tienda o sucursal.

Para empezar, diseñe una plantilla en Adobe Illustrator. La plantilla define claramente los elementos fijos y los variables (estos últimos son los componentes que se pueden personalizar). Por ejemplo, después de parametrizar texto en un archivo de Illustrator, los usuarios finales podrán introducir un texto propio. Asimismo, tras parametrizar un color de fondo como un componente variable, éste se podrá cambiar por un color de fondo diferente.

Dynamic Media Classic ofrece dos flujos de trabajo de publicación de plantillas, uno para casos de uso básicos y otro para casos de uso avanzados. Las funciones básicas permiten crear un diseño en Adobe Illustrator, cargarlo en Dynamic Media Classic y definir elementos variables con parámetros en SPS. Las funciones avanzadas requieren una definición más compleja de las variables. Los casos de uso avanzado permiten crear elementos variables en Adobe Illustrator, cargar el archivo en Dynamic Media Classic y manipular directamente dichos elementos en un nivel XML con llamadas mediante URL. Se llama a este escenario *`*DOM manipulation*`*.

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Descargue el archivo Zip en su disco duro local y extraiga su contenido (el documento de tutorial de Dynamic Media Classic Web-To-printworkflow y los recursos del tutorial).

**Inicio rápido**

Esta sección de inicio rápido describe el flujo de trabajo básico para utilizar archivos de Illustrator y crear productos de impresión personalizables de alta calidad.

**1. Diseño de archivos de Illustrator para la publicación de plantillas**

Diseñe una plantilla en Illustrator. Si desea utilizar el método de manipulación DOM (avanzado) para personalizar la plantilla, defina los ID de elementos de s7 para los elementos variables de Illustrator.

Consulte [Creación de la plantilla inicial en Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) y [Manipulación DOM](dom-manipulation.md#dom_manipulation).

**2. Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Los usuarios de Adobe Creative Cloud pueden utilizar el plugin de Adobe Illustrator para impresión virtual. Este complemento convierte plantillas en FXG de Dynamic Media Classic. Si una plantilla contiene fuentes, los archivos de fuentes correspondientes deben cargarse en Scene7 Publishing System antes de cargar el archivo FXG.

Consulte [Carga de archivos para publicación de plantillas](upload-files-template-publishing.md#upload_files_for_template_publishing).

**3. Ver, definir o perfeccionar parámetros en Dynamic Media Classic**

En las pantallas Vista previa de plantilla y Generar, puede definir y ajustar los elementos variables mediante parámetros, previsualizar los resultados y probarlos. En estas pantallas, podrá:

* Crear y modificar parámetros.
* Especificar valores predeterminados para propiedades y atributos de parámetros.
* Hacer clic en Copiar URL para copiar la URL de previsualización en el portapapeles y previsualizar el resultado en una ventana del explorador.

Consulte [Parametrización de una plantilla en Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. Publicación de una plantilla FXG**

Tras finalizar la definición y la prueba de los parámetros y atributos, publique el archivo. Al publicar la plantilla FXG, ésta se coloca en los servidores de imágenes de Dynamic Media y activa la URL.

Debe publicar todas las imágenes y fuentes asociadas a su plantilla FXG. 

Consulte [Publicación de plantillas FXG](dom-manipulation.md#publish_fxg_templates).

**5. Obtención de la URL**

Mediante esta URL, la plantilla estará lista para incrustarse en el sitio web y para que los usuarios puedan personalizar el contenido variable.

Consulte [Vinculación de una plantilla FXG a una página web](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
