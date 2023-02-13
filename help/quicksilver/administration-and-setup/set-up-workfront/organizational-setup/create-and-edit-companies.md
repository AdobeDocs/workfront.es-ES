---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Crear y editar empresas
description: Puede agregar empresas a [!DNL Workfront] y usarlos para la planificación financiera, con fines de informes, para definir permisos alrededor de los objetos y para mantener la confidencialidad de la información.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Crear y editar empresas

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Una empresa es una unidad organizativa de [!DNL Adobe Workfront] que puede representar a su organización, a un departamento de la organización o a un cliente con el que trabaje. Puede agregar empresas a [!DNL Workfront] y usarlos para la planificación financiera, con fines de informes, para definir permisos alrededor de los objetos y para mantener la confidencialidad de la información.

## Requisitos de acceso

Debe tener lo siguiente para administrar empresas en [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
   <td>[!UICONTROL Team] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Uno de los siguientes:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier empresa del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p>Acceso administrativo para administrar empresas, que le permite editar cualquier empresa del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar empresas asociadas con cualquier grupo al que tenga asignado como administrador de grupo.</p> </li> 
      <li> <p>Para agregar y eliminar usuarios de la [!DNL Workfront] sistema, debe tener una de las siguientes opciones:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator]. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
        <li> <p>En el nivel de acceso, debe seleccionar [!UICONTROL Edit] para la configuración [!UICONTROL Users]. Además, para la configuración [!UICONTROL Usuarios], en [!UICONTROL Ajuste la configuración] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Crear] y al menos una de las dos opciones [!UICONTROL User Admin] deben estar activadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si utiliza la opción [!UICONTROL User Admin (Group Users)], debe ser administrador de grupo de un grupo del que sea miembro el usuario.</p> </li> 
       </ul> <p>Para obtener información sobre la configuración Usuarios en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Ventajas de agregar usuarios a una empresa {#benefits-of-adding-users-to-a-company}

* Puede crear un organigrama de la empresa asociando a los usuarios con informes directos. Solo los usuarios de la misma empresa pueden agregarse como informes directos de otro usuario de esa empresa.
* Como administrador de proyectos, puede identificar los recursos disponibles dentro de la misma empresa.
* Puede mantener la información privada entre empresas eligiendo una o todas las configuraciones siguientes:

   * Los usuarios de la misma empresa pueden ver las solicitudes de los demás.

      Para obtener más información sobre cómo [!DNL Workfront] El administrador puede dar un acceso similar a las solicitudes basadas en la empresa de los usuarios; consulte la sección [Configure las preferencias de tareas y problemas para todos en [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) en el artículo [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

      Para obtener más información sobre cómo un administrador de grupo puede proporcionar un acceso similar a las solicitudes basadas en la empresa de los usuarios, consulte [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Los usuarios solo pueden ver colas de solicitud asociadas a sus empresas. Para obtener más información sobre la restricción de la visibilidad de una cola de solicitudes, consulte [Proporcionar acceso a colas de solicitud](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Puede restringir el acceso de los usuarios solo a los usuarios de su empresa o empresa y de la empresa principal. Para obtener información sobre la funcionalidad principal de la empresa con respecto a la privacidad del usuario, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Los usuarios pueden restringir las actualizaciones que realizan en los elementos para que solo los usuarios de su empresa puedan verlos. Para obtener más información sobre cómo convertir una actualización en privada para una empresa, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Cree o edite una empresa en [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

No hay límite en el número de empresas que puede agregar. Sin embargo, recomendamos que limite el número de empresas que utiliza debido a problemas que pueden producirse con los permisos de objetos; demasiada fragmentación podría interferir con la visibilidad de los usuarios de los elementos de trabajo.

De forma predeterminada, la empresa asociada a su instancia de [!DNL Workfront] ya se ha creado en su [!DNL Workfront] y es la empresa principal de su organización. Tiene el mismo nombre que su nombre de cliente. Para obtener más información sobre su cliente, consulte [!DNL Workfront], consulte [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Para agregar o editar una empresa:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Compañías]**.
1. Si está agregando una empresa, haga clic en **[!UICONTROL Empresa nueva]**.

   O

   Si está editando una empresa existente, seleccione la empresa y haga clic en **[!UICONTROL Editar]**.

1. Utilice las opciones que se muestran para configurar la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sección [!UICONTROL Información básica]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Escriba un nombre para la empresa.</p> </li> 
        <li> <p><b>[!UICONTROL Está Activo]</b>: Cuando esta opción está habilitada, los usuarios pueden encontrar la empresa y adjuntarla a los proyectos que creen y editen. Una empresa inactiva no se puede adjuntar a los proyectos. Esta opción está activada de forma predeterminada.</p> </li> 
        <li> <p><b>[!UICONTROL Esta es la empresa principal]</b>: Asigna a la empresa como la empresa principal de su organización. La empresa principal suele representar su [!DNL Workfront] cuenta donde trabaja la mayoría de los usuarios.</p> <p>Puede tener una empresa o ninguna empresa designada como empresa principal, pero no puede tener varias empresas designadas como empresas principales. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> <p><b>NOTA</b>: Al modificar sus niveles de acceso, puede restringir el acceso de los usuarios a otros usuarios: solo en su empresa principal, o en su empresa asociada y en la empresa principal. Para obtener información sobre cómo funciona la empresa principal con los niveles de acceso de los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Si hay un grupo que realiza negocios con la empresa, puede agregar el nombre del grupo aquí. Esto resulta útil para los administradores de grupos que necesitan informar y administrar todas las empresas con las que sus grupos hacen negocios.</p> <p><b>IMPORTANTE</b>: Si no asocia el grupo que trabajará con esta empresa, los administradores del grupo no podrán acceder a a menos que tengan acceso administrativo a empresas en su nivel de acceso. Para obtener información sobre cómo se concede este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Empiece a escribir el nombre del grupo y, a continuación, pulse <strong>[!UICONTROL Enter]</strong> cuando aparezca.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Cuando asigna un grupo a una empresa, los administradores del grupo obtienen acceso a la empresa a través de [!UICONTROL Administrar]. Para obtener más información, consulte <a href="#group-administrators-and-companies" class="MCXref xref">Administradores de grupos y empresas</a> en este artículo.</p> </li> 
        <li> <p><b>[!UICONTROL Miembros de la compañía]</b>: Agregue usuarios existentes a la empresa. Al hacerlo, asocia a estos usuarios con esta empresa.</p> <p>No hay límite en cuanto a la cantidad de usuarios que asocia con una empresa, pero un usuario no puede asociarse con más de una empresa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección [!UICONTROL Tasas de facturación]</td> 
      <td> <p>Puede anular las tasas de facturación asociadas con las funciones de su trabajo a nivel de empresa. Para obtener información sobre cómo crear funciones de trabajo y asociarlas a tasas de facturación, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> <p>Para obtener más información sobre cómo anular las tasas de facturación a nivel de empresa, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref">Anular las tasas de facturación de funciones de trabajo a nivel de empresa</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección [!UICONTROL Forms personalizado]</td> 
      <td> <p>Si hay campos que desea agregar a su empresa que no están disponibles en [!DNL Workfront], puede crear un formulario personalizado y asociarlo a su empresa. Puede adjuntar este formulario a su empresa seleccionándolo en el menú desplegable. En el menú desplegable solo se muestran las empresas activas. Para obtener información sobre la creación de Forms personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Si está creando una nueva empresa, haga clic en **[!UICONTROL Crear empresa]**.

   O

   Si está editando una empresa existente, haga clic en **[!UICONTROL Guardar cambios]**.

## Administración de suscripciones a la empresa

Para obtener información sobre la administración de suscripciones de una empresa existente, consulte [Administración de suscripciones a la empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Acerca del uso compartido de objetos con empresas

Algunos permisos están disponibles para los usuarios asociados a una empresa, como se explica en la sección [Ventajas de agregar usuarios a una empresa](#benefits-of-adding-users-to-a-company). Además de estos permisos, puede permitir a los usuarios permisos para ver, contribuir o editar objetos en [!DNL Workfront] compartiendo el objeto con su empresa.

En lugar de compartir un objeto con un usuario individual a la vez, puede compartirlo con toda su empresa. Cada usuario de la empresa tiene los mismos permisos sobre ese objeto.

Para obtener más información sobre cómo compartir objetos, consulte [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administradores de grupos y empresas {#group-administrators-and-companies}

Cuando [!DNL Workfront] administrador asigna un grupo a una empresa, los administradores del grupo ganan [!UICONTROL Administrar] acceso a la empresa en [!UICONTROL Configuración]. Esto incluye el acceso a la variable [!UICONTROL Compañías] en [!UICONTROL Configuración], donde pueden ver y administrar la empresa asociada a su grupo.

Con este acceso a la variable [!UICONTROL Compañías] , un administrador de grupo puede asignar un grupo a una empresa, pero debe ser una empresa que el administrador del grupo haya creado. Si el nivel de acceso del administrador del grupo no está configurado con acceso administrativo a las empresas, la variable [!UICONTROL Grupo] es obligatorio cuando el administrador del grupo crea la empresa; su título en negrita indica lo siguiente:

![](assets/manage-company-group-field-req.jpg)

Para obtener información sobre cómo los usuarios obtienen acceso administrativo a las empresas en su nivel de acceso, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obtener información sobre la administración de una empresa en la variable [!UICONTROL Configuración] área, consulte [Cree o edite una empresa en [!DNL Workfront]](#create-or-edit-a-company-in-workfront) en este artículo.
