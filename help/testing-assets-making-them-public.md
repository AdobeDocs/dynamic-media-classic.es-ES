---
title: Prueba de los recursos antes de hacerlos públicos
description: Aprenda a probar los recursos antes de hacerlos públicos.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 54%

---


# Prueba de los recursos antes de hacerlos públicos {#testing-assets-before-making-them-public}

Secure Testing le ayudará a definir un entorno de prueba seguro y generar una solución B2B sólida, basándose en un conjunto de direcciones y rangos IP configurables. Esta funcionalidad le permite hacer coincidir las implementaciones de Dynamic Media Classic con la arquitectura de la plataforma de comercio y administración de contenido.

Con Secure Testing, puede obtener una vista previa de la versión de ensayo del sitio web con contenido no publicado.

Es posible que prefiera crear un entorno de ensayo en lugar de hacer públicos los recursos disponibles por las siguientes razones:

* Previsualizar sitios web antes del lanzamiento público (sitio web de ensayo).
* Disponer de los recursos que requieren acceso limitado, como catálogos electrónicos que muestran los precios en una aplicación web B2B.
* Utilizar recursos detrás de un firewall como parte del sistema de administración de información del producto, aplicación del servicio de atención al cliente, centro de formación, etc.

>[!NOTE]
>
>Secure Testing no afecta al acceso a Dynamic Media Classic. La seguridad de Dynamic Media Classic sigue siendo coherente y requiere las credenciales habituales para acceder a Dynamic Media Classic y a los servicios web relacionados.

## Funcionamiento de Secure Testing {#how-secure-testing-works}

Las mayoría de las empresas ejecutan Internet detrás de un firewall. El acceso a Internet se lleva a cabo a través de ciertas rutas y normalmente desde un rango limitado de direcciones IP públicas.

Desde su red corporativa, puede averiguar su dirección IP pública utilizando sitios web como https://whatismyip.com o solicitar esta información a su organización de TI corporativa.

Con Secure Testing, Dynamic Media Classic establece un servidor de imágenes dedicado para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP de origen. Si la solicitud entrante no está en la lista aprobada de direcciones IP, se devuelve una respuesta de error. El administrador de la empresa de Dynamic Media Classic configura la lista aprobada de direcciones IP para el entorno Secure Testing de su empresa.

Como se debe confirmar la ubicación de la solicitud original, el tráfico del servicio Secure Testing no se enruta a través de una red de distribución de contenido como el tráfico público del servidor de imágenes de Dynamic Media. Las solicitudes al servicio Secure Testing pueden tener una latencia ligeramente mayor que los servidores públicos de imágenes de Dynamic Media.

Los recursos no publicados están disponibles inmediatamente desde los servicios de Secure Testing, sin necesidad de publicarlos. Esto permite ejecutar una vista previa antes de que los recursos se publiquen en un servidor de imágenes público.

***nota **: Los servicios de Secure Testing aprovechan el servidor de catálogo configurado con un contexto de publicación interno. Por lo tanto, si su empresa está configurada para publicar en Secure Testing, tenga en cuenta que cualquier recurso cargado en Dynamic Media Classic estará disponible inmediatamente en los servicios de Secure Testing. Esta funcionalidad es cierta independientemente de si los recursos están marcados para la publicación o para la carga.*

Los servicios de Secure Testing admiten actualmente los siguientes tipos de activos y funcionalidades:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Imágenes.
* Viñetas (solicitudes del servidor de procesamiento).
* Procesar solicitudes de servidor (admitidas, pero el cliente debe solicitarlas explícitamente).
* Conjuntos, incluidos los conjuntos de imágenes, catálogos electrónicos, conjuntos de procesamiento y conjuntos de medios.
* Visores de medios enriquecidos de Dynamic Media Classic estándar.
* Páginas JSP de Dynamic Media Classic OnDemand.
* Contenido estático, como archivos PDF y vídeos de reproducción progresiva.
* Flujo continuo de vídeo HTTP.
* Flujo progresivo de vídeo.

Las siguientes funciones y tipos de recursos no se admiten actualmente:

* Flujo continuo de vídeo RTMP
* Servicios UGC
* Impresión virtual
* Búsqueda de Dynamic Media Classic Info o Catálogo electrónico

