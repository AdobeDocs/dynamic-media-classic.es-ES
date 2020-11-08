---
title: Inserción de conjuntos de ofertas en Adobe Target Standard/Premium
seo-title: Inserción de conjuntos de ofertas en Adobe Target Standard/Premium
description: nulo
seo-description: Aprenda a insertar conjuntos de ofertas en Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 5%

---


# Inserción de conjuntos de ofertas en Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Después de crear o editar un conjunto de ofertas, introdúzcalo en Target Standard/Premium siguiendo estos pasos:

1. In the Test&amp;Target Offer Set screen, click **[!UICONTROL Push Offers]**.
1. Introduzca el código de cliente y las credenciales de inicio de sesión.
1. Haga clic en **[!UICONTROL Inicio de sesión]**.

Durante la transferencia a Target Standard/Premium, el prefijo S7_ se adjunta automáticamente al inicio de nombres de ofertas. Este prefijo se adjunta para garantizar que pueda encontrar fácilmente ofertas de Dynamic Media Classic en la lista de oferta de Test&amp;Destinatario. Por ejemplo, la oferta aparece como S7_&lt;nombre_conjunto_ofertas>_&lt;nombre_oferta>.

Dynamic Media Classic incorpora ofertas de utilidades de Target Standard/Premium. Puede utilizar ofertas en utilidades para alojar su propio contenido de oferta fuera de Target Standard/Premium. Las ofertas de utilidades son similares a una oferta estándar alojada fuera de Target Standard/Premium. Permiten que Target Standard/Premium implemente contenido de oferta almacenado en el servidor, lo que permite un uso más sofisticado y dinámico. Las ofertas en utilidades recuperan contenido de una URL, lo almacenan en la caché y lo ofrecen durante aproximadamente dos horas. Las ofertas de utilidades proporcionan algunas funciones de generación de contenido dinámico que otras ofertas fuera de Target Standard/Premium no proporcionan. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Estos parámetros los puede utilizar un servicio disponible en la dirección URL de la oferta de utilidades para devolver contenido fuera de Target Standard/Premium que utilice información de productos o pedidos de los mboxes. También se puede acceder a la oferta Widget a través de la API para crear ofertas mediante programación fuera de Target Standard/Premium.
