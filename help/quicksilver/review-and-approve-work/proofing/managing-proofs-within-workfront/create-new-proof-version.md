---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Crear una nueva versión de una prueba
description: Administrar comentarios en varias versiones o revisiones de un trabajo puede ser un gran desafío. Workfront simplifica este proceso al permitirle crear y comparar varias versiones de una prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 0%

---

# Crear una nueva versión de una prueba

Administrar comentarios en varias versiones o revisiones de un trabajo puede ser un gran desafío. Workfront simplifica este proceso al permitirle crear y comparar varias versiones de una prueba.

Tenga en cuenta la siguiente información cuando esté creando una nueva versión de una prueba:

* Puede dar a un usuario permiso para ver una versión, pero no otra. Por el contrario, si comparte una versión posterior con un usuario, ese usuario no puede ver versiones anteriores a menos que vuelva atrás y conceda explícitamente al usuario acceso a esas versiones anteriores.
* Para crear una nueva versión de una prueba, debe tener derechos de edición en la prueba.

   Consulte [Administrar funciones de prueba en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) y [Perfiles de permisos de prueba en Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) para obtener más información sobre quién tiene derechos de edición en una prueba.

   Para obtener información sobre cómo compartir versiones de prueba, consulte  [Uso compartido de una prueba en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Si se crea una prueba dentro de Adobe Workfront, cualquier versión nueva creada para esa prueba también se debe crear dentro de Workfront. No se puede crear una nueva versión de una prueba en Workfront Proof si dicha prueba se creó en Workfront.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Creación de una nueva versión de una prueba en Workfront

Existen varias formas de cargar una nueva versión de prueba en Workfront. La configuración de prueba predeterminada puede o no continuar desde la versión anterior dependiendo del método que elija:

* **Generar pruebas automáticamente al cargar documentos**: La configuración de prueba predeterminada no se transfiere. Si tiene esta configuración habilitada en el perfil de usuario, la configuración de prueba predeterminada no se mantiene cuando arrastra y suelta una nueva versión.
* **Crear prueba > Simple**: La configuración de prueba predeterminada no se transfiere. Si elige Simple al crear una nueva versión de prueba, la configuración de prueba predeterminada no se transfiere desde la versión anterior.
* **Agregar nuevo > Versión > Prueba**: La configuración de prueba predeterminada se transfiere desde la versión anterior.
* **Crear prueba > Avanzado**: La configuración de prueba predeterminada se transfiere desde la versión anterior.

   <table>
  <tbody>
  <tr>
  <td>Generar automáticamente revisiones al subir documentos</td>
  <td>La configuración de prueba predeterminada no se transfiere. Si tiene esta configuración habilitada en el perfil de usuario, la configuración de prueba predeterminada no se mantiene cuando arrastra y suelta una nueva versión.</td>
  </tr>
  <tr>
  <td>Crear prueba &gt; Simple</td>
  <td>La configuración de prueba predeterminada no se transfiere. Si elige Simple al crear una nueva versión de prueba, la configuración de prueba predeterminada no se transfiere desde la versión anterior.</td>
  </tr>
  <tr>
  <td>Agregar nuevo &gt; Versión &gt; Prueba</td>
  <td>La configuración de prueba predeterminada se transfiere desde la versión anterior.</td>
  </tr>
  <tr>
  <td>Crear prueba &gt; Avanzado</td>
  <td>La configuración de prueba predeterminada se transfiere desde la versión anterior.</td>
  </tr>
  </tbody>
  </table>




Para crear una nueva versión de una prueba:

1. Abra la lista de documentos que contiene la prueba.
1. Desde el sistema de archivos del equipo, arrastre y suelte un nuevo archivo sobre la prueba.

   O

   Seleccione la fila donde se muestra la prueba, haga clic en **Agregar nuevo** > **Versión** y, a continuación, haga clic en la opción que desee utilizar para añadir la nueva versión de la prueba.

   ![](assets/add-new-version-350x185.png)

## Cree una nueva versión de una prueba desde el visor de pruebas (solo Workfront Proof)

Si utiliza la prueba independiente de Workfront, puede crear una nueva versión de una prueba que contenga un solo archivo o captura web. 

>[!NOTE]
>
>Si su cuenta está en un plan de Enterprise y carga varios archivos o capturas web, se combinarán automáticamente en una única versión nueva. Consulte [Creación de una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) para obtener más información.

Para crear una nueva versión de una prueba en Workfront Proof:

1. Abra la prueba.
1. Haga clic en el **Versión** menú desplegable en la esquina superior izquierda y haga clic en **+ Nueva versión** en el cuadro que aparece.

   En el **Nueva versión de prueba de** que aparece, puede ver todos los revisores de la versión anterior, incluidos sus roles y la configuración de notificación por correo electrónico. Puede editar fácilmente las funciones y notificaciones de los revisores existentes o eliminar los revisores existentes de la nueva versión de esta página.

1. En **Añadir archivos**, cargue un archivo como una nueva versión de la prueba arrastrando y soltando desde el equipo o haciendo clic en **navegar** y seleccione el archivo que desee. Puede escribir una **Nombre de la prueba** para la versión o deje este cuadro en blanco para utilizar el mismo nombre de archivo con un número de versión añadido al final.

   O

   Capture una página web como una nueva versión de la prueba escribiendo una dirección URL.

   >[!NOTE]
   >
   >Arrastrar y soltar solo está disponible con exploradores que admiten HTML5. Esto excluye Internet Explorer 7 a 9 y Safari.

1. En **Flujo de trabajo**, realice cualquiera de los cambios siguientes para especificar los revisores de esta versión de la prueba.

   Los revisores de la versión anterior se sustituyen por los revisores que agregue.

   * Cambie el **Propietario** de la versión a otro usuario de su cuenta.\
      Para obtener información sobre los permisos de propietario, consulte [Perfiles de permisos de prueba en Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Al usar la variable **Escriba el nombre de contacto o la dirección de correo electrónico para agregar un cuadro de destinatario**, agregue revisores a la versión . Puede especificar un **Función de prueba** y **Alertas de correo electrónico** para cada destinatario.

      Para obtener información sobre cómo agregar grupos a la prueba, consulte  [Agregar grupos a una prueba](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Para obtener información sobre las funciones, consulte [Administrar funciones de prueba en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      >[!NOTE]
      >
      >Si el creador o el propietario de la prueba [El correo electrónico de prueba realizada](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) desactivada de forma predeterminada (en su configuración personal), no recibirán ningún correo electrónico de prueba o prueba nueva aunque la casilla Notificar a las personas por correo electrónico esté marcada en la página Nueva prueba . Para obtener información sobre las notificaciones por correo electrónico, consulte [Configuración de las notificaciones por correo electrónico en Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Consulte también [El correo electrónico de prueba realizada](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) y [Nuevo correo electrónico de prueba](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Establezca una fecha límite de prueba para la versión.
   * Pase el ratón sobre el nombre de un revisor para ver las decisiones que ha tomado en una versión anterior.

1. En **Notificación por correo electrónico**, realice una de las acciones siguientes:

   * Especifique si desea notificar a los revisores la nueva versión.\
      La selección se registrará en la sección Actividad de la página Detalles de la prueba . Para obtener más información, consulte [Administrar detalles de prueba en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Añada un asunto y un mensaje personalizados.

1. En el **Organización** , realice una de las acciones siguientes: 

   * Aplique una o más etiquetas a la prueba. Para obtener más información, consulte [Crear y administrar etiquetas en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
      Tenga en cuenta que las etiquetas también se heredan de la versión anterior de la prueba. Si agrega una etiqueta nueva a la nueva versión, también se etiquetarán las versiones anteriores.

   * Añada la versión a una carpeta. Consulte [Administrar carpetas en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) para obtener más información. La carpeta se copia desde la versión anterior de la prueba. Si selecciona una carpeta diferente, se moverá toda la prueba (todas las versiones).

   * Los administradores de facturación y los administradores pueden hacer que el campo de carpeta sea obligatorio en toda la cuenta en la pestaña Configuración . Consulte para obtener más información.

1. En Configuración de prueba, realice cualquiera de los cambios siguientes:

   * Requerir inicio de sesión en la prueba
   * Requerir firmas electrónicas en la prueba (solo Enterprise Plan)
   * Bloquear la prueba cuando se tomen todas las decisiones
   * Permitir o bloquear la descarga del archivo original
   * Uso compartido público de la prueba, incluida la configuración de uso compartido en público
   * Suscripción a la prueba\
      Las selecciones realizadas en esta sección se mostrarán en la página de detalles de la prueba (donde se pueden editar algunos campos). Para obtener más información, consulte [Administrar detalles de prueba en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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

Si había un asunto o mensaje personalizado incluido en la versión anterior de la prueba, se mostrará de forma predeterminada en la página Nueva versión . Puede:

* Edite el asunto y el mensaje.
* Desmarque la casilla Notificar a las personas por correo electrónico , lo que significa que no se enviará ningún correo electrónico a los revisores para notificarles que tienen una nueva versión para revisar.

   >[!NOTE]
    Esto no se ve afectado por ningún asunto o mensaje personalizado predeterminado guardado en su configuración personal.

Si tiene un asunto predeterminado y un mensaje guardados en su configuración personal, esto afectará al mensaje que se muestra de forma predeterminada en la página Nueva versión :

* Si decide notificar a los revisores por correo electrónico la versión anterior de la prueba utilizando el correo electrónico estándar (por ejemplo, sin asunto/mensaje personalizado), su asunto/mensaje personalizado predeterminado (su configuración personal) se mostrará en la página Nueva versión . A continuación, puede editar el asunto y el mensaje personalizados o desmarcar la casilla Notificar a las personas por correo electrónico (lo que significa que no se enviará ningún correo electrónico a los revisores para notificarles que tienen una nueva versión para revisar).
* Si decide no notificar a los revisores por correo electrónico la versión anterior de la prueba (por ejemplo, sin correo electrónico estándar o personalizado), la página Nueva versión no incluirá ningún mensaje de forma predeterminada. Para notificar a los revisores la nueva versión, haga clic en el vínculo Send a Message , que muestra el asunto/mensaje personalizado predeterminado (según su configuración personal). A continuación, puede editar el asunto y el mensaje personalizados si es necesario.

Si no tiene un asunto predeterminado y un mensaje guardados en su configuración personal, se mostrará lo siguiente en la página Nueva versión :

* Si decide notificar a los revisores por correo electrónico la versión anterior de la prueba utilizando el correo electrónico estándar (por ejemplo, sin asunto/mensaje personalizado), la opción Notificar a las personas por correo electrónico se selecciona de forma predeterminada en la página Nueva versión . Para añadir un mensaje personalizado, haga clic en el vínculo .
* Si decide no notificar a los revisores por correo electrónico la versión anterior de la prueba (por ejemplo, sin correo electrónico estándar o personalizado), la página Nueva versión no incluirá ningún mensaje de forma predeterminada. Para notificar a los revisores la nueva versión, haga clic en el vínculo Send a Message . A continuación, puede agregar un asunto y mensaje personalizados haciendo clic en el vínculo Agregar mensaje personalizado .
