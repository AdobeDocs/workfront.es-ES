---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Editar configuración de prueba
description: Después de crear una prueba, puede editar la configuración de la prueba en cualquier momento.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 7%

---

# Editar configuración de prueba

Después de crear una prueba, puede editar la configuración de la prueba en cualquier momento.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
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
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Editar configuración de prueba

Algunos ajustes pueden bloquearse si el administrador de Workfront los ha deshabilitado en la cuenta.

1. Vaya al proyecto, la tarea o el problema en el que desea la prueba y, a continuación, haga clic en el botón **Documentos** pestaña .
1. Pase el ratón sobre la prueba y, a continuación, haga clic en **Detalles del documento**.
1. En el panel izquierdo, haga clic en **Configuración del visor de pruebas**.
1. Ajuste la siguiente configuración:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Se requiere el inicio de sesión. Esta revisión no se puede compartir con usuarios invitados</td> 
      <td> <p>Si necesita niveles más altos de seguridad para el proceso de revisión y aprobación, puede usar requerir inicio de sesión en la prueba. Esto significa que solo se pueden agregar usuarios de Workfront a la prueba. Deben introducir su correo electrónico y contraseña para poder acceder a él.</p> <p>Nota: <em style="font-style: normal;">Si el Inicio de sesión requerido está habilitado, las suscripciones no se pueden habilitar.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td> <p>Puede requerir una firma electrónica de cualquier revisor que tome una decisión sobre la prueba. Cuando un revisor toma una decisión, aparece un mensaje pidiendo que introduzca su correo electrónico y contraseña y que confirme su decisión. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear la prueba cuando se toman todas las decisiones necesarias</td> 
      <td> <p>Puede establecer un estado de prueba para que se bloquee cuando el Aprobador final tome su decisión. Esto resulta útil si desea asegurarse de que los revisores no puedan volver a la prueba y agregar comentarios adicionales o cambiar sus decisiones.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la descarga del archivo original</td> 
      <td> <p>Puede permitir que los revisores de una prueba descarguen el archivo original desde el que se creó una prueba. Esta opción está activada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que se comparta la revisión mediante una dirección URL pública o código para insertar</td> 
      <td>Puede permitir a los usuarios compartir la prueba con una URL pública o un código incrustado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la suscripción a la revisión mediante una dirección URL pública o código para insertar</td> 
      <td> <p>La activación de la suscripción en la prueba permite que las personas que no se hayan añadido explícitamente a la prueba se suscriban a la prueba (es decir, se añadan a la prueba). A continuación, se les asignará la función y la alerta de correo electrónico que seleccione para ellos en la configuración de suscripción.</p> <p>Si la suscripción se ha habilitado en una prueba, los campos siguientes se activarán:</p> 
       <ul> 
        <li><strong>Se requiere la validación del suscriptor</strong> - El suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba<br>Si selecciona esta opción, la persona que se suscriba no obtendrá acceso inmediato a la prueba, pero obtendrá un vínculo a la prueba en un mensaje de correo electrónico. El propósito de la validación del suscriptor es garantizar que la persona ha introducido una dirección de correo electrónico correcta a la que tiene acceso.</li> 
        <li><strong>Función predeterminada para los nuevos suscriptores:</strong> Esta es la función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba.</li> 
        <li><strong>Alerta de correo electrónico predeterminada para nuevos suscriptores</strong> : Esta es la alerta de correo electrónico predeterminada que se asigna a todos los revisores que se suscriben a la prueba.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

 
