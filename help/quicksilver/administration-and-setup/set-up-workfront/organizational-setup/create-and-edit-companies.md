---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Crear y editar compañías
description: Puede agregar compañías a  [!DNL Adobe Workfront] y usarlas para la planificación financiera, con fines de generación de informes, para definir permisos en torno a objetos y para mantener la información confidencial.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 6fb64986260842c419c61fe386e9ccf1a0da8f14
workflow-type: tm+mt
source-wordcount: '1463'
ht-degree: 16%

---

# Crear y editar empresas

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado y se va a lanzar en un despliegue gradual en Producción.</span>

Una compañía es una unidad organizativa de [!DNL Adobe Workfront] que puede representar a su organización, a un departamento dentro de la organización o a un cliente con el que trabaje. Puede agregar compañías a [!DNL Workfront] y utilizarlas para la planificación financiera, la generación de informes, la definición de permisos sobre objetos y la confidencialidad de la información.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] paquete</p> </td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuración de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier compañía del sistema.</p> </li> 
     <li> <p>Acceso administrativo para gestionar empresas, que permite editar cualquier empresa del sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar compañías asociadas a cualquier grupo en el que esté asignado como administrador de grupos.</p> </li> 
      <li> <p>Para agregar y quitar usuarios del sistema [!DNL Workfront], debe tener uno de los siguientes elementos:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>Configuración de <b>[!UICONTROL Usuarios]</b> en su nivel de acceso configurado a <b>[!UICONTROL Editar]</b> acceso, con <b>[!UICONTROL Crear]</b> y al menos una de las dos opciones de <b>[!UICONTROL Administrador de usuario]</b> habilitadas en <b>[!UICONTROL Ajustar la configuración]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>De estas dos opciones, si <b>[!UICONTROL User Admin (Usuarios del grupo)]</b> está habilitado, debe ser administrador de un grupo del que sea miembro el usuario.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ventajas de agregar usuarios a una compañía {#benefits-of-adding-users-to-a-company}

* Puede crear el organigrama de una empresa asociando usuarios con informes directos. Solo los usuarios de la misma compañía pueden agregarse como informes directos de otro usuario de esa compañía.
* Como jefe de proyecto, puede identificar los recursos disponibles en la misma compañía.
* Puede mantener la información privada entre empresas eligiendo una o todas las opciones de configuración siguientes:

   * Los usuarios de la misma compañía pueden ver las solicitudes de los demás.

     Para obtener más información sobre cómo un administrador de [!DNL Workfront] puede conceder acceso similar a las solicitudes según la compañía de los usuarios, consulte la sección [Configurar las preferencias de tareas y problemas para todos en [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) en el artículo [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Para obtener más información sobre cómo un administrador de grupo puede conceder acceso similar a las solicitudes según la compañía de los usuarios, vea [Configurar las preferencias de tareas y problemas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Los usuarios solo pueden ver las colas de solicitudes asociadas a sus empresas. Para obtener más información sobre cómo restringir la visibilidad de una cola de solicitudes, vea [Proporcionar acceso a las colas de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Puede restringir el acceso de los usuarios únicamente a los usuarios de su empresa o compañía y de la compañía principal. Para obtener información acerca de la funcionalidad principal de la compañía con respecto a la privacidad del usuario, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Los usuarios pueden restringir las actualizaciones que realizan en los elementos para que solo los usuarios de su compañía puedan verlos. Para obtener más información acerca de cómo hacer que una actualización sea privada para una compañía, vea [Trabajo de actualización](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Crear o editar una compañía en [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

No hay límite en el número de compañías que puede agregar. Sin embargo, recomendamos que limite el número de compañías que utiliza debido a problemas que pueden producirse con los permisos de objetos; una fragmentación excesiva podría interferir con la visibilidad de los usuarios de los elementos de trabajo.

De manera predeterminada, la compañía asociada con su instancia de [!DNL Workfront] ya se ha creado en su sistema de [!DNL Workfront] y es la compañía principal de su organización. Tiene el mismo nombre que el nombre del cliente. Para obtener más información acerca de la información de sus clientes en [!DNL Workfront], vea [Configurar información básica para su sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Para agregar o editar una compañía:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Compañías]**.

   Se muestra una lista de empresas.

1. Si va a agregar una compañía, haga clic en **[!UICONTROL Nueva compañía]**.

   O

   Si estás editando una empresa existente, selecciona la empresa y luego haz clic en el icono **[!UICONTROL Editar]** ![Editar icono](assets/edit-icon.png) en la parte superior de la lista de la empresa.

1. Actualice la siguiente información en la sección **Información básica**:

   * **Nombre de la compañía** <span class="preview"> o **Nombre**</span>: escriba un nombre para la compañía.
   * **Está activo**: cuando esta opción está habilitada, los usuarios pueden encontrar la compañía y adjuntarla a los proyectos que creen y editen. No se puede adjuntar una empresa inactiva a los proyectos. Esta opción está habilitada de forma predeterminada.
   * **Esta es la compañía primaria** <span class="preview">o **Es primaria**</span>: asigna la compañía como compañía primaria de su organización. La compañía principal suele representar su cuenta de Workfront, donde trabaja la mayoría de los usuarios.

     Puede tener una compañía o ninguna compañía designada como compañía primaria, pero no puede tener varias compañías designadas como compañías primarias. Para obtener más información, consulte [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

     >[!NOTE]
     >
     >Al modificar sus niveles de acceso, puede restringir el acceso de los usuarios a otros usuarios: solo en su compañía principal, o en su compañía asociada y la compañía principal. Para obtener información acerca de cómo funciona la compañía principal con los niveles de acceso de los usuarios, vea [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   * **Grupo**: si hay un grupo que hace negocios con la compañía, puede añadir el nombre del grupo aquí. Esto resulta útil para los administradores de grupos que necesitan informar y administrar todas las compañías con las que hacen negocios sus grupos.

     Si no asocia el grupo que va a trabajar con esta compañía, los administradores del grupo no podrán acceder a la compañía a menos que tengan acceso administrativo a las compañías de su nivel de acceso. Para obtener información acerca de cómo se concede este acceso, vea [Conceder a los usuarios acceso administrativo a ciertas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Empiece a escribir el nombre del grupo y selecciónelo cuando aparezca.

     Cuando asigna un grupo a una empresa, los administradores del grupo obtienen acceso de Administración a la empresa. Para obtener más información, consulte [Administradores de grupos y empresas](#group-administrators-and-companies) en este artículo.

   * **Miembros de la empresa**: añade usuarios existentes a la compañía. Al hacerlo, asocia estos usuarios con esta compañía.

     Empiece a escribir el nombre de un usuario y, a continuación, selecciónelo cuando aparezca.

     No hay límite en la cantidad de usuarios que puedes asociar con una empresa, pero un usuario no puede estar asociado a más de una empresa.

1. Agregue o actualice formularios personalizados en la sección **Forms personalizado**.

   Si hay campos que desea agregar a su empresa y que no están disponibles en Workfront, puede crear un formulario personalizado y asociarlo a su empresa.

   Puede adjuntar este formulario a su empresa seleccionándolo en el menú desplegable. En el menú solo se muestran los formularios personalizados activos.

   >[!NOTE]
   >
   >Las funciones de formulario personalizadas avanzadas, como los campos de búsqueda externa y los campos nativos de Workfront, solo están disponibles cuando abre el registro de empresa en la página de detalles, no en el cuadro de diálogo Editar empresa. (En la lista de empresas, haga clic en el nombre de la empresa para abrir los detalles).

   Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Condicional) Si va a crear una compañía, haga clic en **[!UICONTROL Crear compañía]** <span class="preview">o en **Guardar**.</span>

   O

   Si está editando una compañía existente, haga clic en **[!UICONTROL Guardar cambios]** <span class="preview">o **Guardar**.</span>

## Administrar suscripciones a compañías

Para obtener información acerca de cómo administrar suscripciones para una compañía existente, consulte [Administrar suscripciones a compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Administrar tarifas de facturación

Para obtener información sobre cómo anular las tarifas de facturación en el nivel de compañía, consulte [Anular tarifas de facturación de rol en el nivel de compañía](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Descripción general del uso compartido de objetos con empresas

Ciertos permisos están disponibles para los usuarios asociados con una compañía, como se explica en la sección [Ventajas de agregar usuarios a una compañía](#benefits-of-adding-users-to-a-company). Además de estos permisos, puede permitir a los usuarios permisos para ver, contribuir o editar objetos en [!DNL Workfront] compartiendo el objeto con su compañía.

En lugar de compartir un objeto con un usuario individual a la vez, puede compartirlo con toda su compañía. Cada usuario de la compañía tiene los mismos permisos en ese objeto.

Para obtener más información acerca de cómo compartir objetos, vea [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administradores de grupo y empresas {#group-administrators-and-companies}

Cuando un administrador de [!DNL Workfront] asigna un grupo a una compañía, los administradores del grupo obtienen acceso de [!UICONTROL Administrar] a la compañía en [!UICONTROL Configuración]. Esto incluye acceso a la página [!UICONTROL Compañías] en [!UICONTROL Configuración], donde pueden ver y administrar la compañía asociada con su grupo.

Con este acceso a la página [!UICONTROL Compañías], un administrador de grupo puede asignar un grupo a una compañía, pero debe ser una compañía que el administrador de grupo haya creado. Si el nivel de acceso del administrador del grupo no está configurado con acceso administrativo a las compañías, el campo [!UICONTROL Grupo] es necesario cuando el administrador del grupo crea la compañía (su <span class="preview">asterisco</span> o título en negrita lo indica):

<span class="preview">Imagen de muestra en el entorno de vista previa:</span>
![Se requiere cuadro de diálogo Nueva compañía con grupo](assets/group-admin-add-company-group-required.png)

Imagen de muestra en el entorno de producción:
Se requiere ![grupo en la compañía](assets/group-admin-add-company.png)

Para obtener información sobre cómo los usuarios obtienen acceso administrativo a las compañías en su nivel de acceso, vea [Conceder acceso administrativo a los usuarios a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obtener información sobre cómo administrar una compañía en el área [!UICONTROL Configuración], consulte [Crear o editar una compañía en [!DNL Workfront]](#create-or-edit-a-company-in-workfront) en este artículo.

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
