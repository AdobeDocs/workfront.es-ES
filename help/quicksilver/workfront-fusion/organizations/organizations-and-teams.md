---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organizaciones y equipos de Adobe Workfront Fusion
description: Las funciones de organización y equipos de Adobe Workfront Fusion permiten a las empresas controlar el acceso a escenarios y otras funciones dentro de Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 9828fe3602342520ef203ac174990f0ea03f0588
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 1%

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

<p>**Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licencias</a></p>


## Organizaciones

[!DNL Workfront Fusion] los usuarios pertenecen a una organización.

* [Funciones de organización](#organization-roles)
* [Invitación de usuarios a una organización](#inviting-users-to-an-organization)
* [Cambio entre organizaciones](#switch-between-organizations)

### Funciones de organización

Un usuario tiene una de las siguientes funciones en una organización:

* **[!UICONTROL Propietario]**: el propietario tiene todos los permisos disponibles en la organización.
* **[!UICONTROL Administrador]**: la función de administrador permite a un usuario crear y administrar equipos y usuarios para la organización.
* **[!UICONTROL Miembro]**: los miembros pueden utilizar [!DNL Workfront Fusion] pero no puede realizar cambios organizativos.
* **[!UICONTROL Contable]**: una función de contador solo permite a los usuarios ver la información de licencia en el panel de organización.
* **[!UICONTROL Desarrollador de aplicaciones]**: la funcionalidad de esta función no está disponible actualmente y estará disponible en un futuro próximo. No se recomienda asignar usuarios a esta función en este momento.

### Invitación de usuarios a una organización

De forma predeterminada, un propietario de organización (o usuario autorizado) puede invitar a otra persona a unirse a su organización.

Para invitar a un usuario a unirse a una organización:

1. Clic **[!UICONTROL Cambiar detalles]** en la esquina superior derecha de la pantalla.
1. Seleccionar **[!UICONTROL Invitar a un nuevo usuario]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Rellene la dirección de correo electrónico y el nombre del usuario.
1. Seleccione una función para el usuario. Para obtener más información sobre las funciones, consulte [Funciones de organización](#organization-roles) en este documento.
1. (Opcional) Añada una nota. Esta nota aparece en el correo electrónico de invitación que recibe el usuario.
1. Haga clic en **[!UICONTROL Guardar]**.

[!DNL Fusion] envía un correo electrónico con una invitación a la organización específica y un [!UICONTROL Aceptar La Función] botón.

Cuando el destinatario hace clic en el botón, se le redirige a la página de invitación, donde puede aceptar la invitación.

La invitación caducará dentro de un día.

>[!NOTE]
>
>Si el usuario es nuevo en [!DNL Fusion], [!DNL Fusion] crea automáticamente una cuenta para ellos y envía un correo electrónico con una contraseña temporal, indicando al nuevo usuario que inicie sesión y cambie su contraseña.

### Cambio entre organizaciones

Puede formar parte de más de una organización en Fusion. Los recursos no se comparten entre organizaciones.

Puede cambiar de organización dentro de la Experiencia unificada de Adobe haciendo clic en el nombre de la organización en la esquina superior derecha y seleccionando la nueva organización en el menú desplegable. Solo las organizaciones que tengan una cuenta de Fusion aparecerán en el desplegable, aunque sea miembro de otras organizaciones en Adobe.

## Equipos

Los equipos son grupos de usuarios que comparten el acceso a recursos específicos. Estos recursos pueden incluir:

* Escenarios
* Conexiones
* Webhooks
* Claves
* Almacenes de datos
* Estructuras de datos
* Configuración de notificación de correo electrónico

>[!NOTE]
>
>Dado que los equipos controlan el acceso a los recursos, a veces resulta útil que un equipo tenga solo un miembro. Por ejemplo, los usuarios en formación pueden crear conexiones con su [!DNL Google] cuentas. Cualquier miembro del equipo también podría conectarse a la persona [!DNL Google] , por lo que en este caso es mejor que el usuario sea el único miembro de un equipo de formación.

Las organizaciones pueden tener tantos equipos como necesiten y los usuarios pueden pertenecer a uno o más equipos.

Los usuarios pueden seleccionar su equipo en la lista desplegable del panel de navegación izquierdo. Los usuarios solo ven los equipos de los que son miembros. Si se selecciona un equipo, el usuario podrá acceder a los recursos de dicho equipo.

* [Roles de equipo](#team-roles)
* [Administración de equipo](#team-management)

### Roles de equipo

Un usuario tiene una de las siguientes funciones en cada uno de sus equipos:

* **[!UICONTROL Administrador de equipo]**: además de las capacidades de los otros roles de equipo, la función Administrador permite al usuario añadir, quitar o cambiar la función de un miembro del equipo.
* **[!UICONTROL Miembro del equipo]**: la función de miembro del equipo permite a los usuarios crear y ejecutar escenarios.
* **[!UICONTROL Monitorización del equipo]**: La [!UICONTROL control] permite a los usuarios acceder a la información de ejecución de los escenarios, pero no pueden diseñarlos ni cambiar su estado &quot;Activo&quot;.
* **[!UICONTROL Operador de equipo]**: La [!UICONTROL operador] permite a los usuarios ver los datos de ejecución y cambiar el estado &quot;Activo&quot; de los escenarios.
* **[!UICONTROL Miembro restringido del equipo]**: la funcionalidad de esta función no está disponible actualmente y estará disponible en un futuro próximo. No se recomienda asignar usuarios a esta función en este momento.

Para obtener información sobre las tareas específicas disponibles para los roles de equipo, consulte[Funciones de organización y equipo](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Administración de equipo

* [Crear un equipo](#create-a-team)
* [Establecer opciones de notificación del equipo](#set-team-notification-options)

#### Crear un equipo

Los propietarios y administradores de organizaciones pueden crear equipos.

Para crear un equipo:

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Organización]**
1. Seleccione el **[!UICONTROL Equipo]** pestaña.
1. Clic **[!UICONTROL Añadir un nuevo equipo]** en la lista de equipos.
1. Introduzca un nombre para el nuevo equipo y haga clic en **Añadir**.

#### Establecer opciones de notificación del equipo

Las opciones de notificación por correo electrónico se establecen en el nivel de equipo.

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Equipo]**
1. Seleccione el **[!UICONTROL Opciones de notificación]** pestaña.
1. Habilite las notificaciones que desea que reciba el equipo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Advertencia en ejecución de escenario]'</td> 
      <td> <p>Recibir un correo electrónico cuando haya una advertencia en una ejecución de escenario</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errores en la ejecución de un escenario]</td> 
      <td>Recibir un correo electrónico cuando haya un error en la ejecución de un escenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Desactivación de escenario]</p> </td> 
      <td><p>Reciba un correo electrónico cuando se desactive un escenario.</p><p><b>Nota:</b> Se le notifica la desactivación del escenario solo cuando el escenario se ha desactivado automáticamente debido a errores. No recibe notificaciones sobre escenarios que se desactivan manualmente.</p><p>En algunos casos, un escenario puede ser desactivado por el [!DNL Workfront Fusion] equipo de ingeniería porque el escenario está causando problemas de rendimiento u otros. En estos casos, no recibe notificaciones en [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Los cambios en las opciones de notificación se guardan automáticamente

#### Cambiar entre equipos

Puede formar parte de más de un equipo en Fusion. Dado que los equipos no comparten recursos, es posible que tenga que cambiar de equipo para acceder a escenarios específicos u otros recursos.

Si su organización no está en el Adobe de la experiencia unificada, puede cambiar de equipo si hace clic en el nombre del equipo en el panel de navegación izquierdo y, a continuación, selecciona un equipo en el menú desplegable.

Si su equipo está en la Experiencia unificada de Adobe, puede seleccionar un nuevo equipo haciendo clic en el nombre del equipo en el encabezado y, a continuación, seleccionando un equipo en la lista desplegable. Esta opción está disponible en todas las páginas específicas de un equipo determinado, como una página de escenario o la página Conexiones.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->