---
title: Recorte de imágenes
description: Aprenda a recortar una imagen.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 85%

---


# Recorte de imágenes{#cropping-an-image}

Puede recortar imágenes en Dynamic Media Classic. El sistema retiene información sobre las imágenes que se recortaron para que pueda restaurar su estado original. También puede recortar una imagen y guardar con otro nombre la versión recortada.

Al recortar una imagen, puede quitar el espacio en blanco que la rodea o un área concreta de la imagen.

>[!NOTE]
>
>Después del recorte, puede hacer clic en el botón Guardar como y guardar una versión recortada de la imagen con un nombre diferente. En la ventana Guardar como, elija Guardar como nuevo elemento principal para guardar una segunda copia de la imagen. Elija Guardar como vista adicional de imagen principal para guardar el original y su versión recortada con un nombre diferente. Elija Reemplazar original para eliminar el archivo original en el que recortó la imagen. A continuación, introduzca un nombre para la imagen y seleccione el botón Enviar.

## Recorte para quitar espacio en blanco alrededor de una imagen  {#crop-to-remove-white-space-around-an-image}

Puede recortar los píxeles transparentes o de color sólido del borde de una imagen.

1. Para recortar una imagen, haga clic en su botón de rollover Editar y elija Recortar, o bien muéstrela en el panel Examinar de la vista de detalles y haga clic en el botón Recortar . Aparecerá la pantalla Editor de recorte.
1. Realice una de las siguientes acciones:

   * Para recortar los píxeles de color, elija el menú Recortar y seleccione Color. Aparecerá el cuadro de diálogo Recorte automático por color. Seleccione el menú Esquina y elija una esquina con el color de fondo que desee recortar. Introduzca a continuación un valor de Tolerancia de 0 a 1. El valor 0 recorta píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color. Seleccione el botón Recortar.
   * Para recortar los píxeles transparentes, elija el menú Recortar y seleccione Transparente. Aparecerá el cuadro de diálogo Recorte automático por transparencia. Introduzca un valor de Tolerancia de 0 a 1. El valor 0 recorta píxeles solo si son totalmente transparentes. Los números más cercanos a 1 permiten una mayor transparencia. Seleccione el botón Recortar.

1. Haga clic en **Guardar**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original tras su recorte, muéstrela en la pantalla Editor de recorte y seleccione el botón Restablecer.

## Selección de áreas que recortar  {#select-an-area-to-crop}

1. Para recortar una imagen, haga clic en su botón de rollover Editar y seleccione **Recortar**, o muéstrela en el panel Examinar de la vista de detalles y haga clic en **Recortar**.

1. En la ventana Editor de recorte, coloque la parte de la imagen que no desea recortar en el cuadro de recorte. Lo que aparece dentro del cuadro permanece al hacer clic en **Guardar** y recortar la imagen.
1. Para ajustar el área de recorte, siga uno de estos procedimientos:

   * Arrastre un lado o una esquina del recuadro. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño manteniendo la proporción de aspecto (la forma) del área de recorte.
   * Introduzca medidas de píxel en los cuadros Tamaño.
   * Arrastre para mover el cuadro de recorte. Mueva el puntero dentro de los límites del cuadro. Cuando vea la flecha con cuatro puntas, arrastre el cuadro a una nueva ubicación en la imagen.

1. Haga clic en **Guardar**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original tras su recorte, muéstrela en la pantalla Editor de recorte y seleccione el botón Restablecer.

>[!MORELIKETHIS]
>
>* [Opciones de edición de imágenes al cargarlas](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recorte de espacio en blanco de un archivo PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recorte de los lados de páginas PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

