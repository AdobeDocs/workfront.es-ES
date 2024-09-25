---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Añadir un usuario a una organización en Adobe Workfront Fusion
description: Puede añadir usuarios a organizaciones en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 5cdc438c6757d438b2c09796cf77e59dc19c45d9
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# Añadir un usuario a una organización o equipo en Adobe Workfront Fusion

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al [!DNL Adobe Admin Console]. Si su organización se ha incorporado a [!DNL Adobe Admin Console], debe realizar esta acción mediante [!DNL Adobe Admin Console].
>
>Para obtener instrucciones sobre cómo agregar un usuario después de que su organización se haya movido a [!DNL  Adobe Admin Console] y a la experiencia unificada de Adobe, consulte [Agregar usuarios a [!DNL Adobe Workfront Fusion] mediante [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

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
    <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> 
     <p>Debe ser administrador de [!DNL Workfront Fusion] para su organización.</p>
     <p>Debe ser administrador de [!DNL Workfront Fusion] para su equipo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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

Para agregar usuarios a la organización, debe ser administrador de la organización a la que desee agregar usuarios. Para obtener información acerca de los roles, vea [Roles de organización en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Para añadir un usuario a la organización:

1. Vaya a **[!UICONTROL Organizaciones]** en el menú y seleccione la organización a la que desee agregar un usuario.
1. Abra la ficha **[!UICONTROL Usuarios]** en su panel.
1. Haz clic en **[!UICONTROL Invitar a un nuevo usuario]**. Y envía la invitación haciendo clic en **[!UICONTROL Enviar]**.

   >[!NOTE]
   >
   >   
   >Si no ve el botón [!UICONTROL Invitar a un nuevo usuario], su organización se ha incorporado al [!DNL Adobe Business Platform.]
   >
   >  Para obtener instrucciones sobre cómo agregar un usuario a una organización que se ha incorporado a [!DNL Adobe Business Platform], consulte [Agregar usuarios a [!DNL Adobe Workfront Fusion] a través de [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

1. Rellene el formulario.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Dirección de correo electrónico]</td>
      <td>
        Introduzca la dirección de correo electrónico del usuario
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>
        <p>Introduzca el nombre completo del usuario</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Función] </td>
      <td>Seleccione la función del usuario. Para obtener una explicación de las funciones, vea <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Funciones de organización y equipo.</a></p>
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

Los usuarios se asignan a equipos cuando se crean. Si es necesario añadir un usuario existente a un equipo, puede añadirlo en la página Usuarios del equipo.

La adición de un usuario a un equipo se gestiona desde la página para ese equipo.

1. Vaya al equipo al que desee agregar al usuario seleccionando **Organizaciones** en el panel izquierdo, haciendo clic en la ficha **Equipos** de la página de la organización y seleccionando el equipo.

   O

   Si está en la página de otro equipo, haga clic en el menú desplegable de equipo en la parte superior de la página.

1. En la página Equipo (con el nombre del equipo al principio de la página), seleccione la ficha **Usuarios**.
1. Busque el usuario en la página. Los usuarios de su organización aparecen en esta página aunque no sean miembros del equipo.
1. Haga clic en **Ninguno** a la derecha del nombre del usuario y, a continuación, seleccione la función que desea que tengan en el equipo.

El usuario se añade al equipo.