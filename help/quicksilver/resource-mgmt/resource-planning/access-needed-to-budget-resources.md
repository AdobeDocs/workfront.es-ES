---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Acceso necesario a los recursos del presupuesto en Workfront
description: Puede ver y administrar información sobre la planificación de recursos de los proyectos a los que tiene acceso para ver si tiene determinada configuración de nivel de acceso y los permisos para los elementos de trabajo, usuarios, roles y equipos.
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Acceso necesario a los recursos del presupuesto en Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Cuando su compañía ha adquirido una licencia de Adobe Workfront que incluye Planificación de recursos, puede ver la información de presupuesto de recursos para los proyectos para los que tiene permisos de visualización. Puede ver la información de presupuesto en el Planificador de recursos.

Para obtener información adicional acerca de los requisitos previos para usar las herramientas de presupuestación en Workfront, consulte [Introducción a la planificación de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Para presupuestar recursos, administrar conjuntos de recursos y ver información de costo en las herramientas de planificación de recursos, su compañía y usted deben tener el siguiente acceso: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> 
    <ul> 
     <li> <p>Edite el acceso a la administración de recursos en su nivel de acceso que incluya:</p> 
      <ul> 
       <li> <p>Acceso para editar prioridades de proyecto y horas presupuestadas. </p> </li> 
       <li> <p>Acceso para administrar conjuntos de recursos, si necesita administrarlos.</p> </li> 
      </ul> <p>Para obtener información acerca del nivel de acceso a Administración de recursos, vea el artículo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Conceder acceso a Administración de recursos</a>.</p> </li> 
     <li> <p>Editar el acceso a Proyectos y Usuarios. </p> </li> 
     <li> <p> Edite el acceso a los datos financieros en su nivel de acceso, si necesita ver o administrar la información por coste.</p> <p>Para obtener más información acerca del nivel de acceso a datos financieros, consulte el artículo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acceso a datos financieros</a>.</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos en el proyecto que incluyan permisos de administración de finanzas.</p> <p>Para obtener información acerca de los permisos del proyecto, vea el artículo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartir un proyecto en Adobe Workfront</a>.</p> <p>Para obtener información acerca de los permisos financieros de un proyecto, vea el artículo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartir permisos financieros en un objeto</a></a>.</p>

<p><b>NOTA</b>

Al presupuestar un recurso en la vista de función, si tiene menos de Administrar permisos para al menos un proyecto enumerado en la función, no puede presupuestar horas, ETC ni costos para la función. Solo puede presupuestar los proyectos para los que tiene permisos de Administración.</p> </td>
</tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
