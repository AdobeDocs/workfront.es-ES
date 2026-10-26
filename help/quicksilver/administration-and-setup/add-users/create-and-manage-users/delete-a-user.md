---
title: Eliminar usuarios
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Cuando un usuario abandona la organización, puede eliminarlo de Workfront, aunque se recomienda desactivar a los usuarios en lugar de eliminarlos.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 77%
---
# Eliminar usuarios

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplicaba únicamente a las organizaciones que no se habían incorporado a Admin Console. Dado que su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>  Para obtener instrucciones sobre cómo eliminar un usuario en Adobe Admin Console, consulte la sección &quot;Eliminar usuarios de forma permanente&quot; en el artículo [Administrar usuarios de forma individual](https://helpx.adobe.com/es/enterprise/using/manage-users-individually.html?lang=es) o póngase en contacto con el administrador de Adobe Admin Console.

Cuando un usuario abandona la organización, puede eliminarlo de Adobe Workfront.

La eliminación de un usuario debe realizarse a través de Adobe Admin Console. Para obtener instrucciones, consulte la sección &quot;Eliminar usuarios permanentemente&quot; en el artículo [Administrar usuarios individualmente](https://helpx.adobe.com/es/enterprise/using/manage-users-individually.html?lang=es) o comuníquese con el administrador de Adobe Admin Console.

>[!IMPORTANT]
>
>Al eliminar un usuario del sistema también se elimina la información asociada al usuario que quizás desee conservar. Se recomienda desactivar a los usuarios en lugar de eliminarlos. Para obtener más información, consulte [Desactivar o reactivar un usuario](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Adobe Admin Console.</p> 
    </td> 
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
    >Para obtener más información, consulte [¿Por qué no puedo obtener acceso a un informe propiedad de un usuario desactivado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) del artículo [Preguntas más frecuentes sobre informes](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

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
     >
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


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
