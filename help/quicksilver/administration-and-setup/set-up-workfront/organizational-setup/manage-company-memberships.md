---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Administrar suscripciones a compañías
description: En el área [!UICONTROL Compañías] de Configuración, puede agregar y quitar miembros de una compañía. También puede editar sus perfiles de usuario y recordarles que se registren en  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] system.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 705fc990f2d90ff2102233fc68947fdbe1eb6946
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 31%

---

# Administrar suscripciones a compañías

En el área [!UICONTROL Empresas] de [!UICONTROL Configuración], puede agregar y quitar miembros de una empresa. También puede editar sus perfiles de usuario, recordarles que se registren en [!DNL Workfront], desactivarlos en [!DNL Workfront] y eliminarlos del sistema [!DNL Workfront].

Para obtener información acerca de cómo crear una nueva compañía, vea [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td><p>Actual: [!UICONTROL Equipo] o superior</p>
   <p>O</p>
   <p>Nuevo: cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licencia</p> </td> 
   <td><p>Actual: [!UICONTROL Plan]</p>
   <p>O</p>
   <p>Nuevo: [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong> </td> 
   <td> <p>Uno de los siguientes:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier compañía del sistema.</p> </li> 
     <li> <p>Acceso administrativo para gestionar empresas, que permite editar cualquier empresa del sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar compañías asociadas a cualquier grupo en el que esté asignado como administrador de grupos.</p> </li> 
      <li> <p>Para añadir y quitar usuarios del sistema [!DNL Workfront], debe tener uno de los siguientes niveles de acceso:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator].</p> </li> 
        <li> <p>En su nivel de acceso, [!UICONTROL Edit] debe estar seleccionado para la configuración [!UICONTROL Users]. Además, para la configuración de [!UICONTROL Users], en [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png">, la opción [!UICONTROL Create] y al menos una de las dos opciones de [!UICONTROL User Admin] deben estar habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si utiliza la opción [!UICONTROL User Admin (Group Users)], debe ser administrador de un grupo del que sea miembro el usuario.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Administrar suscripciones a compañías

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Compañías]**.
1. Haga clic en el nombre de la empresa.
1. Haga clic en **[!UICONTROL Miembros de la compañía]** en el panel izquierdo.
1. Realice una de las siguientes acciones:

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
        <li value="2"> <p>Configure las opciones en el cuadro <b>[!UICONTROL Editar usuario]</b> que aparece.</p> <p>Para obtener más información acerca de estas opciones, vea <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar miembro</td> 
      <td> <p>Puede crear un miembro de la compañía copiando uno existente. </p> <p><b>NOTA</b>:  <p>Cuando crea un usuario de esta manera, toda la información se copia del usuario original al usuario recién creado, excepto para los siguientes casos:</p> 
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
         <li> <p><b>[!UICONTROL Eliminar]</b>: elimina el usuario o usuarios del sistema [!DNL Workfront].</p> <p><b>IMPORTANTE</b>: al eliminar un usuario del sistema, también se elimina la información asociada con el usuario que es posible que desee conservar. Se recomienda desactivar a los usuarios en lugar de eliminarlos. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar un comentario a los usuarios y a sus áreas de [!UICONTROL Updates]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleccione al menos un usuario y luego haga clic en <b>Enviar actualización al usuario</b> en la barra de herramientas.</p> </li> 
        <li value="2"> <p>Escriba el comentario que desea enviar a los usuarios y al área de [!UICONTROL Updates] de sus perfiles de usuario.</p>
         <p>Para obtener más información, vea <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Enviar mensajes directos a otros usuarios</a>.</p></li> 
       </ol>
      </td> 
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
