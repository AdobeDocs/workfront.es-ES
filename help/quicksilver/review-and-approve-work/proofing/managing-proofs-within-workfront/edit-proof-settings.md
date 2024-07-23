---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Editar configuración de revisión
description: Puede editar la configuración de prueba en cualquier momento después de crearla.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 7%

---

# Editar configuración de revisión

Puede editar la configuración de prueba en cualquier momento después de crearla.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td role="rowheader">Función de prueba</td> 
   <td>Autor o moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Editar configuración de revisión

Algunas configuraciones pueden bloquearse si el administrador de Workfront las deshabilita en el nivel de cuenta.

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la ficha **Documentos**.
1. Pase el ratón sobre la revisión y luego haga clic en **Detalles del documento**.
1. En el panel izquierdo, haga clic en **Configuración del visor de revisiones**.
1. Ajuste la siguiente configuración:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Se requiere el inicio de sesión. Esta revisión no se puede compartir con usuarios invitados</td> 
      <td> <p>Si necesita niveles más altos de seguridad para el proceso de revisión y aprobación, puede utilizar requerir el inicio de sesión en la prueba. Esto significa que solo se pueden añadir usuarios de Workfront a la revisión. Deben introducir su correo electrónico y contraseña antes de poder acceder a ellos.</p> <p>Nota: <em style="font-style: normal;">Si el inicio de sesión necesario está habilitado, las suscripciones no se pueden habilitar.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td> <p>Puede requerir una firma electrónica de cualquier revisor que tome una decisión sobre la prueba. Cuando un revisor toma una decisión, aparece un mensaje pidiéndole que introduzca su correo electrónico y contraseña y que confirme su decisión. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear la revisión cuando se tomen todas las decisiones necesarias</td> 
      <td> <p>Puede establecer un estado de prueba para que se bloquee cuando el aprobador final tome su decisión. Esto resulta útil si desea asegurarse de que los revisores no puedan volver a la prueba y agregar comentarios adicionales o cambiar sus decisiones.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la descarga del archivo original</td> 
      <td> <p>Puede permitir que los revisores de una prueba descarguen el archivo original desde el que se creó la prueba. Esta opción está habilitada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que se comparta la revisión mediante una dirección URL pública o código para insertar</td> 
      <td>Puede permitir que los usuarios compartan la prueba con una URL pública o un código incrustado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la suscripción a la revisión mediante una dirección URL pública o código para insertar</td> 
      <td> <p>Al habilitar la suscripción en la prueba, las personas que no se hayan agregado explícitamente a la prueba pueden suscribirse a ella (es decir, agregarse a la prueba). A continuación, se les asignará la función y la alerta de correo electrónico que seleccione para ellos en la Configuración de suscripción.</p> <p>Si la suscripción se ha habilitado en una prueba, los campos siguientes se activarán:</p> 
       <ul> 
        <li><strong>Se requiere la validación del suscriptor</strong> - El suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba<br>Al seleccionar esta opción, la persona que se suscriba no obtendrá acceso inmediato a la prueba, pero recibirá un vínculo a la prueba en un mensaje de correo electrónico. El propósito de la validación del suscriptor es garantizar que la persona haya introducido una dirección de correo electrónico correcta a la que tenga acceso.</li> 
        <li><strong>Función predeterminada para los nuevos suscriptores -</strong> Esta es la función de prueba predeterminada que se asignará a todos los revisores que se suscriban a la prueba.</li> 
        <li><strong>Alerta de correo electrónico predeterminada para nuevos suscriptores</strong>: esta es la alerta de correo electrónico predeterminada que se asignará a todos los revisores que se suscriban a la prueba.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

 
