---
title: Acceso necesario para utilizar el espacio de ideación
description: Adobe Workfront Planning ahora ofrece una capacidad adicional para idear antes de iniciar sus campañas. Aproveche la potencia de la IA para transformar datos e insumos directos en planes tangibles y proporcionar a los equipos un punto de partida informado en lugar de una página en blanco con espacio de ideación de Adobe.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 82ebe4df89bd9db39629b36c31c0ae2a4e133838
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 1%
---

# Acceso necesario para utilizar el espacio de ideación

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible como parte del programa **Beta** del espacio de ideación. </span>

<span class="preview">Para obtener más información, consulte [Introducción al espacio de ideación para Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


>[!IMPORTANT]
>
>La información de este artículo hace referencia a la funcionalidad disponible solo para clientes de Workfront que también tienen Adobe Workfront Planning. Su empresa debe adquirir un paquete de Planning adicional.
>
>La funcionalidad que se describe aquí no está disponible si su organización ha adquirido Workfront Planning como producto independiente.
>
>Para obtener información general sobre Workfront Planning, consulte [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

Adobe Workfront Planning ahora ofrece una capacidad adicional para idear antes de iniciar sus campañas.

Al utilizar el espacio de ideas en Workfront, puede aprovechar las capacidades de conversación de Adobe Enterprise CX Coworker en Workfront para transformar datos y dirigir entradas en planes tangibles y proporcionar a los equipos un punto de partida informado en lugar de una página en blanco.

Este artículo describe el acceso y los permisos que debe tener para acceder al espacio de ideación desde Workfront Planning.

Para obtener información general sobre el espacio de ideación, vea [Introducción al espacio de ideación para Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

## Requisitos del producto

<!--section duplicated here: help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md-->

>[!NOTE]
>
>No necesita un inicio de sesión independiente para acceder al espacio de ideación. Está disponible de inmediato si puede iniciar sesión en Workfront cuando también tiene Workfront Planning.
>
>Para obtener más información sobre el acceso necesario para usar el espacio de ideación, consulte [Acceso necesario para usar el espacio de ideación](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md).

Puede acceder al espacio de ideación si su organización y usted tienen acceso a lo siguiente:

* Proveedores de nube:

  * Amazon Web Service (AWS)

    Los proveedores de Azure y GCP no son compatibles con el espacio de ideación.

* Productos:

  * Adobe Workfront con Workfront Planning
  * CX Enterprise Coworker en Workfront

    >[!IMPORTANT]
    >
    >CX Enterprise Coworker no está disponible actualmente para organizaciones de atención médica, finanzas u otros sectores con datos confidenciales. El asistente de IA está disponible para estas organizaciones, pero el espacio de ideación no está disponible para los clientes de Workfront que no tienen Compañero de trabajo.

* Paquetes de Adobe: <!--Et wanted the Coworker added to these-->

  * Durante la versión de Open Beta (a partir del 12 de noviembre de 2026), debe tener lo siguiente:

    * Un paquete de flujo de trabajo de Adobe Workfront con un paquete de Workfront Planning con Adobe CX Enterprise Coworker activado

  * Después del lanzamiento de Disponibilidad general (previsto para el 1 de febrero de 2027), puede tener una de las siguientes opciones:

    * Un paquete de flujo de trabajo de Adobe Workfront con un paquete de Workfront Planning
    * Adobe Workfront Planning como producto independiente

    Ambos paquetes deben tener Adobe CX Enterprise Coworker activado




<!--
No longer the case: 

Your organization must purchase a package for the following products to access the Ideation space: 

* An Adobe Workfront Workflow package in addition to a Planning package

    Or
    
    An Adobe Workfront Planning purchased as a standalone product. 
* An Adobe GenStudio for Performance Marketing license

    >[!TIP]
    >
    >GenStudio for Performance Marketing is needed to have access to the correct font entitlements. 

-->

<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Requisitos del sistema y nivel de acceso

El acceso al espacio de ideación se configura en Workfront activando una combinación de ajustes de nivel de sistema y de nivel de acceso.

Se requiere la siguiente configuración para acceder al espacio de ideación en Workfront:

* Active la configuración de preferencias de Compañero de trabajo y MCP en el área Preferencias del sistema de la Configuración <!--check the UI because Becky was going to change it-->

  Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

  >[!IMPORTANT]
  >
  >CX Enterprise Coworker no está disponible actualmente para organizaciones de atención médica, finanzas u otros sectores con datos confidenciales.
  >
  >Estas organizaciones disponen de un asistente de IA.
  >
  >El espacio de ideación no está disponible para los clientes de Workfront que no tienen Coworker, pero que pueden tener un asistente de IA.

* Anule la selección de la siguiente configuración en la sección Establecer restricciones adicionales del nivel de acceso de un usuario:

  * Desactive el panel CX Coworker en Workfront
  * Deshabilitar espacio de ideación

    >[!TIP]
    >
    >Como administrador de Workfront, puede limitar el acceso al espacio de ideación a determinados usuarios desmarcando la configuración Deshabilitar espacio de ideación en su nivel de acceso.
    >
    > Los administradores del sistema siempre tienen acceso al espacio de ideación.
    >
    >Para obtener más información, vea [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).



## Requisitos de licencia

El nivel de acceso de Workfront debe incluir los siguientes tipos de licencia para acceder al espacio de ideación:

* Una licencia de flujo de trabajo estándar, cuando su empresa compró un paquete de flujo de trabajo además de un paquete de Planning.
* Una licencia de planificación estándar, cuando su empresa compró una de las siguientes opciones:

  * Un flujo de trabajo y un paquete de Planning, durante la versión beta abierta
  * Un flujo de trabajo y un paquete de Planning o Workfront Planning como producto independiente, después de la disponibilidad general.

## Requisitos de permisos de Workfront Planning

Cuando se utiliza el espacio de ideación de Workfront Planning, cada registro de Planning se conecta a un resumen en el espacio de ideación.

Los permisos breves del espacio de ideación se heredan de los permisos de registro de Workfront Planning.

Debe tener permisos de contribución o superiores para un tipo de registro en Planning para crear registros o editar un registro en el espacio de ideación.

Los usuarios de Planning con permisos de Vista en registros pueden ver el espacio de ideación de un registro.

En la tabla siguiente se muestra la conexión entre los permisos de registros de Workfront Planning y los permisos de instrucciones del espacio de ideación:

| Permiso de nivel de registro de Planning | Permisos de nivel breve del espacio de ideación |
|---|---|
| Aportar o permisos superiores a un registro | Puede crear un resumen en el espacio de ideación del registro |
| Ver permisos de un registro | Puede leer el resumen del registro en el espacio de ideación, pero no puede modificarlo |

También puede compartir un lienzo de ideación con otros usuarios. Para obtener más información, consulte la siguiente sección en este artículo.

## Permisos del espacio de ideación

<!--this is also duplicated in the intro of the Share an ideation space article-->

Los permisos de Planning se transfieren al espacio de ideación de un registro.

Además, puede conceder a otros usuarios permisos para utilizar el espacio de ideación y agregarle ideas.

Tenga en cuenta lo siguiente:

* Los creadores de informes de ideación siempre tienen permisos de editor en sus propios informes.

* Debe tener permisos de editor en un espacio de ideación para crear informes y exportarlos a Planning o a un archivo.

A continuación se indican los permisos del espacio de ideación y las capacidades que ofrecen:

| Permiso del espacio de ideación | Competencias |
|---|---|
| Editor | Puede editar, descargar y compartir un espacio de ideación |
| Comentarista | Puede ver y comentar un espacio de ideación |
| Visualizador | Puede ver un espacio de ideación |

Para obtener más información acerca de cómo compartir un espacio de ideas, vea [Compartir un espacio de ideas](/help/quicksilver/planning/ideation/share-the-ideation-space.md).

<!--
there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users
-->


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
