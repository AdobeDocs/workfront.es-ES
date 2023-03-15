---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba avanzada con un flujo de trabajo automatizado
description: Un flujo de trabajo automatizado facilita la administración del proceso de revisión si el proceso es complejo o si envía contenido para su revisión a las mismas personas regularmente. La prueba pasa de un escenario a otro y Adobe Workfront notifica a cada usuario cuando le toca revisarla. Para obtener más información sobre los flujos de trabajo automatizados, consulte Información general sobre los flujos de trabajo automatizados .
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 0%

---

# Creación de una prueba avanzada con un flujo de trabajo automatizado

Un flujo de trabajo automatizado facilita la administración del proceso de revisión si el proceso es complejo o si envía contenido para su revisión a las mismas personas regularmente. La prueba pasa de un escenario a otro y Adobe Workfront notifica a cada usuario cuando le toca revisarla. Para obtener más información sobre los flujos de trabajo automatizados, consulte [Resumen del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Seleccionar o superior</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
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

## Creación de una prueba avanzada con un flujo de trabajo automatizado

1. Vaya al proyecto, la tarea o el problema en el que desea la prueba y, a continuación, haga clic en el botón **Documentos** pestaña .
1. Haga clic en **Agregar nuevo** > Prueba, cargue el contenido y luego trabaje en las secciones enumeradas a continuación.

   o

   Pase el ratón sobre un documento existente y, a continuación, haga clic en la **Crear prueba** > **Prueba avanzada** y trabaje en las secciones enumeradas a continuación.

## Configuración de las etapas de prueba

1. En la sección Tipo de flujo de trabajo , elija **Automatizado**.
1. (Opcional) Si desea utilizar una plantilla de flujo de trabajo automatizado que el administrador de Workfront haya creado y compartido con usted, haga clic en **Agregar plantilla**, seleccione la plantilla en el cuadro que aparece y haga clic en **Agregar plantilla**.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente cuando utilice una plantilla Flujo de trabajo automatizado :
   >   
   >* La configuración de una plantilla Flujo de trabajo automatizado determina lo que puede hacer con el Flujo de trabajo automatizado para una prueba. Por ejemplo, si el botón Add a stage está desactivado en la plantilla, no está visible ya que se trabaja con la configuración de flujo de trabajo automatizado para la prueba.
   >* Cuando se añade una persona a un mensaje en una plantilla Flujo de trabajo automatizado , pero también ya está presente como revisor en la prueba, al aplicar la plantilla, se elimina al revisor de la fase. Si no agrega otro revisor a la fase, un mensaje le pedirá que añada uno.
   >* La capacidad de modificar una plantilla de flujo de trabajo automatizado depende de la configuración de la plantilla del administrador de Workfront, tal como se describe en . Si la capacidad de modificar la plantilla está deshabilitada, solo el propietario de la plantilla puede modificarla.


1. Configure la primera etapa del flujo de trabajo automatizado:

   1. (Opcional) Si desea crear un nombre para la primera etapa, haga clic en **Etapa 1** y, a continuación, escriba el nombre.
   1. En el **Destinatarios** para el escenario, agregue revisores al escenario.

      >[!NOTE]
      >Tenga en cuenta lo siguiente al agregar revisores a una etapa:
      >* Puede añadir usuarios externos a un escenario con una dirección de correo electrónico.
      >* Después de agregar un usuario a una etapa, puede configurar las opciones de ese usuario en la prueba.
      >* Puede arrastrar a los usuarios directamente a otro paso o a un escenario en el **Etapas** diagrama. Para seleccionar varios usuarios, pulse Mayús+Ctrl (en Windows) o Mayús+Comando (en Mac).
      >* Puede agregar un revisor a una prueba solo una vez, lo que significa que no puede agregar la misma persona a más de un paso de la prueba.
      >* Los revisores que no se agregan a un escenario privado no pueden ver ese escenario en la prueba o los comentarios realizados en ese escenario.
      >* De forma predeterminada, agregar un usuario a una etapa concede a ese usuario acceso para ver la prueba desde el momento en que se crea la prueba.\
      >  El administrador de Workfront puede restringir el acceso de los usuarios a la prueba hasta que el flujo de trabajo entre en la fase en la que se agregó el usuario.


   1. Haga clic en **Configuración de escenario**.
   1. Haga clic en **Activar etapa** para indicar cómo desea que se active el escenario.

      Para la primera etapa, solo puede seleccionar **Creación de pruebas**, **En una fecha y hora específicas** o **Manualmente**.

   1. (Condicional) Si ha seleccionado **En una fecha y hora específicas** en el paso anterior, seleccione la fecha y la hora en la que desea activar el escenario en la **Activar en** que aparece.

   1. Utilice cualquiera de las opciones siguientes para configurar aún más el escenario.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Establecer fecha límite</td>
         <td><p>Para establecer una fecha límite para el escenario, haga clic en una opción del <strong>Opciones de fecha límite</strong> lista desplegable. A continuación, debajo de <strong>Fecha límite</strong>, realice una de las siguientes acciones:</p>
          <ul>
           <li>Si elige <strong>Establecer fecha específica</strong>: Seleccione la fecha y la hora límite que desee.</li>
           <li>Si elige <strong>Calcular a partir de la fecha de activación del escenario</strong>: Seleccione el número de días hábiles que desea agregar a la fecha de activación de la etapa para determinar la fecha límite.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bloqueo del escenario</td>
         <td>Especifique cuándo se puede bloquear el escenario. </td>
        </tr>
        <tr>
         <td role="rowheader">Transferir derechos de decisión primaria a</td>
         <td><p>Seleccione el responsable de decisión primario en el escenario (disponible solo después de agregar al menos una persona a la fase que tenga una función de prueba de Aprobador o superior). Si selecciona un responsable de decisión principal, la variable <strong>Solo se requiere una decisión</strong> está desactivada en esta etapa.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Requerir solo una decisión para esta fase</td>
         <td>Finaliza todo el proceso de revisión cuando uno de los responsables de la toma de decisiones toma una decisión.<p>Esta opción no está disponible si ha designado un usuario en la variable <strong>Creador de decisiones principal</strong>menú desplegable.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Convertir este paso en privado</td>
         <td>Permite que solo las siguientes personas vean los comentarios y decisiones realizados durante esta fase: Supervisores, administradores de Workfront y administradores de Workfront Proof</td>
        </tr>
       </tbody>
      </table>

1. Para agregar y configurar otro paso:

   1. Haga clic en **Nueva etapa**.
   1. (Opcional) Si desea crear un nombre para la primera etapa, haga clic en **Etapa 2** (o **Etapa 3**, **Fase 4**, etc.), luego escriba el nombre.

   1. Haga clic en el **Activar etapa** y, a continuación, seleccione una opción para especificar si el escenario se activa automática o manualmente.

      Además de las opciones **Creación de pruebas**, **En una fecha y hora específicas** o **Manualmente**, puede seleccionar una opción que dependa de lo ocurrido en el paso anterior:

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Si ha seleccionado una opción de etapa de activación que depende de lo que se haya producido en el paso anterior, utilice las opciones que aparecen para configurar la configuración de activación.

      Por ejemplo, si seleccionó **Cuando cambia el estado de la etapa anterior**, seleccione **Etapa anterior** y, a continuación, seleccione el estado en la variable **El estado cambió a** en la ventana

1. Repita el paso anterior según sea necesario para agregar más etapas.

   A medida que se añaden etapas al flujo de trabajo automatizado, aparece un diagrama en la pantalla para representarlas:

   ![](assets/stages-diagram-350x213.png)

1. Continuar con [Configurar las opciones de correo electrónico para la prueba](#configure-email-settings-for-the-proof) más abajo.

## Configurar las opciones de correo electrónico para la prueba {#configure-email-settings-for-the-proof}

1. En el **Notificación por correo electrónico** , seleccione si desea enviar notificaciones por correo electrónico y un mensaje personalizado a los usuarios seleccionados en [Creación de una prueba avanzada con un flujo de trabajo automatizado](#workflow) anteriormente en este artículo:

   <table>
      <tbody>
      <tr>
      <td>Notificar a los destinatarios sobre esta prueba</td>
      <td>Seleccione esta opción para enviar una notificación por correo electrónico a los usuarios. When <strong>Uso compartido básico</strong> se selecciona en la variable <strong>Flujo de trabajo</strong> , se envía una notificación por correo electrónico cuando se crea la prueba. When <strong>Flujo de trabajo automatizado</strong> se selecciona en la variable <strong>Flujo de trabajo</strong> , se envía una notificación por correo electrónico cuando la prueba entra en la fase del flujo de trabajo automatizado al que está asociado el usuario.</td>
      </tr>
      <tr>
      <td>Añadir mensaje personalizado</td>
      <td>Seleccione esta opción para incluir un mensaje personalizado en la notificación. Puede especificar un asunto y un cuerpo del mensaje. El cuerpo del mensaje puede incluir formato de texto enriquecido, como negrita, viñetas e hipervínculos.</td>
      </tr>
      </tbody>
      </table>


1. Continuar con [Configuración de los ajustes de prueba](#configure-proof-settings) más abajo.

## Configuración de los ajustes de prueba {#configure-proof-settings}

1. En el **Configuración de prueba** seleccione cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Requerir inicio de sesión: la prueba solo se puede compartir con otros usuarios</td> 
      <td>Cuando esta opción está desactivada (opción predeterminada), cualquier persona con la URL puede ver la prueba. <br>Cuando se selecciona esta opción:
       <ul>
        <li>Solo los usuarios de Workfront Proof pueden ver la prueba.</li>
        <li>Los usuarios no pueden iniciar sesión en la prueba a menos que se hayan añadido a ella.</li>
        <li>Las suscripciones no se pueden habilitar.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solo se requiere una decisión para esta prueba</td> 
      <td>Cuando se selecciona esta opción, la revisión se completa después de que uno de los responsables de la toma de decisiones tome una decisión.<br>Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td>Los usuarios deben especificar su nombre de usuario y contraseña en el momento en que toman una decisión sobre una prueba.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear la prueba cuando se toman todas las decisiones necesarias</td> 
      <td>Cuando esta configuración está habilitada, el estado de prueba se bloquea después de tomar todas las decisiones. El estado se cambia automáticamente de desbloqueado a bloqueado cuando el aprobador final decide.<br>Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descargar archivo original</td> 
      <td>Cuando se selecciona esta opción, los revisores pueden descargar el archivo original desde el que se creó la prueba.<br>Cuando se anula la selección de esta opción, el icono Descargar deja de estar visible.<br>Esta opción está activada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comparta la prueba mediante una URL pública o código incrustado</td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suscripción a la prueba mediante URL pública o código incrustado</td> 
      <td>Cuando se selecciona esta opción, las personas que no se hayan agregado explícitamente a la prueba pueden suscribirse a la prueba. A la persona suscrita a la prueba se le concede la función y el correo electrónico que usted define en la siguiente configuración:
       <ul>
        <li><strong>Función del suscriptor:</strong> La función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba. </li>
        <li><strong>Configuración de alertas de correo electrónico para suscriptores:</strong> La alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la prueba.</li>
       </ul><p>
        <ul>
         <li><strong>Probar el acceso a través del vínculo de correo electrónico requerido para:</strong> Configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (no se requiere un vínculo de correo electrónico para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un enlace a la prueba por correo electrónico sin ninguna verificación), o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba; el objetivo de esta opción es asegurarse de que la persona ha introducido una dirección de correo electrónico correcta a la que tiene acceso).</li>
        </ul><p><strong>Nota:</strong> Si las pruebas tienen el flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación a los propietarios de la prueba, por lo que podrían decidir en qué fase se debe añadir a la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Crear prueba**.

   Workfront comienza a generar una prueba de los documentos o sitios web seleccionados. Según el tamaño y el tipo del archivo, el tiempo de retraso en la carga de un documento puede variar. Tenga paciencia, ya que los archivos más grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando su archivo. El tamaño máximo de carga de archivos es de 4 GB.

1. Una vez generada la prueba, haga clic en **Abrir prueba** para iniciar el visor de pruebas.

   ![](assets/open-proof-350x132.png)

   Los usuarios que no tengan las pruebas habilitadas en su cuenta podrán ver el documento y realizar comentarios en la prueba [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
