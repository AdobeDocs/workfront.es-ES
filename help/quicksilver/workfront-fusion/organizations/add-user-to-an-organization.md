---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Añadir un usuario a una organización en Adobe Workfront Fusion
description: Puede añadir usuarios a organizaciones en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2884f709ef9ea89f275ff88db41ddde725dbd781
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Añadir un usuario a una organización en Adobe Workfront Fusion

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al [!DNL Adobe Admin Console]. Si su organización se ha incorporado al [!DNL Adobe Admin Console], debe realizar esta acción a través de [!DNL Adobe Admin Console].
>
>Para obtener instrucciones sobre cómo agregar un usuario a la lista[!DNL  Adobe Admin Console], consulte la sección &quot;Editar detalles del usuario&quot; en el artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) o póngase en contacto con su [!UICONTROL Adobe Admin Console] Administrador.
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
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> 
     <p>Debe ser un [!DNL Workfront Fusion] administrador de su organización.</p>
     <p>Debe ser un [!DNL Workfront Fusion] administrador de su equipo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Añadir usuarios a una organización

<p>El procedimiento para añadir un usuario a su organización de Fusion difiere en función de si su organización se ha incorporado a Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Añadir un usuario a una organización que se haya incorporado a Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Agregar un usuario a una organización que no se haya incorporado a la Consola de Adobe empresarial</a> </p> </li>
</ul>
<div>
<p><strong>Añadir un usuario a una organización que se haya incorporado a Adobe Business Platform</strong></p>
<p>Si su organización se ha incorporado a Adobe Business Platform, debe realizar esta acción a través de Adobe Admin Console.</p>
<p>Para obtener instrucciones sobre cómo agregar un usuario en Adobe Admin Console:</p>
<ul>
<li> <p>Consulte <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Creación de usuarios en Workfront con Adobe Admin Console</a></p> </li>
<li> <p>Consulte la sección "Agregar usuarios" en el artículo <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Administrar usuarios individualmente</a></p> </li>
<li> <p>Póngase en contacto con el administrador de Adobe Admin Console.</p> </li>
</ul>
<p>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Business Platform, consulte <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Agregar un usuario a una organización que no se haya incorporado a la Consola de Adobe empresarial</strong></p>

Para agregar usuarios a la organización, debe ser administrador de la organización a la que desee agregar usuarios. Para obtener información sobre las funciones, consulte [Funciones de organización en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Para añadir un usuario a la organización:

1. Vaya a **[!UICONTROL Organizaciones]** en el menú y seleccione la organización a la que desee añadir un usuario.
1. Abra el **[!UICONTROL Usuarios]** en el panel.
1. Clic **[!UICONTROL Invitar a un nuevo usuario]**, rellene el formulario (correo electrónico, mensaje, función) y envíe la invitación haciendo clic en **[!UICONTROL Enviar]**.

>[!NOTE]
>
>   
><p>Si no ve el botón [!UICONTROL Invitar a un nuevo usuario], su organización se ha incorporado al [!DNL Adobe Business Platform.] </p>
>
>   <p>Para obtener instrucciones sobre cómo agregar un usuario a una organización que se ha incorporado al [!DNL Adobe Business Platform], consulte <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Añada un usuario a una organización que se haya incorporado al [!DNL Adobe Business Platform]</a></p>

El usuario recibe un correo electrónico de invitación en el que puede aceptar la invitación.
