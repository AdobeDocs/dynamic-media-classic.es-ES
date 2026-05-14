---
title: Administrar variaciones de contenido
description: Obtenga información sobre cómo administrar las variaciones de contenido en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 65b8c314-7ec1-417f-8a7b-aa13762072a1
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:40:29.070Z'
TQID: 'https://experienceleague.adobe.com/KjKdz4CAeSdJ3P-LKvdmsoGlkroeOZ60AvydF2FBHaI'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 248
ht-degree: 44%

---

# Administrar variaciones de contenido{#managing-content-variations}

Use conjuntos de plantillas para gestionar la forma en que se publican las variaciones de recursos.

Cree un conjunto de plantillas para gestionar las variaciones de una plantilla. Puede controlar qué variación se utiliza sin cambiar el código de su sitio. Este método ayuda a los administradores de contenido a girar el contenido sin que sea necesario cambiar una dirección URL en el código web.

Las direcciones URL universales se utilizan para mostrar la variación de plantilla que aparece en la página, según el orden en que aparezcan en el conjunto. La plantilla de la parte superior de la lista de conjuntos de plantillas siempre se publica.

Puede utilizar cualquier URL de ajuste preestablecido de imagen de la lista. Las URL de ajustes preestablecidos de imagen son como URL universales. Puede haber más de una URL de ajuste preestablecido de imagen.

1. Vaya a **[!UICONTROL Compilación]** > **[!UICONTROL Conjuntos de plantillas]**.
1. En el generador, seleccione una plantilla y, a continuación, seleccione **[!UICONTROL Agregar/Vista previa]**.
1. Modifique las propiedades de la plantilla y seleccione **[!UICONTROL Guardar como]** para crear otra versión.
1. Escriba un nombre y, a continuación, seleccione **[!UICONTROL Guardar]**.

   Tanto el recurso como la plantilla deben publicarse.

1. Vaya a la página de detalles para obtener una URL de copia desde la sección de las URL.

Puede cambiar el orden de una plantilla (por ejemplo, moverla a la parte superior de la lista), arrastrándola a su nueva ubicación. Vuelva a publicar para enviar el orden nuevo.

>[!NOTE]
>
>Si es necesario, borre la caché para ver los cambios. El cambio solo aparece en el sitio web después de que se haya completado el ciclo de la caché.
