---
title: Recorte de imágenes
description: Aprenda a recortar una imagen.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Administración de recursos
role: Business Practitioner
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 51%

---

# Recorte de imágenes{#cropping-an-image}

Puede recortar imágenes en Dynamic Media Classic. El sistema retiene información sobre las imágenes que se recortaron para que pueda restaurar su estado original. También puede recortar una imagen y guardar con otro nombre la versión recortada.

Al recortar una imagen, puede quitar el espacio en blanco que la rodea o un área concreta de la imagen.

>[!NOTE]
>
>Después del recorte, puede hacer clic en el botón Guardar como y guardar una versión recortada de la imagen con un nombre diferente. En la ventana Guardar como, elija Guardar como nuevo elemento principal para guardar una segunda copia de la imagen. Haga clic en **[!UICONTROL Guardar como vista de adición de maestro]** para guardar el original y su versión recortada con un nombre diferente. Haga clic en **[!UICONTROL Reemplazar original]** para eliminar el archivo original del que recortó la imagen. A continuación, introduzca un nombre para la imagen y haga clic en **[!UICONTROL Submit]**.

## Recorte para quitar espacio en blanco alrededor de una imagen {#crop-to-remove-white-space-around-an-image}

Puede recortar los píxeles transparentes o de color sólido del borde de una imagen.

1. Para recortar una imagen, haga clic en su botón de rollover **[!UICONTROL Editar]** y elija **[!UICONTROL Recortar]**, o muéstrela en el panel Examinar de la vista de detalles y haga clic en el botón **[!UICONTROL Recortar]**.
1. En la página Editor de recorte, realice una de las siguientes acciones:

   * Para recortar los píxeles de color, haga clic en **[!UICONTROL Recortar]** > **[!UICONTROL Color]**. Aparecerá el cuadro de diálogo Recorte automático por color. Haga clic en el menú **[!UICONTROL Corner]** y elija una esquina con el color de fondo que desee recortar. A continuación, introduzca una configuración de **[!UICONTROL Tolerancia]** de 0 a 1. El valor 0 recorta píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color. Haga clic en el botón **[!UICONTROL Crop]**.
   * Para recortar píxeles transparentes, seleccione haga clic en **[!UICONTROL Recortar]** > **[!UICONTROL Transparente]**. Aparecerá el cuadro de diálogo Recorte automático por transparencia. Introduzca un valor de Tolerancia de 0 a 1. El ajuste 0 recorta píxeles solo si son transparentes. Los números más cercanos a 1 permiten una mayor transparencia. Haga clic en **[!UICONTROL Recortar]**.

1. Haga clic en **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original después de recortarla, muestre la imagen en la pantalla Editor de recorte y haga clic en **[!UICONTROL Restaurar]**.

## Selección de áreas que recortar {#select-an-area-to-crop}

1. Para recortar una imagen, haga clic en su botón de rollover **[!UICONTROL Editar]** y elija **[!UICONTROL Recortar]** o muéstrela en el panel Examinar de la vista de detalles y haga clic en **[!UICONTROL Recortar]**.

1. En la ventana Editor de recorte, coloque la parte de la imagen que no desea recortar en el cuadro de recorte. Lo que aparece dentro del cuadro es lo que queda cuando hace clic en **[!UICONTROL Guardar]** y recorta la imagen.
1. Para ajustar el área de recorte, siga uno de estos procedimientos:

   * Arrastre un lado o una esquina del recuadro. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño manteniendo la proporción de aspecto (la forma) del área de recorte.
   * Introduzca medidas de píxel en los cuadros Tamaño.
   * Arrastre para mover el cuadro de recorte. Mueva el puntero dentro de los límites del cuadro. Cuando vea la flecha con cuatro puntas, arrastre el cuadro a una nueva ubicación en la imagen.

1. Haga clic en **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original después de recortarla, muestre la imagen en la pantalla Editor de recorte y haga clic en **[!UICONTROL Restaurar]**.

>[!MORELIKETHIS]
>
>* [Opciones de edición de imágenes al cargarlas](image-editing-options-upload.md#image-editing-options-at-upload)
* [Recorte de espacio en blanco de un archivo PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
* [Recorte de los lados de páginas PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

