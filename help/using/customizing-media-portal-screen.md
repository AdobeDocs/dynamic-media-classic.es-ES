---
title: Personalizar la pantalla de Media Portal
description: Aprenda a personalizar la pantalla de Media Portal en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 16%

---

# Personalizar la pantalla de Media Portal{#customizing-the-media-portal-screen}

Los ajustes de estilo de Media Portal le permiten aplicar un estilo de marca a la pantalla de Media Portal, con los colores y el logotipo de su empresa. Utilice la configuración de estilo para incluir la marca de su empresa en Media Portal.

Para acceder a la configuración de estilo, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Configuración de Media Portal]** > **[!UICONTROL Configuración de estilo]**. Asegúrese de seleccionar **[!UICONTROL Guardar]** para guardar la configuración después de hacerla. Puede seleccionar **[!UICONTROL Restaurar]** para recuperar la configuración predeterminada. A medida que realiza sus elecciones, el panel Vista previa le muestra cómo aparecen.

* **[!UICONTROL Logotipo]** - Seleccionar **[!UICONTROL Examinar]** y, a continuación, elija un gráfico en la ventana Seleccionar imagen de logotipo.

* **[!UICONTROL Aplicación]** - Crear una mezcla de colores de degradado mediante la selección de opciones en los menús de los Colores de degradado de fondo.

* **[!UICONTROL Árbol]** - Elija un color de rollover (el color que aparece al mover el puntero sobre un elemento) y un color de selección (el color que aparece al seleccionar un elemento).

* **[!UICONTROL Acordeón]** : elija colores de fondo, un estilo de borde y colores de rollover y seleccionados para el acordeón que aparece a la derecha de la pantalla en la vista Detalles.

* **[!UICONTROL Encabezado de acordeón]** - Elija si desea hacer que el texto en el encabezado de acordeón aparezca en negrita.

* **[!UICONTROL Datagrid]** - Elija colores para la fila de encabezado en las cuadrículas de datos.

* **[!UICONTROL Alerta]** - Elija un color de fondo para los cuadros de mensaje de alerta.

* **[!UICONTROL Barra de progreso]** : elija un color para la barra que indique el progreso de las cargas y descargas.

Para que los usuarios de Media Portal puedan ver la configuración de estilo que ha elegido, deben adjuntar `?company=(company name)` a la URL con la que acceden a Media Portal. Por ejemplo, para ver la configuración de estilo, los usuarios de Media Portal que acceden a la empresa PortalCo en las siguientes direcciones:

`https://s7sps1.scene7.com/MediaPortal`

En su lugar, utilice la siguiente URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Al incluir el nombre de la empresa en la URL, Media Portal puede reconocer a qué empresa desea acceder un usuario y aplicar la configuración de estilo de la empresa en consecuencia.

Para obtener información sobre cómo comunicar los cambios de URL a los usuarios de Media Portal, así como sobre cómo configurar un mensaje de correo electrónico de bienvenida para que los usuarios nuevos reciban la URL de Media Portal correcta.

Consulte [Configuración del mensaje de correo electrónico de bienvenida para los usuarios de Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
