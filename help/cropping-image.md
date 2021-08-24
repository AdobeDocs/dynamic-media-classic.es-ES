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
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 39%

---

# Recortar una imagen{#cropping-an-image}

Puede recortar imágenes en Dynamic Media Classic. El sistema retiene información sobre las imágenes que se recortaron para que pueda restaurar su estado original. También puede recortar una imagen y guardar con otro nombre la versión recortada.

Al recortar una imagen, puede quitar el espacio en blanco que la rodea o un área concreta de la imagen.

>[!NOTE]
>
>Después de recortar, puede seleccionar **[!UICONTROL Guardar como]** y guardar una versión recortada de la imagen con un nombre diferente. En la ventana Guardar como, elija Guardar como nuevo elemento principal para guardar una segunda copia de la imagen. Seleccione **[!UICONTROL Guardar como vista de adición de maestro]** para que pueda guardar el original y su versión recortada con un nombre diferente. Seleccione **[!UICONTROL Reemplazar original]** para eliminar el archivo original del que recortó la imagen. A continuación, introduzca un nombre para la imagen y seleccione **[!UICONTROL Enviar]**.

## Recorte para quitar espacio en blanco alrededor de una imagen {#crop-to-remove-white-space-around-an-image}

Puede recortar los píxeles transparentes o de color sólido del borde de una imagen.

1. Para recortar una imagen, seleccione su botón de rollover **[!UICONTROL Editar]** y elija **[!UICONTROL Recortar]**, o muéstrela en el panel Examinar en la vista de detalles y seleccione el botón **[!UICONTROL Recortar]**.
1. En la página Editor de recorte, realice una de las siguientes acciones:

   * Para recortar los píxeles de color, vaya a **[!UICONTROL Recortar]** > **[!UICONTROL Color]**. En el cuadro de diálogo **[!UICONTROL Recortar automáticamente por color]**, seleccione el menú **[!UICONTROL Esquina]** y elija una esquina con el color de fondo que desea recortar. A continuación, introduzca una configuración de **[!UICONTROL Tolerancia]** de 0 a 1. El valor 0 recorta píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color. Seleccione **[!UICONTROL Recortar]**.
   * Para recortar píxeles transparentes, vaya a **[!UICONTROL Recortar]** > **[!UICONTROL Transparente]**. En el cuadro de diálogo **[!UICONTROL Recorte automático por transparencia]**, introduzca un ajuste de tolerancia de 0 a 1. El ajuste 0 recorta píxeles solo si son transparentes. Los números más cercanos a 1 permiten una mayor transparencia. Seleccione **[!UICONTROL Recortar]**.

1. Seleccione **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original después de recortarla, muestre la imagen en la pantalla Editor de recorte y seleccione **[!UICONTROL Restaurar]**.

## Selección de áreas que recortar {#select-an-area-to-crop}

1. Para recortar una imagen, seleccione su botón de rollover **[!UICONTROL Editar]** y elija **[!UICONTROL Recortar]**, o muéstrela en el panel Examinar de la vista de detalles y seleccione **[!UICONTROL Recortar]**.

1. En la ventana Editor de recorte, coloque la parte de la imagen que no desea recortar en el cuadro de recorte. Lo que aparezca dentro del cuadro es lo que quedará después de seleccionar **[!UICONTROL Guardar]** y recortar la imagen.
1. Para ajustar el área de recorte, siga uno de estos procedimientos:

   * Arrastre un lado o una esquina del recuadro. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño manteniendo la proporción de aspecto (la forma) del área de recorte.
   * Introduzca medidas de píxel en los cuadros Tamaño.
   * Arrastre para mover el cuadro de recorte. Mueva el puntero dentro de los límites del cuadro. Cuando vea la flecha con cuatro puntas, arrastre el cuadro a una nueva ubicación en la imagen.

1. Seleccione **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original después de recortarla, muestre la imagen en la pantalla Editor de recorte y seleccione **[!UICONTROL Restaurar]**.

>[!MORELIKETHIS]
>
>* [Opciones de edición de imágenes al cargar](image-editing-options-upload.md#image-editing-options-at-upload)
* [Recortar espacio en blanco de un archivo PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
* [Recortar desde los lados de las páginas PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

