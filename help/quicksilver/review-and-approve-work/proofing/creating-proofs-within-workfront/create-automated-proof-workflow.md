---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Crear una revisión avanzada con un flujo de trabajo automatizado
description: Un flujo de trabajo automatizado facilita la administración del proceso de revisión si el proceso es complejo o si envía contenido para su revisión a las mismas personas con regularidad. La revisión pasa de una fase a otra y Adobe Workfront notifica a cada usuario cuándo es su turno de revisarla. Para obtener más información sobre los flujos de trabajo automatizados, consulte Información general de flujo de trabajo automatizado.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 99%

---

# Crear una revisión avanzada con un flujo de trabajo automatizado

<!-- Audited: 2/2024 -->

Un flujo de trabajo automatizado facilita la administración del proceso de revisión si el proceso es complejo o si envía contenido para su revisión a las mismas personas con regularidad. La revisión pasa de una fase a otra y Adobe Workfront notifica a cada usuario cuándo es su turno de revisarla. Para obtener más información sobre los flujos de trabajo automatizados, consulte [Información general de flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Nuevo: cualquiera</p><p>Plan actual: Pro o superior</p><p>Plan heredado: Select o superior</p> <p>Para obtener más información sobre el acceso de revisión en los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar</p><p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una revisión avanzada con un flujo de trabajo automatizado

1. Vaya al proyecto, tarea o problema donde desee la revisión y, a continuación, haga clic en la pestaña **Documentos**.
1. Haga clic en **Añadir nuevo** > Revisión, cargue el contenido y trabaje en las secciones que se indican a continuación.

   o

   Pase el puntero por encima de un documento existente, haga clic en **Crear revisión** > **Revisión avanzada** y trabaje en las secciones que se indican a continuación.

## Configuración de las fases de revisión

1. En la sección Tipo de flujo de trabajo, elija **Automatizado**.
1. (Opcional) Si desea usar una plantilla de flujo de trabajo automatizado que el administrador de Workfront haya creado y compartido con usted, haga clic en **Añadir plantilla**, seleccione la plantilla en el cuadro que aparece y, a continuación, haga clic en **Añadir plantilla**.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente cuando utilice una plantilla de flujo de trabajo automatizado:
   >   
   >* La configuración de una plantilla de flujo de trabajo automatizado determina lo que puede hacer con el flujo de trabajo automatizado para una revisión. Por ejemplo, si el botón Añadir fase está deshabilitado en la plantilla, no estará visible mientras trabaja con la configuración del flujo de trabajo automatizado para la revisión.
   >* Cuando se añade una persona a una fase en una plantilla de flujo de trabajo automatizado, pero también está presente como revisor en la revisión, al aplicar la plantilla se elimina al revisor de la fase. Si no añade otro revisor a la fase, aparecerá un mensaje que le pide que añada uno.
   >* La posibilidad de modificar una plantilla de flujo de trabajo automatizado depende de la configuración de la plantilla que establezca el administrador de Workfront, tal como se describe en . Si la capacidad para modificar la plantilla está deshabilitada, solo el propietario de la plantilla puede modificarla.

1. Configure la primera fase del flujo de trabajo automatizado:

   1. (Opcional) Si desea crear un nombre para la primera fase, haga clic en **Fase 1** y, a continuación, escriba el nombre.
   1. En la sección **Destinatarios** de la fase, añada revisores a la fase.

      >[!NOTE]
      >
      >Tenga en cuenta lo siguiente al añadir revisores a una fase:
      >   
      >* Puede añadir usuarios externos a una fase con una dirección de correo electrónico.
      >* Después de añadir un usuario a una fase, puede establecer la configuración de ese usuario en la revisión.
      >* Puede arrastrar a los usuarios directamente a otra fase o arrastrarlos a una fase del diagrama **Fases**. Para seleccionar varios usuarios, presione Mayús+Ctrl (en Windows) o Mayús+Comando (en Mac).
      >* Puede añadir un revisor a una revisión solo una vez, lo que significa que no puede añadir a la misma persona a más de una fase de la revisión.
      >* Los revisores que no se añaden a una fase privada no pueden ver esa fase en la revisión ni en los comentarios realizados en esa fase.
      >* De forma predeterminada, al añadir un usuario a una fase se concede a ese usuario acceso para ver la prueba desde el momento de su creación. El administrador de Workfront puede restringir el acceso de los usuarios a la prueba hasta que el flujo de trabajo entre en la fase en la que se añadió el usuario.

   1. Haga clic en **Configuración de la fase**.
   1. Haga clic en una opción **Activar fase** para indicar cómo desea que se active la fase.

      En la primera fase, solo puede seleccionar **Creación de revisión**, **En una fecha y hora específicas** o **Manualmente**.

   1. (Condicional) Si seleccionó **En una fecha y hora específicas** en el paso anterior, seleccione la fecha y la hora en que desea activar el escenario en el cuadro **Activar el** que aparece.

   1. Utilice cualquiera de las opciones siguientes para más configuraciones de la fase.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Establecer una fecha límite para la fase</td>
         <td><p>Para establecer una fecha límite para la fase, haga clic en una opción de la lista desplegable <strong>Opciones de fecha límite</strong>. A continuación, en <strong>Fecha límite</strong>, realice una de las siguientes acciones:</p>
          <ul>
           <li>Si elige <strong>Establecer fecha específica</strong>: seleccione la fecha y la hora límite que desee.</li>
           <li>Si elige <strong>Calcular a partir de la fecha de activación de la fase</strong>: seleccione el número de días laborables que desea añadir a la fecha de activación de la fase para determinar la fecha límite.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bloquear fase</td>
         <td>Especifique cuándo se puede bloquear la fase. </td>
        </tr>
        <tr>
         <td role="rowheader">Transferir derechos de decisión principales a</td>
         <td><p>Seleccione el responsable de la toma de decisiones principal de la fase (solo disponible después de añadir al menos una persona a la fase que tenga la función de prueba de Aprobador o superior). Si selecciona un responsable de la toma de decisiones principal, se deshabilita la opción <strong>Solo se requiere una decisión</strong> en este escenario.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Requerir solo una decisión para esta fase</td>
         <td>Finaliza todo el proceso de revisión cuando uno de los responsables de la toma de decisiones toma una decisión.<p>Esta opción no está disponible si ha designado un usuario en el menú desplegable <strong>Responsable principal de la toma de decisiones</strong>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Convertir esta fase en privada</td>
         <td>Permite que solo supervisores, administradores de Workfront y administradores de Workfront Proof vean los comentarios y las decisiones tomadas durante esta fase</td>
        </tr>
       </tbody>
      </table>

1. Para añadir y configurar otra fase, haga lo siguiente:

   1. Haga clic en **Nueva fase**.
   1. (Opcional) Si desea crear un nombre para la primera fase, haga clic en **Fase 2** (o **Fase 3**, **Fase 4**, etc.) y luego escriba el nombre.

   1. Haga clic en **Activar fase** y, a continuación, seleccione una opción para especificar si la fase se activará automática o manualmente.

      Además de las opciones **Creación de revisión**, **En una fecha y hora específicas** o **Manualmente**, puede seleccionar una opción que dependa de lo que haya ocurrido en el paso anterior:

      ![Activar opciones de fase](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Si seleccionó una opción Activar fase que depende de lo ocurrido en el paso anterior, utilice las opciones que aparecen para configurar la configuración de activación.

      Por ejemplo, si seleccionó **Cuando cambia el estado de la fase anterior**, seleccione la **Fase anterior** y luego seleccione el estado en el cuadro **Estado cambiado a**.

1. Repita el paso anterior según sea necesario para añadir más etapas.

   A medida que se añaden fases al flujo de trabajo automatizado, se forma un diagrama en la pantalla para representarlas:

   ![Diagrama de etapas](assets/stages-diagram-350x213.png)

1. Continúe con [Configurar opciones de correo electrónico para la revisión](#configure-email-settings-for-the-proof) que se muestra a continuación.

## Configurar opciones de correo electrónico para la revisión {#configure-email-settings-for-the-proof}

1. En la sección **Notificaciones por correo electrónico**, seleccione si desea enviar notificaciones por correo electrónico y un mensaje personalizado a los usuarios seleccionados en [Crear una prueba avanzada con un flujo de trabajo automatizado](#workflow), descrito anteriormente en este artículo:

   <table>
      <tbody>
      <tr>
      <td>Notificar a los destinatarios sobre esta prueba</td>
      <td>Seleccione esta opción para enviar una notificación por correo electrónico a los usuarios. Cuando se selecciona <strong>Uso compartido básico</strong> en la sección <strong>Flujo de trabajo</strong>, se envía una notificación por correo electrónico cuando se crea la prueba. Cuando se selecciona <strong>Flujo de trabajo automatizado</strong> en la sección <strong>Flujo de trabajo</strong>, se envía una notificación por correo electrónico cuando la prueba entra en la fase del flujo de trabajo automatizado con el que se asocia el usuario.</td>
      </tr>
      <tr>
      <td>Añadir mensaje personalizado</td>
      <td>Seleccione esta opción para incluir un mensaje personalizado en la notificación. Puede especificar el asunto y el cuerpo del mensaje. El cuerpo del mensaje puede incluir formato de texto enriquecido, como negrita, viñetas e hipervínculos.</td>
      </tr>
      </tbody>
      </table>


1. Continúe con [Configurar opciones de prueba](#configure-proof-settings) que se muestra a continuación.

## Configurar opciones de prueba {#configure-proof-settings}

1. En la sección **Configuración de prueba**, seleccione cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Inicio de sesión obligatorio: la prueba solo se puede compartir con otros usuarios</td> 
      <td>Cuando esta opción está deshabilitada (predeterminada), cualquier persona con la URL puede ver la prueba. <br>Cuando se selecciona esta opción:
       <ul>
        <li>Solo los usuarios de Workfront Proof pueden ver la prueba.</li>
        <li>Los usuarios no pueden iniciar sesión en la prueba a menos que se les haya añadido a la prueba.</li>
        <li>No se pueden habilitar las suscripciones.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solo se requiere una decisión para esta prueba</td> 
      <td>Cuando se selecciona esta opción, la prueba se completa después de que uno de los responsables de la toma de decisiones tome su decisión.<br>Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td>Los usuarios deben especificar su nombre de usuario y contraseña en el momento en que tomen una decisión sobre una prueba.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prueba cuando se toman todas las decisiones necesarias</td> 
      <td>Cuando esta configuración está habilitada, el estado de prueba se bloquea después de que se hayan tomado todas las decisiones. El estado cambia automáticamente de desbloqueado a bloqueado cuando el aprobador final toma su decisión.<br>Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descargar archivo original</td> 
      <td>Cuando se selecciona esta opción, los revisores pueden descargar el archivo original desde el que se creó la prueba.<br>Cuando esta opción no está seleccionada, el icono Descargar ya no es visible.<br>Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que se comparta la prueba mediante una dirección URL pública o código incrustado</td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suscribirse a la prueba mediante una dirección URL pública o código incrustado</td> 
      <td>Si se selecciona esta opción, las personas que no se hayan añadido explícitamente a la prueba podrán suscribirse a ella. A la persona que se suscribe a la prueba se le concede la función y el correo electrónico que defina en la siguiente configuración:
       <ul>
        <li><strong>Función de suscriptor:</strong> la función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba.</li>
        <li><strong>Configuración de alertas de correo electrónico para suscriptores:</strong> la alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la revisión.</li>
       </ul><p>
        <ul>
         <li><strong>Se requiere acceso a la prueba mediante vínculo de correo electrónico para:</strong> configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (el vínculo de correo electrónico no es necesario para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico sin ninguna verificación) o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba, el propósito de esta opción es garantizar que la persona haya escrito una dirección de correo electrónico correcta a la que tenga acceso).</li>
        </ul><p><strong>Nota:</strong> Si las pruebas tienen un flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación a los propietarios de la prueba para que puedan decidir a qué fase se debe añadir a la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Crear prueba**.

   Workfront comienza a generar una prueba de los documentos o sitios web seleccionados. Según el tamaño y el tipo de archivo, el tiempo de retraso de la carga de un documento puede variar. Tenga en cuenta que los archivos grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando el archivo. El tamaño máximo de carga del archivo es de 4 GB.

1. Una vez generada la prueba, haga clic en **Abrir prueba** para iniciar el visor de corrección.

   ![Abrir revisión](assets/open-proof-350x132.png)

   Los usuarios que no tengan habilitada la revisión en su cuenta aún pueden ver el documento y realizar comentarios en la prueba [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
