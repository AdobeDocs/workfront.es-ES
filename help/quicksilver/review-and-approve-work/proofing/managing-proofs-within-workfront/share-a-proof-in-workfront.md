---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Compartir una prueba en Adobe Workfront
description: Puede compartir un documento protegido en Adobe Workfront compartiendo el documento o agregando usuarios a la prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Compartir una prueba en Adobe Workfront

Puede compartir un documento protegido en Adobe Workfront compartiendo el documento o agregando usuarios a la prueba.

Si comparte la prueba, como se explica en este artículo, el destinatario tiene el mismo acceso al documento y a la prueba. Además, se puede solicitar la aprobación de la prueba al destinatario.

>[!TIP]
>
>También puede compartir una prueba desde el visor de pruebas. Para obtener instrucciones, consulte [Compartir una prueba desde el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Función de prueba</td> 
   <td>Autor o moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Compartir un vínculo de prueba

El uso compartido de un vínculo de prueba otorga a los usuarios de Workfront acceso de visualización. Los usuarios pueden comentar la prueba y suscribirse a las notificaciones por correo electrónico para la prueba con sus credenciales de inicio de sesión de Workfront. Los usuarios que no estén a favor de la prueba pueden realizar comentarios y suscribirse utilizando una dirección de correo electrónico y un nombre para mostrar.

>[!IMPORTANT]
>
>La configuración Permitir compartir prueba mediante URL pública o código incrustado debe estar habilitada.

1. Seleccione el documento que contiene la prueba que desea compartir con los usuarios.

   Sólo se puede seleccionar un documento. No se puede compartir el vínculo de varios documentos al mismo tiempo.

1. Haga clic en **Compartir** > **Vínculo de prueba**.
1. En el **Vínculo de prueba** que aparece, realice una de las acciones siguientes:

   * Para copiar el vínculo en el portapapeles, haga clic en **Copiar vínculo**.

      Ahora puede distribuir el vínculo a través de una herramienta de terceros, como un chat o una aplicación de correo electrónico.

   * Para enviar el vínculo directamente desde Adobe Workfront por correo electrónico, haga lo siguiente:

      1. En el **O enlace de correo electrónico a** , empiece a escribir y seleccione el nombre del destinatario. O especifique la dirección de correo electrónico de un usuario externo con el que desee compartir.

         >[!NOTE]
         >
         >Si ve un correo electrónico con alias al compartir una prueba, no cree un nuevo usuario invitado introduciendo el correo electrónico original si existe el correo electrónico con alias correspondiente.

      1. Seleccione entre las siguientes opciones:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Enviar vínculo público</td>
            <td><p>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a la prueba dentro del visor de pruebas que están utilizando y concede acceso a la vista.</p><p>If <strong>Suscripción a la prueba mediante URL pública o código incrustado</strong> está desactivado para la prueba, los usuarios pueden iniciar sesión con sus credenciales de inicio de sesión de Workfront para agregar comentarios a la prueba. Si está activada, cualquier persona que proporcione su dirección de correo electrónico y su nombre (no se requiere contraseña) puede firmar y agregar comentarios a la prueba.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Enviar vínculo de descarga</td>
            <td>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a una página de descarga y que proporciona detalles del archivo, el nombre del archivo y el tamaño del archivo, y el archivo se muestra en línea. Los usuarios pueden hacer clic en el vínculo Descargar de la página de descarga para descargar el archivo.</td>
           </tr>
           <tr>
            <td role="rowheader">Añadir mensaje personalizado</td>
            <td>Permite especificar un asunto y un cuerpo personalizados para la notificación por correo electrónico.</td>
           </tr>
          </tbody>
         </table>

      1. Haga clic en **Enviar**.

         Los destinatarios reciben una notificación por correo electrónico que contiene información sobre la prueba y los botones que ha elegido incluir.

         ![](assets/proof-share-email-350x87.png)

## Agregar usuarios a una prueba

Puede agregar cualquier usuario de Workfront a la prueba si tiene derechos de edición en la prueba. Si la prueba tiene varias etapas, agregue el usuario a una etapa individual

>[!NOTE]
>
>Tenga en cuenta lo siguiente si utiliza un plan de Workfront heredado en el que las pruebas se puedan habilitar y deshabilitar para un usuario:
>
>* Los destinatarios no necesitan tener habilitadas las pruebas para poder revisar la prueba.
>* Cuando Flujo de trabajo automatizado está habilitado y agrega un usuario a la prueba que no tiene la prueba habilitada en Workfront, se crea una nueva etapa en el Flujo de trabajo automatizado. El usuario que está agregando se agrega automáticamente a esta nueva etapa cuando ve la prueba por primera vez. (Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>


### Agregar usuarios a una prueba existente desde la pestaña Documentos

1. Seleccione el documento que contiene la prueba a la que desea agregar usuarios.
1. Si la prueba no tiene un flujo de trabajo automatizado (etapas), haga clic en el botón **Más** en la esquina superior derecha de la sección Etapa 1 y, a continuación, haga clic en **Compartir** en el menú desplegable.

   O

   Si la prueba tiene un flujo de trabajo automatizado, haga clic en el botón **Más** en la esquina superior derecha del escenario en el que desea agregar el revisor y, a continuación, haga clic en **Compartir** en el menú desplegable.

1. En el **Compartir esta versión** que aparece, en **Compartir**, empiece a escribir el nombre o la dirección de correo electrónico de un usuario con el que desee compartir la prueba y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

1. (Opcional) Repita este paso para agregar varios usuarios a la prueba.
1. (Opcional) Establezca una fecha límite para los revisores.
1. (Opcional) Asegúrese de que **Notificar a las personas por correo electrónico** está seleccionada si desea informar a los revisores de que los ha añadido a la prueba.
1. (Opcional) **Añadir un mensaje personalizado** al correo electrónico.
1. Cuando haya agregado todos los revisores, haga clic en **Compartir**.

### Agregar usuarios a una prueba existente desde el visor de pruebas

Puede agregar usuarios a una prueba mientras revisa una prueba en el visor de pruebas web y en el visor de pruebas de escritorio.

Para obtener más información, consulte [Compartir una prueba agregándole usuarios](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) en el artículo [Compartir una prueba desde el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Informe sobre pruebas de aprobaciones

Puede crear un informe que genere informes sobre las aprobaciones de pruebas que se han compartido en Workfront. Este informe proporciona la siguiente información de aprobación de pruebas en su sistema:

* Documento presentado para su aprobación
* Nombre del aprobador
* Versión de prueba
* Identificador de revisión
* Fecha de creación de la prueba

Puede acceder a esta aprobación al crear un informe basado en un objeto, tal como se describe en [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objeto Proof Approvals , consulte la [Informar sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) en [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Aprobar una prueba compartida

Cuando un usuario le agrega a una prueba y concede la función Aprobador o la función Revisor y Aprobador mediante Flujo de trabajo automatizado, la solicitud de aprobación se muestra en la pestaña Aprobaciones de su Página principal o Mi área de trabajo. A continuación, puede ver la prueba y tomar una decisión de aprobación sobre la prueba directamente desde Workfront.

Para obtener información sobre cómo tomar decisiones de aprobación desde el área Mi trabajo, consulte [Aprobar trabajo desde el área de inicio](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) o [Aprobación del trabajo](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) en [Aprobación del trabajo](../../../review-and-approve-work/manage-approvals/approving-work.md).
