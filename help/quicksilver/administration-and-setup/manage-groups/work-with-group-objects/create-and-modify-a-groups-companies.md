---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Crear y modificar las compañías de un grupo
description: Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas al grupo y a cualquiera de sus subgrupos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# Crear y modificar las compañías de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas al grupo y a cualquiera de sus subgrupos.

Si hay grupos por encima de su grupo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

+++

## Vea, trabaje con y cree compañías para su grupo desde el área Grupos

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar compañías.
1. En el panel izquierdo, haga clic en **Compañías** para enumerar las compañías asociadas con el grupo y los subgrupos que pueda tener.
1. (Opcional) Para agregar una empresa, haga clic en **Agregar empresa** y, a continuación, configure la empresa con las opciones que se indican a continuación. Cuando termine, haga clic en **Crear compañía**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sección Información básica</td> 
      <td> 
       <ul> 
        <li> <p><b>Nombre de la compañía</b>: escriba un nombre para la compañía.</p> </li> 
        <li> <p><b>Está activo</b>: cuando esta opción está habilitada, los usuarios pueden encontrar la compañía y adjuntarla a los proyectos que creen y editen. No se puede adjuntar una empresa inactiva a los proyectos. Esta opción está habilitada de forma predeterminada.</p> </li> 
        <li> <p><b>Esta es la compañía primaria</b>: asigna la compañía como compañía primaria de su organización. La compañía principal suele representar su cuenta de Workfront, donde trabaja la mayoría de los usuarios.</p> <p>Al modificar sus niveles de acceso, puede restringir el acceso de los usuarios a otros usuarios:</p> 
         <ul> 
          <li>Solo en su compañía principal</li> 
          <li> <p>En la compañía asociada y en la compañía primaria</p> <p>Para obtener información acerca de la funcionalidad principal de la compañía dentro de los niveles de acceso de los usuarios, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> <p>Sólo puede haber una o ninguna compañía designada como compañía primaria, pero no puede haber varias compañías designadas como compañía primaria. Para obtener más información, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupo</b>: si hay un grupo que hace negocios con la compañía, puede agregar el nombre del grupo aquí. Esto resulta útil para los administradores de grupos que necesitan informar y administrar todas las compañías con las que hacen negocios sus grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">El sistema rellena el campo <strong>Grupo</strong> de la nueva compañía con el grupo que está viendo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si tiene acceso administrativo a las compañías de su nivel de acceso, puede quitar el grupo de la compañía y asignar una diferente, o dejar la compañía sin un grupo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si no tiene acceso administrativo a las empresas, el campo <strong>Grupo</strong> es obligatorio y solo puede seleccionar los grupos que administra o cualquier subgrupo de esos grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Para obtener información acerca del acceso administrativo a las compañías, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder acceso administrativo a los usuarios a ciertas áreas</a>.</p> </li> 
        <li> <p><b>Miembros de la compañía</b>: Agregue usuarios existentes a la compañía. Al hacerlo, asocia estos usuarios con esta compañía.</p> <p>No hay límite en cuanto a la cantidad de usuarios que asocia con una empresa, pero un usuario no puede asociarse con más de una empresa.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Sección de Forms personalizado</td> 
      <td> <p>Si hay campos que desea agregar a su empresa y que no están disponibles en Workfront, puede crear un formulario personalizado y asociarlo a su empresa. Puede adjuntar este formulario a su empresa seleccionándolo en el menú desplegable. En el menú desplegable sólo aparecen las empresas activas. Para obtener información acerca de cómo crear formularios personalizados, vea <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Diseñar un formulario con el diseñador de formularios</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si tiene acceso administrativo a las compañías de su nivel de acceso, también puede hacer clic en Agregar más compañías en la parte inferior de la lista. Esto agrega una fila en la que puede configurar rápidamente la nueva compañía.

1. (Opcional) Para editar o eliminar empresas, seleccione al menos una empresa y, a continuación, utilice los botones de la barra de herramientas para editar ![](assets/edit-icon.png) o eliminarla ![](assets/delete.png).

   Para obtener información acerca de cómo editar una compañía, vea la sección [Crear o editar una compañía en Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) en el artículo [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Opcional) Para exportar la lista de empresas, haga clic en el icono Exportar ![](assets/export.png) y, a continuación, seleccione el formato de archivo que desee para la lista exportada.
