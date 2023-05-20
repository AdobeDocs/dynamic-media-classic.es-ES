---
title: Recortar una imagen
description: Aprenda a recortar una imagen en Adobe Dynamic Media Classic.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# Recortar una imagen{#cropping-an-image}

Puede recortar imágenes en Adobe Dynamic Media Classic. El sistema retiene información sobre las imágenes que se recortaron para que pueda restaurar su estado original. También puede recortar una imagen y guardar con otro nombre la versión recortada.

Al recortar una imagen, puede quitar el espacio en blanco que la rodea o un área concreta de la imagen.

>[!NOTE]
>
>Después de recortar, puede seleccionar **[!UICONTROL Guardar como]** y guarde una versión recortada de la imagen con un nombre diferente. En la ventana Guardar como, seleccione **[!UICONTROL Guardar como nuevo elemento principal]** para guardar una segunda copia de la imagen. Seleccionar **[!UICONTROL Guardar Como Vista De Adición Del Principal]** para poder guardar el original y su versión recortada con un nombre diferente. Seleccionar **[!UICONTROL Reemplazar original]** para eliminar el archivo original desde el que recortó la imagen. A continuación, introduzca un nombre para la imagen y seleccione **[!UICONTROL Enviar]**.

## Recorte para quitar espacio en blanco alrededor de una imagen {#crop-to-remove-white-space-around-an-image}

Puede recortar los píxeles transparentes o de color sólido del borde de una imagen.

1. Para recortar una imagen, seleccione su rollover **[!UICONTROL Editar]** y luego seleccione **[!UICONTROL Recorte]**, o visualícelo en el panel de exploración en la vista de detalles y seleccione **[!UICONTROL Recorte]** botón.
1. En la página Editor de recorte, realice una de las acciones siguientes:

   * Para recortar píxeles de color, vaya a **[!UICONTROL Recortar]** > **[!UICONTROL Color]**. En el **[!UICONTROL Recorte automático por color]** , seleccione la opción **[!UICONTROL Esquina]** y elija una esquina con el color de fondo que desee recortar. A continuación, introduzca un **[!UICONTROL Tolerancia]** configuración de 0 a 1. El valor 0 recorta píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color. Seleccionar **[!UICONTROL Recorte]**.
   * Para recortar píxeles transparentes, vaya a **[!UICONTROL Recortar]** > **[!UICONTROL Transparente]**. En el **[!UICONTROL Recorte automático por transparencia]** , introduzca una configuración de tolerancia de 0 a 1. El ajuste 0 recorta píxeles solo si son transparentes. Los números más cercanos a 1 permiten una mayor transparencia. Seleccionar **[!UICONTROL Recorte]**.

1. Seleccionar **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original después de haberla recortado, muestre la imagen en la pantalla del Editor de recorte y seleccione **[!UICONTROL Restablecer]**.

## Selección de áreas que recortar {#select-an-area-to-crop}

1. Para recortar una imagen, seleccione su rollover **[!UICONTROL Editar]** y elija **[!UICONTROL Recorte]**, o muéstrelo en el panel de exploración en la vista de detalles y seleccione **[!UICONTROL Recorte]**.

1. En la ventana Editor de recorte, coloque la parte de la imagen que no desea recortar en el cuadro de recorte. Lo que aparezca dentro del cuadro es lo que permanecerá después de seleccionarlo **[!UICONTROL Guardar]** y recorte la imagen.
1. Para ajustar el área de recorte, siga uno de estos procedimientos:

   * Arrastre un lado o una esquina del recuadro. Mantenga pulsada la tecla Mayús mientras arrastra para cambiar el tamaño manteniendo la proporción de aspecto (la forma) del área de recorte.
   * Introduzca medidas de píxel en los cuadros Tamaño.
   * Arrastre para mover el cuadro de recorte. Mueva el puntero dentro de los límites del cuadro. Cuando vea la flecha con cuatro puntas, arrastre el cuadro a una nueva ubicación en la imagen.

1. Seleccionar **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Para restaurar una imagen a su estado original después de haberla recortado, muestre la imagen en la pantalla del Editor de recorte y seleccione **[!UICONTROL Restablecer]**.

>[!MORELIKETHIS]
>
>* [Opciones para la edición de imágenes al cargar](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recortar espacio en blanco de un archivo de PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recortar desde los lados de las páginas PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

