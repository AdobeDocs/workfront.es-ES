---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Editar la configuración de una revisión
description: Puede editar la configuración de una prueba en cualquier momento después de crearla.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: a036a99c13d80a2ba2305ebcdc799ad6e5b62b39
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 100%

---

# Editar la configuración de una revisión

Puede editar la configuración de una prueba en cualquier momento después de crearla.

## Requisitos de acceso

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
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Función de prueba</td> 
   <td>Autor o moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Editar la configuración de una revisión

Algunas configuraciones pueden bloquearse si el administrador de Workfront las deshabilita a nivel de cuenta.

1. Vaya al proyecto, tarea o problema donde desee la revisión y, a continuación, haga clic en la pestaña **Documentos**.
1. Pase el ratón sobre la revisión y luego haga clic en **Detalles del documento**.
1. En el panel izquierdo, haga clic en **Configuración del visor de corrección**.
1. Ajuste la siguiente configuración:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Se requiere el inicio de sesión. Esta revisión no se puede compartir con usuarios invitados</td> 
      <td> <p>Si necesita niveles más altos de seguridad para el proceso de revisión y aprobación, puede requerir el inicio de sesión en la revisión. Esto significa que solo se pueden añadir usuarios de Workfront a la revisión. Deben introducir su correo electrónico y contraseña antes de poder acceder.</p> <p>Nota: <em style="font-style: normal;">Si se ha habilitado que el inicio de sesión sea necesario, las suscripciones no se pueden habilitar.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td> <p>Puede requerir la firma electrónica de cualquier revisor que tome una decisión sobre la revisión. Cuando un revisor toma una decisión, aparece un mensaje pidiéndole que introduzca su correo electrónico y contraseña y que confirme su decisión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prueba cuando se toman todas las decisiones necesarias</td> 
      <td> <p>Puede establecer que un estado de revisión se bloquee cuando el aprobador final tome su decisión. Esto resulta útil si desea asegurarse de que los revisores no puedan volver a la revisión y añadir comentarios adicionales o cambiar sus decisiones.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la descarga del archivo original</td> 
      <td> <p>Puede permitir que los revisores de una revisión descarguen el archivo original desde el que se creó la revisión. Esta opción está activada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que se comparta la revisión mediante una dirección URL pública o código incrustado</td> 
      <td>Puede permitir que los usuarios compartan la revisión con una URL pública o un código incrustado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la suscripción a la revisión mediante una dirección URL pública o código incrustado</td> 
      <td> <p>Al habilitar la suscripción en la revisión, los usuarios que no se hayan añadido explícitamente a la revisión pueden suscribirse a ella (es decir, añadirse a la revisión). A continuación, se les asignará la función y la alerta de correo electrónico que seleccione para ellos en la Configuración de suscripción.</p> <p>Si se ha habilitado la suscripción en una revisión, los campos siguientes se activarán:</p> 
       <ul> 
        <li><strong>Se requiere la validación del suscriptor</strong>: el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una revisión<br>Al seleccionar esta opción, la persona que se suscriba no obtendrá acceso inmediato a la revisión, pero recibirá un vínculo a la misma en un mensaje de correo electrónico. El propósito de la validación del suscriptor es garantizar que la persona haya introducido una dirección de correo electrónico correcta a la que tenga acceso.</li> 
        <li><strong>Función predeterminada para los nuevos suscriptores:</strong> esta es la función de revisión predeterminada que se asignará a todos los revisores que se suscriban a la revisión.</li> 
        <li><strong>Alerta de correo electrónico predeterminada para nuevos suscriptores</strong>: esta es la alerta de correo electrónico predeterminada que se asignará a todos los revisores que se suscriban a la revisión.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

 
