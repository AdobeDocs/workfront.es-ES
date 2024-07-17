---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Etiquete a los usuarios para compartir una prueba
description: Cuando comenta una prueba en el visor de pruebas, puede etiquetar a otros usuarios para que presten atención a su comentario por correo electrónico y para añadirlos al flujo de trabajo de la prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Etiquete a los usuarios para compartir una prueba

Cuando comenta una prueba en el visor de pruebas, puede etiquetar a otros usuarios para que presten atención a su comentario por correo electrónico y para añadirlos al flujo de trabajo de la prueba.

Al etiquetar a los usuarios en comentarios de una prueba, es posible que los usuarios a los que puede etiquetar difieran según varios factores, como los permisos de usuario individuales y la pertenencia a la organización:

* Si es el creador de la prueba, el propietario o tiene permisos específicos habilitados, puede etiquetar a los usuarios fuera del flujo de trabajo de prueba y compartir la prueba con ellos.
* Si se le añadió a la prueba como usuario externo y es miembro de otro entorno con una cuenta de prueba diferente, solo puede etiquetar a esos usuarios del entorno original. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Requisitos de acceso {#access-requirements}

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Función de prueba</td> 
   <td>Autor, moderador</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Supervisor o administrador</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Etiquete a los usuarios para compartir una prueba

Los usuarios con el perfil de permiso de revisión o la función de revisión descrita en la sección [Requisitos de acceso](#access-requirements) anterior pueden etiquetar a los usuarios para que compartan una revisión de forma predeterminada. También puede etiquetar usuarios para compartir una prueba independientemente del perfil de permiso de prueba o la función de prueba si es el propietario o creador de la prueba. Puede habilitar a los usuarios con un perfil de permiso de prueba menor o funciones de prueba para que etiqueten a los usuarios para que compartan una prueba al crearla. Para obtener más información, consulte la sección [Configurar el flujo de trabajo y agregar revisores](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) en el artículo [Crear una prueba avanzada con un flujo de trabajo básico](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).

>[!NOTE]
>
>Puede etiquetar a un colaborador externo utilizando su dirección de correo electrónico solo si se cumple alguna de las siguientes condiciones:>
>* Un usuario de la cuenta de Workfront de su organización ha añadido anteriormente la dirección de correo electrónico del colaborador a una prueba.
>* El colaborador ha utilizado la dirección de correo electrónico para suscribirse a una revisión en la cuenta de Workfront de su organización anteriormente.
>

Para etiquetar a alguien y compartir una prueba en un comentario:

1. Cuando comente una prueba, escriba un signo arroba (@) seguido del nombre o la dirección de correo electrónico de la persona. Cuando empiece a escribir, los nombres disponibles aparecen en una lista desplegable.
1. Seleccione el nombre de la persona cuando lo vea en la lista desplegable.

   >[!TIP]
   >
   >Si desea cerrar la lista desplegable sin seleccionar a nadie, puede presionar la tecla **Esc** o hacer clic en cualquier lugar fuera de la lista.

1. Repita los pasos del 1 al 2 con los demás usuarios que desee etiquetar en el comentario.
1. Finalice el comentario y haga clic en **Post**.
1. (Condicional) Si ha etiquetado a alguien que aún no se haya agregado a la prueba, especifique un valor de **Función de prueba** y **Alertas por correo electrónico** para cada usuario enumerado en el cuadro que aparece y, a continuación, haga clic en **Agregar personas y publicar comentario**.

   ![](assets/add-people-to-proof-350x220.png)

   Para obtener información sobre las funciones de prueba, consulte . Para obtener información acerca de las alertas de prueba por correo electrónico, consulte la sección en el artículo [Configuración de notificaciones por correo electrónico en Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Si la prueba tiene un flujo de trabajo automatizado, los usuarios que etiquete se añadirán a la fase en la que se encuentre. Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Cualquier persona a la que etiquete recibirá un correo electrónico de notificación sobre el comentario de la prueba, independientemente de la configuración de alertas de correo electrónico de prueba que utilice:

   * Si el usuario recibe un resumen diario o un correo electrónico de resumen por hora, Workfront envía la notificación por separado e incluye información sobre el comentario de la prueba en el correo electrónico de resumen.
   * Si el usuario recibe alertas para todas las actividades o para las respuestas a sus comentarios, la notificación reemplaza las notificaciones sobre estos comentarios y respuestas.

Para obtener información acerca de otras formas de agregar usuarios a una revisión, vea [Compartir una revisión en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
