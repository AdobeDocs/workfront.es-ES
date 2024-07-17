---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Crear una nueva versión de una revisión
description: Gestionar los comentarios en varias versiones o revisiones de una parte del trabajo puede ser un gran desafío. Workfront simplifica este proceso al permitirle crear y comparar varias versiones de una prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1723'
ht-degree: 0%

---

# Crear una nueva versión de una revisión

Gestionar los comentarios en varias versiones o revisiones de una parte del trabajo puede ser un gran desafío. Workfront simplifica este proceso al permitirle crear y comparar varias versiones de una prueba.

Tenga en cuenta la siguiente información al crear una nueva versión de una prueba:

* Puede conceder permiso a un usuario para ver una versión, pero no otra. Por el contrario, si comparte una versión posterior con un usuario, ese usuario no puede ver las versiones anteriores a menos que vuelva atrás y conceda explícitamente al usuario acceso a esas versiones anteriores.
* Para crear una nueva versión de una prueba, debe tener derechos de edición sobre la prueba.

  Consulte [Administrar roles de prueba en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) y [Permisos de prueba en Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) para obtener más información sobre quién tiene derechos de edición en una prueba.

  Para obtener información sobre cómo compartir versiones de prueba, consulte  [Compartir una revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Si se crea una prueba en Adobe Workfront, también se deben crear en Workfront las nuevas versiones creadas para esa prueba. No puede crear una nueva versión de una prueba en Workfront Proof si dicha prueba se creó en Workfront.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Creación de una nueva versión de una prueba en Workfront

Existen varias formas de cargar una nueva versión de prueba en Workfront. La configuración de prueba predeterminada puede ser o no transferida de la versión anterior según el método que elija:

* **Generar automáticamente revisiones al cargar documentos**: La configuración de revisión predeterminada no se transfiere. Si tiene esta configuración habilitada en el perfil de usuario, la configuración de prueba predeterminada no se traslada al arrastrar y soltar una nueva versión.
* **Crear revisión > Simple**: la configuración de revisión predeterminada no se transfiere. Si elige Simple al crear una nueva versión de prueba, los ajustes de prueba predeterminados no se transfieren de la versión anterior.
* **Agregar nuevo > Versión > Prueba**: la configuración de prueba predeterminada se transfiere desde la versión anterior.
* **Crear revisión > Avanzado**: la configuración de revisión predeterminada se transfiere desde la versión anterior.

  <table>
  <tbody>
  <tr>
  <td>Generar automáticamente revisiones al subir documentos</td>
  <td>La configuración de prueba predeterminada no se transfiere. Si tiene esta configuración habilitada en el perfil de usuario, la configuración de prueba predeterminada no se traslada al arrastrar y soltar una nueva versión.</td>
  </tr>
  <tr>
  <td>Crear prueba &gt; Sencilla</td>
  <td>La configuración de prueba predeterminada no se transfiere. Si elige Simple al crear una nueva versión de prueba, los ajustes de prueba predeterminados no se transfieren de la versión anterior.</td>
  </tr>
  <tr>
  <td>Añadir nuevo &gt; Versión &gt; Prueba</td>
  <td>La configuración de prueba predeterminada se transfiere desde la versión anterior.</td>
  </tr>
  <tr>
  <td>Creación de una prueba &gt; Avanzada</td>
  <td>La configuración de prueba predeterminada se transfiere desde la versión anterior.</td>
  </tr>
  </tbody>
  </table>




Para crear una nueva versión de una prueba:

1. Abra la lista de documentos que contiene la prueba.
1. Desde el sistema de archivos del equipo, arrastre y suelte un nuevo archivo sobre la prueba.

   O

   Seleccione la fila donde aparece la revisión, haga clic en **Agregar nueva** > **Versión** y, a continuación, haga clic en la opción que desee usar para agregar la nueva versión de la revisión.

   ![](assets/add-new-version-350x185.png)

## Crear una nueva versión de una revisión desde el visor de pruebas (solo Workfront Proof)

Si utiliza el Workfront Proof independiente, puede crear una nueva versión de una prueba que contenga un solo archivo o captura web. 

>[!NOTE]
>
>Si su cuenta está en un plan Enterprise y carga varios archivos o capturas web, se combinarán automáticamente en una sola versión nueva. Consulte [Crear una revisión de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) para obtener más información.

Para crear una nueva versión de una prueba en Workfront Proof:

1. Abra la prueba.
1. Haga clic en el menú desplegable **Versión** en la esquina superior izquierda y, a continuación, haga clic en **+ Nueva versión** en el cuadro que aparece.

   En la página **Nueva versión de revisión de** que aparece, puede ver todos los revisores de la versión anterior, incluidos sus roles y la configuración de las notificaciones por correo electrónico. Puede editar fácilmente las funciones y notificaciones de los revisores existentes o eliminar los existentes de la nueva versión de esta página.

1. En **Agregar archivos**, cargue un archivo como una nueva versión de la revisión arrastrando y soltando desde el equipo o haciendo clic en **examinar** y seleccionando el archivo que desee. Puede escribir un **Nombre de revisión** para la versión o dejar este cuadro en blanco para usar el mismo nombre de archivo con un número de versión agregado al final.

   O

   Capture una página web como una nueva versión de la prueba escribiendo una dirección URL.

   >[!NOTE]
   >
   >Arrastrar y soltar solo está disponible con navegadores totalmente compatibles con HTML5. Esto excluye Internet Explorer 7 a 9 y Safari.

1. En **Flujo de trabajo**, realice cualquiera de los cambios siguientes para especificar los revisores de esta versión de la revisión.

   Los revisores de la versión anterior se sustituyen por los revisores que agregue.

   * Cambie **Owner** de la versión a otro usuario de su cuenta.\
     Para obtener información acerca de los permisos de propietario, consulte [Perfiles de permisos de revisión en Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Usando **Escriba el nombre de contacto o la dirección de correo electrónico para agregar un cuadro de destinatario**, agregue revisores a la versión. Puede especificar un **Rol de prueba** y un tipo de **Alertas por correo electrónico** para cada destinatario.

     Para obtener información sobre cómo agregar grupos a la prueba, consulte  [Agregar grupos a una revisión](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Para obtener información sobre los roles, consulte [Administrar roles de prueba en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Si el creador o propietario de  Si la prueba tiene [Correo electrónico de prueba hecha](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) deshabilitado de forma predeterminada (en su configuración personal), no recibirá ningún correo electrónico de prueba hecha o nueva prueba aunque el cuadro Notificar a las personas por correo electrónico esté marcado en la página Nueva prueba. Para obtener información acerca de las notificaciones por correo electrónico, consulte [Configuración de notificaciones por correo electrónico en Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Ver también [Correo electrónico sobre la prueba hecha](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) y [Nuevo correo electrónico sobre la prueba](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Establezca un plazo de prueba para la versión.
   * Pase el ratón sobre el nombre de un revisor para ver qué decisiones ha tomado en una versión anterior.

1. En **Notificación por correo electrónico**, realice una de las acciones siguientes:

   * Especifique si desea notificar la nueva versión a los revisores.\
     Su selección se registrará en la sección Actividad de la página Detalles de la prueba. Para obtener más información, consulte [Administrar detalles de revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Añada un asunto y un mensaje personalizados.

1. En la sección **Organización**, realice una de las acciones siguientes: 

   * Aplique una o más etiquetas a la prueba. Para obtener más información, consulte [Crear y administrar etiquetas en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
     Tenga en cuenta que las etiquetas también se heredan de la versión anterior de la prueba. Si añade una etiqueta nueva a la nueva versión, las versiones anteriores también se etiquetan.

   * Añada la versión a una carpeta. Consulte [Administrar carpetas en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) para obtener más información. La carpeta se copiará de la versión anterior de la revisión. Si selecciona una carpeta diferente, se moverá toda la prueba (todas las versiones).

   * Los administradores de facturación y los administradores pueden hacer que el campo de carpeta sea obligatorio en toda la cuenta en la pestaña Configuración. Consulte para obtener más información.

1. En Configuración de prueba, realice cualquiera de los cambios siguientes:

   * Requerir inicio de sesión en la prueba
   * Requerir firmas electrónicas en la prueba (solo para el plan empresarial)
   * Bloquear la prueba cuando se tomen todas las decisiones
   * Permitir o bloquear la descarga del archivo original
   * Uso compartido público de la prueba, incluida la configuración de uso compartido público
   * Suscripción a la prueba\
     Las selecciones realizadas en esta sección se mostrarán en la página Proof details (donde se pueden editar algunos campos). Para obtener más información, consulte [Administrar detalles de revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## Acerca del mensaje Nueva versión

Si había un asunto/mensaje personalizado incluido en la versión anterior de la prueba, se mostrará de forma predeterminada en la página Nueva versión. Puede:

* Edite el asunto y el mensaje.
* Anule la selección del cuadro Notificar a las personas por correo electrónico, lo que significa que no se enviará ningún correo electrónico a los revisores para notificarles que tienen una nueva versión que revisar.

  >[!NOTE]
  >
  > Esto no se ve afectado por ningún asunto o mensaje personalizado predeterminado guardado en su configuración personal.

Si tiene un asunto y un mensaje predeterminados guardados en su configuración personal, esto afectará en qué mensaje se muestra de forma predeterminada en la página Nueva versión:

* Si decide notificar a los revisores por correo electrónico la versión anterior de la prueba mediante el correo electrónico estándar (por ejemplo, sin asunto/mensaje personalizado), el asunto/mensaje personalizado predeterminado (su configuración personal) se mostrará en la página Nueva versión. A continuación, puede editar el asunto y el mensaje personalizados o anular la selección del cuadro Notificar a las personas por correo electrónico (lo que significa que no se enviará ningún correo electrónico a los revisores para notificarles que tienen una nueva versión que revisar).
* Si decide no notificar a los revisores por correo electrónico la versión anterior de la prueba (por ejemplo, sin correo electrónico estándar o personalizado), la página Nueva versión no incluirá ningún mensaje de forma predeterminada. Para notificar la nueva versión a los revisores, haga clic en el vínculo Enviar un mensaje, que mostrará el asunto o mensaje personalizado predeterminado (según su configuración personal). A continuación, puede editar el asunto y el mensaje personalizados si es necesario.

Si no tiene un asunto y un mensaje predeterminados guardados en su configuración personal, se mostrará lo siguiente en la página Nueva versión:

* Si decide notificar a los revisores por correo electrónico la versión anterior de la prueba mediante el correo electrónico estándar (por ejemplo, sin asunto/mensaje personalizado), la opción Notificar a las personas por correo electrónico se seleccionará de forma predeterminada en la página Nueva versión. Para añadir un mensaje personalizado, haga clic en el vínculo.
* Si decide no notificar a los revisores por correo electrónico la versión anterior de la prueba (por ejemplo, sin correo electrónico estándar o personalizado), la página Nueva versión no incluirá ningún mensaje de forma predeterminada. Para notificar la nueva versión a los revisores, haga clic en el vínculo Enviar un mensaje. A continuación, puede agregar un asunto y un mensaje personalizados haciendo clic en el vínculo Agregar mensaje personalizado.
