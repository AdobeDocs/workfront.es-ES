---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organizaciones y equipos de Adobe Workfront Fusion
description: Las funciones Organización y equipos de Adobe Workfront Fusion permiten a las empresas controlar el acceso a escenarios y otras funciones dentro de Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] organizaciones y equipos

[!DNL Adobe Workfront Fusion]Las funciones de organización y equipos de permiten a las empresas controlar el acceso a escenarios y otras funciones dentro de Fusion.

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
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>Workfront Fusion para automatización e integración del trabajo,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> 
     <p>Debe ser [!DNL Workfront Fusion] administrador de su organización.</p>
     <p>Debe ser [!DNL Workfront Fusion] administrador de su equipo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

<p>**Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licencias</a></p>


## Organizaciones

[!DNL Workfront Fusion] los usuarios pertenecen a una organización. Su [!DNL Fusion] licencia determina cuántos escenarios y conectores activos hay disponibles en su organización.

[!DNL Fusion] las licencias determinan el número de escenarios activos y aplicaciones activas disponibles para una organización. [!DNL Fusion] muestra el recuento actual de &quot;Situaciones activas&quot; y &quot;Aplicaciones activas&quot; en el panel de organización.

* [Funciones de organización](#organization-roles)
* [Invitación de usuarios a una organización](#inviting-users-to-an-organization)

### Funciones de organización

Un usuario tiene una de las siguientes funciones en una organización:

* **[!UICONTROL Propietario]**: El propietario tiene todos los permisos disponibles en la organización.
* **[!UICONTROL Administrador]**: La función de administrador permite a un usuario crear y administrar equipos y usuarios para la organización.
* **[!UICONTROL Miembro]**: Los miembros pueden utilizar [!DNL Workfront Fusion] pero no se pueden realizar cambios organizativos.
* **[!UICONTROL Contador]**: Una función de contable solo permite a los usuarios ver la información de licencia en el panel de organización.
* **[!UICONTROL Desarrollador de aplicaciones]**: Actualmente, la funcionalidad de esta función no está disponible y estará disponible próximamente. No se recomienda asignar usuarios a esta función en este momento.

### Invitación de usuarios a una organización

De forma predeterminada, el propietario de una organización (o el usuario autorizado) puede invitar a otra persona a unirse a su organización.

Para invitar a un usuario a unirse a una organización:

1. Haga clic en **[!UICONTROL Detalles del cambio]** en la esquina superior derecha de la pantalla.
1. Select **[!UICONTROL Invitar a un nuevo usuario]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Rellene la dirección de correo electrónico y el nombre del usuario.
1. Seleccione una función para el usuario. Para obtener más información sobre las funciones, consulte [Funciones de organización](#organization-roles) en este documento.
1. (Opcional) Agregue una nota. Esta nota aparece en el correo electrónico de invitación que recibe el usuario.
1. Haga clic en **[!UICONTROL Guardar]**.

[!DNL Fusion] envía un correo electrónico con una invitación a la organización específica y un [!UICONTROL Aceptar La Función] botón.

![](assets/accept-the-role.png)

Cuando el destinatario hace clic en el botón , se redirige a la página de invitación, donde puede aceptar la invitación.

La invitación caducará en un día.

>[!NOTE]
>
>Si el usuario es nuevo en [!DNL Fusion], [!DNL Fusion] crea automáticamente una cuenta para ellos y envía un correo electrónico con una contraseña temporal, que indica al nuevo usuario que inicie sesión y cambie su contraseña.

## Equipos

Los equipos son grupos de usuarios que comparten acceso a recursos específicos. Estos recursos pueden incluir:

* Escenarios
* Conexiones
* Enlaces web
* Claves
* Almacenes de datos
* Estructuras de datos
* Configuración de notificaciones por correo electrónico

>[!NOTE]
>
>Dado que los equipos controlan el acceso a los recursos, a veces resulta útil que un equipo tenga un solo miembro. Por ejemplo, los usuarios formados pueden crear conexiones con su individuo [!DNL Google] cuentas. Cualquier miembro del equipo también podría conectarse al individuo [!DNL Google] por lo tanto, en este caso es mejor que el usuario sea el único miembro de un equipo de formación.

Las organizaciones pueden tener tantos equipos como necesiten y los usuarios pueden pertenecer a uno o más equipos.

Los usuarios pueden seleccionar su equipo en la lista desplegable del panel de navegación izquierdo. Los usuarios solo ven equipos de los que son miembros. La selección de un equipo permitirá que un usuario acceda a los recursos de dicho equipo.

* [Funciones de equipo](#team-roles)
* [Administración de equipos](#team-management)

### Funciones de equipo

Un usuario tiene una de las siguientes funciones en cada uno de sus equipos:

* **[!UICONTROL Administrador del equipo]**: Además de las funciones de las demás funciones de equipo, la función de administrador permite al usuario añadir, quitar o cambiar la función de un miembro del equipo.
* **[!UICONTROL Miembro del equipo]**: La función de miembro del equipo permite a los usuarios crear y ejecutar escenarios.
* **[!UICONTROL Monitorización del equipo]**: La variable [!UICONTROL monitorización] permite a los usuarios acceder a la información de ejecución de los escenarios, pero no pueden diseñar escenarios ni cambiar su estado &quot;Activo&quot;.
* **[!UICONTROL Operador de equipo]**: La variable [!UICONTROL operador] permite a los usuarios ver los datos de ejecución y cambiar el estado &quot;Activo&quot; de los escenarios.
* **[!UICONTROL Miembro restringido de equipo]**: Actualmente, la funcionalidad de esta función no está disponible y estará disponible próximamente. No se recomienda asignar usuarios a esta función en este momento.

### Administración de equipos

* [Crear un equipo](#create-a-team)
* [Definir opciones de notificación de equipo](#set-team-notification-options)

#### Crear un equipo

Los propietarios y administradores de la organización pueden crear equipos.

Para crear un equipo:

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Organización]**
1. Seleccione el **[!UICONTROL Equipo]** pestaña .
1. Haga clic en **[!UICONTROL Agregar un nuevo equipo]** en la lista de equipos.
1. Escriba un nombre para el nuevo equipo y haga clic en **Agregar**.

#### Definir opciones de notificación de equipo

Las opciones de notificación por correo electrónico se establecen en el nivel de equipo.

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Equipo]**
1. Seleccione el **[!UICONTROL Opciones de notificación]** pestaña .
1. Active las notificaciones que desee que reciba el equipo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Advertencia en ejecución de escenario]'</td> 
      <td> <p>Recibir un correo electrónico cuando haya una advertencia en una ejecución de escenario</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errores en la ejecución del escenario]</td> 
      <td>Reciba un correo electrónico cuando haya un error en una ejecución de escenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Desactivación del escenario]</p> </td> 
      <td><p>Reciba un correo electrónico cuando se desactive un escenario.</p><p><b>Nota:</b> Solo se le notifica sobre la desactivación del escenario cuando este se ha desactivado automáticamente debido a errores. No recibe notificaciones sobre escenarios que se desactivan manualmente.</p><p>En algunos casos, un escenario podría ser desactivado por el [!DNL Workfront Fusion] equipo de ingeniería porque el escenario está causando problemas de rendimiento u otros. En estos casos, no recibe notificaciones en [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Cambios en las opciones de notificación guardar automáticamente

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->