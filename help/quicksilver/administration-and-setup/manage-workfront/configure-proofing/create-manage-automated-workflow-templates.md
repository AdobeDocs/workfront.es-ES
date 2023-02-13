---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Creación y administración de plantillas de flujo de trabajo automatizadas
description: Como administrador de Adobe Workfront, si el proceso de revisión de contenido de su organización a menudo se repite o las mismas personas suelen revisar el contenido, puede crear plantillas de flujo de trabajo automatizado que contengan estos revisores con las funciones de prueba y la configuración de notificación que especifique. Una plantilla de flujo de trabajo automatizado puede ser sencilla con solo uno o dos revisores o compleja con muchas etapas y dependencias.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# Creación y administración de plantillas de flujo de trabajo automatizadas

Como administrador de Adobe Workfront, si el proceso de revisión de contenido de su organización a menudo se repite o las mismas personas suelen revisar el contenido, puede crear plantillas de flujo de trabajo automatizado que contengan estos revisores con las funciones de prueba y la configuración de notificación que especifique. Una plantilla de flujo de trabajo automatizado puede ser sencilla con solo uno o dos revisores o compleja con muchas etapas y dependencias.

Las plantillas de flujo de trabajo automatizados facilitan la creación de una prueba con un flujo de trabajo automatizado. Cuando un usuario crea una prueba, simplemente elige la plantilla que necesita.

Puede cambiar fácilmente cualquier plantilla de flujo de trabajo automatizado, agregando o eliminando revisores y etapas, en cualquier momento. Además, los creadores de prueba que utilicen la plantilla pueden agregar o eliminar revisores para la prueba.

Tenga en cuenta lo siguiente cuando utilice una plantilla Flujo de trabajo automatizado :

1. La configuración de una plantilla Flujo de trabajo automatizado determina lo que puede hacer con el Flujo de trabajo automatizado para una prueba. Por ejemplo, si el botón Add a stage está desactivado en la plantilla, no está visible ya que se trabaja con la configuración de flujo de trabajo automatizado para la prueba.
1. Cuando se añade una persona a un mensaje en una plantilla Flujo de trabajo automatizado , pero también ya está presente como revisor en la prueba, al aplicar la plantilla, se elimina al revisor de la fase. Si no agrega otro revisor a la fase, un mensaje le pedirá que añada uno.
1. La capacidad de modificar una plantilla de flujo de trabajo automatizado depende de la configuración de la plantilla del administrador de Workfront, tal como se describe en . Si la capacidad de modificar la plantilla está deshabilitada, solo el propietario de la plantilla puede modificarla.

