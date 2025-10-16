---
product-area: projects
navigation-topic: manage-tasks
title: Convertir una tarea en un proyecto
description: Cuando una tarea de un proyecto requiere un esfuerzo mayor en completarse que el planificado originalmente, puede convertirla en un proyecto.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 81%

---

# Convertir una tarea en un proyecto

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

Cuando una tarea de un proyecto requiere un esfuerzo mayor en completarse que el planificado originalmente, puede convertirla en un proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> <p>Ver o acceder a las plantillas, al convertirlas en un proyecto mediante una plantilla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración de una tarea</p> <p>Permisos de visualización de una plantilla cuando se convierte un proyecto con una plantilla</p> <p>Después de crear el proyecto, tendrá los permisos de administración del proyecto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>View or higher access to&nbsp;Templates, when converting to a project using a template</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>View permissions on a template, if converting to a project using a template</p> <p>After creating the project, you have Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Consideraciones para convertir tareas en proyectos

* Puede convertir una tarea en un proyecto en blanco o en un proyecto mediante una plantilla.
* Se elimina la tarea original.
* Todas las subtareas, problemas y notas se transfieren al nuevo proyecto.
* Los documentos, las versiones de los documentos y las pruebas se mueven al nuevo proyecto.
* Al convertir una tarea en un proyecto, existe un límite de procesamiento de 5 minutos. Si la tarea tiene un gran número de documentos adjuntos y no se puede convertir, es posible que tenga que eliminar algunos de los documentos e intentarlo de nuevo.
* Se conservan el estado y el porcentaje completado de todas las subtareas y problemas.
* Los usuarios asignados a la tarea y el usuario que convierte la tarea en el proyecto se convierten en usuarios compartidos en el proyecto.
* La fecha de inicio del proyecto se establece en la fecha de inicio de la tarea.
* En la tabla siguiente se muestra la información del proyecto y si se transfiere desde la plantilla o desde la tarea:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Descripción</td> 
    <td> <p>La descripción de la tarea se transfiere al nuevo proyecto. </p> <p> Si no hay descripción en la tarea, se transfiere al proyecto la descripción de la plantilla. </p> <p>Si el campo Descripción está vacío tanto para la tarea como para la plantilla, el campo del proyecto queda vacío. </p> </td> 
    </tr> 
    <tr> 
    <td>Estado</td> 
    <td> Estado predeterminado seleccionado para el grupo en la plantilla. Si la plantilla no está asociada al grupo, el estado del proyecto se establece en el estado predeterminado definido por el administrador de Workfront en el área de Configuración Preferencias del proyecto. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configurar las preferencias del proyecto en todo el sistema</a>

  Existen los siguientes escenarios para actualizar el estado del proyecto:
  <ul>
    <li> Si el estado de la tarea es “Nuevo”, el estado del proyecto se establecerá en “Planificando”.</li>
    <li> Si el estado de la tarea es “En curso”, el estado del proyecto se establece en “Actual”.</li>
    <li> Si el estado de la tarea es “Completado”, el estado del proyecto se establece en “Completado”.</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Prioridad</td> 
    <td>Se transfiere de la tarea al proyecto o se transfiere desde la plantilla, si se utiliza una en la conversión. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>La URL de la tarea se transfiere al nuevo proyecto. </p> <p> Si no se especifica ninguna dirección URL en la tarea, la URL de la plantilla se transfiere al proyecto. </p> <p>Si el campo de la URL está vacío tanto para el problema como para la plantilla, este queda vacío en el proyecto. </p> </td> 
    </tr> 
    <tr> 
    <td>Tipo de condición del proyecto</td> 
    <td>Se transfiere desde la plantilla.</td> 
    </tr> 
    <tr> 
    <td>Condición del proyecto</td> 
    <td>Coincide con la preferencia predeterminada del sistema, según lo que determine el administrador de Workfront en el área de Configuración. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Establecer una condición personalizada como predeterminada para los proyectos</a>
    </td> 
    </tr> 
    <tr> 
    <td>Programar desde</td> 
    <td>Se transfiere desde la plantilla.</td> 
    </tr> 
    <tr> 
    <td>Fechas del proyecto</td> 
    <td> 
      <ul> 
      <li> <p><b>Fecha de inicio planificada</b>: debe preseleccionarse el tiempo de trabajo más cercano basado en el tiempo de trabajo de programación de la plantilla, de acuerdo con la zona horaria. Este campo está desactivado si el campo de programación “Desde” está establecido como Desde la finalización. </p> </li> 
      <li> <p><b>Fecha planificada de finalización</b>: debe preseleccionarse el tiempo de trabajo más cercano basado en el tiempo de trabajo de programación de la plantilla, de acuerdo con la zona horaria. Este campo está desactivado si el campo de programación “Desde” está establecido como Desde el inicio. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portafolio</td> 
    <td>Se transfiere desde la plantilla. De lo contrario, este campo queda vacío.</td> 
    </tr> 
    <tr> 
    <td>Programa</td> 
    <td>Se transfiere desde la plantilla. De lo contrario, este campo queda vacío.</td> 
    </tr> 
    <tr> 
    <td>Grupo</td> 
    <td><p> Se dan los siguientes escenarios:</p>
      <ul><li>Si se especifica un grupo durante la conversión, este se convierte en el grupo del proyecto</li>
      <li>Si convierte a un proyecto mediante una plantilla y hay un grupo en la plantilla, y durante la conversión no especifica ningún grupo, el grupo de la plantilla se convierte en el grupo del nuevo proyecto</li>
      <li> Si no hay ningún grupo en la plantilla y no especifica ningún grupo durante la conversión, el grupo del proyecto del problema original se convierte en el grupo del nuevo proyecto</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Compañía</td>    
    <td>  Se transfiere desde la plantilla. De lo contrario, este campo queda vacío.</td>

  </tr> 
    <tr> 
    <td>Propietario del proyecto</td> 
    <td>Se transfiere desde el campo Propietario de la plantilla en esta. De lo contrario, se establece en el usuario que ha iniciado sesión y que realiza la conversión. </td> 
    </tr> 
    <tr> 
    <td>Patrocinador de proyecto</td> 
    <td>Se transfiere desde el campo Patrocinador de la plantilla en esta. De lo contrario, este campo queda vacío.</td> 
    </tr> 
    <tr> 
    <td>Gerente de recursos</td> 
    <td>Se transfiere desde la plantilla. De lo contrario, este campo queda vacío.</td> 
    </tr> 
    <tr> 
    <td>Configuración de tarea</td> 
    <td>Transferencia desde la plantilla.</td> 
    </tr> 
    <tr> 
    <td>Configuración de problema</td> 
    <td>Transferencia desde la plantilla. </td> 
    </tr> 
    <tr> 
    <td>Acceso</td> 
    <td> <p>Transferencias desde la sección Acceso en la plantilla. </p> </td> 
    </tr> 
    <tr> 
    <td>Rutas de aprobación</td> 
    <td>Transferencia desde la plantilla. Las aprobaciones asociadas con la tarea se eliminan durante la conversión. </td> 
    </tr> 
  </tbody> 
  </table>


