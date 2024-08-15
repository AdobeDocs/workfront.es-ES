---
title: Eliminar usuarios
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Cuando un usuario abandona la organización, puede eliminarlo de Workfront, aunque se recomienda desactivar usuarios en lugar de eliminarlos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: f18bf59202ba524173774a0215f4071bd6e77432
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 1%

---

# Eliminar usuarios

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica solo a las organizaciones que aún no se han incorporado a Adobe Business Platform. Si se le ha incorporado a Adobe Business Platform, debe eliminar usuarios en Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Business Platform, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

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

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
     <li> <p>El nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Editar</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si el usuario <b>Admin (usuarios del grupo)</b> está habilitado, debe ser administrador de un grupo del que el usuario sea miembro.</p> <p>Para obtener más información sobre la configuración de <b>Usuarios</b> en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Eliminar o desactivar un usuario

Al desactivar un usuario, suceden las siguientes cosas:

* Quita las licencias del usuario tanto a Workfront como a Workfront Proof si el componente de Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información acerca de Workfront Proof, vea [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
* Ya no se puede asignar trabajo al usuario.
* El usuario ya no puede añadirse a las actualizaciones.
* El usuario ya no se puede agregar a equipos o grupos.
* Los objetos ya no se pueden compartir con el usuario.
* Su asociación con los siguientes objetos permanece intacta:

   * Tareas, problemas, proyectos, portafolios
   * Paneles

     >[!NOTE]
     >
     >Si desactiva un usuario y ya no puede ver los informes o tableros asociados con un usuario, es posible que tenga que actualizar el campo **Ejecutar este informe con los derechos de acceso de:**.\
     >Para obtener más información, consulte [¿Por qué no puedo acceder a un informe propiedad de un usuario desactivado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) sección del artículo [Preguntas más frecuentes sobre informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Documentos
   * Actualizaciones
   * Horas

* Si el usuario tiene documentos desprotegidos, éstos permanecen desprotegidos cuando se desactivan. Solo un administrador de Workfront puede volver a registrarlos. Para obtener más información acerca de cómo desproteger documentos, vea [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

Al eliminar un usuario, ocurren las siguientes cosas:

* Quita las licencias del usuario tanto a Workfront como a Workfront Proof, si el componente de Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información acerca de Workfront Proof, vea [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
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
     >Para obtener más información, consulte [¿Cómo puedo acceder a un tablero que contiene un informe propiedad de un usuario eliminado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) sección del artículo [Preguntas más frecuentes sobre informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Actualizaciones
   * Horas

     >[!NOTE]
     >
     >Estos objetos permanecen en Workfront, pero su propietario está ahora en blanco.

* Si el usuario ha cargado algún documento en el área Documentos de la barra de navegación global, los documentos también se eliminan.
* Si el usuario ha retirado los documentos que le pertenecen y los documentos se cargan en el área principal de Documentos (a la que se accede desde el menú principal), los documentos se eliminan con el usuario. Para obtener más información acerca de cómo desproteger documentos, vea [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

Para obtener más información sobre cómo desactivar usuarios, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Puede eliminar usuarios de forma permanente de uno en uno, o bien puede eliminar varios usuarios de forma simultánea de forma permanente. Cuando elimine usuarios individuales, debe esperar a que se complete el proceso de eliminación antes de pasar a otras actividades en Workfront. El proceso de eliminar varios usuarios se ejecuta simultáneamente como un proceso en segundo plano, por lo que puede seguir utilizando Workfront a medida que se eliminan los usuarios.

## Eliminar uno o más usuarios

{{step-1-to-users}}

1. Seleccione al menos un usuario que desee eliminar, haga clic en el menú Más ![](assets/more-icon.png) y luego haga clic en **Eliminar**.
1. En el cuadro que aparece, haga clic en **Eliminar** para confirmar la eliminación.

   El proceso de eliminación de usuarios se ejecuta como un proceso en segundo plano, por lo que puede seguir utilizando Workfront a medida que se eliminan los usuarios.

   Según el número de usuarios que esté eliminando, el proceso puede tardar varios minutos o incluso unas horas.

   Tras recibir en Workfront la confirmación de que los usuarios se han eliminado, es posible que siga viéndolos en el sistema hasta que el proceso de eliminación se complete en segundo plano.

   Posteriormente, si descubre que uno o más usuarios no se han eliminado correctamente, intente eliminarlos de uno en uno.
