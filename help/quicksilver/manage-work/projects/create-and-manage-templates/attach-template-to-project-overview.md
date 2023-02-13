---
content-type: overview
product-area: templates
keywords: sobrescribir,campo,sobrescrito
navigation-topic: templates-navigation-topic
title: Descripción general de cómo adjuntar una plantilla a un proyecto
description: Al adjuntar una plantilla a un proyecto existente, se modifica parte de la información del proyecto según la plantilla. Parte de la información sobre el proyecto permanece sin cambios.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 5%

---

# Descripción general de cómo adjuntar una plantilla a un proyecto

Al adjuntar una plantilla a un proyecto existente, se modifica parte de la información del proyecto según la plantilla. Parte de la información sobre el proyecto permanece sin cambios.

Para obtener información sobre cómo adjuntar una plantilla a un proyecto, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Consideraciones al agregar plantillas a proyectos

Tenga en cuenta lo siguiente al agregar plantillas a proyectos:

* Solo puede adjuntar plantillas activas a los proyectos.
* Puede adjuntar una plantilla a un proyecto cuando el proyecto esté en estado Completado, Muerto o Pendiente de aprobación, solo cuando el administrador de Adobe Workfront o un administrador de grupo hayan activado esta funcionalidad en el área Preferencias del proyecto. Para obtener información sobre cómo definir las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* A menos que se excluyan tareas de plantilla específicas de la adición en el proceso de archivo adjunto, todas las tareas de plantilla se añaden al proyecto existente.
* La mayoría de los ajustes de plantilla se agregan al proyecto. Se conservan algunos ajustes del proyecto. Para obtener más información, consulte la sección [Comprender los cambios en los campos del proyecto al adjuntar una plantilla](#understand-changes-to-project-fields-when-attaching-a-template) en este artículo.

## Comprender los cambios en los campos del proyecto al adjuntar una plantilla {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Adjuntar una plantilla a un proyecto no es lo mismo que crear un proyecto a partir de una plantilla. Cuando crea un proyecto a partir de una plantilla, todos los campos de plantilla se transfieren al nuevo proyecto. Al adjuntar una plantilla, algunos de los campos de proyecto existentes quedan sin cambiar.

Algunas configuraciones de plantilla se transfieren automáticamente al proyecto, a menos que se marque específicamente para que se excluyan durante el proceso de archivo adjunto de la plantilla. Cuando marca que se van a excluir, se conservan los valores de campo del proyecto.

Sin embargo, no todos los campos del proyecto están disponibles para su administración en el proceso de adjuntar una plantilla a un proyecto. Para obtener más información, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

En la tabla siguiente se describe el comportamiento predeterminado de lo que sucede con los campos del proyecto cuando se adjunta una plantilla y los campos que se pueden administrar durante el proceso de archivo adjunto para anular el comportamiento predeterminado:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campo</td> 
   <td>Qué sucede de forma predeterminada en el proceso de adjuntar una plantilla</td> 
   <td>Capacidad para administrar las actualizaciones de campo en el proceso de archivos adjuntos </td> 
  </tr> 
  <tr> 
   <td>Descripción</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Estado</p> </td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dirección URL</td> 
   <td>Se transfiere desde la plantilla, si el campo está vacío en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Prioridad</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de condición</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de horario</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fechas planificadas</td> 
   <td>Podría cambiar en función de las tareas añadidas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fechas reales</td> 
   <td>Podría cambiar en función de las tareas añadidas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portafolio</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programar</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compañía</td> 
   <td>Se transfiere desde la plantilla, si el campo está vacío en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Horas planificadas</td> 
   <td>Podría cambiar en función de las tareas añadidas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Propietario del proyecto</td> 
   <td>Se transfiere desde la plantilla, si el campo está vacío en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Patrocinador de proyecto</td> 
   <td>Se transfiere desde la plantilla, si el campo está vacío en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gerente de recursos</td> 
   <td>Se ha agregado a la lista de administradores de recursos existentes en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado</td> 
   <td>Se ha agregado al proyecto, además de los formularios que ya están en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Presupuesto</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Divisa</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>MIR</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>CAE</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Beneficio planificado</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Beneficio real</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruta de hitos</td> 
   <td>Se transfiere desde la plantilla, si el campo está vacío en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de finalización</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de finalización de resumen</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de actualización</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Horario</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tiempo de espera del usuario desactivado</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de nivelación de recursos</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Riesgo (campo de proyecto)</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Conjuntos de recursos</td> 
   <td>Se agregó a la lista de grupos de recursos existentes en el proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipos de horas</td> 
   <td> <p>Si se anula la selección durante el proceso de archivo adjunto, la configuración Tipos de horas del proyecto permanece sin cambios. </p> <p>Si se selecciona, la configuración de la plantilla se transfiere al proyecto. Si el filtro Tipo de hora está establecido en Sí, tanto en el proyecto como en la plantilla, los tipos de hora de la plantilla se añaden a los del proyecto.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Notificaciones de recordatorio</td> 
   <td> <p>Se ha agregado a la lista de recordatorios existentes en el proyecto. </p> <p>Si se anula la selección durante el proceso de archivo adjunto, las notificaciones de recordatorio del proyecto permanecen sin cambios. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Proceso predeterminado de aprobación de tarea</td> 
   <td>Se conserva la información del proyecto</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Forms personalizado predeterminado de tarea</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Esfuerzo de trabajo</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Permitir que los usuarios agreguen problemas en línea</span> </td> 
   <td><span>Se conserva la información del proyecto</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Todos los ajustes</td> 
   <td>La configuración de plantilla sobrescribe a las del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tareas</td> 
   <td>Se agrega al final de la lista de tareas, además de las tareas de proyecto existentes</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Se ha agregado al proyecto, además de los documentos de proyecto existentes</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Riesgos (objetos del área Riesgos del proyecto)</td> 
   <td>Se agregó al proyecto, además de los riesgos de proyecto existentes </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Proceso de aprobación</td> 
   <td>Transferido desde plantilla</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tarifas de facturación</td> 
   <td> <p>Se transfiere desde la plantilla además de las tasas de facturación existentes en el proyecto. </p> <p>Si hay una tasa diferente para la misma función de trabajo tanto en el proyecto como en la plantilla, la tasa del proyecto permanece sin cambios. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Registros de facturación</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gastos</td> 
   <td>Transferido de la plantilla además de los gastos existentes en el proyecto</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Información financiera</td> 
   <td> <p>Cuando se selecciona en el proceso de archivo adjunto, los campos siguientes se transfieren o se añaden al proyecto: </p> 
    <ul> 
     <li> <p>Costo fijo</p> <p>Cuando se selecciona la opción , el coste fijo actualizado del proyecto se calcula mediante la fórmula siguiente:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Ingresos fijos</p> <p>Cuando se selecciona la opción , los ingresos fijos del proyecto se calculan con la fórmula siguiente:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Tipo de coste en tareas</p> <p>Transferido desde plantilla</p> </li> 
     <li> <p>Tipo de ingresos en tareas</p> <p>Transferido desde plantilla</p> </li> 
    </ul> <p>Si se anula la selección de este campo durante el proceso de archivo adjunto, se produce lo siguiente:</p> 
    <ul> 
     <li> <p>Se conservan el coste fijo y los ingresos fijos del proyecto.</p> </li> 
     <li> <p>Los tipos de costo e ingresos de las tareas agregadas desde la plantilla se establecen en Sin costo y No facturable</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Horas</td> 
   <td>Se conserva la información del proyecto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Detalles de cola, Grupos de temas, Temas de cola, Reglas de enrutamiento</td> 
   <td> <p>Transferido desde plantilla</p> <p>Si selecciona la opción <strong>Configuración de problemas y propiedades de cola</strong> durante el proceso de archivo adjunto, los detalles de cola de la plantilla sobrescriben los del proyecto. En este caso, las reglas de enrutamiento, los temas de cola y los grupos de temas de la plantilla se añaden a los del proyecto. <br>Si el proyecto está configurado como cola de solicitudes y la plantilla adjunta al proyecto no está configurada como cola de solicitudes, la información de la cola del proyecto se elimina si deja el <strong>Configuración de problemas y propiedades de cola</strong> casilla marcada. <br>Si anula la selección de <strong>Propiedades de cola y configuración de problemas</strong> , se conservan todas las opciones de configuración de cola del proyecto y no se adjunta ninguna configuración de configuración de cola de la plantilla.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Restricciones de tareas</td> 
   <td> <p>Transferido desde plantilla </p> <p>Si se anula la selección durante el proceso de archivo adjunto, las restricciones de tareas se establecen en Tan pronto como sea posible o lo antes posible, según la configuración Programar desde del proyecto. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Predecesoras de la tarea</td> 
   <td> <p>Transferido desde plantilla</p> <p>Si se anula la selección durante el proceso de conexión, se eliminan todas las conexiones predecesoras entre las tareas de plantilla.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Opciones de uso compartido</td> 
   <td> <p>Si se anula la selección durante el proceso de archivo adjunto, los permisos de proyecto permanecen inalterados.</p> <p>Si se selecciona durante el proceso de archivo adjunto, los permisos de plantilla se añaden o sobrescriben a los del proyecto. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Si el usuario A tiene permiso de vista para el proyecto, pero tiene permisos de administración en la plantilla, después de adjuntar la plantilla, el usuario A obtendrá acceso de administración al proyecto.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

 

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom&nbsp;Forms</b>:&nbsp;Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start&nbsp;From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project&nbsp;Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p>&nbsp;</p>
</div>
-->

 
