---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Añadir un usuario a una organización en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 87%

---

# Añadir un usuario a una organización o equipo en Adobe Workfront Fusion

>[!IMPORTANT]
>
>Este artículo se eliminará en un futuro próximo, ya que todas las organizaciones se trasladan a Adobe Admin Console.

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al [!DNL Adobe Admin Console]. Si su organización se ha incorporado a [!DNL Adobe Admin Console], debe realizar esta acción mediante [!DNL Adobe Admin Console].
>
>Para obtener instrucciones sobre cómo añadir un usuario después de que su organización se haya movido a [!DNL  Adobe Admin Console] y a la experiencia unificada de Adobe, consulte [Añadir usuarios a [!DNL Adobe Workfront Fusion] mediante [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).
>
>Para obtener una lista de procedimientos que difieren según si su organización ha sido incorporada a la Adobe Admin Console, consulte [Diferencias de administración basada en plataforma (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para usar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> 
     <p>Debe ser administrador de [!DNL Workfront Fusion] de su organización.</p>
     <p>Debe ser administrador de [!DNL Workfront Fusion] de su equipo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Añadir usuarios a una organización


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->
>[!NOTE]
>
>Si su organización se encuentra actualmente en el proceso de pasar a Adobe Admin Console, no puede administrar usuarios en Workfront (añadiendo o eliminando usuarios). Puede realizar estas acciones en Adobe Admin Console una vez completada la migración.

Para añadir usuarios a la organización, debe ser administrador de la organización a la que desee añadir usuarios. Para obtener información acerca de los roles, consulte [Roles de organización en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Para añadir un usuario a la organización:

1. Vaya a **[!UICONTROL Organizaciones]** en el menú y seleccione la organización a la que desee añadir un usuario.
1. Abra la pestaña **[!UICONTROL Usuarios]** en su panel.
1. Haga clic en **[!UICONTROL Invitar a un nuevo usuario]**, envíe la invitación haciendo clic en **[!UICONTROL Enviar]**.

   >[!NOTE]
   >
   >   
   >Si no ve el botón [!UICONTROL Invitar a un nuevo usuario], su organización se ha incorporado al [!DNL Adobe Business Platform.]
   >
   >  Para obtener instrucciones sobre cómo añadir un usuario a una organización que se ha incorporado a [!DNL Adobe Business Platform], consulte [Añadir usuarios a [!DNL Adobe Workfront Fusion] a través de [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

1. Rellene el formulario.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Email address]</td>
      <td>
        Introduzca la dirección de correo electrónico del usuario
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>Introduzca el nombre completo del usuario</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Role] </td>
      <td>Seleccione la función del usuario. Para obtener una explicación de las funciones, consulte <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Funciones de organización y equipo.</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Equipos</td>
      <td>Seleccione todos los equipos de los que desee que sea miembro el usuario.</td>
    </tr>
    <tr>
      <td role="rowheader">Nota</td>
      <td>Introduzca una nota para el usuario. Esta nota aparecerá en el correo electrónico de invitación del usuario.</td>
    </tr>
  </tbody>
</table>

El usuario recibe un correo electrónico de invitación en el que puede aceptar la invitación.

## Añadir un usuario a un equipo

Sus usuarios se asignan a equipos cuando usted los crea. Si es necesario añadir un usuario existente a un equipo, puede añadirlo en la página Usuarios del equipo.

La adición de un usuario a un equipo se gestiona desde la página para ese equipo.

1. Ve al equipo al que deseas añadir al usuario seleccionando **Organizaciones** en el panel de navegación izquierdo, haciendo clic en la pestaña **Equipos** en la página de la organización, y seleccionando el equipo.

   O

   Si está en la página de otro equipo, haga clic en el menú desplegable de equipo en la parte superior de la página.

1. En la página Equipo (con el nombre del equipo al principio de la página), seleccione la pestaña **Usuarios**.
1. Busque el usuario en la página. Los usuarios de su organización aparecen en esta página aunque no sean miembros del equipo.
1. Haga clic en **Ninguno** a la derecha del nombre del usuario y, a continuación, seleccione la función que desea que tengan en el equipo.

El usuario se añade al equipo.