Para obtener información sobre los flujos de trabajo automatizados, consulte [Resumen del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Premium o Select</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe tener el administrador seleccionado en el perfil de permisos de prueba. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuración del acceso de prueba de un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Creación de una plantilla de flujo de trabajo automatizado

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.
1. Haga clic en **Flujos de trabajo** en el panel izquierdo.
1. En el **Flujo de trabajo** , haga clic en **Nuevo** > **Nueva plantilla**.

1. En el **Detalles** especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de la plantilla</td> 
      <td>(Obligatorio) Escriba un nombre para la plantilla. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propietario de la plantilla</td> 
      <td>Puede seleccionar el administrador de Workfront o el administrador de prueba de Workfront que administrará la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de plantillas</td> 
      <td> <p> Si los flujos de trabajo automatizados de su organización están organizados en grupos, puede seleccionar el nombre del grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Crear grupos de plantillas de flujo de trabajo automatizado</a> más adelante en este artículo para obtener más información.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Zona horaria de plantilla </td> 
      <td> <p>La zona horaria predeterminada para la plantilla es la que está trabajando. Si la zona horaria de los creadores y revisores de prueba que van a utilizar la plantilla es diferente, puede cambiarla aquí para asegurarse de que los plazos de ensayo se establecen en los momentos adecuados para esos usuarios. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>Puede seleccionar las actividades de escenario que desee que estén disponibles para la persona que crea pruebas con la plantilla .</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Etapas** , configure cada etapa de la plantilla Flujo de trabajo automatizado .

   Puede añadir varias etapas y crear entre ellas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>El nombre del escenario aparece en el diagrama de flujo de trabajo automatizado en la parte superior de la sección Flujo de trabajo, en la página Detalles de prueba y en las notificaciones por correo electrónico enviadas a los revisores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activar etapa</td> 
      <td> <p>Especifique si el escenario se activa de forma automática o manual. Para la primera etapa, puede seleccionar <strong>Creación de pruebas</strong>, <strong>En una fecha y hora específicas</strong>o <strong>Manualmente</strong>.</p> <p>Las demás opciones estarán disponibles cuando agregue una segunda etapa, ya que requieren que seleccione una etapa principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha límite calculada a partir de</td> 
      <td> <p>Especifique cómo desea que se calcule la fecha límite:</p> 
       <ul> 
        <li> <p><strong>Creación de prueba</strong>: En la lista desplegable debajo de <strong>Plazo (+ días hábiles)</strong>, seleccione el número de días hábiles que desee agregar a la fecha de creación de la prueba para establecer automáticamente una fecha límite en la prueba.</p> </li> 
        <li><strong>Cuando comienza el escenario</strong>: En la lista desplegable debajo de <strong>Plazo (+ días hábiles)</strong>, seleccione el número de días hábiles que desee agregar a la fecha de activación del escenario para establecer automáticamente una fecha límite en la prueba.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloqueo del escenario</td> 
      <td>Especifique si desea permitir que el escenario se bloquee para comentarios. Las opciones son bloquear una etapa de forma manual o automática, ya sea cuando se inicie la siguiente etapa o cuando se tomen todas las decisiones en la etapa principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Responsable de toma de decisiones principal</td> 
      <td> <p>Los responsables de la toma de decisiones disponibles aparecen en la lista solo después de agregar los revisores a la fase.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solamente se requiere una decisión</td> 
      <td>El proceso de examen de la etapa se completará en cuanto uno de los encargados de adoptar decisiones presente su decisión. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuración de pruebas en Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fase privada</td> 
      <td>Oculta los comentarios y las decisiones de a las personas que no se agregan al escenario o que no son administradores de Workfront&lt;!&gt;— BORRADO EN FLARE: Supervisores y superiores

       -->. Para obtener más información, consulte &lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>Resumen del flujo de trabajo automatizado&lt;/a>.&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">No permitir que se elimine esta etapa</td> 
      <td> <p>Hace que la etapa sea obligatoria.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Si las pruebas que utilizan esta plantilla siempre se envían a las mismas personas en el escenario, agréguelas aquí para que los usuarios no tengan que agregarlas cada vez que creen una prueba.

   Elija el **Función** en las pruebas que utilizarán esta plantilla y la variable **Alertas de correo electrónico** desea que el usuario reciba cuando trabaje en pruebas que utilicen esta plantilla.

   Para obtener información sobre los roles de una prueba, consulte [Configuración de las funciones de prueba predeterminadas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Para obtener información sobre las alertas de correo electrónico de prueba, consulte la sección [Configuración de los valores predeterminados de prueba para un usuario](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) en el artículo  [Configuración de las notificaciones por correo electrónico en Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Cada usuario puede agregarse a una sola etapa. Puede agregar tantos usuarios como desee a un escenario.

   >[!TIP]
   >
   >Puede arrastrar y soltar nombres de revisores entre etapas en el diagrama de etapas. Los escenarios disponibles se resaltan en azul.

1. Repita los dos pasos anteriores para cualquier otra etapa que desee agregar a la plantilla.

   En la parte superior del **Flujo de trabajo** , puede ver un diagrama del flujo de trabajo automatizado que está configurando. A medida que continúa añadiendo etapas, aparecen en el diagrama con líneas que muestran las dependencias entre ellas. Puede hacer clic en un escenario del diagrama para ver la configuración de dicho escenario.

   Si no necesita ver el diagrama, puede hacer clic en **Ocultar diagrama**.

1. En el **Compartir plantilla con** , haga clic en una opción (si la plantilla no se ha compartido con toda la organización) para especificar quién puede utilizarla.

   De forma predeterminada, las nuevas plantillas de flujo de trabajo automatizado se comparten con todos los miembros de su organización.

1. Haga clic en **Crear**.

## Modificar una plantilla de flujo de trabajo automatizado

Como administrador de pruebas de Workfront, puede modificar una plantilla de flujo de trabajo automatizado. Los cambios se guardan automáticamente a medida que los realiza.

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.
1. Haga clic en **Flujos de trabajo** en el panel izquierdo.
1. En el **Plantillas de flujo de trabajo** que aparece, haga clic en la plantilla que desee modificar.
1. En el **Detalles** especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de la plantilla</td> 
      <td>(Obligatorio) Escriba un nombre para la plantilla. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propietario de la plantilla</td> 
      <td>Puede seleccionar el administrador de Workfront o el administrador de prueba de Workfront que administrará la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de plantillas</td> 
      <td> <p> Si los flujos de trabajo automatizados de su organización están organizados en grupos, puede seleccionar el nombre del grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Crear grupos de plantillas de flujo de trabajo automatizado</a> más adelante en este artículo para obtener más información.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zona horaria de plantilla </td> 
      <td> <p>La zona horaria predeterminada para la plantilla es la que está trabajando. Si la zona horaria de los creadores y revisores de prueba que van a utilizar la plantilla es diferente, puede cambiarla aquí para asegurarse de que los plazos de ensayo se establecen en los momentos adecuados para esos usuarios. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>Seleccione las actividades de escenario que desee que estén disponibles para los que crean pruebas con la plantilla . </p> <p><b>ADVERTENCIA</b>: Si no selecciona las opciones Añadir un escenario y Añadir personas a escenarios, ni el propietario de la plantilla ni el propietario de ninguna prueba que utilice esta plantilla podrán añadir un escenario ni compartir la prueba.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Flujo de trabajo** , cambie el nombre de cualquier escenario y amplíe su configuración ![](assets/arrow-button.png) para realizar los cambios necesarios:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fecha límite calculada a partir de</td> 
      <td> <p>Especifique cómo desea que se calcule la fecha límite:</p> 
       <ul> 
        <li> <p><strong>Plazo calculado a partir de la creación de la prueba</strong>: En el <strong>Establecer la fecha límite de la etapa</strong> en la lista desplegable, seleccione el número de días hábiles que desee agregar a la fecha de creación de la prueba para establecer automáticamente una fecha límite en la prueba.</p> </li> 
        <li><strong>Plazo calculado a partir de la activación de la etapa</strong>: En el <strong>Establecer la fecha límite de la etapa</strong> en la lista desplegable, seleccione el número de días hábiles que desee agregar a la fecha de activación del escenario para establecer automáticamente una fecha límite en la prueba.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activar etapa</td> 
      <td> <p>Especifique si el escenario se activa de forma automática o manual. Para la primera etapa, puede seleccionar <strong>Creación de pruebas</strong>, <strong>En una fecha y hora específicas</strong>o <strong>Manualmente</strong>.</p> <p>Las demás opciones estarán disponibles cuando agregue una segunda etapa, ya que requieren que seleccione una etapa principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloqueo del escenario</td> 
      <td>Especifique si desea permitir que el escenario se bloquee para comentarios. Las opciones son bloquear una etapa de forma manual o automática, ya sea cuando se inicie la siguiente etapa o cuando se tomen todas las decisiones en la etapa principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisión</td> 
      <td>Finaliza la etapa la primera vez que uno de los responsables de la toma de decisiones presenta su decisión. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuración de pruebas en Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacidad</td> 
      <td>Oculta comentarios y decisiones de a personas que no se añaden al escenario o que no son supervisores o superiores en la cuenta. Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminación de escenario</td> 
      <td>Hace que la etapa sea obligatoria.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Más <img src="assets/more-icon.png"></td> 
      <td>Agregue revisores a la etapa o elimine la etapa.<p>Si cada una de las pruebas se envía a las mismas personas en un escenario en particular, puede especificar sus nombres aquí name para que no tenga que añadirlos cada vez que cree una prueba. Escriba y seleccione el nombre de un usuario que desea agregar al escenario y, a continuación, agregue su <strong>Función</strong> en la prueba y <strong>Alertas de correo electrónico</strong> configuración que desee para el usuario. Para obtener información sobre las funciones de prueba, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configuración de las funciones de prueba predeterminadas</a>. Para obtener información sobre las alertas de correo electrónico de prueba, consulte la sección <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configuración de los valores predeterminados de prueba para un usuario</a> en el artículo <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configuración de las notificaciones por correo electrónico en Workfront Proof</a>.</p><p>Puede agregar tantos usuarios como desee a un escenario</p><p>Sugerencia: Puede arrastrar y soltar nombres de revisores entre etapas en el diagrama de etapas. Los escenarios disponibles se resaltan en azul.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Repita el paso para cualquier otra etapa que desee agregar a la plantilla.

   En la parte superior del **Flujo de trabajo** , puede ver un diagrama del flujo de trabajo automatizado que está configurando. A medida que continúa añadiendo etapas, aparecen en el diagrama con líneas que muestran las dependencias entre ellas. Puede hacer clic en un escenario del diagrama para ver la configuración de dicho escenario.

   Si no necesita ver el diagrama, puede hacer clic en **Ocultar diagrama**.

1. En el **Compartido con** , si desea eliminar un usuario, haga clic en Más ![](assets/more-icon.png) a la derecha, haga clic en **Eliminar**.

## Crear grupos de plantillas de flujo de trabajo automatizado {#create-automated-workflow-template-groups}

Como administrador de Workfront, puede ver y administrar todas las plantillas de flujo de trabajo automatizado en la cuenta de su organización. Puede resultar útil organizar las plantillas en grupos.

Para crear un grupo de plantillas de flujo de trabajo automatizado:

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.
1. Haga clic en **Flujos de trabajo** en el panel izquierdo.
1. En el **Flujo de trabajo** , haga clic en **Nuevo** > **Nuevo grupo de plantillas**.
1. Escriba un nombre descriptivo para el nuevo grupo de plantillas y pulse **Entrar**.

Puede mover las plantillas entre grupos arrastrándolas y soltándolas.

## Administrar plantillas de flujo de trabajo automatizadas

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.

1. En el panel izquierdo de Workfront Proof, haga clic en **Flujos de trabajo**.
1. En el **Flujos de trabajo** que aparezca, realice una de las acciones siguientes:

   * Añadir una plantilla nueva
   * Agregar un nuevo grupo de plantillas
   * Eliminar uno o más grupos de plantillas
   * Acceso a los detalles de una plantilla
   * Arrastrar una plantilla a otro grupo de plantillas
