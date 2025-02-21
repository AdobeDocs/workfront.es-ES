---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Etiquetar a los usuarios para compartir una revisión
description: Cuando comenta una revisión en el visor de corrección, puede etiquetar a otros usuarios para que presten atención a su comentario por correo electrónico y para añadirlos al flujo de trabajo de la revisión.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 99%

---

# Etiquetar a los usuarios para compartir una revisión

Cuando comenta una revisión en el visor de corrección, puede etiquetar a otros usuarios para que presten atención a su comentario por correo electrónico y para añadirlos al flujo de trabajo de la revisión.

Al etiquetar a los usuarios en los comentarios de una revisión, es posible que los usuarios a los que puede etiquetar difieran según diversos factores, como los permisos de cada usuario individual y el abono a la organización:

* Si es el creador de la revisión, el propietario o tiene permisos específicos habilitados, puede etiquetar a usuarios de fuera del flujo de trabajo de la revisión y compartir la revisión con ellos.
* Si se le añadió a la revisión como usuario externo y es abonado de otro entorno con una cuenta de revisión diferente, solo puede etiquetar a los usuarios de su entorno original. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Requisitos de acceso {#access-requirements}

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: pro o superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre el acceso de revisión en los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: trabajo o plan</p> <p>Plan heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Función de prueba</td> 
   <td>Autor, moderador</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Supervisor o administrador</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con el administrador de Workfront o de Workfront Proof.

+++

## Etiquetar a los usuarios para compartir una revisión

Los usuarios con el perfil de permiso de revisión o la función de revisión descrita en la sección [Requisitos de acceso](#access-requirements) anterior pueden etiquetar a los usuarios para compartir una revisión de forma predeterminada. Si es usted el propietario o creador de la revisión, también puede etiquetar usuarios para compartir una revisión independientemente del perfil de permiso de revisión o la función de revisión. Puede habilitar a los usuarios con un perfil de permiso de revisión o funciones de revisión inferiores para que etiqueten a los usuarios para que compartan una revisión al crearla. Para obtener más información, consulte la sección [Configurar el flujo de trabajo y añadir revisores](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) en el artículo [Crear una revisión avanzada con un flujo de trabajo básico](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).

>[!NOTE]
>
>Puede etiquetar a un colaborador externo utilizando su dirección de correo electrónico solo si se cumple alguna de las siguientes condiciones:
>* Un usuario de la cuenta de Workfront de su organización ha añadido anteriormente la dirección de correo electrónico del colaborador a una revisión.
>* El colaborador ha utilizado la dirección de correo electrónico para suscribirse a una revisión en la cuenta de Workfront de su organización anteriormente.
>

Para etiquetar a alguien y compartir una revisión en un comentario:

1. Cuando comente una revisión, escriba un signo de arroba (@) seguido del nombre o la dirección de correo electrónico de la persona. Cuando empiece a escribir, los nombres disponibles aparecen en una lista desplegable.
1. Seleccione el nombre de la persona cuando lo vea en la lista desplegable.

   >[!TIP]
   >
   >Si desea cerrar la lista desplegable sin seleccionar a nadie, puede presionar la tecla **Esc** o hacer clic en cualquier lugar fuera de la lista.

1. Repita los pasos del 1 al 2 con los demás usuarios que desee etiquetar en el comentario.
1. Finalice el comentario y, a continuación, haga clic en **Publicar**.
1. (Condicional) Si ha etiquetado a alguien que aún no se ha añadido a la revisión, especifique una **Función de revisión** y una opción **Alertas por correo electrónico** para cada usuario enumerado en el cuadro que aparece y, a continuación, haga clic en **Añadir personas y publicar comentario**.

   ![Agregar personas a la revisión](assets/add-people-to-proof-350x220.png)

   Para obtener información sobre las funciones de revisión, consulte . Para obtener información sobre las alertas de revisión por correo electrónico, consulte la sección del artículo [Configurar notificaciones por correo electrónico en Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Si la revisión tiene un flujo de trabajo automatizado, los usuarios que etiquete se añadirán a la fase en la que se encuentre. Para más información, consulte [Información general de flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Cualquier persona a la que etiquete recibirá un correo electrónico de notificación sobre el comentario de la revisión, independientemente de la configuración de alertas de revisión por correo electrónico que utilice:

   * Si el usuario recibe un resumen diario o un correo electrónico de resumen por hora, Workfront envía la notificación por separado e incluye información sobre el comentario de la revisión en el correo electrónico de resumen.
   * Si el usuario recibe alertas para todas las actividades o para las respuestas a sus comentarios, la notificación reemplaza las notificaciones sobre estos comentarios y respuestas.

Para obtener información sobre otras formas de añadir usuarios a una revisión, consulte [Compartir una revisión en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
