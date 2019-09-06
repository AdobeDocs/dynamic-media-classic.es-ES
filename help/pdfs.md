---
title: Uso de archivos PDF
seo-title: Uso de archivos PDF
description: nulo
seo-description: Aprenda a trabajar con archivos PDF en Dynamic Media Classic.
uuid: 26 d 70 d 28-9393-49 b 1-9051-d 70456 deca 67
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 5 a 073 de 3-6 b 1 d -4 c 3 e -8 c 03-9182 f 9 f 3874 a
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Uso de archivos PDF{#working-with-pdfs}

Los archivos PDF (Portable Document Format) se utilizan con más frecuencia en Dynamic Media Classic para crear catálogos electrónicos. Al cargar un archivo PDF, Dynamic Media Classic rasteriza, o extrae, las páginas de forma predeterminada para que las páginas puedan utilizarse para generar medios enriquecidos.

## Opciones de carga de archivos PDF {#pdf-upload-options}

Al cargar un archivo PDF, puede darle formato de varios modos. Puede recortar sus páginas, extraer palabras de búsqueda, introducir una resolución de píxeles por pulgada y elegir un espacio de color. Los archivos PDF muchas veces contienen un margen y marcas de recorte, marcas de registro y otras marcas de impresión. Estas marcas se pueden recortar de los lados de las páginas al cargar un archivo PDF.

Las opciones para cargar archivos PDF se encuentran en la pantalla Cargar, en Opciones de PDF.

**Procesamiento**

Las opciones de Procesamiento son:

**Rasterizar** (predeterminado) Extrae las páginas del archivo PDF y convierte los gráficos vectoriales en imágenes de mapa de bits. Elija esta opción para crear un catálogo electrónico. 

**Extraer palabras de búsqueda** Extrae palabras del archivo PDF para que el archivo pueda buscarse por palabra clave en un visor de catálogos electrónicos.

**Extraer vínculos** Extrae vínculos de los archivos PDF y los convierte en mapas de imagen que se utilizan en un visor de catálogos electrónicos.

**Generar catálogo electrónico automáticamente con PDF de varias páginas crea** automáticamente un catálogo electrónico a partir del archivo PDF. El catálogo electrónico recibe el mismo nombre que el archivo PDF cargado. (Esta opción solo está disponible si rasteriza el archivo PDF al cargarlo).

**Resolución**

Determina el valor de la resolución. Este valor determina cuántos píxeles se muestran por pulgada en el archivo PDF. El valor predeterminado es 150.

**Espacio de color**

Seleccione el menú Espacio de color y elija un espacio de color para el archivo PDF. La mayoría de los archivos PDF tienen imágenes de color RGB y CMYK. El espacio de color RGB es preferible para la visualización en línea.

**Detectar Retiene automáticamente** el espacio de color del archivo PDF.

**Forzar RGB** Convierte al espacio de color RGB.

**Forzar CMYK** Convierte al espacio de color CMYK.

**Forzar escala de grises** convierte al espacio de color Escala de grises.

**Perfil de color**

Elija una opción de Perfil de color:

**Convertir a SRGB** Convierte a SRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

**Mantener espacio de color original** Conserva el espacio de color original.

**Personalizar &gt; Para** abrir menús para que pueda elegir un espacio de color Convertir de y Convertir a. Puede elegir un espacio de color estándar de Photoshop o uno que haya cargado en SPS. 

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

## Recorte de espacio en blanco de un archivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para recortar automáticamente píxeles de espacio en blanco de un archivo PDF al cargarlo, seleccione el menú Recortar y elija Recortar.
1. Especifique las opciones siguientes:

   **Recortar basándose en** elegir si se desea recortar según color o transparencia:

   **Color** Elija la opción Color. A continuación, seleccione el menú Esquina y elija la esquina del PDF que mejor represente el color de espacio en blanco que desea recortar.

   **Transparencia Elija** la opción Transparencia.

   **Tolerancia** Arrastre el control deslizante para especificar una tolerancia de 0 a 1:

   **Recorte basado en color** Especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PDF. Los números más cercanos a 1 permiten una mayor diferencia de color.

   **Recorte basado en transparencia** Especifique 0 para recortar píxeles solo si son totalmente transparentes; los números más cercanos a 1 permiten una mayor transparencia.

## Recorte de los lados de páginas PDF {#cropping-from-the-sides-of-pdf-pages}

Se pueden quitar manualmente las marcas de impresión de los lados de páginas en un archivo PDF al cargarlo.

1. Seleccione el menú Recortar y elija Manual.
1. Introduzca valores de píxeles en los cuadros de texto Superior, Derecha, Inferior e Izquierda para recortar de las partes superior e inferior, así como los lados, de las páginas.

La cantidad que se recorte de la página dependerá del valor de resolución en píxeles/pulgada que se introduzca para el archivo PDF. Por ejemplo, si se introduce 150 (valor predeterminado) como valor de resolución en píxeles/pulgada y se recortan 75 píxeles de los lados de las páginas, se recortará media pulgada, ya que, a 150 píxeles por pulgada, 75 píxeles equivalen a media pulgada.
