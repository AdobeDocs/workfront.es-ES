---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear temas de cola
description: Los temas de cola funcionan junto con las reglas de enrutamiento para asignar automáticamente el trabajo entrante a un usuario, función de trabajo, equipo o para colocarlo en un proyecto. Los temas de cola definen las condiciones que deben darse para implementar la regla de enrutamiento.
author: Alina
feature: Work Management
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# Crear temas de cola

Los temas de cola funcionan junto con las reglas de enrutamiento para asignar automáticamente el trabajo entrante a un usuario, función de trabajo, equipo o para colocarlo en un proyecto. Los temas de cola definen las condiciones que deben darse para implementar la regla de enrutamiento.

No hay límite en el número de temas de cola que se pueden asignar a un grupo de temas o a un proyecto. Los temas de cola son un tipo de objeto que se puede informar.

## Requisitos de acceso

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administrar permisos para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront

## Crear un tema de cola

1. Cree una regla de enrutamiento, un grupo de temas y un formulario personalizado si desea asociarlos al tema de cola.\
   Para obtener más información sobre cómo crear reglas de enrutamiento, grupos de temas o formularios personalizados, consulte los siguientes artículos:

   * [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. Vaya al proyecto que eligió habilitar como cola de solicitud de ayuda y donde desea crear un nuevo tema de cola.\
   Para obtener más información sobre cómo designar un proyecto como cola de solicitud de ayuda, consulte el siguiente artículo:\
   [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

   Puede organizar los temas de cola relacionados en un grupo de temas o directamente en el proyecto designado como cola de solicitud de ayuda. Esto proporcionará al solicitante una serie de menús desplegables al realizar una solicitud.\
   Puede anidar los temas de cola directamente en el proyecto designado como cola de solicitud de ayuda, sin un grupo de temas.

   Para obtener información sobre la creación de grupos de temas, consulte [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Haga clic en **Temas de cola** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**, luego **Temas de cola**.
1. Haga clic en **Nuevo tema de cola**.
1. En el **Nuevo tema de cola** especifique lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nombre</strong> </td> 
      <td> Nombre del tema de cola.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td>Describir la cola de solicitud. La descripción se muestra cuando los usuarios seleccionan el tema de la cola en el proceso de envío de una nueva solicitud. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Agregar a grupo de temas</strong> </td> 
      <td> Si no hay grupos de temas en el proyecto, el nombre del proyecto se establecerá de forma predeterminada como grupo de temas.<br>Si desea crear grupos de temas adicionales desde aquí, seleccione <strong>Crear nuevo grupo de temas</strong> en el menú desplegable.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_Within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formularios personalizados</strong> </td> 
      <td>Seleccione los formularios personalizados que desee asociar con el tema de la cola. Debe crear formularios personalizados para los problemas antes de poder asociarlos a temas de cola. Para obtener información sobre la creación de formularios personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprobación predeterminada</td> 
      <td> <p>Asocie un proceso de aprobación a este tema de cola. En este menú desplegable solo están visibles los procesos de aprobación de problemas. Todos los problemas enviados a esta cola se asociarán con este proceso de aprobación. El administrador de Adobe Workfront debe definir los procesos de aprobación a nivel de sistema para poder asociarlos a los temas de la cola. <span>Un usuario con acceso administrativo a procesos de aprobación también puede crear procesos de aprobación específicos del grupo.</span> Para obtener más información sobre la creación de procesos de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creación de un proceso de aprobación para elementos de trabajo</a>.<br></p> 
       <div> 
        <p>Importante: Si el grupo del proyecto cambia, el proceso de aprobación específico del grupo asociado a problemas existentes se convierte en un proceso de aprobación de un solo uso. Para obtener más información sobre cómo los cambios en el grupo del proyecto o en el proceso de aprobación afectan a la configuración de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Efecto de los cambios en el grupo y el proceso de aprobación en los procesos de aprobación asignados</a>.</p> 
        <p>Tenga en cuenta lo siguiente al agregar procesos de aprobación a temas de cola: </p> 
        <ul style="list-style-type: circle;"> 
         <li>En la lista solo se muestran los procesos de aprobación activos. </li> 
         <li> <p>En la lista se muestran los procesos de aprobación de todo el sistema y de grupos específicos. Un proceso de aprobación asociado a un grupo que no sea el del proyecto no se muestra en la lista.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Duración predeterminada</strong> </td> 
      <td>Esta es la duración predeterminada de la solicitud y la Fecha de finalización planeada de la solicitud se calcula en función de este valor.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ruta predeterminada</strong> </td> 
      <td>Especifique la regla de enrutamiento que desea asociar con el tema de cola. Debe crear la regla de enrutamiento para poder adjuntarla a un tema de cola.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipos de solicitud</strong> </td> 
      <td> <p>Elija qué tipo de solicitudes almacena este tema de cola. Las opciones visibles se establecen en la variable <strong>Detalles de cola</strong> del proyecto. Este campo es obligatorio. </p> <p>Nota: Los tipos de solicitud se muestran como una selección en el área Solicitudes solo si el tipo de solicitud está seleccionado en las páginas Detalles de la cola y Tema de la cola. Para obtener información sobre la configuración del área Detalles de cola de un proyecto, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a>. </p> <p>Seleccione entre los siguientes tipos:</p> 
       <ul> 
        <li>Informe de errores</li> 
        <li>Solicitud de cambio</li> 
        <li>Problema</li> 
        <li>Solicitud</li> 
       </ul> <p>Es posible que el administrador de Workfront haya cambiado el nombre de algunas de estas opciones. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-queue-topic-box-nwe-350x375.png)

1.  
1. Haga clic en **Guardar**.\
   El tema de cola ya está disponible para su uso y se puede ver en el área Solicitudes de Workfront, después de seleccionar una cola de solicitud y un grupo de temas.
