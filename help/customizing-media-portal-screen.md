---
title: Personalización de la pantalla de Media Portal
seo-title: Personalización de la pantalla de Media Portal
description: nulo
seo-description: Obtenga información sobre cómo personalizar la pantalla de Media Portal.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 53%

---


# Personalización de la pantalla de Media Portal{#customizing-the-media-portal-screen}

Los ajustes de estilo de Media Portal le permiten aplicar un estilo de marca a la pantalla de Media Portal, con los colores y el logotipo de su empresa. Utilice los ajustes de estilo para poner el sello de su empresa en Media Portal.

Para acceder a los ajustes de estilo, elija **Ajustes** > **Configuración de Media Portal** > **Configuración de estilo**. Asegúrese de hacer clic en **Guardar** para guardar la configuración después de realizarla. Puede hacer clic en **Restaurar** para recuperar la configuración predeterminada. A medida que vaya seleccionando, el panel Vista previa irá mostrando cómo quedan las opciones que vaya eligiendo.

**** LogotipoHaga clic en Examinar y elija un gráfico en la ventana Seleccionar imagen de logotipo.

**** AplicaciónCree una mezcla de colores de degradado mediante las opciones de los menús Colores de degradado de fondo.

**** ÁrbolElija un color de rollover (el color que aparece al mover el puntero sobre un elemento) y un color de selección (el color que aparece al seleccionar un elemento).

**** AcordeónElija colores de fondo, un estilo de borde y colores de rollover y seleccionados para el acordeón que aparece a la derecha de la pantalla en la vista Detalles.

**Encabezado** de acordeónElija si desea que el texto del encabezado de acordeón aparezca en negrita.

**Barra** de datosElija colores para la fila de encabezado en las cuadrículas de datos.

**** AlertaElija un color de fondo para los cuadros de mensaje de alerta.

**Barra** de progresoElija un color para la barra que indique el progreso de las cargas y descargas.

Para que los usuarios de Media Portal puedan ver la configuración de estilo que elija, deben anexar `?company=(company name)` a la URL con la que acceden a Media Portal. Por ejemplo, para ver los ajustes de estilo, los usuarios de Media Portal que accedan a la empresa PortalCo mediante la siguiente URL:

`https://s7sps1.scene7.com/MediaPortal`

utilizarían la siguiente URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Al incluir el nombre de la empresa en la URL, Media Portal puede reconocer la empresa a la que un usuario desea acceder y aplicar los ajustes de estilo de la empresa de la forma oportuna.

Para obtener información sobre cómo comunicar los cambios de URL a los usuarios de Media Portal, así como sobre cómo configurar un mensaje de correo electrónico de bienvenida para que los usuarios nuevos reciban la URL de Media Portal correcta.

Consulte [Configuración del mensaje de correo electrónico de bienvenida para los usuarios de Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
