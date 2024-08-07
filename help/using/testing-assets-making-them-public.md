---
title: Pruebe los recursos antes de hacerlos públicos
description: Obtenga información sobre cómo probar recursos en Adobe Dynamic Media Classic antes de publicarlos.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# Pruebe los recursos antes de hacerlos públicos {#testing-assets-before-making-them-public}

Las pruebas seguras le ayudan a definir un entorno de prueba seguro y a crear una solución B2B sólida basada en un conjunto configurable de direcciones IP e intervalos. Esta funcionalidad le permite hacer coincidir las implementaciones de Adobe Dynamic Media Classic con la arquitectura del sistema empresarial y de administración de contenido.

Con Secure Testing, puede obtener una vista previa de la versión de ensayo del sitio web con contenido no publicado.

Si lo desea, cree un entorno de ensayo en lugar de publicar los recursos por los siguientes motivos:

* Previsualizar sitios web antes del lanzamiento público (sitio web de ensayo).
* Proporcione recursos que requieran acceso restringido, como catálogos electrónicos que muestran precios en una aplicación web B2B.
* Utilice recursos detrás de un cortafuegos como parte de un sistema de gestión de la información sobre productos, una aplicación de servicio al cliente, un sitio de formación, etc.

>[!NOTE]
>
>Prueba segura no afecta al acceso a Adobe Dynamic Media Classic. La seguridad de Adobe Dynamic Media Classic sigue siendo coherente y requiere las credenciales habituales para acceder a Adobe Dynamic Media Classic y a los servicios web relacionados.

## Funcionamiento de Secure Testing {#how-secure-testing-works}

Las mayoría de las empresas ejecutan Internet detrás de un firewall. El acceso a Internet se lleva a cabo a través de ciertas rutas y normalmente desde un rango limitado de direcciones IP públicas.

Desde su red corporativa, puede averiguar su dirección IP pública usando sitios web como [https://www.whatismyip.com](https://www.whatismyip.com/) o solicitar esta información a su organización de TI corporativa.

Con las pruebas seguras, Adobe Dynamic Media Classic crea un servidor de imágenes específico para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP de origen. Si la solicitud entrante no se encuentra dentro de la lista aprobada de direcciones IP, se devuelve una respuesta de error. El administrador de la empresa de Adobe Dynamic Media Classic configura la lista aprobada de direcciones IP para el entorno de prueba segura de su empresa.

Dado que la ubicación de la solicitud original debe confirmarse, el tráfico del servicio Prueba segura no se enruta a través de una red de distribución de contenido como el tráfico público de Dynamic Media Image Server. Las solicitudes al servicio Secure Testing tienen una latencia ligeramente superior en comparación con los servidores de imágenes de Dynamic Media públicos.

Los recursos no publicados están disponibles inmediatamente desde los servicios de Secure Testing, sin necesidad de publicarlos. De este modo, puede ejecutar una previsualización antes de que los recursos se publiquen en su servidor de imágenes público.

>[!NOTE]
>
>Los servicios de prueba segura utilizan el servidor de catálogos configurado con un contexto de publicación interno. Por lo tanto, si su empresa está configurada para publicar en pruebas seguras, todos los recursos cargados en Adobe Dynamic Media Classic estarán disponibles inmediatamente en los servicios de pruebas seguras. Esta funcionalidad se cumple independientemente de si los recursos se marcan para su publicación durante la carga.

Actualmente, los servicios de prueba segura admiten los siguientes tipos de recursos y funcionalidades:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Imágenes.
* Viñetas (solicitudes del servidor de procesamiento).
* Procesar solicitudes del servidor (compatible, pero el cliente debe solicitarlo explícitamente).
* Conjuntos, incluidos los conjuntos de imágenes, catálogos electrónicos, conjuntos de procesamiento y conjuntos de medios.
* Visores de medios enriquecidos estándar de Adobe Dynamic Media Classic.
* Páginas JSP de Adobe Dynamic Media Classic OnDemand.
* Contenido estático, como archivos PDF y vídeos de reproducción progresiva.
* Flujo continuo de vídeo HTTP.
* Flujo progresivo de vídeo.

Las siguientes funciones y tipos de recursos no se admiten actualmente:

* Búsqueda en catálogo electrónico o información de Adobe Dynamic Media Classic
* Flujo continuo de vídeo RTMP
* Impresión virtual
* Servicios de UGC (contenido generado por el usuario)

>[!IMPORTANT]
>
>La compatibilidad con recursos de imagen vectorial UGC nuevos o existentes en Adobe Dynamic Media Classic finalizó el 30 de septiembre de 2021.

## Prueba del servicio Secure Testing {#testing-the-secure-testing-service}

Pruebe el servicio Prueba segura para asegurarse de que funciona según lo esperado.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Preparación de la cuenta

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Póngase en contacto con el Servicio de atención al cliente de Adobe y solicite que habiliten Prueba segura en su cuenta.
1. En Adobe Dynamic Media Classic, en la barra de navegación global, ve a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de Publish]** > **[!UICONTROL Servidor de imágenes]**.
1. En la página Publish del servidor de imágenes, en la lista desplegable **[!UICONTROL `Publish Context`]**, seleccione **[!UICONTROL Probar servicio de imágenes]**.
1. Para el Filtro de direcciones de cliente, seleccione **[!UICONTROL Agregar]**.
1. Active la casilla de verificación para que la dirección esté habilitada (activada) y, a continuación, escriba una dirección IP y una máscara de red en los campos de texto correspondientes.

   >[!NOTE]
   >
   >Si agrega una sola dirección IP y máscara de red, esa dirección puede realizar llamadas de recurso. Sin embargo, no se permite que ninguna otra dirección IP ni máscara de red que agregue realice llamadas a recursos. De este modo, puede desactivar (desactivar) la casilla de verificación del paso anterior para desactivar la capacidad de especificar una dirección IP y una máscara de red. Al hacerlo, *todas* las direcciones IP pueden realizar llamadas de recurso y todas aparecerán.

