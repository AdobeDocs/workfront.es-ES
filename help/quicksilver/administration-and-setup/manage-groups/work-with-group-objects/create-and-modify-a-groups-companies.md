---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Crear y modificar las empresas de un grupo
description: Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas con el grupo y con cualquiera de sus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Crear y modificar las empresas de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas con el grupo y con cualquiera de sus subgrupos.

Si hay algún grupo por encima de su grupo, sus administradores también pueden hacer esto por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Ver, trabajar con y crear empresas para su grupo desde el área Grupos

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar empresas.
1. En el panel izquierdo, haga clic en **Compañías** para enumerar las empresas asociadas con el grupo y los subgrupos que pueda tener.
1. (Opcional) Para agregar una empresa, haga clic en **Agregar empresa** y, a continuación, configure la empresa utilizando las opciones que se enumeran a continuación. Cuando haya terminado, haga clic en **Crear empresa**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sección Información básica</td> 
      <td> 
       <ul> 
        <li> <p><b>Nombre de la empresa</b>: Escriba un nombre para la empresa.</p> </li> 
        <li> <p><b>Está activo</b>: Cuando esta opción está habilitada, los usuarios pueden encontrar la empresa y adjuntarla a los proyectos que creen y editen. Una empresa inactiva no se puede adjuntar a los proyectos. Esta opción está activada de forma predeterminada.</p> </li> 
        <li> <p><b>Esta es la empresa principal</b>: Asigna a la empresa como la empresa principal de su organización. La empresa principal suele representar la cuenta de Workfront donde trabaja la mayoría de los usuarios.</p> <p>Al modificar sus niveles de acceso, puede restringir el acceso de los usuarios a otros usuarios:</p> 
         <ul> 
          <li>Solo en su empresa principal</li> 
          <li> <p>En su empresa asociada y en la empresa principal</p> <p>Para obtener información sobre la funcionalidad principal de la empresa dentro de los niveles de acceso de los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> <p>Solo se puede designar una empresa o ninguna como empresa principal, pero no se pueden designar varias empresas como empresas principales. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupo</b>: Si hay un grupo que realiza negocios con la empresa, puede agregar el nombre del grupo aquí. Esto resulta útil para los administradores de grupos que necesitan informar y administrar todas las empresas con las que sus grupos hacen negocios.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">El sistema rellena el <strong>Grupo</strong> para la nueva empresa con el grupo que está viendo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si tiene acceso administrativo a empresas en su nivel de acceso, puede quitar el grupo de la empresa y asignarlo a otro, o dejar la empresa sin un grupo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si no tiene acceso administrativo a las empresas, la variable <strong>Grupo</strong> es obligatorio y solo puede seleccionar los grupos que administra o cualquier subgrupo debajo de esos grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Para obtener información sobre el acceso administrativo a las empresas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </li> 
        <li> <p><b>Miembros de la compañía</b>: Agregue usuarios existentes a la empresa. Al hacerlo, asocia a estos usuarios con esta empresa.</p> <p>No hay límite en cuanto a la cantidad de usuarios que asocia con una empresa, pero un usuario no puede asociarse con más de una empresa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección Tasas de Facturación</td> 
      <td> <p>Puede anular las tasas de facturación asociadas con las funciones de su trabajo a nivel de empresa. Para obtener información sobre cómo crear funciones de trabajo y asociarlas a tasas de facturación, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">Crear y administrar funciones de trabajo</a>.</p> <p>Para obtener más información sobre cómo anular las tasas de facturación a nivel de empresa, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">Anular las tasas de facturación de funciones de trabajo a nivel de empresa</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección Forms personalizada</td> 
      <td> <p>Si hay campos que desea agregar a su empresa que no están disponibles en Workfront, puede crear un formulario personalizado y asociarlo a su empresa. Puede adjuntar este formulario a su empresa seleccionándolo en el menú desplegable. En el menú desplegable solo se muestran las empresas activas. Para obtener información sobre la creación de Forms personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Crear o editar un formulario personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si tiene acceso administrativo a empresas en su nivel de acceso, también puede hacer clic en Agregar más empresas en la parte inferior de la lista. Esto agrega una fila donde puede configurar rápidamente la nueva empresa.

1. (Opcional) Para editar o eliminar empresas, seleccione al menos una empresa y, a continuación, utilice los botones de la barra de herramientas para editar ![](assets/edit-icon.png) o eliminar ![](assets/delete.png) es así.

   Para obtener información sobre la edición de una empresa, consulte la sección [Crear o editar una empresa en Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) en el artículo [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Opcional) Para exportar la lista de empresas, haga clic en el icono Exportar ![](assets/export.png)y, a continuación, seleccione el formato de archivo que desee para la lista exportada.
