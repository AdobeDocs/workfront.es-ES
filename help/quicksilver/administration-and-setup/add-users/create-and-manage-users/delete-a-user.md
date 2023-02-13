---
title: Eliminar usuarios
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Cuando un usuario abandona la organización, puede eliminarlo de Workfront, aunque se recomienda desactivar los usuarios en lugar de eliminarlos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Eliminar usuarios

Cuando un usuario abandona la organización, puede eliminarlo de Adobe Workfront.

>[!IMPORTANT]
>
>* Al eliminar un usuario del sistema, también se elimina la información asociada al usuario que podría querer conservar. Se recomienda desactivar los usuarios en lugar de eliminarlos. Para obtener más información, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Eliminación de un usuario del [!DNL Adobe Admin Console] desactiva el usuario en [!DNL Workfront], pero no los elimina de [!DNL Workfront].
>
>  Para obtener instrucciones sobre la eliminación de un usuario en Adobe Admin Console, consulte la sección &quot;Eliminar usuarios de forma permanente&quot; del artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) o póngase en contacto con su administrador de Adobe Admin Console.
>
>  Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

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
   <td> <p>Debe tener una de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p><b>Usuarios</b> en el nivel de acceso configurado para <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si es Usuario <b>Administración (usuarios del grupo)</b> está activada, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> <p>Para obtener más información sobre la variable <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminación o desactivación de un usuario

Desactivar un usuario hace que sucedan las siguientes cosas:

* Elimina las licencias del usuario a Workfront y a Workfront Proof si el componente Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información sobre la Prueba de Workfront, consulte [Prueba de Workfront](../../../workfront-proof/workfront-proof.md).
* Ya no se puede asignar trabajo al usuario.
* El usuario ya no se puede agregar a las actualizaciones.
* El usuario ya no se puede agregar a equipos o grupos.
* Los objetos ya no se pueden compartir con el usuario.
* Su asociación con los siguientes objetos permanece intacta:

   * Tareas, problemas, proyectos, portafolios
   * Paneles

      >[!NOTE]
      >
      >Si desactiva un usuario y ya no puede ver los informes o tableros asociados a él, es posible que tenga que actualizar la variable **Ejecute este informe con los derechos de acceso de:** campo .\
      >Para obtener más información, consulte la [¿Por qué no puedo acceder a un informe propiedad de un usuario desactivado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) de la sección [Preguntas más frecuentes sobre los informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artículo.

   * Documentos
   * Actualizaciones
   * Horas

* Si el usuario ha retirado los documentos, estos permanecen desprotegidos cuando los desactiva. Solo los administradores de Workfront pueden volver a iniciarlos. Para obtener más información sobre la comprobación de documentos, consulte [Ver documentos](../../../documents/managing-documents/check-out-documents.md).

Al eliminar un usuario, suceden las siguientes cosas:

* Elimina las licencias del usuario a Workfront y a Workfront Proof si el componente Workfront Proof está asociado a su cuenta de Workfront. Para obtener más información sobre la Prueba de Workfront, consulte [Prueba de Workfront](../../../workfront-proof/workfront-proof.md).
* Ya no se puede asignar trabajo al usuario.
* El usuario ya no se puede agregar a las actualizaciones.
* El usuario ya no se puede agregar a equipos o grupos.
* Los objetos ya no se pueden compartir con el usuario.
* Elimina la asociación de ese usuario con los siguientes objetos:

   * Tareas, problemas, proyectos, portafolio
   * Paneles

      >[!NOTE]
      >
      >También se pierde acceso a las secciones personalizadas que contenían tableros asociados al usuario eliminado.\
      >Para obtener más información, consulte la [¿Cómo puedo acceder a un tablero que contiene un informe propiedad de un usuario eliminado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) de la sección [Preguntas más frecuentes sobre los informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artículo.

   * Actualizaciones
   * Horas

      >[!NOTE]
      >
      >Estos objetos permanecen en Workfront, pero el propietario del objeto está ahora en blanco.

* Si el usuario ha cargado cualquier documento en el área Documentos de la barra de navegación global, también se eliminan los documentos.
* Si el usuario ha extraído documentos que posee y los documentos se cargan en el área de documentos principal (a la que se accede desde el menú principal), los documentos se eliminan con el usuario. Para obtener más información sobre la comprobación de documentos, consulte [Ver documentos](../../../documents/managing-documents/check-out-documents.md).

Para obtener más información sobre la desactivación de usuarios, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Puede eliminar usuarios de forma permanente de uno en uno, o puede eliminar varios usuarios de forma permanente simultáneamente. Al eliminar usuarios individuales, debe esperar a que se complete el proceso de eliminación antes de pasar a otras actividades en Workfront. El proceso de eliminación de varios usuarios simultáneamente se ejecuta como un proceso en segundo plano, por lo que puede seguir utilizando Workfront a medida que se eliminan los usuarios.

## Eliminar uno o más usuarios

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Usuarios**.
1. Seleccione al menos un usuario que desee eliminar y haga clic en el menú Más ![](assets/more-icon.png)y haga clic en **Eliminar**.
1. En el cuadro que aparece, haga clic en **Eliminar** para confirmar la eliminación.

   El proceso de eliminación de usuarios se ejecuta como un proceso en segundo plano, por lo que puede continuar usando Workfront mientras se eliminan los usuarios.

   En función del número de usuarios que elimine, el proceso puede tardar varios minutos o incluso unas horas.

   Después de recibir la confirmación en Workfront de que se eliminaron los usuarios, puede seguir viéndolos en el sistema hasta que el proceso de eliminación se complete en segundo plano.

   Posteriormente, si descubre que uno o más usuarios no se eliminaron correctamente, intente eliminarlos de uno en uno.
