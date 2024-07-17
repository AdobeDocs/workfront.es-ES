---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Administrar suscripciones a compañías
description: En el área [!UICONTROL Compañías] de Configuración, puede agregar y quitar miembros de una compañía. También puede editar sus perfiles de usuario y recordarles que se registren en  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] system.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Administrar suscripciones a compañías

En el área [!UICONTROL Empresas] de [!UICONTROL Configuración], puede agregar y quitar miembros de una empresa. También puede editar sus perfiles de usuario, recordarles que se registren en [!DNL Workfront], desactivarlos en [!DNL Workfront] y eliminarlos del sistema [!DNL Workfront].

Para obtener información acerca de cómo crear una nueva compañía, vea [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Requisitos de acceso

Debe tener lo siguiente para administrar compañías en [!DNL Workfront]:

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
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Uno de los siguientes:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier compañía del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
     <li> <p>Acceso administrativo para gestionar empresas, que permite editar cualquier empresa del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a ciertas áreas</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar empresas asociadas a cualquier grupo al que esté asignado como administrador del grupo.</p> </li> 
      <li> <p>Para agregar y quitar usuarios del sistema [!DNL Workfront], debe tener uno de los siguientes elementos:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator]. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
        <li> <p>En su nivel de acceso, [!UICONTROL Edit] debe estar seleccionado para la opción [!UICONTROL Users]. Además, para la configuración de [!UICONTROL Usuarios], en [!UICONTROL Ajustar la configuración] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Crear] y al menos una de las dos opciones de [!UICONTROL Administración de usuarios] deben estar habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si utiliza la opción [!UICONTROL User Admin (Usuarios del grupo)], debe ser administrador de un grupo del que sea miembro el usuario.</p> </li> 
       </ul> <p>Para obtener información sobre la configuración Usuarios en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Administrar suscripciones a compañías

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Compañías]**.
1. Haga clic en el nombre de la empresa.
1. Con la sección **[!UICONTROL Miembros de la compañía]** seleccionada en el panel izquierdo, realice una de las siguientes acciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Agregar un miembro</td> 
      <td> <p>Haga clic en <b>[!UICONTROL Agregar miembro]</b> y, a continuación, seleccione una de estas opciones en el menú desplegable que se muestra:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Nuevo usuario]</b>: Agregue un usuario que aún no se haya agregado a [!DNL Workfront].</p> <p>Para obtener información sobre cómo agregar usuarios a [!DNL Workfront], consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Agregar usuarios</a> y <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Añada un usuario que ya exista en el sistema y que tenga acceso para editar.</p> <p><b>IMPORTANTE</b>: si el usuario ya es miembro de otra compañía, la nueva asignación invalidará la anterior. El usuario pierde el acceso a los elementos compartidos con la compañía anterior y obtiene acceso a los elementos compartidos con esta compañía.</p> </li> 
        <li> <p><b>[!UICONTROL Importar usuarios]</b>: importe usuarios cargando un archivo de importación de hoja de cálculo. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importar usuarios</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar miembros</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleccione al menos un usuario y, a continuación, haga clic en el icono de [!UICONTROL Edit] <img src="assets/edit-icon.png"> de la barra de herramientas.</p> </li> 
        <li value="2"> <p>Configure las opciones en el cuadro <b>[!UICONTROL Editar usuario]</b> que aparece.</p> <p>Para obtener información acerca de estas opciones, vea <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar miembro</td> 
      <td> <p>Puede crear un miembro de la compañía copiando uno existente. </p> <p><b>NOTA</b>:  <p>Cuando crea un usuario de esta manera, toda la información se copia del usuario original al usuario recién creado, excepto para lo siguiente:</p> 
        <ul> 
         <li>La información de la sección [!UICONTROL Información personal].</li> 
         <li>[!UICONTROL Cuando inicio sesión, mostrar]: la ficha de aterrizaje predeterminada del nivel de acceso está seleccionada en este cuadro.</li> 
         <li>[!UICONTROL Subordinados directos]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Seleccione el usuario y, a continuación, haga clic en el icono de [!UICONTROL Copy] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>En el cuadro <b>[!UICONTROL Nuevo usuario]</b> que aparece, edite los campos disponibles para el nuevo usuario.</p> <p>Para obtener información acerca de todos los campos asociados con un usuario, vea <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</p> </li> 
        <li value="3"> <p>Haga clic en <strong>[!UICONTROL Agregar este usuario]</strong>.</p> <p>O</p> <p>Haga clic en <strong>[!UICONTROL Agregar usuario de persona e iniciar otro]</strong> para guardar el nuevo usuario y agregar otro.</p> </li> 
       </ol> <p>Esto crea una nueva cuenta en [!DNL Workfront] para el usuario.</p> <p>Si seleccionó la opción para enviar una invitación al usuario, este debería recibir un correo electrónico donde pueda seguir un vínculo para crear su contraseña de [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quitar usuarios</td> 
      <td> 
       <div> 
        <p>Seleccione al menos un usuario, haga clic en <b>[!UICONTROL Quitar usuarios]</b> y, a continuación, seleccione una de las siguientes opciones en el menú desplegable que se muestra:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Quitar de la compañía]</b>: quita el usuario o usuarios de la compañía.</p> </li> 
         <li> <p><b>[!UICONTROL Eliminar]</b>: elimina el usuario o usuarios del sistema [!DNL Workfront].</p> <p><b>IMPORTANTE</b>: al eliminar un usuario del sistema, también se elimina la información asociada con el usuario que es posible que desee conservar. Se recomienda desactivar usuarios en lugar de eliminarlos. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar un comentario a los usuarios y a sus áreas de [!UICONTROL Updates]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleccione al menos un usuario y, a continuación, haga clic en el icono de [!UICONTROL Comment] <img src="assets/comment-icon.png"> de la barra de herramientas.</p> </li> 
        <li value="2"> <p>Escriba el comentario que desea enviar a los usuarios y al área de [!UICONTROL Updates] de sus perfiles de usuario.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar la lista de miembros de la empresa</td> 
      <td> <p>Haga clic en el icono [!UICONTROL Export] <img src="assets/export.png"> de la barra de herramientas y, a continuación, seleccione el formato que desee para el archivo exportado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desactivar miembros en el sistema</td> 
      <td> <p>Seleccione al menos un usuario, haga clic en el icono [!UICONTROL Más] <img src="assets/more-icon.png"> de la barra de herramientas y, a continuación, seleccione <b>[!UICONTROL Desactivar]</b>.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Recordar a un usuario registrarse en el sistema</td> 
      <td> <p> En la columna <b>[!UICONTROL Name]</b>, <b>[!UICONTROL No registrado]</b> aparece junto al nombre de cada usuario no registrado. Para recordar a estos usuarios que se registren en el sistema, selecciónelos, haga clic en el icono [!UICONTROL Más] <img src="assets/more-icon.png"> de la barra de herramientas y, a continuación, seleccione <b>[!UICONTROL Recordar al usuario que se registre]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
