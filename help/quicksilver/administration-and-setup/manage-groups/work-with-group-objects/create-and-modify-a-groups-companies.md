---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Crear y modificar las compañías de un grupo
description: Cuando visualice un grupo que gestiona en el área de Grupos, puede ver y trabajar con las empresas asociadas al grupo y a cualquiera de sus subgrupos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 88%

---

# Crear y modificar las empresas de un grupo

Cuando visualice un grupo que gestiona en el área de Grupos, puede ver y trabajar con las empresas asociadas al grupo y a cualquiera de sus subgrupos.

Si hay grupos por encima del suyo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td>
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vea, trabaje con y cree compañías para su grupo desde el área Grupos

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar compañías.
1. En el panel de navegación izquierdo, haz clic en **Empresas** para listar las empresas asociadas al grupo y a cualquier subgrupo que pueda tener.
1. (Opcional) Para añadir una empresa, haga clic en **Añadir empresa** y, a continuación, configure la empresa con las opciones que se indican a continuación. Cuando termine, haga clic en **Crear compañía**.

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
          <li> <p>En la compañía asociada y en la compañía primaria</p> <p>Para obtener información sobre la funcionalidad de empresa principal dentro de los niveles de acceso de los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> <p>Solamente puede haber una o ninguna compañía designada como compañía primaria, pero no puede haber varias compañías designadas como compañía primaria. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupo</b>: si hay un grupo que hace negocios con la compañía, puede añadir el nombre del grupo aquí. Esto resulta útil para los administradores de grupos que necesitan informar y administrar todas las compañías con las que hacen negocios sus grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">El sistema rellena el campo <strong>Grupo</strong> de la nueva compañía con el grupo que está viendo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si tiene acceso administrativo a las empresas en tu nivel de acceso, puede eliminar el grupo de la empresa y asignar uno diferente, o dejar la empresa sin un grupo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si no tienes acceso administrativo a las empresas, el campo <strong>Grupo</strong> es obligatorio y solo puedes seleccionar los grupos que gestionas o cualquier subgrupo bajo esos grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Para obtener información acerca del acceso administrativo a las compañías, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </li> 
        <li> <p><b>Miembros de la empresa</b>: añade usuarios existentes a la compañía. Al hacerlo, asocia estos usuarios con esta compañía.</p> <p>No hay límite en la cantidad de usuarios que puedes asociar con una empresa, pero un usuario no puede estar asociado a más de una empresa.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Información general sobre formularios personalizados</td> 
      <td> <p>Si hay campos que deseas añadir a tu empresa y no están disponibles en Workfront, puede crear un formulario personalizado y asociarlo a tu empresa. Puede adjuntar este formulario a su empresa seleccionándolo en el menú desplegable. En el menú desplegable solamente aparecen las empresas activas. Para obtener información sobre cómo crear formularios personalizados, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Crear un formulario personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si tiene acceso administrativo a las empresas en tu nivel de acceso, también puede hacer clic en Añadir Más Empresas en la parte inferior de la lista. Esto añade una fila donde puede configurar rápidamente la nueva empresa.

1. (Opcional) Para editar o eliminar empresas, selecciona al menos una y, a continuación, usa los botones de la barra de herramientas para editar el ![icono Editar](assets/edit-icon.png) o eliminar el ![icono Eliminar](assets/delete.png).

   Para obtener información sobre cómo editar una empresa, consulte la sección [Crear o editar una empresa en Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) en el artículo [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Opcional) Para exportar la lista de empresas, haga clic en el icono Exportar ![Icono Exportar](assets/export.png) y, a continuación, seleccione el formato de archivo que desee para la lista exportada.