1. Realice una de las siguientes acciones:
   * Repita los dos pasos anteriores si debe agregar más direcciones IP.
   * Continúe con el paso siguiente.
1. En la parte inferior izquierda de la página Publish del servidor de imágenes, seleccione **[!UICONTROL Guardar]**
1. Cargue las imágenes que desee en su cuenta de Adobe Dynamic Media Classic.

   Ver [Cargar archivos](uploading-files.md#uploading_files).

1. Asegúrese de que algunas imágenes estén marcadas para su publicación y otras no, y luego envíe el trabajo de publicación.

   Ver [archivos de Publish](publishing-files.md#publishing_files).

1. Determine el nombre de su servicio de pruebas seguras en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración general]**.
1. En el grupo de servidores de la página Configuración general de la aplicación, busque el nombre a la derecha de la opción **[!UICONTROL Nombre del servidor del contexto de publicación de prueba]**.

Póngase en contacto con el Servicio de atención al Adobe si falta el nombre del servidor o si las direcciones URL del servidor no funcionan.

### Preparación de las variaciones del sitio web

Se necesitan dos variaciones de un sitio web que vincule los recursos publicados y no publicados:

* Versión pública: Vincule los recursos con la sintaxis tradicional de URL de Adobe Dynamic Media Classic.
* Versión de ensayo: vincule los recursos con la misma sintaxis pero con el nombre del sitio de prueba segura.

### Ejecución de las pruebas

Realice las siguientes pruebas:

1. Compruebe si los recursos son visibles desde la red de la empresa.

   Desde la red corporativa identificada por el intervalo de direcciones IP previamente definido, la versión de ensayo del sitio web muestra todas las imágenes, estén marcadas para publicación o no. Como tal, puede realizar pruebas sin poner accidentalmente las imágenes a disposición antes de la aprobación de la vista previa o el lanzamiento del producto.

   Confirme que la versión pública del sitio muestra los recursos publicados tal como se experimentó anteriormente con Adobe Dynamic Media Classic.

1. Desde fuera de la red corporativa, compruebe que los recursos no publicados (es decir, sin marcar para publicación) estén protegidos frente al acceso de terceros.

   Acceda a la red desde fuera (por ejemplo, desde el equipo doméstico o a través de una conexión 3G) y, a continuación, compruebe que la versión pública del sitio muestre todos los recursos publicados, pero ninguno de los contenidos no publicados.

   Compruebe que la versión de ensayo no muestra ningún recurso, ya que está accediendo al servicio Secure Testing desde una dirección IP no autorizada.
