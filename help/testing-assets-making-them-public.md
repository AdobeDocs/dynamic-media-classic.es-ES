---
title: Prueba de los recursos antes de hacerlos públicos
seo-title: Prueba de los recursos antes de hacerlos públicos
description: nulo
seo-description: Aprenda a probar los recursos antes de hacerlos públicos.
uuid: 5 e 8 f 3 bec -6 cf 1-408 e -8 ea 1-aebde 0012 a 70
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/upload_ and_ publish_ assets
discoiquuid: 52 fadf 99-7 d 11-46 f 7-8483-a 9 f 87 ffc 2 f 67
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Prueba de los recursos antes de hacerlos públicos {#testing-assets-before-making-them-public}

Secure Testing le ayudará a definir un entorno de prueba seguro y generar una solución B2B sólida, basándose en un conjunto de direcciones y rangos IP configurables. Esta funcionalidad le permite equiparar las implementaciones de Dynamic Media Classic con la arquitectura de su plataforma comercial y de administración de contenido.

Con Secure Testing, puede obtener una vista previa de la versión de ensayo del sitio web con contenido no publicado.

Es posible que prefiera crear un entorno de ensayo en lugar de hacer públicos los recursos disponibles por las siguientes razones:

* Previsualizar sitios web antes del lanzamiento público (sitio web de ensayo).
* Disponer de los recursos que requieren acceso limitado, como catálogos electrónicos que muestran los precios en una aplicación web B2B.
* Utilizar recursos detrás de un firewall como parte del sistema de administración de información del producto, aplicación del servicio de atención al cliente, centro de formación, etc.

>[!NOTE]
>
>Secure Testing no afecta al acceso a Scene7 Publishing System. La seguridad de SPS sigue siendo la misma y requiere las credenciales habituales para acceder a SPS y los servicios web relacionados.

## Funcionamiento de Secure Testing {#how-secure-testing-works}

Las mayoría de las empresas ejecutan Internet detrás de un firewall. El acceso a Internet se lleva a cabo a través de ciertas rutas y normalmente desde un rango limitado de direcciones IP públicas.

Desde la red de la empresa, puede averiguar su dirección IP pública utilizando sitios web como https://whatismyip.com o solicitar esta información a su organización de TI corporativa.

Con Secure Testing, Dynamic Media Classic establece un servidor de imágenes dedicado para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP de origen. Si la solicitud entrante no está en la lista aprobada de direcciones IP, se devuelve una respuesta de error. El administrador de empresa de Media Media Classic configura la lista aprobada de direcciones IP para el entorno Secure Testing de su empresa.

Debido a que debe confirmarse la ubicación de la solicitud original, el tráfico del servicio Secure Testing no se enruta a través de una red de distribución de contenido como el tráfico del servidor de imágenes de Dynamic Media. Las solicitudes al servicio Secure Testing pueden tener una latencia ligeramente mayor en comparación con los servidores de imágenes de Dynamic Media.

Los recursos no publicados están disponibles inmediatamente desde los servicios de Secure Testing, sin necesidad de publicarlos. Esto permite ejecutar una vista previa antes de que los recursos se publiquen en un servidor de imágenes público.

***nota**: Los servicios Secure Testing aprovechan el servidor de catálogo configurado con un contexto de publicación interna. Por lo tanto, si su empresa está configurada para publicar en Secure Testing, tenga en cuenta que cualquier recurso cargado en Scene7 Publishing System queda inmediatamente disponible en los servicios de Secure Testing. Esta funcionalidad es cierta independientemente de si los recursos están marcados para la publicación o para la carga.*

Los servicios Secure Testing actualmente admiten los siguientes tipos de recursos y funciones:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Imágenes.
* Viñetas (solicitudes del servidor de procesamiento).
* Solicitudes del servidor de procesamiento (admitido, pero debe ser solicitado explícitamente por el cliente).
* Conjuntos, incluidos los conjuntos de imágenes, catálogos electrónicos, conjuntos de procesamiento y conjuntos de medios.
* Visores de medios enriquecidos estándar de Media Media Classic.
* Páginas de Dynamic Media Classic ondemand JSP.
* Contenido estático, como archivos PDF y vídeos de reproducción progresiva.
* Flujo continuo de vídeo HTTP.
* Flujo progresivo de vídeo.

Las siguientes funciones y tipos de recursos no se admiten actualmente:

* Flujo continuo de vídeo RTMP
* Servicios UGC
* Impresión virtual
* Información de medios dinámicos o búsqueda de catálogos electrónicos

## Prueba del servicio Secure Testing {#testing-the-secure-testing-service}

Es conveniente que pruebe el servicio Secure Testing para asegurarse de que funciona como se espera.

**Preparación de la cuenta**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Póngase en contacto con el servicio de asistencia técnica y solicite que Secure Testing se habilite en su cuenta.
1. En Scene7 Publishing System, haga clic en **Ajustes** &gt; **Ajustes de publicación** &gt; **Servidor de imágenes**.
1. En la lista desplegable Contexto de publicación de la página Servidor de imágenes, seleccione **Probar servicio de imágenes**.
1. En el filtro de direcciones de clientes, haga clic en **Agregar**.
1. Marque la casilla de verificación para habilitar (activar) la dirección y, seguidamente, escriba una dirección IP y una máscara de red en los respectivos los campos de texto.
1. Repita los dos pasos anteriores para agregar más direcciones IP. De lo contrario, continúe con el paso siguiente.
1. En la parte inferior izquierda de la página Servidor de imágenes, haga clic en **Guardar**.
1. Cargue las imágenes deseadas en su cuenta de Scene7 Publishing System.

   Consulte [Carga de archivos](uploading-files.md#uploading_files).

1. Asegúrese de que algunas imágenes se han marcado para publicación y otros están sin marcar y, a continuación, envíe el trabajo de publicación.

   Consulte [Publicación](publishing-files.md#publishing_files).

1. Para determinar el nombre de su servicio Secure Testing, haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Configuración general**.
1. En el grupo de servidores de la página Configuración general de la aplicación, busque el nombre a la derecha de la opción **Nombre del servidor del contexto de publicación de prueba**.

Póngase en contacto con el servicio de soporte técnico si falta el nombre del servidor o si las URL del servidor no funcionan.

**Preparación de las variaciones del sitio web**

Se necesitan dos variaciones de un sitio web que vincule los recursos publicados y no publicados:

* Versión pública: Vinculación de recursos mediante la sintaxis tradicional de URL de Dynamic Media Classic
* Versión de ensayo: enlaza los recursos con la misma sintaxis pero con el nombre del sitio de Secure Testing

**Ejecución de las pruebas**

Realice las siguientes pruebas:

1. Compruebe si los recursos son visibles desde la red de la empresa.

   Desde la red de la empresa identificada por el rango de direcciones IP definido anteriormente, la versión de ensayo del sitio web debe mostrar todas las imágenes, con independencia de si están marcadas para su publicación. Esto le permitirá probarlas sin que las imágenes queden disponibles accidentalmente antes de previsualizar el lanzamiento del producto o la aprobación.

   Confirme que la versión pública del sitio muestra recursos publicados como antes con Dynamic Media Classic.

1. Desde fuera de la red de la empresa, compruebe que los recursos no publicados (es decir, sin marcar para publicación) están protegidos contra el acceso de terceros.

   Acceda a la red desde fuera (por ejemplo, desde su ordenador personal o a través de una conexión 3G) y, a continuación, compruebe que la versión pública del sitio muestra todos los recursos publicados pero ninguno del contenido sin publicar.

   Compruebe que la versión de ensayo no muestra ningún recurso, ya que está accediendo al servicio Secure Testing desde una dirección IP no autorizada.

