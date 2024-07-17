---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Configuración de acceso y suscripción para una prueba
description: Puede configurar ciertos ajustes de acceso y suscripción para pruebas individuales, como exigir a los usuarios que inicien sesión y permitir que se suscriban a la prueba. Puede configurar los ajustes de acceso y suscripción de una prueba mientras la está creando, o bien puede configurarlos para una prueba que ya existe en Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Configuración de acceso y suscripción para una prueba

Puede configurar ciertos ajustes de acceso y suscripción para pruebas individuales, como exigir a los usuarios que inicien sesión y permitir que se suscriban a la prueba. Puede configurar los ajustes de acceso y suscripción de una prueba mientras la está creando, o bien puede configurarlos para una prueba que ya existe en Workfront.

## Requisitos de acceso

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
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Configuración de acceso y suscripción al crear una prueba

Para configurar los ajustes de acceso y suscripción de una prueba mientras la está creando:

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la sección **Documentos**.
1. Haga clic en **Agregar nuevo** en el área superior derecha.
1. Desplácese a la sección **Configuración de prueba** en la esquina inferior derecha de la página **Nueva prueba**.

1. Configure las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Permitir que se comparta la revisión mediante una dirección URL pública o código para insertar</strong> </td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Permitir la suscripción a la revisión mediante una dirección URL pública o código para insertar</strong> </td> 
      <td>Si se selecciona esta opción, las personas que no se hayan añadido explícitamente a la prueba podrán suscribirse a ella. A la persona que se suscribe a la prueba se le concede la función y el correo electrónico que defina en la siguiente configuración:
       <ul>
        <li><p><strong>Rol de suscriptor:</strong> El rol de prueba predeterminado que se asigna a todos los revisores que se suscriben a la prueba. </p><p>Importante: Si <strong>Permitir que se comparta con</strong> se establece en cualquier valor distinto de <strong>Todos</strong> en la configuración de Workfront Proof, la suscripción solo funcionará para las personas de la organización. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurar opciones de revisión en Workfront Proof</a>.</p></li>
        <li><strong>Configuración de alertas de correo electrónico para suscriptores:</strong> La alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la revisión.</li>
       </ul><p>
        <ul>
         <li><strong>Se requiere acceso a la prueba mediante un vínculo de correo electrónico para:</strong> Configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (el vínculo de correo electrónico no es necesario para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico sin ninguna verificación) o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba, el propósito de esta opción es garantizar que la persona haya escrito una dirección de correo electrónico correcta a la que tenga acceso).</li>
        </ul><p>Nota:  Si las pruebas tienen un flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación a los propietarios de la prueba para que puedan decidir a qué fase se debe agregar a la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe creando la revisión.

## Configuración de acceso y suscripción para una revisión existente

Para configurar los ajustes de acceso y suscripción de una revisión que ya existe en Workfront:

1. En el área Documentos, seleccione el documento que contiene la revisión para la que desea establecer la configuración y haga clic en **Detalles del documento**.
1. En el panel izquierdo, haga clic en **Configuración del visor de revisiones**.
1. Configure las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Permitir que se comparta la revisión mediante una dirección URL pública o código para insertar</strong><strong>e</strong> </td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Permitir la suscripción a la revisión mediante una dirección URL pública o código para insertar</strong> </td> 
      <td>Si se selecciona esta opción, las personas que no se hayan añadido explícitamente a la prueba podrán suscribirse a ella. A la persona que se suscribe a la prueba se le concede la función y el correo electrónico que defina en la siguiente configuración:
       <ul>
        <li><p><strong>Rol de suscriptor:</strong> El rol de prueba predeterminado que se asigna a todos los revisores que se suscriben a la prueba. </p><p>Importante: Si <strong>Permitir que se comparta con</strong> se establece en cualquier valor distinto de <strong>Todos</strong> en la configuración de Workfront Proof, la suscripción solo funcionará para las personas de la organización. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurar opciones de revisión en Workfront Proof</a>.</p></li>
        <li><strong>Configuración de alertas de correo electrónico para suscriptores:</strong> La alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la revisión.</li>
       </ul><p>
        <ul>
         <li><strong>Se requiere acceso a la prueba mediante un vínculo de correo electrónico para:</strong> Configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (el vínculo de correo electrónico no es necesario para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico sin ninguna verificación) o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba, el propósito de esta opción es garantizar que la persona haya escrito una dirección de correo electrónico correcta a la que tenga acceso).</li>
        </ul><p>Nota:  Si las pruebas tienen un flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación a los propietarios de la prueba para que puedan decidir a qué fase se debe agregar a la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
