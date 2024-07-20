---
title: Preparación para la actualización
description: Una lista de comprobación de preparación para la actualización cuando desee avanzar de [!DNL Adobe Dynamic Media Classic] a [!DNL Dynamic Media] en [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# Lista de comprobación de preparación para actualización

Utilice la siguiente lista de comprobación para ayudarle a comprender y preparar una actualización de [!DNL Dynamic Media Classic] a [!DNL Dynamic Media].

|  | Tarea | Descripción |
| :--- | :--- | --- |
| **Fase 1: Licencias** | Ejecutar contrato | En función del tráfico y el almacenamiento, el equipo de la cuenta de Adobe trabajará con usted para cambiar de la licencia [!DNL Dynamic Media Classic] a la renovación de la licencia [!DNL Dynamic Media]. |
| **Fase 2: preparación** | Validar el uso de funcionalidades | Confirme que las características que se están usando en [!DNL Dynamic Media Classic] están disponibles en [!DNL Dynamic Media]. Consulte la página [Comparación de características](/help/using/upgrade-feature-comparison.md). Las funciones clave que aún no están disponibles en [!DNL Dynamic Media] son las siguientes:<br>· Configurador visual (autor de imágenes, procesador de imágenes).<br>· Plantillas de imagen (plantilla 1:1).<br>· Catálogos electrónicos.<br>Si se están utilizando las características anteriores, la actualización puede realizarse suponiendo que se podría obtener acceso a esas características mediante [!DNL Dynamic Media Classic]. |
|   | Identificar recursos | Busque y prepare los recursos y ajustes preestablecidos que se utilizarán para la actualización. |
| **Fase 3: Entorno** | Actualizar [!DNL Adobe Experience Manager] | Todas las instancias de [!DNL Adobe Experience Manager] deben actualizarse a la versión más reciente. |
|   | Configuración [!DNL Dynamic Media] | Adobe Consulting o un socio configuran [!DNL Dynamic Media] con sus credenciales. |
| **Fase 4: actualizar** | Replicar recursos | Durante el proceso de actualización, los recursos designados [!DNL Dynamic Media Classic] se replican en Dynamic Media. |
| **Fase 5: Configuración administrativa** | Configuración de usuarios y permisos | Cree usuarios y conceda los permisos adecuados. |
|   | Configuración de perfiles de codificación de vídeo | Cree perfiles de codificación de vídeo. |
|   | Configurar ajustes preestablecidos del visor | Crear ajustes preestablecidos de visor. |
|   | Establecer ajustes preestablecidos de imagen | Configurar ajustes preestablecidos de imagen. |
| **Fase 6: Validación** | Validación | Compruebe casos de uso, recursos, vínculos y API. |
