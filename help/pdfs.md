---
title: Uso de archivos PDF
description: Aprenda a trabajar con archivos PDF en Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Administración de recursos
role: Business Practitioner
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 45%

---

# Uso de archivos PDF{#working-with-pdfs}

Los archivos PDF (Portable Document Format) se usan con mayor frecuencia en Dynamic Media Classic para crear catálogos electrónicos. Al cargar un archivo PDF, Dynamic Media Classic rasteriza o desgarra las páginas de forma predeterminada para que se puedan usar las páginas para crear medios enriquecidos.

## Opciones de carga de archivos PDF {#pdf-upload-options}

Al cargar un archivo PDF, puede darle formato de varios modos. Puede recortar sus páginas, extraer palabras de búsqueda, introducir una resolución de píxeles por pulgada y elegir un espacio de color. Los archivos PDF muchas veces contienen un margen y marcas de recorte, marcas de registro y otras marcas de impresión. Estas marcas se pueden recortar de los lados de las páginas al cargar un archivo PDF.

Las opciones para cargar archivos PDF se encuentran en la página Cargar, en Opciones de PDF.

### Opciones de procesamiento

**Rasterizar** : (predeterminado) arrastra las páginas del archivo PDF y convierte los gráficos vectoriales en imágenes de mapa de bits. Para crear un catálogo electrónico, seleccione esta opción.

**Extraer palabras de búsqueda** : extrae palabras del archivo PDF para que el archivo se pueda buscar por palabra clave en un visualizador de catálogos electrónicos.

**Extraer vínculos** : extrae vínculos de los archivos PDF y los convierte en mapas de imágenes que se utilizan en un visor de catálogos electrónicos.

**Generación automática de catálogos electrónicos con PDF de varias páginas** : crea automáticamente un catálogo electrónico a partir del archivo PDF. El catálogo electrónico recibe el mismo nombre que el archivo PDF cargado. (Esta opción solo está disponible si rasteriza el archivo PDF al cargarlo).

### Resolución

Determina el valor de la resolución. Este valor determina cuántos píxeles se muestran por pulgada en el archivo PDF. El valor predeterminado es 150.

### Espacio de color opciones

Seleccione el menú Espacio de color y elija un espacio de color para el archivo PDF. La mayoría de los archivos PDF tienen imágenes de color RGB y CMYK. El espacio de color RGB es preferible para la visualización en línea.

* **Detectar automáticamente** : conserva el espacio de color del archivo PDF.

* **Forzar como RGB** : Convierte al espacio de color RGB.

* **Forzar como CMYK** : convierte al espacio de color CMYK.

* **Forzar como escala de grises** : se convierte al espacio de color de escala de grises.

### Opciones de perfiles de color

* **Convertir a sRGB** : convierte a sRGB (azul verde rojo estándar). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

* **Mantener espacio de color original** : conserva el espacio de color original.

* **Personalizar de > A** : abre los menús para que pueda elegir los espacios de color Convertir en y Convertir en. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Dynamic Media Classic.

Consulte también [Perfiles ICC](/help/icc-profiles.md#icc_profiles).

## Recorte de espacio en blanco de un archivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para recortar automáticamente píxeles de espacio en blanco de un archivo PDF al cargarlo, seleccione el menú Recortar y elija Recortar.
1. Especifique las opciones siguientes:

   * **Separar en función de** : elija si recortar en función del color o la transparencia:

   * **Color** : elija la opción Color. A continuación, seleccione el menú Esquina y elija la esquina del PDF que mejor represente el color de espacio en blanco que desea recortar.

   * **Transparencia** : elija la opción Transparencia.

   * **Tolerancia** : arrastre el control deslizante para especificar una tolerancia de 0 a 1.

   * **Recorte basado en el color** : especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PDF. Los números más cercanos a 1 permiten una mayor diferencia de color.

   * **Recorte basado en la transparencia** : especifique 0 para recortar píxeles solo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.

## Recorte de los lados de páginas PDF {#cropping-from-the-sides-of-pdf-pages}

Se pueden quitar manualmente las marcas de impresión de los lados de páginas en un archivo PDF al cargarlo.

1. En el menú Recortar, haga clic en **[!UICONTROL Manual]**.
1. Introduzca valores de píxeles en los cuadros de texto Superior, Derecha, Inferior e Izquierda para recortar de las partes superior e inferior, así como los lados, de las páginas.

La cantidad que se recorte de la página dependerá del valor de resolución en píxeles/pulgada que se introduzca para el archivo PDF. Por ejemplo, si introduce 150 (el valor predeterminado) como ajuste Resolución PX/Pulgada y recorta 75 píxeles de los lados de las páginas, se recortará media pulgada; a 150 píxeles por pulgada, 75 píxeles equivalen a media pulgada.
