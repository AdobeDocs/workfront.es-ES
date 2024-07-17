---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear reglas de enrutamiento
description: Las reglas de enrutamiento controlan lo que Adobe Workfront hace con los problemas cuando se envían a una cola de solicitudes. Para obtener más información sobre la creación de colas de solicitudes, vea Crear una cola de solicitudes.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Crear reglas de enrutamiento

<!-- Audited: 12/2023 -->

Las reglas de enrutamiento controlan lo que Adobe Workfront hace con los problemas cuando se envían a una cola de solicitudes. Para obtener más información sobre la creación de colas de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Las reglas de enrutamiento envían problemas a usuarios específicos o a funciones de trabajo que estén mejor equipadas para resolver el problema o la solicitud enviados. Las reglas de enrutamiento suelen estar asociadas a temas de colas, que se utilizan para controlar qué regla de enrutamiento se aplicará al problema o la solicitud.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<!--drafted - replace the table at P&P:

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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
    <p>Nuevo: estándar</p>
    <p>o</p>
    <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administración de permisos del proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una regla de enrutamiento

1. Vaya al proyecto en el que desea agregar las reglas de enrutamiento para sus solicitudes.
1. Haga clic en **Reglas de enrutamiento** en el panel izquierdo. Es posible que deba hacer clic en **Mostrar más** y luego en **Reglas de enrutamiento**.
1. Haga clic en **Nueva regla de enrutamiento** para agregar la nueva regla.
1. Introduzca la siguiente información para la regla de enrutamiento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nombre</strong> </td> 
      <td>Nombre de la regla de enrutamiento. Puede ver la regla de enrutamiento si tiene acceso para ver esta información en el proyecto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td>Añada una descripción para la regla de enrutamiento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Usuario asignado predeterminado*</strong> </td> 
      <td>Agregue un usuario activo o un rol activo a quien se deben asignar los nuevos problemas. Solo puede tener un usuario asignado predeterminado en este campo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Equipo predeterminado*</strong> </td> 
      <td>Añada un equipo activo al que se deba asignar el nuevo problema. Solo puede tener un equipo predeterminado en este campo.

   <p><b>NOTA</b></p>

   Una vez enviado el problema, puede editar sus asignaciones y asignar otros usuarios, funciones o equipos. Para obtener más información, consulte <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Asignar problemas</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ruta al proyecto</strong> </td> 
      <td>Este es el proyecto donde se agrega el problema.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Si un usuario, rol o equipo se desactivan después de asociarse con una regla de enrutamiento, las solicitudes se siguen redirigiendo a ellos. Debe realizar periódicamente un inventario de todas las reglas de enrutamiento y reemplazar las asignaciones desactivadas por las activas.

   Cuando enruta un problema a un proyecto, los usuarios con permisos sobre el problema reciben los permisos establecidos en ese proyecto. Para obtener información acerca de cómo establecer permisos en proyectos, vea [Compartir un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![Nuevo cuadro de regla de enrutamiento](assets/new-routing-rule-box.png)

1. Haga clic en **Guardar**.

   Este proceso sólo define la regla de enrutamiento. Para asegurarse de que el problema se enrute cuando se envíe a la cola de solicitudes, debe seleccionar la regla de enrutamiento en la ficha **Detalles de cola** en **Ruta predeterminada**.

   Para obtener información sobre cómo agregar una ruta predeterminada a una cola de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Si desea asociar varias reglas de enrutamiento a la cola de solicitudes, debe crear varios temas de cola y asociar cada uno de ellos con una regla de enrutamiento independiente. Para obtener más información acerca de cómo crear un tema de cola, vea [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
