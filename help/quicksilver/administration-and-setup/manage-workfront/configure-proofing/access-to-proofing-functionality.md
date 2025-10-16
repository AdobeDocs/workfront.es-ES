---
user-type: administrator
content-type: reference;overview
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Acceso a la funcionalidad de corrección en Workfront
description: La funcionalidad de revisión disponible para los usuarios depende del plan de Workfront que haya adquirido la organización.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 30a41ae9-9755-4c7b-9e3b-d4a8b0ad7ee8
source-git-commit: 882c3e58e0e47c549be70dff3f5ac410b34a090f
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 87%

---

# Acceso a la funcionalidad de revisión en Workfront

La revisión se incluye automáticamente para todas las licencias de Workfront. Las licencias determinan lo que los usuarios pueden hacer.

<!--Workfront instances using enterprise storage do not have access to proofing functionality. Instead, they use the native integration with Frame.io. For more information, see -->

Los paquetes de Workfront heredados de 2017 incluyen pruebas automáticas para licencias de trabajo y plan si tiene los planes profesionales, empresariales o de Workfront empresariales. Estos planes se están eliminando gradualmente.

Si es una persona con la función de administrador de Workfront, puede comprobar y ver qué plan tiene su instancia accediendo a Configuración > Sistema > Licencias.

## Funciones de revisión en Workfront

Para obtener información sobre cómo conceder y revocar el acceso de un usuario para crear y ver pruebas en Workfront, consulte [Configurar el acceso de revisión de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

* Genere pruebas estáticas o interactivas en documentos y direcciones URL externos. Para obtener más información, consulte [Crear pruebas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).
* Incluya flujos de trabajo automatizados en las pruebas. Para obtener más información, consulte [Información general sobre los flujos de trabajo automatizados](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).
* Establezca la configuración de acceso y suscripciones en las pruebas. Para obtener más información, consulte [Configurar las opciones de acceso y suscripción para una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md).
* Asigne perfiles de permisos de prueba personalizados al habilitar las funciones de revisión para un usuario en Workfront. Para obtener más información, consulte [Habilitar y deshabilitar la revisión para un usuario (solo planes heredados)](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md#enabling-and-disabling-proofing-for-a-user) en [Configurar el acceso de revisión de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).
* Rastree el progreso y el estado de la prueba. Para obtener más información, consulte [Información general sobre el progreso y el estado de la prueba](../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).
* Establezca el perfil de permisos de Workfront Proof al crear usuarios de revisión en Workfront, tal como se describe en esta sección.

  Estos perfiles afectan a los permisos solo en los permisos de Workfront Proof, no en Workfront.

* Compare dos pruebas o dos versiones de la misma prueba. Para obtener más información, consulte [Comparar pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).
* Cree un informe de aprobación de pruebas. Para obtener más información, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* Vea la fase de prueba actualmente activa en cada versión del documento en el informe Versión del documento. El nombre de la fase se muestra en la columna “Fases de prueba activas”. Si actualmente no hay ninguna fase activa en el documento, la columna está en blanco. Para obtener más información sobre los campos disponibles en vistas e informes, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
* Configure cuándo los usuarios asociados a una fase determinada pueden ver las pruebas con un flujo de trabajo automatizado. Para obtener más información, consulte [Configurar la visibilidad de la prueba en función de la actividad de la fase de flujo de trabajo](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md#configuring-proof-visibility-based-on-workflow-stage-activity) en [Configurar la configuración de uso compartido para los usuarios](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).
* Acceso sin problemas a Workfront Proof directamente desde la barra de navegación global de Workfront (no se requiere inicio de sesión adicional). Para obtener más información, consulte [Acceder a Workfront Proof desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

<!--
>[!NOTE]
>
>There are some capabilities included in Workfront Proof standalone that are not included in Proofing in Workfront. To learn more, see [Standalone Workfront Proof to Integrated Proofing in Workfront overview](../../../administration-and-setup/manage-workfront/configure-proofing/move-to-proofing-in-workfront.md)
-->
