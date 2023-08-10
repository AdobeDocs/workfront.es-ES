---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Configurar plantillas de correo electrónico
description: Como administrador de Adobe Workfront, puede configurar plantillas de correo electrónico para que admitan notificaciones de recordatorio.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: 1129f8ab93d349325bed56bc2b3ba94c2600c03f
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 1%

---

# Configurar plantillas de correo electrónico

Como administrador de Adobe Workfront, puede configurar plantillas de correo electrónico para que admitan notificaciones de recordatorio.

Las plantillas de correo electrónico contienen el mensaje enviado a los usuarios cuando se inicia una notificación de recordatorio.\
Sin una plantilla de correo electrónico, la notificación de recordatorio se envía como contenido vacío en el cuerpo del correo electrónico.

Las plantillas de correo electrónico se pueden asociar con notificaciones de recordatorio para problemas, tareas, proyectos y plantillas de horas. Al crear plantillas de correo electrónico, el administrador de Workfront puede proporcionar contenido para el correo electrónico y una línea de asunto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Administrador del sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crear una nueva plantilla de correo electrónico {#create-a-new-email-template}

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel de la izquierda, haga clic en **Correo electrónico** > **Notificaciones**> **Plantillas de correo electrónico**.

![](assets/email-templates-tab-under-setup-email-notifications-area.png)

1. Clic **Nueva plantilla de correo electrónico**.

1. En el **Nueva plantilla de correo electrónico** , especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td>Título de la plantilla de correo electrónico (obligatorio).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto</td> 
      <td>Especifique el tipo de objeto con el que desea asociar la plantilla (obligatorio; de forma predeterminada, se establecerá en Problema).</td> 
     </tr>
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Descripción de la plantilla.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Asunto </td> 
      <td>Asunto que se muestra cuando se envía el mensaje de correo electrónico (obligatorio).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuerpo </td> 
      <td> <p>Contenido mostrado cuando se envía el mensaje de correo electrónico.</p> <p>Puede utilizar el formato de HTML para el contenido del correo electrónico, tal como se describe en <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Añadir el formato de HTML a una plantilla de correo electrónico</a> en este artículo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

## Añadir el formato de HTML a una plantilla de correo electrónico {#add-html-formatting-to-an-email-template}

Puede añadir HTML a las plantillas de correo electrónico para generar notificaciones personalizadas.\
Comience a crear la plantilla de correo electrónico como se describe en [Crear una nueva plantilla de correo electrónico](#create-a-new-email-template).

El formato de HTML puede enriquecer las plantillas de correo electrónico, como se muestra en las secciones siguientes.

* [Vínculo a objetos de Workfront](#link-to-workfront-objects)
* [Vínculo a campos personalizados con HTML](#link-to-custom-fields-with-html)
* [ejemplos de correo electrónico de HTML](#html-email-examples)

### Vínculo a objetos de Workfront {#link-to-workfront-objects}

Puede incluir vínculos a campos de Workfront utilizando `$$` comodín para indicar al generador de correo electrónico que busque valores de la base de datos asociada a un objeto específico.

Por ejemplo, el cuerpo del correo electrónico de una notificación que alerta al usuario asignado de la tarea que la tarea está a punto de iniciar puede seguir esta estructura:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

Para obtener el valor &quot;comodín&quot; para un objeto, realice una de las siguientes acciones:

<!-- Refer to the API Explorer and select the names of your objects from the Fields tab of any object. For more information about the API Explorer, see [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

* Utilice el valor &quot;valuefield&quot; que encuentre dentro de una vista de modo de texto de un informe. Para obtener más información sobre los valores del modo de texto, consulte [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

  El valor &quot;heading&quot; puede ser el nombre del objeto, tal como desea que aparezca en el cuerpo del correo electrónico.

### Vínculo a campos personalizados con HTML {#link-to-custom-fields-with-html}

Puede incluir vínculos a usuarios y campos personalizados utilizando **$$** comodín para indicar al generador de correo electrónico que busque valores de la base de datos asociada al objeto. Deben estar presentes a ambos lados de la referencia de atributo de la base de datos.

Por ejemplo, si agrega el siguiente texto como HTML, agregará el nombre del usuario asignado a la notificación de recordatorio asociada con una tarea:

`assignedTo:firstName`

Para agregar campos personalizados con el mismo formato, puede agregar lo siguiente en la notificación por correo electrónico:

`DE:Custom Field As It Appears in Workfront`

Por ejemplo, se trata de una plantilla de correo electrónico que incluye una referencia a un campo personalizado denominado Fecha de entrega y se supone que el campo Fecha de entrega pertenece a una tarea.

Reemplazar `<your domain>` con el dominio Workfront de su empresa, sin los corchetes:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>Si el campo pertenece a un proyecto, reemplace la tarea por el proyecto:
>
>`DE:Project:Delivery Date`

### ejemplos de correo electrónico de HTML {#html-email-examples}

* [Notificación de recordatorio de proyecto tardío (ejemplo)](#late-project-reminder-notification-example)
* [Recordatorio de tarea o problema a punto de iniciarse (ejemplo)](#task-or-issue-about-to-start-reminder-example)

#### Notificación de recordatorio de proyecto tardío (ejemplo) {#late-project-reminder-notification-example}

Para editar una plantilla de correo electrónico para un recordatorio de proyecto tardío, tenga en cuenta esta información para los campos Asunto y Contenido.

Reemplazar `<your domain>` con el dominio Workfront de su empresa, sin los corchetes.

**Asunto:**

Un Proyecto Que Administra Se Ha Retrasado

**Contenido:**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

Esto genera un correo electrónico similar al siguiente:

![](assets/screen-shot-2016-09-16-at-3.52.54-pm-350x103.png)

#### Recordatorio de tarea o problema a punto de iniciarse {#task-or-issue-about-to-start-reminder-example}

También es posible que desee crear una notificación de recordatorio para una tarea o un problema próximo.

El siguiente código se puede incluir en una plantilla de correo electrónico para su uso para las notificaciones de recordatorio de tarea y problema que se envían cualquier número de días antes de la fecha de inicio planificada de la tarea o problema.

Reemplazar `<your domain>` con el dominio Workfront de su empresa, sin los corchetes.

Para usar esto con un correo electrónico de problema, cambie el `/task/view.` valor en el vínculo del elemento de trabajo a `/issue/view`.

**Asunto:**

`$$name$$ to start on $$plannedStartDate$$`

**Contenido:**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_sent.png](assets/email-template-delivered.png)

Una vez creada una plantilla de correo electrónico, los usuarios pueden asociarla con notificaciones de recordatorio, tal como se describe en [Configuración de notificaciones de recordatorio](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
