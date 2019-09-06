---
title: '" Inicio rápido: Integración de Dynamic Media Classic y Adobe Analytics "'
seo-title: '" Inicio rápido: Integración de Dynamic Media Classic y Adobe Analytics "'
description: nulo
seo-description: Una introducción e Inicio rápido para integrar Dynamic Media Classic y Adobe Analytics para ayudarle a empezar a utilizarlo rápidamente.
uuid: 3 f 9 e 2 c 91-15 d 4-4 b 53-8220-9 b 1 ca 57 c 0 b 1 d
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: abec 9 a 85-013 c -4030-b 129-bf 27 a 89 cb 464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Inicio rápido: Integración de Dynamic Media Classic y Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics es un producto líder de la industria que ofrece a los vendedores un lugar donde pueden medir, analizar y optimizar datos integrados de todas las iniciativas en línea a través de múltiples canales de marketing.

Después de integrar Adobe Analytics con Scene 7 Publishing System, puede obtener informes sobre el comportamiento de los visitantes del sitio web mediante visores de Dynamic Media Classic en su sitio web. Por ejemplo, cuando un visitante de un sitio web hace clic en un destino de zoom en un visor de zoom de Media Media Classic, Adobe Analytics registra esta acción. Los informes de Adobe Analytics pueden recopilar información acumulativa sobre la actividad de los usuarios en los visores de Dynamic Media Classic.

Con el uso de los informes de Adobe Analytics, podrá obtener una imagen clara de la actividad de los clientes en su sitio web. Podrá averiguar cuáles son las presentaciones de productos que producen ventas y cuáles las que no despiertan el interés de los clientes.

Consulte también [Medición de vídeo en Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Se requiere una cuenta válida de Adobe Analytics para integrar Analytics con Scene7 Publishing System y generar informes de Analytics.

**Inicio rápido**

Este inicio rápido se ha diseñado para ayudarle en el uso inicial del kit de instrumentación de Adobe Analytics.

**1. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>Para poder configurar informes de Adobe Analytics y combinar variables de informes de Adobe Analytics con los eventos de Dynamic Media Classic, compruebe que se haya agregado como miembro del grupo Acceso a servicio Web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web de Marketing Cloud independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, haga clic en **Herramientas de administración** &gt; **Administración de usuario** &gt; **Editar grupos**.

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** &gt; **Application Setup** &gt; **Adobe Analytics**. En la página de configuración de Adobe Analytics, haga clic en **Inicio de sesión de Adobe Analytics**.

Consulte [Inicio de sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

En el cuadro de diálogo Inicio de sesión de Adobe Analytics, escriba su ID de organización de Marketing Cloud (opcional) y sus credenciales completas y, a continuación, haga clic **en Iniciar sesión**. En el menú desplegable Grupo de informes, seleccione el nombre del grupo de informes que desee utilizar.

**2. Asigne variables de informes de Adobe Analytics a eventos de visor de Dynamic Media Classic y variables de Dynamic Media Classic**

En la página de configuración de Adobe Analytics, especifique la información que desee incluir en los informes de Adobe Analytics. Para cada evento de visor de Dynamic Media Classic en el que desee información, elija una variable de Adobe Analytics (de su grupo de informes) y una variable de Dynamic Media Classic.

* Los eventos del visor describen la actividad de los usuarios que desea registrar en los informes.
* Las variables de Dynamic Media Classic describen los datos sobre los eventos de usuario que desea que entreguen los informes.

La pantalla de configuración de Adobe Analytics también incluye herramientas para activar, editar y eliminar eventos de visor.

Después de hacer clic en Guardar en la pantalla de configuración de Adobe Analytics, se inserta un código de seguimiento personalizado para medir la actividad de los usuarios en los visores de Dynamic Media Classic. Esta funcionalidad permite realizar el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics.

Consulte [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Publicación de los visores de Dynamic Media Classic**

Publique los visores de Dynamic Media Classic para que los visores (con código para el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics) se carguen en servidores de Dynamic Media Classic. Después de la publicación, esta información se incluye en los visores y puede emplearse en los análisis de Adobe Analytics.

Consulte [Publicación de la información de configuración](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Coloque los visores de Dynamic Media Classic en el sitio web**

Coloque los visores de Dynamic Media Classic con el código de seguimiento de Adobe Analytics en su sitio web.

**5. Prueba de la integración de Adobe Analytics mediante un informe de Adobe Analytics**

Para ver los informes de Adobe Analytics, visite el sitio web de Adobe Analytics. En la página de informes puede consultar los datos y generar gráficos y diagramas para medir la actividad de los usuarios con diferentes visores. 

Consulte [Prueba de la integración de Adobe Analytics mediante un informe de Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
