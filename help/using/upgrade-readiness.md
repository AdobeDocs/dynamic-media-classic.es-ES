---
title: Lista de comprobación de preparación para actualización
description: Una lista de comprobación de preparación para la actualización cuando desee avanzar de [!DNL Adobe Dynamic Media Classic] a [!DNL Dynamic Media] en [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
autotag-review: '2026-05-13T20:16:07.073Z'
TQID: 'https://experienceleague.adobe.com/3Kcp3UwvJV8Mkzk6RBRgOJQ7JKF3Ldek-SiOeqS5EKE'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: bbfeefce82fc757d71e5ad0038120752eb0683c1
workflow-type: tm+mt
source-wordcount: 223
ht-degree: 1%

---

# Lista de comprobación de preparación para actualización

Utilice la siguiente lista de comprobación para ayudarle a comprender y preparar una actualización de [!DNL Dynamic Media Classic] a [!DNL Dynamic Media].

|  | Tarea | Descripción |
| :--- | :--- | --- |
| **Fase 1: Licencias** | Ejecutar contrato | En función del tráfico y el almacenamiento, el equipo de la cuenta de Adobe trabaja con usted para realizar la transición de la licencia [!DNL Dynamic Media Classic] a la renovación con la licencia [!DNL Dynamic Media]. |
| **Fase 2: preparación** | Validar el uso de funcionalidades | Confirme que las características que se están usando en [!DNL Dynamic Media Classic] están disponibles en [!DNL Dynamic Media]. Consulte la página [Comparación de características](/help/using/upgrade-feature-comparison.md). Entre las funciones clave que aún no están disponibles en [!DNL Dynamic Media] se incluyen las siguientes:<br>· Configurador visual (autor de imágenes, procesador de imágenes).<br>· Plantillas de imagen (plantilla 1:1).<br>· Catálogos electrónicos.<br>Si se están utilizando las características anteriores, la actualización puede seguir produciéndose suponiendo que dichas características serían accesibles mediante [!DNL Dynamic Media Classic]. |
|   | Identificar recursos | Busque y prepare los recursos y ajustes preestablecidos que se utilizarán para la actualización. |
| **Fase 3: Entorno** | Actualizar [!DNL Adobe Experience Manager] | Todas las instancias de [!DNL Adobe Experience Manager] deben actualizarse a la versión más reciente. |
|   | Configuración [!DNL Dynamic Media] | Adobe Consulting o un socio configuran [!DNL Dynamic Media] con sus credenciales. |
| **Fase 4: actualizar** | Replicar recursos | Durante el proceso de actualización, los recursos designados [!DNL Dynamic Media Classic] se replican en Dynamic Media. |
| **Fase 5: Configuración administrativa** | Configuración de usuarios y permisos | Cree usuarios y conceda los permisos adecuados. |
|   | Configuración de perfiles de codificación de vídeo | Cree perfiles de codificación de vídeo. |
|   | Configurar ajustes preestablecidos del visor | Crear ajustes preestablecidos de visor. |
|   | Establecer ajustes preestablecidos de imagen | Configurar ajustes preestablecidos de imagen. |
| **Fase 6: Validación** | Validación | Compruebe casos de uso, recursos, vínculos y API. |