## Convertir una tarea en un proyecto

1. Vaya a la tarea que desea convertir en proyecto.
1. Haga clic en el icono **Más** ![](assets/more-icon.png) y, a continuación, en **Convertir en un proyecto**.
1. Elija alguna de las siguientes opciones:

   * **Nuevo proyecto**, para crear un proyecto sin usar una plantilla
   * Una plantilla en la sección **Seleccionar desde plantillas**

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Haga clic en **Continuar** en la notificación que aparece.
1. En el cuadro **Convertir en proyecto**, especifique lo siguiente:

   * **Nombre**: asigne un nombre al proyecto. El nombre predeterminado es el nombre de la tarea. Este campo es obligatorio.
   * **Descripción**: describe el propósito de este proyecto.
   * (Condicional) Si ha seleccionado crear un proyecto a partir de una plantilla, actualice los campos disponibles en el cuadro **Convertir en proyecto**.

     Para obtener más información sobre cómo editar campos en proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Para actualizar los campos de la sección Finanzas del cuadro Convertir en proyecto, debe tener acceso de edición a los datos financieros en su nivel de acceso. Si tiene acceso de visualización de datos financieros en su nivel de acceso, toda la información financiera de la plantilla se transfiere al nuevo proyecto y no puede editarla mientras convierte el problema. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) y [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Opcional) Añada **Formularios personalizados** al nuevo proyecto.

     >[!TIP]
     >
     >Si un formulario personalizado de varios objetos adjunto a la tarea se ha configurado para utilizarse con tareas y proyectos, se conserva toda la información guardada en el formulario cuando realice la conversión.
     >
     >
     >Si utiliza una plantilla para la conversión y un formulario personalizado adjunto a la plantilla contiene un campo personalizado que también se encuentra en un formulario personalizado adjunto a la tarea, se utiliza el valor de campo de la tarea para el nuevo proyecto. Sin embargo, si el campo personalizado está vacío en la tarea, se utiliza el valor de la plantilla.

1. Haga clic en **Convertir en proyecto**.