## Prueba del servicio Secure Testing {#testing-the-secure-testing-service}

Es conveniente que pruebe el servicio Secure Testing para asegurarse de que funciona como se espera.

Nota: Si no menciona ninguna IP en Configuración > Publicar configuración > Servidor de imágenes > Probar servicio de imágenes
si agrega una IP solamente, esta podrá llamar a los recursos y no se permitirá que ninguna otra IP realice las llamadas. Siempre que no se mencione ninguna IP en esa sección, todas las IP podrán realizar las llamadas para los recursos y aparecerán.

**Preparación de la cuenta**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Póngase en contacto con el servicio de asistencia técnica y solicite que Secure Testing se habilite en su cuenta.
1. En Dynamic Media Classic, haga clic en **Configuración** > **Publicar configuración** > **Image Server**.
1. En la lista desplegable Contexto de publicación de la página Servidor de imágenes, seleccione **Probar servicio de imágenes**.
1. En el filtro de direcciones de clientes, haga clic en **Agregar**.
1. Marque la casilla de verificación para habilitar (activar) la dirección y, seguidamente, escriba una dirección IP y una máscara de red en los respectivos los campos de texto.

   >[!NOTE]
   >
   >Si agrega una sola dirección IP y una máscara de red, esa dirección puede realizar llamadas de recursos. Sin embargo, cualquier otra dirección IP y máscara de red que agregue no podrán realizar llamadas de recursos. Como tal, puede considerar la posibilidad de desactivar (desactivar) la casilla de verificación en el paso anterior para desactivar la capacidad de especificar una dirección IP y una máscara de red. Al hacerlo, *todas* direcciones IP pueden realizar llamadas de recursos, y todas aparecerán.

1. Realice una de las siguientes acciones:
   * Repita los dos pasos anteriores para agregar más direcciones IP.
   * Continúe con el paso siguiente.
1. En la parte inferior izquierda de la página Servidor de imágenes, haga clic en **Guardar**.
1. Cargue las imágenes que desee en su cuenta de Dynamic Media Classic.

   Consulte [Carga de archivos](uploading-files.md#uploading_files).

1. Asegúrese de que algunas imágenes se han marcado para publicación y otros están sin marcar y, a continuación, envíe el trabajo de publicación.

   Consulte [Publicación](publishing-files.md#publishing_files).

1. Para determinar el nombre de su servicio Secure Testing, haga clic en **Ajustes** > **Ajustes de aplicación** > **Configuración general**.
1. En el grupo de servidores de la página Configuración general de la aplicación, busque el nombre a la derecha de la opción **Nombre del servidor del contexto de publicación de prueba**.

Póngase en contacto con el servicio de atención al Adobe si falta el nombre del servidor o si las direcciones URL del servidor no funcionan.

**Preparación de las variaciones del sitio web**

Se necesitan dos variaciones de un sitio web que vincule los recursos publicados y no publicados:

* Versión pública : vincule recursos con su sintaxis URL clásica de Dynamic Media Classic.
* Versión de ensayo : vincule los recursos con la misma sintaxis pero con el nombre del sitio Secure Testing.

**Ejecución de las pruebas**

Realice las siguientes pruebas:

1. Compruebe si los recursos son visibles desde la red de la empresa.

   Desde la red de la empresa identificada por el rango de direcciones IP definido anteriormente, la versión de ensayo del sitio web debe mostrar todas las imágenes, con independencia de si están marcadas para su publicación. Esto le permitirá probarlas sin que las imágenes queden disponibles accidentalmente antes de previsualizar el lanzamiento del producto o la aprobación.

   Confirme que la versión pública del sitio muestra los recursos publicados tal y como se experimentaron anteriormente con Dynamic Media Classic.

1. Desde fuera de la red de la empresa, compruebe que los recursos no publicados (es decir, sin marcar para publicación) están protegidos contra el acceso de terceros.

   Acceda a la red desde fuera (por ejemplo, desde su ordenador personal o a través de una conexión 3G) y, a continuación, compruebe que la versión pública del sitio muestra todos los recursos publicados pero ninguno del contenido sin publicar.

   Compruebe que la versión de ensayo no muestra ningún recurso, ya que está accediendo al servicio Secure Testing desde una dirección IP no autorizada.

