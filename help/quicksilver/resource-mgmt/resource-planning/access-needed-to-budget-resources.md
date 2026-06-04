---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Se necesita acceso para presupuestar recursos en Workfront
description: Consulte y administre información sobre la planificación de recursos de los proyectos a los que tenga acceso para ver si cuenta con determinada configuración de nivel de acceso y los permisos para los elementos de trabajo, usuarios, funciones y equipos.
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
TQID: https://experienceleague.adobe.com/X0g8M77au0kHvFSt6q-v0TOc9Lh3VxaHtUngvg-uoUk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d1573eb8-a2e8-4a06-9526-9c3410bf4914id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 62%

---

# Se necesita acceso para presupuestar recursos en Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Cuando una compañía adquiera una licencia de Adobe Workfront que incluya la planificación de recursos, verá la información de presupuestos de recursos de aquellos proyectos de los que tenga permisos de visualización. Consulte la información de presupuestos en el Planificador de recursos.

Para obtener información adicional acerca de los requisitos previos para el uso de las herramientas de presupuestación en Workfront, consulte [Comenzar con la planificación de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Para presupuestar recursos, administrar conjuntos de recursos y ver información de costo en las herramientas de planificación de recursos, su compañía y usted deben tener el siguiente acceso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> 
    <ul> 
     <li> <p>Edite el acceso a la administración de recursos en su nivel de acceso que incluya:</p> 
      <ul> 
       <li> <p>Acceso para editar las prioridades del proyecto y horas presupuestadas. </p> </li> 
       <li> <p>Acceso para administrar conjuntos de recursos, si necesita administrarlos.</p> </li> 
      </ul> <p>Para obtener información acerca del nivel de acceso a la Administración de recursos, consulte el artículo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Conceder acceso a la Administración de recursos</a>.</p> </li> 
     <li> <p>Acceso de edición a Proyectos y Usuarios. </p> </li> 
     <li> <p> Edite el acceso a los datos financieros en su nivel de acceso, que incluye el acceso a Ver o Editar Tasas de Coste y Ver o Editar Finanzas Generales, si necesita ver o gestionar información por Coste.</p> <p>Para obtener más información acerca del nivel de acceso a datos financieros, consulte el artículo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concesión de acceso a los datos financieros</a>.</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos en el proyecto que incluyan los permisos Editar tasas de coste y Editar finanzas generales.</p> <p>Para obtener información acerca de los permisos de los proyectos, consulte el artículo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de proyectos en Adobe Workfront</a>.</p> <p>Para obtener información acerca de los permisos financieros de un proyecto, consulte el artículo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Uso compartido de permisos financieros en un objeto</a></a>.</p>

<p><b>NOTA:</b> Al presupuestar recursos en la vista de rol, si tiene menos de Permisos de administración para al menos un proyecto enumerado en el rol, no puede presupuestar horas, ETC ni Costo para el rol. Solo será posible presupuestar aquellos proyectos para los que se tengan permisos de administración.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
