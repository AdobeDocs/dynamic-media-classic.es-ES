---
title: Uso de archivos PDF
description: Aprenda a trabajar con archivos PDF en Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 56%

---


# Uso de archivos PDF{#working-with-pdfs}

Los archivos PDF (formato de Documento portátil) se utilizan con mayor frecuencia en Dynamic Media Classic para crear catálogos electrónicos. Al cargar un archivo PDF, Dynamic Media Classic rasteriza o extrae las páginas de forma predeterminada para que se puedan utilizar las páginas para crear medios enriquecidos.

## Opciones de carga de archivos PDF {#pdf-upload-options}

Al cargar un archivo PDF, puede darle formato de varios modos. Puede recortar sus páginas, extraer palabras de búsqueda, introducir una resolución de píxeles por pulgada y elegir un espacio de color. Los archivos PDF muchas veces contienen un margen y marcas de recorte, marcas de registro y otras marcas de impresión. Estas marcas se pueden recortar de los lados de las páginas al cargar un archivo PDF.

Las opciones para cargar archivos PDF se encuentran en la pantalla Cargar, en Opciones de PDF.

**Procesamiento**

Las opciones de Procesamiento son:

**Rasterizar**  (predeterminado) Extrae las páginas del archivo PDF y convierte los gráficos vectoriales en imágenes de mapa de bits. Elija esta opción para crear un catálogo electrónico. 

**Extraer** palabras de búsquedaExtrae palabras del archivo PDF para que el archivo se pueda buscar por palabra clave en un visor de catálogos electrónicos.

**Extraer** vínculosExtrae vínculos de los archivos PDF y los convierte en mapas de imagen que se utilizan en un visor de catálogos electrónicos.

**Generar catálogo electrónico automáticamente con** PDFA de varias páginas crea automáticamente un catálogo electrónico a partir del archivo PDF. El catálogo electrónico recibe el mismo nombre que el archivo PDF cargado. (Esta opción solo está disponible si rasteriza el archivo PDF al cargarlo).

**Resolución**

Determina el valor de la resolución. Este valor determina cuántos píxeles se muestran por pulgada en el archivo PDF. El valor predeterminado es 150.

**Espacio de color**

Seleccione el menú Espacio de color y elija un espacio de color para el archivo PDF. La mayoría de los archivos PDF tienen imágenes de color RGB y CMYK. El espacio de color RGB es preferible para la visualización en línea.

**Detectar** automáticamenteConserva el espacio de color del archivo PDF.

**Forzar como** RGBConvierte al espacio de color RGB.

**Forzar como** CMYKConvierte al espacio de color CMYK.

**Forzar** escala de grisesConvierte al espacio de color de escala de grises.

**Perfil de color**

Elija una opción de Perfil de color:

**Convertir a** sRGBConvertidos a sRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

**Mantener** espacio de color originalConserva el espacio de color original.

**Personalizado de >** AAbre los menús para que pueda elegir un espacio de color Convertir de y Convertir a. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Dynamic Media Classic.

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

## Recorte de espacio en blanco de un archivo PDF  {#cropping-white-space-from-a-pdf-file}

1. Para recortar automáticamente píxeles de espacio en blanco de un archivo PDF al cargarlo, seleccione el menú Recortar y elija Recortar.
1. Especifique las opciones siguientes:

   **Recortar según** OnElija si desea recortar según el color o la transparencia:

   **** ColorElija la opción Color. A continuación, seleccione el menú Esquina y elija la esquina del PDF que mejor represente el color de espacio en blanco que desea recortar.

   **** TransparenciaElija la opción Transparencia.

   **** ToleranciaArrastre el control deslizante para especificar una tolerancia de 0 a 1:

   **Recorte basado en** colorEspecifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PDF. Los números más cercanos a 1 permiten una mayor diferencia de color.

   **Recorte basado en** transparenciaEspecifique 0 para recortar píxeles solo si son totalmente transparentes; los números más cercanos a 1 permiten una mayor transparencia.

## Recorte de los lados de páginas PDF {#cropping-from-the-sides-of-pdf-pages}

Se pueden quitar manualmente las marcas de impresión de los lados de páginas en un archivo PDF al cargarlo.

1. Seleccione el menú Recortar y elija Manual.
1. Introduzca valores de píxeles en los cuadros de texto Superior, Derecha, Inferior e Izquierda para recortar de las partes superior e inferior, así como los lados, de las páginas.

La cantidad que se recorte de la página dependerá del valor de resolución en píxeles/pulgada que se introduzca para el archivo PDF. Por ejemplo, si se introduce 150 (valor predeterminado) como valor de resolución en píxeles/pulgada y se recortan 75 píxeles de los lados de las páginas, se recortará media pulgada, ya que, a 150 píxeles por pulgada, 75 píxeles equivalen a media pulgada.
