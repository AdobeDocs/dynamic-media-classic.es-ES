---
title: Inserción de conjuntos de ofertas en Adobe Target Classic
seo-title: Inserción de conjuntos de ofertas en Adobe Target Classic
description: nulo
seo-description: Aprenda a insertar conjuntos de ofertas en Adobe Target Classic.
uuid: 8 c 895 a 7 c -21 b 4-4 d 85-8 b 0 b-a 3 d 2 a 420 bf 2 e
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/target_ classic_ integration
discoiquuid: 39 a 05654-4 f 66-4 f 1 e-aec 5-ebe 6 d 174353 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Inserción de conjuntos de ofertas en Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

Después de crear o editar un conjunto de ofertas, introdúzcalo en Target Classic siguiendo estos pasos:

1. En la pantalla Conjunto de ofertas de Target Classic, haga clic en el botón Insertar ofertas.
1. Introduzca sus credenciales de inicio de sesión.
1. Haga clic en el botón Iniciar sesión.

Durante la transferencia a Target Classic, el prefijo S 7_ se adjunta automáticamente al inicio de los nombres de ofertas. Este prefijo se adjunta para garantizar que pueda encontrar fácilmente las ofertas de Dynamic Media Classic en la lista de ofertas de Target Classic. Por ejemplo, la oferta aparece como S7_&lt;nombre_conjunto_ofertas&gt;_&lt;nombre_oferta&gt;.

SPS inserta en ofertas de utilidades de Target Classic. Puede utilizar ofertas de widget para alojar su propio contenido de ofertas fuera de Target Classic. Las ofertas de utilidades son similares a una oferta estándar alojada fuera de Target Classic. Permiten a Target Classic implementar contenido de ofertas almacenado en su servidor, lo que permite un uso más sofisticado y dinámico. Las ofertas de utilidades recuperan contenido de una URL, lo almacenan en caché y lo presentan durante unas dos horas aproximadamente. Las ofertas en utilidades proporcionan algunas funcionalidades de generación de contenido dinámico que otras ofertas fuera de Target Classic no. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Estos parámetros pueden ser utilizados por un servicio disponible en la URL de la oferta de utilidades para devolver contenido fuera de Target Classic que utilice información de productos o pedidos de los mboxes. También se puede acceder a la oferta de utilidades a través de la API para crear ofertas mediante programación fuera de Target Classic.
