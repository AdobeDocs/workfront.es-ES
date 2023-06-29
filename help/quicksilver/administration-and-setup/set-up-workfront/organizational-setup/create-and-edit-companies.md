---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Crear y editar compañías
description: Puede agregar compañías a [!DNL Workfront] y utilizarlos para la planificación financiera, con fines de creación de informes, para definir permisos sobre objetos y para mantener la confidencialidad de la información.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# Crear y editar compañías

{{highlighted-preview}}

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Una empresa es una unidad organizativa de [!DNL Adobe Workfront] que puede representar a su organización, a un departamento dentro de la organización o a un cliente con el que trabaje. Puede agregar compañías a [!DNL Workfront] y utilizarlos para la planificación financiera, con fines de creación de informes, para definir permisos sobre objetos y para mantener la confidencialidad de la información.

## Requisitos de acceso

Debe tener lo siguiente para poder administrar compañías en [!DNL Workfront]:

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
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier compañía del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p>Acceso administrativo para gestionar empresas, que permite editar cualquier empresa del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar empresas asociadas a cualquier grupo al que esté asignado como administrador del grupo.</p> </li> 
      <li> <p>Para agregar y eliminar usuarios de la [!DNL Workfront] del sistema, debe tener uno de los siguientes:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator]. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
        <li> <p>En su nivel de acceso, [!UICONTROL Edit] debe estar seleccionado para la opción [!UICONTROL Users]. Además, para la configuración de [!UICONTROL Usuarios], en [!UICONTROL Ajustar la configuración] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Create] y al menos una de las dos opciones de [!UICONTROL User Admin] deben estar habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si utiliza la opción [!UICONTROL User Admin (Usuarios del grupo)], debe ser administrador de un grupo del que sea miembro el usuario.</p> </li> 
       </ul> <p>Para obtener información sobre la configuración Usuarios en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concesión de acceso a los usuarios</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Ventajas de agregar usuarios a una compañía {#benefits-of-adding-users-to-a-company}

* Puede crear el organigrama de una empresa asociando usuarios con informes directos. Solo los usuarios de la misma compañía pueden agregarse como informes directos de otro usuario de esa compañía.
* Como jefe de proyecto, puede identificar los recursos disponibles en la misma compañía.
* Puede mantener la información privada entre empresas eligiendo una o todas las opciones de configuración siguientes:

   * Los usuarios de la misma compañía pueden ver las solicitudes de los demás.

     Para obtener más información acerca de cómo [!DNL Workfront] Un administrador de puede otorgar un acceso similar a las solicitudes en función de la compañía de los usuarios. Consulte la sección [Configurar las preferencias de tareas y problemas para todos los usuarios en [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) en el artículo [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Para obtener más información sobre cómo un administrador de grupo puede otorgar un acceso similar a las solicitudes en función de la compañía de los usuarios, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Los usuarios solo pueden ver las colas de solicitudes asociadas a sus empresas. Para obtener más información sobre cómo restringir la visibilidad de una cola de solicitudes, consulte [Proporcionar acceso a las colas de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Puede restringir el acceso de los usuarios únicamente a los usuarios de su empresa o compañía y de la compañía principal. Para obtener información sobre la funcionalidad principal de la empresa en relación con la privacidad del usuario, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Los usuarios pueden restringir las actualizaciones que realizan en los elementos para que solo los usuarios de su compañía puedan verlos. Para obtener más información sobre cómo hacer que una actualización sea privada para una compañía, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Creación o edición de una compañía en [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

No hay límite en el número de compañías que puede agregar. Sin embargo, recomendamos que limite el número de compañías que utiliza debido a problemas que pueden producirse con los permisos de objetos; una fragmentación excesiva podría interferir con la visibilidad de los usuarios de los elementos de trabajo.

De forma predeterminada, la compañía asociada a su instancia de [!DNL Workfront] ya se ha creado en su [!DNL Workfront] y es la compañía primaria de su organización. Tiene el mismo nombre que el nombre del cliente. Para obtener más información sobre la información de sus clientes en [!DNL Workfront], consulte [Configurar la información básica del sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Para agregar o editar una compañía:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Compañías]**.
1. Si va a añadir una empresa, haga clic en **[!UICONTROL Nueva compañía]**.

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
        <li> <p><b>[!UICONTROL Nombre de la compañía]</b>: escriba un nombre para la compañía.</p> </li> 
        <li> <p><b>[!UICONTROL Está Activo]</b>: cuando esta opción está habilitada, los usuarios pueden encontrar la compañía y adjuntarla a los proyectos que crean y editan. No se puede adjuntar una empresa inactiva a los proyectos. Esta opción está habilitada de forma predeterminada.</p> </li> 
        <li> <p><b>[!UICONTROL Ésta es la compañía principal]</b>: asigna la compañía como compañía principal de la organización. La compañía principal suele representar a su [!DNL Workfront] cuenta donde trabajan la mayoría de los usuarios.</p> <p>Puede tener una compañía o ninguna compañía designada como compañía primaria, pero no puede tener varias compañías designadas como compañías primarias. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> <p><b>NOTA</b>: Al modificar sus niveles de acceso, puede restringir el acceso de los usuarios a otros usuarios: solo en su compañía principal, o en su compañía asociada y la compañía principal. Para obtener información sobre cómo funciona la compañía principal con los niveles de acceso de los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Grupo]</b>: Si hay un grupo que hace negocios con la compañía, puede agregar el nombre del grupo aquí. Esto resulta útil para los administradores de grupos que necesitan informar y administrar todas las compañías con las que hacen negocios sus grupos.</p> <p><b>IMPORTANTE</b>: Si no asocia el grupo que va a trabajar con esta compañía, los administradores del grupo no pueden acceder a a menos que tengan acceso administrativo a las compañías en su nivel de acceso. Para obtener información sobre cómo se concede este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Empiece a escribir el nombre del grupo y pulse <strong>[!UICONTROL Entrar]</strong> cuando aparezca.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Cuando asigna un grupo a una compañía, los administradores del grupo obtienen acceso a [!UICONTROL Administrar]. Para obtener más información, consulte <a href="#group-administrators-and-companies" class="MCXref xref">Administradores de grupo y empresas</a> en este artículo.</p> </li> 
        <li> <p><b>[!UICONTROL Miembros de la compañía]</b>: Añada los usuarios existentes a la compañía. Al hacerlo, asocia estos usuarios con esta compañía.</p> <p>No hay límite en cuanto a la cantidad de usuarios que asocia con una empresa, pero un usuario no puede asociarse con más de una empresa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección [!UICONTROL Tarifas de facturación]</td> 
      <td> <p><span class="preview">Esta sección se ha eliminado en el entorno de vista previa.</span></p><p>Puede anular las tarifas de facturación asociadas con sus funciones en el nivel de compañía. Para obtener información sobre la creación de funciones y su asociación con las tarifas de facturación, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar roles</a>.</p> <p>Para obtener más información sobre la anulación de tarifas de facturación en el nivel de compañía, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref">Anular las tarifas de facturación de funciones en el nivel de compañía</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección [!UICONTROL Custom Forms]</td> 
      <td> <p>Si hay campos que desea agregar a su compañía que no están disponibles en [!DNL Workfront], puede crear un formulario personalizado y asociarlo a su empresa. Puede adjuntar este formulario a su empresa seleccionándolo en el menú desplegable. En el menú desplegable sólo aparecen las empresas activas. Para obtener información sobre la creación de Forms personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Si va a crear una nueva empresa, haga clic en **[!UICONTROL Crear compañía]**.

   O

   Si está editando una empresa existente, haga clic en **[!UICONTROL Guardar cambios]**.

## Administrar suscripciones a compañías

Para obtener información sobre la administración de suscripciones para una compañía existente, consulte [Administrar suscripciones a compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Administrar tarifas de facturación

Para obtener información sobre la anulación de tarifas de facturación en el nivel de compañía, consulte [Anular las tarifas de facturación de funciones en el nivel de compañía](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Acerca del uso compartido de objetos con compañías

Algunos permisos están disponibles para los usuarios asociados a una empresa, como se explica en la sección [Ventajas de agregar usuarios a una compañía](#benefits-of-adding-users-to-a-company). Además de estos permisos, puede permitir a los usuarios permisos para ver, contribuir o editar objetos en [!DNL Workfront] compartiendo el objeto con su compañía.

En lugar de compartir un objeto con un usuario individual a la vez, puede compartirlo con toda su compañía. Cada usuario de la compañía tiene los mismos permisos en ese objeto.

Para obtener más información sobre cómo compartir objetos, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administradores de grupo y empresas {#group-administrators-and-companies}

Cuando un [!DNL Workfront] El administrador asigna un grupo a una empresa y los administradores del grupo vuelven a asignarlo [!UICONTROL Administrar] acceso a la compañía en [!UICONTROL Configurar]. Esto incluye el acceso a la [!UICONTROL Compañías] página en [!UICONTROL Configurar], donde pueden ver y gestionar la empresa asociada a su grupo.

Con este acceso a la [!UICONTROL Compañías] , un administrador de grupo puede asignar un grupo a una empresa, pero debe ser una empresa que el administrador de grupo haya creado. Si el nivel de acceso del administrador del grupo no está configurado con acceso administrativo a las empresas, la variable [!UICONTROL Grupo] Este campo es necesario cuando el administrador del grupo crea la empresa; su título en negrita indica lo siguiente:

![](assets/manage-company-group-field-req.jpg)

Para obtener información sobre cómo los usuarios obtienen acceso administrativo a las compañías en su nivel de acceso, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obtener información acerca de cómo administrar una compañía en [!UICONTROL Configurar] área, consulte [Creación o edición de una compañía en [!DNL Workfront]](#create-or-edit-a-company-in-workfront) en este artículo.
