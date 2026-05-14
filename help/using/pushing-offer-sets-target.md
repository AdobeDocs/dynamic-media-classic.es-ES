---
title: Insertar conjuntos de ofertas en Adobe Target Standard/Premium
description: Obtenga información sobre cómo insertar conjuntos de ofertas en Adobe Target Standard/Premium desde Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:55:22.850Z'
TQID: 'https://experienceleague.adobe.com/8j9sRn1zhAhgj-wMV6hYix1F9aARZjDUiFZofcVVcBw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 0%

---

# Insertar conjuntos de ofertas en Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Después de crear o editar un conjunto de ofertas, insértelo en Adobe Target Standard/Premium siguiendo estos pasos:

1. En la pantalla Conjunto de ofertas de Test&amp;Target, seleccione **[!UICONTROL Ofertas push]**.
1. Introduzca el código de cliente y las credenciales de inicio de sesión.
1. Seleccione **[!UICONTROL Iniciar sesión]**.

Durante la transferencia a Adobe Target Standard/Premium, el prefijo `S7_` se adjunta automáticamente al inicio de los nombres de las ofertas. Este prefijo se adjunta para garantizar que pueda encontrar fácilmente ofertas de Adobe Dynamic Media Classic en la lista de ofertas de Test&amp;Target. Por ejemplo, la oferta aparece como `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic inserta ofertas de widgets de Adobe Target Standard/Premium. Puede utilizar ofertas de widget para alojar su propio contenido ofrecido en Adobe Target Standard/Premium. Las ofertas de widget son similares a una oferta estándar alojada en Adobe Target Standard/Premium. Permiten a Adobe Target Standard/Premium implementar contenido de ofertas almacenado en el servidor, lo que permite un uso más sofisticado y dinámico. Las ofertas de widget pueden recuperar contenido de una dirección URL, almacenarlo en caché y ofrecerlo durante aproximadamente dos horas. Las ofertas de widget proporcionan algunas funciones de generación de contenido dinámico que otras ofertas fuera de Adobe Target Standard/Premium no. Si el mbox que sirve la oferta contiene parámetros de mbox, como `mboxProductID` y `mbox.offerId`, los parámetros de URL `productId=[PRODUCT_ID]` y `offerID=[OFFERID]` se anexan a la dirección URL solicitada. Estos parámetros los utiliza un servicio disponible en la dirección URL de la oferta del widget para devolver contenido fuera de Adobe Target Standard/Premium que utiliza información del producto o del pedido de sus mboxes. También se puede acceder a la oferta de Widget a través de la API para poder crear ofertas fuera de Adobe Target Standard/Premium mediante programación.
