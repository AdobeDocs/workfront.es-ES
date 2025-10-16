---
title: Eliminar usuarios
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Cuando un usuario abandona la organización, puede eliminarlo de Workfront, aunque se recomienda desactivar a los usuarios en lugar de eliminarlos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 18c39c5b1959c31b6fd0018476b48643b4b15021
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 93%

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
>Al eliminar un usuario del sistema también se elimina la información asociada al usuario que quizás desee conservar. Se recomienda desactivar a los usuarios en lugar de eliminarlos. Para obtener más información, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Edición</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si <b>Administrador de usuarios (usuarios de grupo)</b> está habilitado, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar o desactivar un usuario

Al desactivar un usuario, sucede lo siguiente:

* Se eliminan las licencias del usuario tanto a Workfront como a Workfront Proof si el componente de Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información acerca de Workfront Proof, consulte [Workfront Proof: índice de artículos](../../../workfront-proof/workfront-proof.md).
* Ya no se puede asignar trabajo al usuario.
* El usuario ya no puede añadirse a las actualizaciones.
* El usuario ya no se puede añadir a equipos o grupos.
* Los objetos ya no se pueden compartir con el usuario.
* Su asociación con los siguientes objetos permanece intacta:

   * Tareas, problemas, proyectos, portafolios
   * Paneles de control

     >[!NOTE]
     >
     >Si desactiva un usuario y ya no puede ver los informes o tableros asociados con un usuario, es posible que deba actualizar el campo **Ejecutar este informe con los derechos de acceso de:**.\
     >Para obtener más información, consulte [¿Por qué no puedo acceder a un informe que pertenece a un usuario desactivado?Sección &#x200B;](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) del artículo [Preguntas más frecuentes sobre informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Documentos
   * Actualizaciones
   * Horas

* Si el usuario tiene documentos desprotegidos, estos permanecen desprotegidos cuando se desactivan. Solo un administrador de Workfront puede volver a registrarlos. Para obtener más información acerca de cómo desproteger documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

Al eliminar un usuario, sucede lo siguiente:

* Se eliminan las licencias del usuario tanto en Workfront como en Workfront Proof, si el componente de Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información acerca de Workfront Proof, consulte [Workfront Proof: índice de artículos](../../../workfront-proof/workfront-proof.md).
* Ya no se puede asignar trabajo al usuario.
* El usuario ya no puede añadirse a las actualizaciones.
* El usuario ya no se puede añadir a equipos o grupos.
* Los objetos ya no se pueden compartir con el usuario.
* Se elimina la asociación del usuario con los siguientes objetos:

   * Tareas, problemas, proyectos, portafolios
   * Paneles de control

  <!--
     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.
     -->

   * Actualizaciones
   * Horas

     >[!NOTE]
     >
     >Estos objetos permanecen en Workfront, pero su propietario está ahora en blanco.

* Si el usuario ha cargado algún documento en el área de documentos de la barra de navegación global, los documentos también se eliminan.
* Si el usuario ha retirado los documentos que le pertenecen y los documentos se cargan en el área principal de Documentos (a la que se accede desde el menú principal), los documentos se eliminan con el usuario. Para obtener más información acerca de cómo desproteger documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

Para obtener más información sobre cómo desactivar usuarios, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Puede eliminar usuarios de forma permanente de uno en uno, o bien puede eliminar varios usuarios de forma simultánea de forma permanente. Cuando elimine usuarios individuales, debe esperar a que se complete el proceso de eliminación antes de continuar con otras actividades en Workfront. El proceso de eliminar varios usuarios se ejecuta simultáneamente como un proceso en segundo plano, por lo que puede seguir utilizando Workfront a medida que se eliminan los usuarios.

## Eliminar uno o más usuarios

{{step-1-to-users}}

1. Seleccione al menos un usuario que desee eliminar, haga clic en el icono Más del menú ![Más](assets/more-icon.png) y, a continuación, haga clic en **Eliminar**.
1. En el cuadro que aparece, haga clic en **Eliminar** para confirmar la eliminación.

   El proceso de eliminación de usuarios se ejecuta como un proceso en segundo plano, por lo que puede seguir utilizando Workfront a medida que se eliminan los usuarios.

   Según el número de usuarios que esté eliminando, el proceso puede durar varios minutos o incluso varias horas.

   Tras recibir en Workfront la confirmación de que los usuarios se han eliminado, es posible que siga viéndolos en el sistema hasta que el proceso de eliminación se complete en segundo plano.

   Posteriormente, si descubre que uno o más usuarios no se han eliminado correctamente, intente eliminarlos de uno en uno.
