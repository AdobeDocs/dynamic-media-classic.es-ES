---
title: Trabajar con PDF
description: Aprenda a trabajar con PDF en Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: ac9cba2c33fb1df65e64746dea2557632b7b2903
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Trabajar con PDF{#working-with-pdfs}

Los archivos de PDF (Portable Document Format) se usan con mayor frecuencia en Adobe Dynamic Media Classic para crear catálogos electrónicos. Al cargar un archivo de PDF, Adobe Dynamic Media Classic rasteriza o quita las páginas de forma predeterminada para que se puedan usar las páginas para crear medios enriquecidos.

>[!NOTE]
>
>Cuando se carga un PDF para la extracción de páginas, el Adobe impone la siguiente guía de prácticas recomendadas y límite obligatorio.
>
>* Número máximo de páginas por PDF que se consideran para la extracción
   >   * Práctica recomendada: 100
   >   * Límite obligatorio: 1000 (para actualizar cargas)


## Opciones de carga de archivos PDF {#pdf-upload-options}

Al cargar un archivo PDF, puede darle formato de varios modos. Puede recortar sus páginas, extraer palabras de búsqueda, introducir una resolución de píxeles por pulgada y elegir un espacio de color. Los archivos PDF muchas veces contienen un margen y marcas de recorte, marcas de registro y otras marcas de impresión. Estas marcas se pueden recortar de los lados de las páginas al cargar un archivo PDF.

Las opciones para cargar archivos PDF se encuentran en la página Cargar , en Opciones del PDF.

### Opciones de procesamiento

**[!UICONTROL Rasterizar]** - (Predeterminado) Extrae las páginas del archivo PDF y convierte los gráficos vectoriales en imágenes de mapa de bits. Para crear un catálogo electrónico, seleccione esta opción.

**[!UICONTROL Extraer palabras de búsqueda]** - Extrae palabras del archivo PDF para que el archivo se pueda buscar por palabra clave en un visor de catálogos electrónicos.

**[!UICONTROL Extraer vínculos]** - Extrae enlaces de los archivos PDF y los convierte en mapas de imágenes que se usan en un visor de catálogos electrónicos.

**[!UICONTROL Generación automática de catálogos electrónicos con PDF de varias páginas]** - Crea automáticamente un catálogo electrónico a partir del archivo PDF. El catálogo electrónico recibe el mismo nombre que el archivo PDF cargado. (Esta opción solo está disponible si rasteriza el archivo PDF al cargarlo).

### Resolución

Determina el valor de la resolución. Este valor determina cuántos píxeles se muestran por pulgada en el archivo PDF. El valor predeterminado es 150.

### Espacio de color opciones

Seleccione el menú Espacio de color y elija un espacio de color para el archivo PDF. La mayoría de los archivos PDF tienen imágenes de color RGB y CMYK. El espacio de color RGB es preferible para la visualización en línea.

* **[!UICONTROL Detectar automáticamente]** - Conserva el espacio de color del archivo PDF.

* **[!UICONTROL Forzar como RGB]** - Convierte al espacio de color del RGB.

* **[!UICONTROL Forzar como CMYK]** - Convierte al espacio de color CMYK.

* **[!UICONTROL Forzar como escala de grises]** - Convierte al espacio de color Escala de grises .

### Opciones de perfiles de color

* **[!UICONTROL Convertir a sRGB]** - Convierte a sRGB (azul verde rojo estándar). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

* **[!UICONTROL Mantener espacio de color original]** - Conserva el espacio de color original.

* **[!UICONTROL Personalizado desde]** > **[!UICONTROL Hasta]** - Abre los menús para que pueda elegir un espacio de color Convertir de y Convertir en . Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic.

Consulte también [Perfiles ICC](/help/icc-profiles.md#icc_profiles).

## Recortar espacio en blanco de un archivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para recortar automáticamente píxeles de espacio en blanco de un archivo PDF al cargarlo, seleccione el menú Recortar y elija Recortar.
1. Especifique las opciones siguientes:

   * **[!UICONTROL Separar en función de]** - Elija si desea recortar según el color o la transparencia:

      * **[!UICONTROL Color]** - Seleccione la opción Color. A continuación, seleccione la **[!UICONTROL Esquina]** y elija la esquina del PDF con el color que mejor represente el color del espacio en blanco que desea recortar.

      * **[!UICONTROL Transparencia]** - Elija la opción Transparencia .
   * **[!UICONTROL Tolerancia]** - Arrastre el control deslizante para especificar una tolerancia de 0 a 1.

   * **[!UICONTROL Recorte basado en el color]** - Especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PDF. Los números más cercanos a 1 permiten una mayor diferencia de color.

   * **[!UICONTROL Recorte basado en la transparencia]** - Especifique 0 para recortar píxeles solo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.


## Recortar desde los lados de las páginas del PDF {#cropping-from-the-sides-of-pdf-pages}

Se pueden quitar manualmente las marcas de impresión de los lados de páginas en un archivo PDF al cargarlo.

1. En el menú Recortar, seleccione **[!UICONTROL Manual]**.
1. Introduzca valores de píxeles en los cuadros de texto Superior, Derecha, Inferior e Izquierda para recortar de las partes superior e inferior, así como los lados, de las páginas.

La cantidad que se recorte de la página dependerá del valor de resolución en píxeles/pulgada que se introduzca para el archivo PDF. Por ejemplo, si introduce 150 (el valor predeterminado) como ajuste Resolución PX/Pulgada y recorta 75 píxeles de los lados de las páginas, se recortará media pulgada; a 150 píxeles por pulgada, 75 píxeles equivalen a media pulgada.
