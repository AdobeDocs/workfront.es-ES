---
title: Acceso necesario para utilizar el espacio de ideación
description: Adobe Workfront Planning ahora ofrece una capacidad adicional para idear antes de iniciar sus campañas. Aproveche la potencia de la IA para transformar datos e insumos directos en planes tangibles y proporcionar a los equipos un punto de partida informado en lugar de una página en blanco con espacio de ideación de Adobe.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---


# Acceso necesario para utilizar el espacio de ideación

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible como parte del programa **Beta** del espacio de ideación. </span>

<span class="preview">Para obtener más información, consulte [Introducción al espacio de ideación para Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


{{planning-important-intro}}

Adobe Workfront Planning ahora ofrece una capacidad adicional para idear antes de iniciar sus campañas. Aproveche la potencia de la IA para transformar datos e insumos directos en planes tangibles y proporcionar a los equipos un punto de partida informado en lugar de una página en blanco con espacio de ideación de Adobe.

Este artículo describe el acceso y los permisos que debe tener para acceder al espacio de ideación desde Workfront Planning.

Para obtener información general sobre el espacio de ideación, vea [Introducción al espacio de ideación para Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

## Requisitos del producto

El espacio de ideación no es un producto independiente. Requiere un paquete de Workfront Planning y solo se puede acceder a él desde Workfront Planning. También requiere productos adicionales.

Su organización debe adquirir un paquete para los siguientes productos para acceder al espacio de ideación:

* Un paquete de flujo de trabajo de Adobe Workfront además de un paquete de Planning

  O

  Un producto de Adobe Workfront Planning adquirido como independiente.
* Licencia de Adobe GenStudio for Performance Marketing

  >[!TIP]
  >
  >GenStudio for Performance Marketing es necesario para tener acceso a los derechos de fuente correctos.


<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Requisitos de nivel de acceso de Workfront Planning

El acceso al espacio de ideación está configurado en Workfront.

El nivel de acceso de Workfront debe incluir lo siguiente para acceder al espacio de ideación:

* Una licencia de flujo de trabajo estándar, cuando su empresa compró un paquete de flujo de trabajo además de un paquete de Planning.
* Una licencia de planificación estándar, cuando su empresa compró un flujo de trabajo y un paquete de planificación, o una licencia de planificación de Workfront como producto independiente.
* La configuración Deshabilitar espacio de ideación en la sección Establecer restricción adicional de su nivel de acceso debe estar desseleccionada. <!--***********check the UI for this***********-->

## Requisitos de permisos de Workfront Planning

Cada registro de Planning está conectado a un informe en el espacio de ideación.

Los permisos breves del espacio de ideación se heredan de los permisos de registro de Workfront Planning. <!--not sure if this is right, because now you can share the ideation with others??-->

Debe tener permisos de administración para un tipo de registro en Planning para crear registros o editar un registro en el espacio de ideación.

Los usuarios de Planning con permisos de Vista en registros pueden ver el espacio de ideación de un registro.

En la tabla siguiente se muestra la conexión entre los permisos de registros de Workfront Planning y los permisos de instrucciones del espacio de ideación:

| Permiso de nivel de registro de Planning | Permisos de nivel breve del espacio de ideación |
|---|---|
| Administración de permisos de un registro | Puede crear un resumen en el espacio de ideación del registro |
| Ver permisos de un registro | Puede leer el resumen de ese registro en el espacio de ideación, pero no puede modificarlo |

## Permisos del espacio de ideación

<!--this is also duplicated in the intro of the Share an ideation space article-->

Los permisos de Planning se transfieren al espacio de ideación de un registro.

Además, puede conceder a otros usuarios permisos para utilizar el espacio de ideación y agregarle ideas.

Tenga en cuenta lo siguiente:

* Los creadores de ideaciones siempre tienen permisos de edición en sus propias ideaciones.

* Debe tener permisos de editor en un espacio de ideación para crear informes y exportarlos a otras aplicaciones.

A continuación se indican los permisos del espacio de ideación y las capacidades que ofrecen:

| Permiso del espacio de ideación | Competencias |
|---|---|
| Editor | Puede editar, descargar y compartir el espacio de ideación |
| Comentarista | Puede ver el espacio de ideación y realizar comentarios en él |
| Visualizador | Puede ver el espacio de ideación |

Para obtener más información acerca de cómo compartir un espacio de ideas, vea [Compartir un espacio de ideas](/help/quicksilver/planning/ideation/share-the-ideation-space.md).

<!--there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
