---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Configuración de acceso y suscripción para una prueba
description: Puede configurar ciertos ajustes de acceso y suscripción para pruebas individuales, como si se requiere que los usuarios inicien sesión y si se permite a los usuarios suscribirse a la prueba. Puede configurar la configuración de acceso y suscripción para una prueba mientras la crea, o puede configurarlas para una prueba que ya exista en Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 3%

---

# Configuración de acceso y suscripción para una prueba

Puede configurar ciertos ajustes de acceso y suscripción para pruebas individuales, como si se requiere que los usuarios inicien sesión y si se permite a los usuarios suscribirse a la prueba. Puede configurar la configuración de acceso y suscripción para una prueba mientras la crea, o puede configurarlas para una prueba que ya exista en Workfront.

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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Configuración de acceso y suscripción al crear una prueba

Para configurar la configuración de acceso y suscripción de una prueba mientras la crea:

1. Vaya al proyecto, la tarea o el problema en el que desea la prueba y, a continuación, haga clic en el botón **Documentos** para obtener más información.
1. Haga clic en **Agregar nuevo** en el área superior derecha.
1. Desplácese hasta el **Configuración de prueba** en la esquina inferior derecha de la **Nueva prueba** página.

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
      <td>Cuando se selecciona esta opción, las personas que no se hayan agregado explícitamente a la prueba pueden suscribirse a la prueba. A la persona suscrita a la prueba se le concede la función y el correo electrónico que usted define en la siguiente configuración:
       <ul>
        <li><p><strong>Función del suscriptor:</strong> La función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba. </p><p>Importante: If <strong>Permitir uso compartido con</strong> se configura en cualquier valor que no sea <strong>Todos</strong> en la configuración de prueba de Workfront, la suscripción solo funciona para personas de la organización. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuración de pruebas en Workfront Proof</a>.</p></li>
        <li><strong>Configuración de alertas de correo electrónico para suscriptores:</strong> La alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la prueba.</li>
       </ul><p>
        <ul>
         <li><strong>Probar el acceso a través del vínculo de correo electrónico requerido para:</strong> Configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (no se requiere un vínculo de correo electrónico para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un enlace a la prueba por correo electrónico sin ninguna verificación), o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba; el objetivo de esta opción es asegurarse de que la persona ha introducido una dirección de correo electrónico correcta a la que tiene acceso).</li>
        </ul><p>Nota:  Si las pruebas tienen el flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación a los propietarios de la prueba, por lo que podrían decidir en qué fase se debe añadir a la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe creando la prueba.

## Configuración de acceso y suscripción para una prueba existente

Para configurar la configuración de acceso y suscripción de una prueba que ya existe en Workfront:

1. En el área Documentos, seleccione el documento que contiene la prueba para la que desea configurar la configuración y, a continuación, haga clic en **Detalles del documento**.
1. En el panel izquierdo, haga clic en **Configuración del visor de pruebas**.
1. Configure las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Permitir el uso compartido de pruebas mediante una URL pública o código incrustado</strong><strong>e</strong> </td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Permitir la suscripción a la revisión mediante una dirección URL pública o código para insertar</strong> </td> 
      <td>Cuando se selecciona esta opción, las personas que no se hayan agregado explícitamente a la prueba pueden suscribirse a la prueba. A la persona suscrita a la prueba se le concede la función y el correo electrónico que usted define en la siguiente configuración:
       <ul>
        <li><p><strong>Función del suscriptor:</strong> La función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba. </p><p>Importante: If <strong>Permitir uso compartido con</strong> se configura en cualquier valor que no sea <strong>Todos</strong> en la configuración de prueba de Workfront, la suscripción solo funciona para personas de la organización. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuración de pruebas en Workfront Proof</a>.</p></li>
        <li><strong>Configuración de alertas de correo electrónico para suscriptores:</strong> La alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la prueba.</li>
       </ul><p>
        <ul>
         <li><strong>Probar el acceso a través del vínculo de correo electrónico requerido para:</strong> Configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (no se requiere un vínculo de correo electrónico para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un enlace a la prueba por correo electrónico sin ninguna verificación), o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba; el objetivo de esta opción es asegurarse de que la persona ha introducido una dirección de correo electrónico correcta a la que tiene acceso).</li>
        </ul><p>Nota:  Si las pruebas tienen el flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación a los propietarios de la prueba, por lo que podrían decidir en qué fase se debe añadir a la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
