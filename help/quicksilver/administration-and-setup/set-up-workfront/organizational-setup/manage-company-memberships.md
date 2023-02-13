---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Administración de suscripciones a la empresa
description: En el [!UICONTROL Compañías] en Configuración, puede agregar y quitar los miembros de una empresa. También puede editar sus perfiles de usuario, recordarles que se registren en [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Administración de suscripciones a la empresa

En el [!UICONTROL Compañías] área [!UICONTROL Configuración], puede agregar y eliminar miembros de una empresa. También puede editar sus perfiles de usuario, recordarles que se registren en [!DNL Workfront], desactívelos en [!DNL Workfront]y elimínelos de la función [!DNL Workfront] sistema.

Para obtener información sobre la creación de una nueva empresa, consulte [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

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
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong> </td> 
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

## Administración de suscripciones a la empresa

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Compañías]**.
1. Haga clic en el nombre de la empresa.
1. Con la variable **[!UICONTROL Miembros de la compañía]** seleccionada en el panel izquierdo, realice una de las acciones siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Agregar un miembro</td> 
      <td> <p>Haga clic en <b>[!UICONTROL Agregar miembro]</b>y, a continuación, seleccione una de estas opciones en el menú desplegable que muestra:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Nuevo usuario]</b>: Agregar un usuario que aún no se haya agregado a [!DNL Workfront].</p> <p>Para obtener información sobre cómo agregar usuarios a [!DNL Workfront], consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Agregar usuarios</a> y <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Agregue un usuario que ya exista en el sistema y que tenga acceso a la edición.</p> <p><b>IMPORTANTE</b>: Si el usuario ya es miembro de otra empresa, la nueva asignación anula la antigua. El usuario pierde el acceso a los elementos compartidos con la empresa anterior y obtiene acceso a los elementos compartidos con esta empresa.</p> </li> 
        <li> <p><b>[!UICONTROL Importar usuarios]</b>: Importar usuarios cargando un archivo de importación de hoja de cálculo. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importar usuarios</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar miembros</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleccione al menos un usuario y, a continuación, haga clic en el icono [!UICONTROL Editar] <img src="assets/edit-icon.png"> en la barra de herramientas.</p> </li> 
        <li value="2"> <p>Configure las opciones en la variable <b>[!UICONTROL Editar usuario]</b> que se muestra.</p> <p>Para obtener información sobre estas opciones, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar miembro</td> 
      <td> <p>Puede crear un miembro de compañía copiando uno existente. </p> <p><b>NOTA</b>:  <p>Cuando crea un usuario de esta forma, toda la información se copia del usuario original al usuario recién creado, excepto lo siguiente:</p> 
        <ul> 
         <li>La información de la sección [!UICONTROL Información personal].</li> 
         <li>[!UICONTROL Cuando inicio sesión, mostrar]: La pestaña de aterrizaje predeterminada para el nivel de acceso está seleccionada en esta casilla.</li> 
         <li>[!UICONTROL Informes directos]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Seleccione el usuario y, a continuación, haga clic en el icono [!UICONTROL Copy] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>En el <b>[!UICONTROL Nuevo usuario]</b> que se muestra, edite los campos disponibles para el nuevo usuario.</p> <p>Para obtener información sobre todos los campos asociados a un usuario, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a>.</p> </li> 
        <li value="3"> <p>Haga clic en <strong>[!UICONTROL Agregar este usuario]</strong>.</p> <p>O</p> <p>Haga clic en <strong>[!UICONTROL Agregar usuario de persona e iniciar otro]</strong> para guardar el nuevo usuario y agregar otro.</p> </li> 
       </ol> <p>Esto crea una nueva cuenta en [!DNL Workfront] para el usuario.</p> <p>Si ha seleccionado la opción para enviar una invitación al usuario, debe recibir un correo electrónico en el que pueda seguir un vínculo para crear su [!DNL Workfront] contraseña.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quitar usuarios</td> 
      <td> 
       <div> 
        <p>Seleccione al menos un usuario, haga clic en <b>[!UICONTROL Eliminar usuarios]</b>y, a continuación, seleccione una de las siguientes opciones en el menú desplegable que se muestra:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Quitar de la empresa]</b>: Quita al usuario o usuarios de la empresa.</p> </li> 
         <li> <p><b>[!UICONTROL Eliminar]</b>: Elimina al usuario o usuarios del [!DNL Workfront] sistema.</p> <p><b>IMPORTANTE</b>: Al eliminar un usuario del sistema, también se elimina la información asociada al usuario que podría querer conservar. Se recomienda desactivar los usuarios en lugar de eliminarlos. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar un comentario a los usuarios y a sus áreas de [!UICONTROL Actualizaciones]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleccione al menos un usuario y, a continuación, haga clic en el icono [!UICONTROL Comentario] <img src="assets/comment-icon.png"> en la barra de herramientas.</p> </li> 
        <li value="2"> <p>Escriba el comentario que desea enviar a los usuarios y al área [!UICONTROL Actualizaciones] de sus perfiles de usuario.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar la lista de miembros de la empresa</td> 
      <td> <p>Haga clic en el icono [!UICONTROL Export] <img src="assets/export.png"> en la barra de herramientas, seleccione el formato que desee para el archivo exportado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desactivar miembros en el sistema</td> 
      <td> <p>Seleccione al menos un usuario, haga clic en el icono [!UICONTROL Más] <img src="assets/more-icon.png"> en la barra de herramientas, seleccione <b>[!UICONTROL Desactivar]</b>.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Recordar a un usuario que se registre en el sistema</td> 
      <td> <p> En el <b>[!UICONTROL Name]</b> , <b>[!UICONTROL No registrado]</b> se muestra junto al nombre de cada usuario no registrado. Para recordar a estos usuarios que se registren en el sistema, seleccione los usuarios y haga clic en el icono [!UICONTROL Más] <img src="assets/more-icon.png"> en la barra de herramientas, seleccione <b>[!UICONTROL Recordar al usuario que se registre]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
