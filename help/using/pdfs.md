---
title: Trabajo con PDF
description: Aprenda a trabajar con PDF en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 26%

---

# Trabajo con PDF{#working-with-pdfs}

Los archivos de PDF (formato de documento portátil) se utilizan principalmente en Adobe Dynamic Media Classic para crear catálogos electrónicos. Al cargar un archivo de PDF, Adobe Dynamic Media Classic rasteriza o extrae las páginas de forma predeterminada para que puedan utilizarse en la creación de medios enriquecidos.

Al cargar un PDF para la extracción de páginas, el Adobe aplica el siguiente límite:

| Tipo de límite | Límite impuesto | Cambio del límite el 31 de diciembre de 2022 |
| --- | --- | --- |
| Número máximo de páginas para que un PDF se considere para la extracción | 5000 (para nuevas cargas) | 100 (para todos los PDF) |

Ver también [limitaciones de Dynamic Media](/help/using/limitations.md).

## Opciones de carga de archivos PDF {#pdf-upload-options}

Al cargar un archivo PDF, puede darle formato de varios modos. Puede recortar sus páginas, extraer palabras de búsqueda, introducir una resolución de píxeles por pulgada y elegir un espacio de color. Los archivos de PDF suelen contener un margen de recorte, marcas de recorte, marcas de registro y otras marcas de impresora. Estas marcas se pueden recortar de los lados de las páginas al cargar un archivo PDF.

Las opciones para cargar archivos de PDF se encuentran en la página Cargar, en Opciones de PDF.

### Opciones de procesamiento

**[!UICONTROL Rasterizar]**: (Predeterminado) rasga las páginas del archivo PDF y convierte los gráficos vectoriales en imágenes de mapa de bits. Para crear un catálogo electrónico, elija esta opción.

**[!UICONTROL Extraer palabras de búsqueda]**: extrae palabras del archivo del PDF para que las palabras clave del archivo se puedan buscar en un visor de catálogos electrónicos.

**[!UICONTROL Extraer vínculos]**: extrae vínculos de los archivos del PDF y los convierte en mapas de imágenes que se utilizan en un visor de catálogos electrónicos.

**[!UICONTROL Generar catálogo electrónico automáticamente con el PDF de varias páginas]**: Crea automáticamente un catálogo electrónico a partir del archivo de PDF. El catálogo electrónico recibe el mismo nombre que el archivo PDF cargado. (Esta opción solo está disponible si rasteriza el archivo PDF al cargarlo).

### Resolución

Determina el valor de la resolución. Este valor determina cuántos píxeles se muestran por pulgada en el archivo PDF. El valor predeterminado es 150.

### Opciones de espacio de color

Seleccione el menú Espacio de color y elija un espacio de color para el archivo PDF. La mayoría de los archivos PDF tienen imágenes de color RGB y CMYK. El espacio de color RGB es preferible para la visualización en línea.

* **[!UICONTROL Detectar automáticamente]**: conserva el espacio de color del archivo del PDF.

* **[!UICONTROL Forzar como RGB]**: se convierte al espacio de color del RGB.

* **[!UICONTROL Forzar como CMYK]**: se convierte al espacio de color CMYK.

* **[!UICONTROL Forzar como escala de grises]**: se convierte al espacio de color de escala de grises.

### Opciones de perfiles de color

* **[!UICONTROL Convertir a sRGB]**: Convierte a sRGB (azul rojo y verde estándar). sRGB es el espacio de color recomendado para mostrar imágenes en una página Web.

* **[!UICONTROL Conservar el espacio de color original]**: conserva el espacio de color original.

* **[!UICONTROL Personalizar desde]** > **[!UICONTROL hasta]**: abre menús para que pueda elegir un espacio de color Convertir desde y Convertir a. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic.

Consulte también [Perfiles ICC](/help/using/icc-profiles.md#icc_profiles).

## Recortar espacio en blanco de un archivo de PDF {#cropping-white-space-from-a-pdf-file}

Puede recortar automáticamente los píxeles de espacio en blanco de un archivo de PDF a medida que lo carga.

1. Seleccione el menú Recortar y elija Recortar.
1. Especifique las opciones siguientes:

   * **[!UICONTROL Recortar basándose en]**: elige si recortar basándose en el color o la transparencia:

      * **[!UICONTROL Color]**: elige la opción Color. A continuación, seleccione el menú **[!UICONTROL Esquina]** y elija la esquina del PDF con el color que mejor represente el color del espacio en blanco que desea recortar.

      * **[!UICONTROL Transparencia]**: elija la opción Transparencia.

   * **[!UICONTROL Tolerancia]**: arrastre el regulador para especificar una tolerancia de 0 a 1.

   * **[!UICONTROL Recorte basado en el color]**: especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PDF. Los números más cercanos a 1 permiten una mayor diferencia de color.

   * **[!UICONTROL Recorte basado en la transparencia]**: especifique 0 para recortar píxeles sólo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.

## Recortar desde los lados de las páginas PDF {#cropping-from-the-sides-of-pdf-pages}

Puede quitar manualmente las marcas de impresora de los lados de las páginas en un archivo de PDF a medida que lo carga.

1. En el menú Recortar, seleccione **[!UICONTROL Manual]**.
1. Introduzca valores de píxeles en los cuadros de texto Superior, Derecha, Inferior e Izquierda para recortar de las partes superior e inferior, así como los lados, de las páginas.

La cantidad que se recorte de la página dependerá del valor de resolución en píxeles/pulgada que se introduzca para el archivo PDF. Por ejemplo, suponga que especifica 150 (valor predeterminado) como valor de Resolución PX/Pulgada. A continuación, se recortan 75 píxeles de los lados de las páginas. En tal caso, 0,5 pda. se ha recortado. A 150 píxeles por pulgada, 75 píxeles equivale a media pulgada.
