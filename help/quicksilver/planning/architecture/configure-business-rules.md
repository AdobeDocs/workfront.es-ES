---
title: Configurar reglas de negocio de tipo de registro
description: Puede configurar reglas empresariales de tipo de registro que definan cómo se administran los registros de ese tipo en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 85c9f757134bc84e4b5038e4001f9a9fe1430f2a
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 13%

---


# Configurar reglas empresariales de tipo de registro

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Puede configurar reglas de negocio para los tipos de registros de Adobe Workfront Planning que definen cómo se administran los registros de ese tipo.

Puede permitir las siguientes acciones en los registros si se cumplen las reglas de negocio definidas:

* Edición de un registro
* Eliminación de un registro

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para realizar los pasos de este artículo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p></li>
O
<li><p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar de planificación</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo y en un tipo de registro</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al configurar reglas empresariales

* Puede configurar reglas que indiquen cuándo se pueden editar o eliminar los registros.

  Por ejemplo, puede crear condiciones para requerir que ciertos campos tengan un valor. Si falta el valor en esos campos, los usuarios no pueden editar ni eliminar ese registro.
* No se pueden agregar reglas de negocio a los tipos de registro global en sus espacios de trabajo primarios o secundarios.
* No se pueden configurar reglas para cuándo se crean los registros. Todas las personas con permisos de administración en el tipo de registro pueden crear registros.
* Puede crear una condición para la regla de negocio que haga referencia a todos los tipos de campo excepto a los siguientes:
  * Campos de fórmula
  * Campos de búsqueda
  * Campos de referencia

## Configurar reglas empresariales

1. Vaya a un tipo de registro.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Reglas de negocio**.

   Se abre la página Reglas de negocio.
1. Haga clic en **Nueva regla empresarial**.
1. En el cuadro Nueva regla de negocio, agregue un nombre para la regla de negocio en el primer campo disponible. Este campo es obligatorio
1. (Opcional) Añada una descripción para definir la regla de negocio.

<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today.
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.



### Before you start

A couple of things need to be true before you can configure rules:

1. **The feature has to be turned on for your organization.** This is done on Adobe's side (via a feature flag), not something you enable yourself. If you don't see the business rules section described below, check with your Adobe contact to confirm it's been enabled for your tenant.
2. **You need admin or workspace-configurator permissions.** Regular planners can't create or edit rules — only people managing the workspace setup can.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.



### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->