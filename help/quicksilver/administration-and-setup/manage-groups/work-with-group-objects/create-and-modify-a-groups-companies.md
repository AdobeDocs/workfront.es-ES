---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Crear y modificar las compañías de un grupo
description: Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas al grupo y a cualquiera de sus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: ab7877c048ea87180dd518c978b258d266e0f95c
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 0%

---

# Crear y modificar las compañías de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas al grupo y a cualquiera de sus subgrupos.

Si hay grupos por encima de su grupo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

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

## Vea, trabaje con y cree compañías para su grupo desde el área Grupos

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar compañías.
1. En el panel izquierdo, haga clic en **Compañías** para enumerar las empresas asociadas con el grupo y los subgrupos que pueda tener.
1. (Opcional) Para agregar una empresa, haga clic en **Agregar compañía**, luego configure la compañía utilizando las opciones enumeradas a continuación. Cuando haya terminado, haga clic en **Crear compañía**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sección Información básica</td> 
      <td> 
       <ul> 
        <li> <p><b>Nombre de empresa</b>: escriba un nombre para la compañía.</p> </li> 
        <li> <p><b>Está activo</b>: cuando esta opción está habilitada, los usuarios pueden encontrar la compañía y adjuntarla a los proyectos que crean y editan. No se puede adjuntar una empresa inactiva a los proyectos. Esta opción está habilitada de forma predeterminada.</p> </li> 
        <li> <p><b>Esta es la compañía primaria</b>: asigna la compañía como compañía principal de la organización. La compañía principal suele representar su cuenta de Workfront, donde trabaja la mayoría de los usuarios.</p> <p>Al modificar sus niveles de acceso, puede restringir el acceso de los usuarios a otros usuarios:</p> 
         <ul> 
          <li>Solo en su compañía principal</li> 
          <li> <p>En la compañía asociada y en la compañía primaria</p> <p>Para obtener información sobre la funcionalidad principal de la empresa en los niveles de acceso de los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> <p>Sólo puede haber una o ninguna compañía designada como compañía primaria, pero no puede haber varias compañías designadas como compañía primaria. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupo</b>: Si hay un grupo que hace negocios con la compañía, puede agregar el nombre del grupo aquí. Esto resulta útil para los administradores de grupos que necesitan informar y administrar todas las compañías con las que hacen negocios sus grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">El sistema rellena el <strong>Grupo</strong> para la nueva empresa con el grupo que está viendo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si tiene acceso administrativo a las compañías de su nivel de acceso, puede quitar el grupo de la compañía y asignar una diferente, o dejar la compañía sin un grupo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si no tiene acceso administrativo a las empresas, la variable <strong>Grupo</strong> es obligatorio y solo puede seleccionar los grupos que administra o cualquier subgrupo bajo esos grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Para obtener información sobre el acceso administrativo a las empresas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </li> 
        <li> <p><b>Miembros de empresa</b>: Añada los usuarios existentes a la compañía. Al hacerlo, asocia estos usuarios con esta compañía.</p> <p>No hay límite en cuanto a la cantidad de usuarios que asocia con una empresa, pero un usuario no puede asociarse con más de una empresa.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Sección de Forms personalizado</td> 
      <td> <p>Si hay campos que desea agregar a su empresa y que no están disponibles en Workfront, puede crear un formulario personalizado y asociarlo a su empresa. Puede adjuntar este formulario a su empresa seleccionándolo en el menú desplegable. En el menú desplegable sólo aparecen las empresas activas. Para obtener información sobre la creación de Forms personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Crear o editar un formulario personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si tiene acceso administrativo a las compañías de su nivel de acceso, también puede hacer clic en Agregar más compañías en la parte inferior de la lista. Esto agrega una fila en la que puede configurar rápidamente la nueva compañía.

1. (Opcional) Para editar o eliminar empresas, seleccione al menos una empresa y, a continuación, utilice los botones de la barra de herramientas para editar ![](assets/edit-icon.png) o eliminar ![](assets/delete.png) it.

   Para obtener información sobre cómo editar una empresa, consulte la sección [Crear o editar una empresa en Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) en el artículo [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Opcional) Para exportar la lista de empresas, haga clic en el icono Exportar ![](assets/export.png), luego seleccione el formato de archivo que desee para la lista exportada.
