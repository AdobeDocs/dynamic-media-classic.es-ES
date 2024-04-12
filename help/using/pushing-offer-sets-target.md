---
title: Insertar conjuntos de ofertas en Adobe Target Standard/Premium
description: Obtenga información sobre cómo insertar conjuntos de ofertas en Adobe Target Standard/Premium desde Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Insertar conjuntos de ofertas en Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Después de crear o editar un conjunto de ofertas, insértelo en Adobe Target Standard/Premium siguiendo estos pasos:

1. En la pantalla Conjunto de ofertas de Test&amp;Target, seleccione **[!UICONTROL Transferir ofertas]**.
1. Introduzca el código de cliente y las credenciales de inicio de sesión.
1. Seleccionar **[!UICONTROL Iniciar sesión]**.

Durante la transferencia a Adobe Target Standard/Premium, el prefijo `S7_` se adjunta automáticamente al principio de los nombres de las ofertas. Este prefijo se adjunta para garantizar que pueda encontrar fácilmente ofertas de Adobe Dynamic Media Classic en la lista de ofertas de Test&amp;Target. Por ejemplo, la oferta aparece como `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic inserta ofertas de widgets de Adobe Target Standard/Premium. Puede utilizar ofertas de widget para alojar el contenido que ofrece fuera de Adobe Target Standard/Premium. Las ofertas de widget son similares a una oferta estándar alojada fuera de Adobe Target Standard/Premium. Permiten a Adobe Target Standard/Premium implementar contenido de ofertas almacenado en el servidor, lo que permite un uso más sofisticado y dinámico. Las ofertas de widget pueden recuperar contenido de una dirección URL, almacenarlo en caché y ofrecerlo durante aproximadamente dos horas. Las ofertas de widget proporcionan algunas funciones de generación de contenido dinámico que otras ofertas fuera de Adobe Target Standard/Premium no. Si el mbox que sirve la oferta contiene parámetros de mbox como `mboxProductID` y `mbox.offerId`, el `productId=[PRODUCT_ID]`y `offerID=[OFFERID]` Los parámetros de URL se anexan a la dirección URL solicitada. Estos parámetros los puede utilizar un servicio disponible en la URL de la oferta del widget para devolver contenido fuera de Adobe Target Standard/Premium que utilice información del producto o del pedido de sus mboxes. También se puede acceder a la oferta de Widget a través de la API para crear ofertas mediante programación fuera de Adobe Target Standard/Premium.
