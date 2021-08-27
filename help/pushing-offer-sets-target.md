---
title: Insertar conjuntos de ofertas en Adobe Target Standard/Premium
description: Obtenga información sobre cómo insertar conjuntos de ofertas en Adobe Target Standard/Premium desde Adobe Dynamic Media Classic.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Insertar conjuntos de ofertas en Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Después de crear o editar un conjunto de ofertas, introdúzcalo en Adobe Target Standard/Premium siguiendo estos pasos:

1. En la pantalla Conjunto de ofertas de Test&amp;Target, seleccione **[!UICONTROL Ofertas push]**.
1. Introduzca el código de cliente y las credenciales de inicio de sesión.
1. Seleccione **[!UICONTROL Login]**.

Durante la transferencia a Adobe Target Standard/Premium, el prefijo `S7_` se adjunta automáticamente al inicio de los nombres de las ofertas. Este prefijo se adjunta para garantizar que pueda encontrar fácilmente ofertas de Adobe de Dynamic Media Classic en la lista de ofertas de Test&amp;Target. Por ejemplo, la oferta aparece como `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic incorpora las ofertas de utilidades de Adobe Target Standard/Premium. Puede utilizar ofertas en utilidades para alojar su propio contenido de ofertas fuera de Adobe Target Standard/Premium. Las ofertas en utilidades son similares a una oferta estándar alojada fuera de Adobe Target Standard/Premium. Permiten a Adobe Target Standard/Premium implementar contenido de ofertas almacenado en el servidor, lo que permite un uso más sofisticado y dinámico. Las ofertas en utilidades pueden recuperar contenido de una dirección URL, almacenarlo en caché y servirlo durante aproximadamente dos horas. Las ofertas en utilidades proporcionan algunas funciones de generación de contenido dinámico que otras ofertas fuera de Adobe Target Standard/Premium no proporcionan. Si el mbox que sirve la oferta contiene parámetros de mbox como `mboxProductID` y `mbox.offerId`, los parámetros de URL `productId=[PRODUCT_ID]`y `offerID=[OFFERID]` se agregan a la dirección URL solicitada. Estos parámetros puede utilizarlos un servicio disponible en la dirección URL de la oferta en utilidades para devolver contenido fuera de Adobe Target Standard/Premium que use información de productos o pedidos de sus mboxes. También se puede acceder a la oferta en utilidades a través de la API para crear ofertas mediante programación fuera de Adobe Target Standard/Premium.
