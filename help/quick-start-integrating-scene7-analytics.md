---
title: '"Inicio rápido: Integración de Dynamic Media Classic y Adobe Analytics "'
seo-title: '"Inicio rápido: Integración de Dynamic Media Classic y Adobe Analytics "'
description: nulo
seo-description: Introducción y Inicio rápido a la integración de Dynamic Media Classic y Adobe Analytics para ayudarle en el uso inicial.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: 2fb7e34b734dba1e0bd1d150580d7d6c74ee1b79
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 47%

---


# Inicio rápido: Integración de Dynamic Media Classic y Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics es un producto líder de la industria que ofrece a los vendedores un lugar donde pueden medir, analizar y optimizar datos integrados de todas las iniciativas en línea a través de múltiples canales de marketing.

Después de integrar Adobe Analytics con Scene7 Publishing System, puede obtener informes sobre el comportamiento de los visitantes del sitio web mediante los visores de Dynamic Media Classic en el sitio web. Por ejemplo, cuando un visitante de un sitio web hace clic en un destinatario de zoom en un visor de zoom Dynamic Media Classic, Adobe Analytics registra esta acción. Los informes de Adobe Analytics pueden recopilar información acumulativa sobre la actividad de los usuarios en los visores de Dynamic Media Classic.

Con el uso de los informes de Adobe Analytics, podrá obtener una imagen clara de la actividad de los clientes en su sitio web. Podrá averiguar cuáles son las presentaciones de productos que producen ventas y cuáles las que no despiertan el interés de los clientes.

Consulte también [Medición de vídeo en Adobe Analytics](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Se requiere una cuenta válida de Adobe Analytics para integrar Analytics con Scene7 Publishing System y generar informes de Analytics.

**Inicio rápido**

Este inicio rápido se ha diseñado para ayudarle en el uso inicial del kit de instrumentación de Adobe Analytics.

**1. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>Antes de configurar los informes de Adobe Analytics y hacer coincidir las variables de informes de Adobe Analytics con los eventos de Dynamic Media Classic, compruebe que se le ha agregado como miembro del grupo Acceso a servicios web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web de Marketing Cloud independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, haga clic en **Herramientas de administración** > **Administración de usuario** > **Editar grupos**.

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** > **Application Setup** > **Adobe Analytics**. En la página de configuración de Adobe Analytics, haga clic en **Inicio de sesión de Adobe Analytics**.

Consulte [Inicio de sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

En el cuadro de diálogo Inicio de sesión de Adobe Analytics, escriba su ID de organización de Marketing Cloud (opcional) y sus credenciales completas y, a continuación, haga clic en **Iniciar sesión**. En el menú desplegable Grupo de informes, seleccione el nombre del grupo de informes que desee utilizar.

**2. Asignar variables de informes de Adobe Analytics a eventos de visor de Dynamic Media Classic y variables de Dynamic Media Classic**

En la página de configuración de Adobe Analytics, especifique la información que desee incluir en los informes de Adobe Analytics. Para cada evento de visor de Dynamic Media Classic del que desee obtener información, elija una variable de Analytics de Adobe (del grupo de informes) y una variable de Dynamic Media Classic.

* Los eventos del visor describen la actividad de los usuarios que desea registrar en los informes.
* Las variables de Dynamic Media Classic describen los datos sobre los eventos de usuario que desea que los informes proporcionen.

La pantalla de configuración de Adobe Analytics también incluye herramientas para activar, editar y eliminar eventos de visor.

Después de hacer clic en Guardar en la pantalla de configuración de Adobe Analytics, se inserta un código de seguimiento personalizado para medir la actividad del usuario en los visores de Dynamic Media Classic. Esta funcionalidad permite realizar el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics.

Consulte [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Publicación de los visores de Dynamic Media Classic**

Publique los visores de Dynamic Media Classic para que los visores (con código para el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics) se carguen en los servidores de Dynamic Media Classic. Después de la publicación, esta información se incluye en los visores y puede emplearse en los análisis de Adobe Analytics.

Consulte [Publicación de la información de configuración](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Coloque los visores de Dynamic Media Classic en el sitio web**

Coloque los visores de Dynamic Media Classic con el código de seguimiento de Analytics de Adobe en el sitio web.

**5. Prueba de la integración de Adobe Analytics mediante un informe de Adobe Analytics**

Para ver los informes de Adobe Analytics, visite el sitio web de Adobe Analytics. En la página de informes puede consultar los datos y generar gráficos y diagramas para medir la actividad de los usuarios con diferentes visores. 

Consulte [Prueba de la integración de Adobe Analytics mediante un informe de Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
