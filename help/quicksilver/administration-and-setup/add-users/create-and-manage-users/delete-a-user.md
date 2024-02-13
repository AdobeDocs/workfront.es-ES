---
title: Eliminar usuarios
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Cuando un usuario abandona la organización, puede eliminarlo de Workfront, aunque se recomienda desactivar usuarios en lugar de eliminarlos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: b3717fc89e45983b80471fdd629c79b82086c6ff
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Eliminar usuarios

Cuando un usuario abandona la organización, puede eliminarlo de Adobe Workfront.

>[!IMPORTANT]
>
>Al eliminar a un usuario del sistema también se elimina la información asociada con el usuario que es posible que desee conservar. Se recomienda desactivar usuarios en lugar de eliminarlos. Para obtener más información, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p><b>Usuarios</b> en su nivel de acceso configurado en <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajuste la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si el usuario <b>Administrador (usuarios de grupo)</b> está habilitada, debe ser administrador de un grupo del que sea miembro el usuario.</p> <p>Para obtener más información sobre <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concesión de acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminar o desactivar un usuario

Al desactivar un usuario, suceden las siguientes cosas:

* Quita las licencias del usuario tanto a Workfront como a Workfront Proof si el componente de Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información sobre Workfront Proof, consulte [Workfront Proof: índice de artículos](../../../workfront-proof/workfront-proof.md).
* Ya no se puede asignar trabajo al usuario.
* El usuario ya no puede añadirse a las actualizaciones.
* El usuario ya no se puede agregar a equipos o grupos.
* Los objetos ya no se pueden compartir con el usuario.
* Su asociación con los siguientes objetos permanece intacta:

   * Tareas, problemas, proyectos, portafolios
   * Paneles

     >[!NOTE]
     >
     >Si desactiva un usuario y ya no puede ver los informes o paneles asociados a él, es posible que tenga que actualizar el **Ejecutar este informe con los derechos de acceso de:** field.\
     >Para obtener más información, consulte la [¿Por qué no puedo acceder a un informe propiedad de un usuario desactivado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) de la sección [Preguntas frecuentes sobre informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artículo.

   * Documentos
   * Actualizaciones
   * Horas

* Si el usuario tiene documentos desprotegidos, éstos permanecen desprotegidos cuando se desactivan. Solo un administrador de Workfront puede volver a registrarlos. Para obtener más información sobre la retirada de documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

Al eliminar un usuario, ocurren las siguientes cosas:

* Quita las licencias del usuario tanto a Workfront como a Workfront Proof, si el componente Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información sobre Workfront Proof, consulte [Workfront Proof: índice de artículos](../../../workfront-proof/workfront-proof.md).
* Ya no se puede asignar trabajo al usuario.
* El usuario ya no puede añadirse a las actualizaciones.
* El usuario ya no se puede agregar a equipos o grupos.
* Los objetos ya no se pueden compartir con el usuario.
* Elimina la asociación de ese usuario con los siguientes objetos:

   * Tareas, problemas, proyectos, portafolio
   * Paneles

     >[!NOTE]
     >
     >También pierde acceso a las secciones personalizadas que contenían paneles asociados al usuario eliminado.\
     >Para obtener más información, consulte la [¿Cómo puedo acceder a un tablero que contiene un informe propiedad de un usuario eliminado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) de la sección [Preguntas frecuentes sobre informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artículo.

   * Actualizaciones
   * Horas

     >[!NOTE]
     >
     >Estos objetos permanecen en Workfront, pero su propietario está ahora en blanco.

* Si el usuario ha cargado algún documento en el área Documentos de la barra de navegación global, los documentos también se eliminan.
* Si el usuario ha retirado los documentos que le pertenecen y los documentos se cargan en el área principal de Documentos (a la que se accede desde el menú principal), los documentos se eliminan con el usuario. Para obtener más información sobre la retirada de documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

Para obtener más información sobre la desactivación de usuarios, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Puede eliminar usuarios de forma permanente de uno en uno, o bien puede eliminar varios usuarios de forma simultánea de forma permanente. Cuando elimine usuarios individuales, debe esperar a que se complete el proceso de eliminación antes de pasar a otras actividades en Workfront. El proceso de eliminar varios usuarios se ejecuta simultáneamente como un proceso en segundo plano, por lo que puede seguir utilizando Workfront a medida que se eliminan los usuarios.

## Eliminar uno o más usuarios

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Clic **Usuarios**.
1. Seleccione al menos un usuario que desee eliminar y haga clic en el menú Más ![](assets/more-icon.png), luego haga clic en **Eliminar**.
1. En el cuadro que aparece, haga clic en **Eliminar** para confirmar la eliminación.

   El proceso de eliminación de usuarios se ejecuta como un proceso en segundo plano, por lo que puede seguir utilizando Workfront a medida que se eliminan los usuarios.

   Según el número de usuarios que esté eliminando, el proceso puede tardar varios minutos o incluso unas horas.

   Tras recibir en Workfront la confirmación de que los usuarios se han eliminado, es posible que siga viéndolos en el sistema hasta que el proceso de eliminación se complete en segundo plano.

   Posteriormente, si descubre que uno o más usuarios no se han eliminado correctamente, intente eliminarlos de uno en uno.
