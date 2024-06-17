---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Crear y administrar plantillas de flujo de trabajo automatizado
description: Como administrador de Adobe Workfront, si el proceso de revisión de contenido de su organización se repite con frecuencia o el contenido lo revisan las mismas personas, puede crear plantillas de flujo de trabajo automatizadas que contengan los revisores con las funciones de prueba y la configuración de notificación que especifique. Una plantilla de Flujo de trabajo automatizado puede ser sencilla con solo uno o dos revisores, o compleja con muchas fases y dependencias.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# Crear y administrar plantillas de flujo de trabajo automatizado

<!-- Audited: 2/2024 -->

Como administrador de Adobe Workfront, si el proceso de revisión de contenido de su organización se repite con frecuencia o el contenido lo revisan las mismas personas, puede crear plantillas de flujo de trabajo automatizadas que contengan los revisores con las funciones de prueba y la configuración de notificación que especifique. Una plantilla de Flujo de trabajo automatizado puede ser sencilla con solo uno o dos revisores, o compleja con muchas fases y dependencias.

Las plantillas de flujo de trabajo automatizado facilitan la creación de una prueba con un flujo de trabajo automatizado. Cuando un usuario crea una prueba, simplemente elige la plantilla que necesita.

Puede cambiar fácilmente cualquier plantilla de flujo de trabajo automatizado, agregando o eliminando revisores y fases, en cualquier momento. Y los creadores de pruebas que utilicen la plantilla pueden agregar o quitar revisores para la prueba.

Tenga en cuenta lo siguiente cuando utilice una plantilla de flujo de trabajo automatizado:

1. La configuración de una plantilla de Flujo de trabajo automatizado determina lo que puede hacer con el Flujo de trabajo automatizado para una prueba. Por ejemplo, si el botón Add a stage está desactivado en la plantilla, no está visible mientras trabaja con la configuración del flujo de trabajo automatizado para la prueba.
1. Cuando se añade una persona a una etapa en una plantilla de flujo de trabajo automatizado, pero también está presente como revisor en la prueba, al aplicar la plantilla se elimina al revisor de la etapa. Si no agrega otro revisor al escenario, aparecerá un mensaje en el que se le pedirá que agregue uno.
1. La posibilidad de modificar una plantilla de flujo de trabajo automatizado depende de la configuración de la plantilla que establezca el administrador de Workfront, tal como se describe en Si la capacidad para modificar la plantilla está desactivada, solo el propietario de la plantilla puede modificarla.

Para obtener información sobre los flujos de trabajo automatizados, consulte [Resumen del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Nuevo: Cualquiera</p><p>Actual: Pro o Superior</p><p>Heredado: Premium o Select</p> <p>Para obtener más información sobre la revisión del acceso con los diferentes planes, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar</p><p>Actual: Trabajo o Plan</p> <p>Heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe haber seleccionado Administrador en el perfil de permisos de revisión. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una plantilla de flujo de trabajo automatizado

{{step1-to-proofing}}

1. Clic **Flujos de trabajo** en el panel izquierdo.
1. En el **Flujo de trabajo** pestaña, haga clic en **Nuevo** > **Nueva plantilla**.

1. En el **Detalles** , especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de plantilla</td> 
      <td>(Obligatorio) Escriba un nombre para la plantilla. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propietario de plantilla</td> 
      <td>Puede seleccionar el administrador de Workfront o de Workfront Proof que administrará la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de plantillas</td> 
      <td> <p> Si los flujos de trabajo automatizados de su organización están organizados en grupos, puede seleccionar el nombre del grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Crear grupos de plantillas de flujo de trabajo automatizado</a> más adelante en este artículo para obtener más información.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Zona horaria de plantilla </td> 
      <td> <p>La zona horaria predeterminada para la plantilla es la que utiliza. Si la zona horaria de los creadores y revisores de prueba que utilizarán la plantilla es diferente, puede cambiarla aquí para asegurarse de que los plazos de las fases se establezcan en los momentos adecuados para esos usuarios. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>Puede seleccionar las actividades de fase que desea que estén disponibles para la persona que crea las pruebas mediante la plantilla.</p> 
      <p><b>ADVERTENCIA</b>: Si no selecciona las opciones Añadir una fase y Añadir personas a las fases, ni el propietario de la plantilla ni el propietario de ninguna prueba que utilice esta plantilla podrán añadir una fase o compartir la prueba. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Fases** , configure cada fase de la plantilla Flujo de trabajo automatizado.

   Puede agregar varias fases y crear interacciones.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>El nombre de la fase se muestra en el diagrama de flujo de trabajo automatizado en la parte superior de la sección Flujo de trabajo, en la página Detalles de la prueba y en las notificaciones por correo electrónico enviadas a los revisores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activar fase</td> 
      <td> <p>Especifique si la fase se activa automática o manualmente. Para la primera fase, puede seleccionar <strong>Al crear la prueba</strong>, <strong>En una fecha y hora específicas</strong>, o <strong>Manualmente</strong>.</p> <p>Las demás opciones estarán disponibles cuando añada una segunda fase, ya que es necesario seleccionar una fase principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Plazo calculado a partir de</td> 
      <td> <p>Especifique cómo desea calcular la fecha límite:</p> 
       <ul> 
        <li> <p><strong>Creación de pruebas</strong>: en la lista desplegable debajo de <strong>Plazo (+ días laborables)</strong>, seleccione el número de días laborables que desee añadir a la fecha de creación de la prueba para establecer automáticamente una fecha límite en la prueba.</p> </li> 
        <li><strong>Cuando comienza la fase</strong>: en la lista desplegable debajo de <strong>Plazo (+ días laborables)</strong>, seleccione el número de días laborables que desee añadir a la fecha de activación de la fase para establecer automáticamente una fecha límite en la prueba.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear fase</td> 
      <td>Especifique si desea permitir que la fase se bloquee para comentarios. Las opciones son bloquear una etapa manual o automáticamente, ya sea cuando comience la siguiente etapa o cuando se tomen todas las decisiones en la etapa principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Responsable de toma de decisiones principal</td> 
      <td> <p>Los responsables de la toma de decisiones disponibles solo se muestran en la lista después de agregar los revisores a la fase.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solamente se requiere una decisión</td> 
      <td>El proceso de revisión de la fase se completará tan pronto como uno de los responsables de la toma de decisiones presente su decisión. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuración de revisión en Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fase privada</td> 
      <td>Oculta los comentarios y las decisiones de a las personas que no se agregan al escenario o que no son administradores de Workfront. Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">No permitir que se elimine esta fase</td> 
      <td> <p>Convierte la fase en obligatoria.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Si las pruebas que utilizarán esta plantilla siempre se envían a las mismas personas en la fase, agréguelas aquí para que los usuarios no tengan que agregarlas cada vez que creen una prueba.

   Elija la de cada persona **Rol** en las pruebas que utilizarán esta plantilla y la variable **Alertas de correo electrónico** desea que el usuario reciba cuando trabaje en pruebas que utilicen esta plantilla.

   Para obtener información sobre las funciones de una prueba, consulte [Configurar funciones de corrección predeterminadas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Para obtener información sobre las alertas de prueba por correo electrónico, consulte la sección [Configurar valores predeterminados de prueba para un usuario](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) en el artículo  [Configuración de notificaciones por correo electrónico en Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Cada usuario solo puede agregarse a una fase. Puede agregar tantos usuarios como desee a una fase.

   >[!TIP]
   >
   >Puede arrastrar y soltar los nombres de los revisores entre las fases del diagrama de fases. Las fases disponibles se resaltan en azul.

1. Repita los dos pasos anteriores para cualquier otra etapa que desee agregar a la plantilla.

   En la parte superior del **Flujo de trabajo** , puede ver un diagrama del flujo de trabajo automatizado que está configurando. A medida que vaya añadiendo fases, estas aparecerán en el diagrama con líneas que muestran las dependencias entre ellas. Puede hacer clic en un escenario del diagrama para ver la configuración de dicho escenario.

   Si no necesita ver el diagrama, puede hacer clic en **Ocultar diagrama**.

1. En el **Compartir plantilla con** , haga clic en una opción (si la plantilla aún no se ha compartido con toda la organización) para especificar quién podrá utilizarla.

   De forma predeterminada, las nuevas plantillas de flujo de trabajo automatizado se comparten con todos los miembros de la organización.

1. Haga clic en **Crear**.

## Modificación de una plantilla de flujo de trabajo automatizado

Como administrador de Workfront Proof, puede modificar una plantilla de flujo de trabajo automatizado. Los cambios se guardan automáticamente a medida que los realiza.

{{step1-to-proofing}}

1. Clic **Flujos de trabajo** en el panel izquierdo.
1. En el **Plantillas de flujo de trabajo** que aparece, haga clic en la plantilla que desee modificar.
1. En el **Detalles** , especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de plantilla</td> 
      <td>(Obligatorio) Escriba un nombre para la plantilla. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propietario de plantilla</td> 
      <td>Puede seleccionar el administrador de Workfront o de Workfront Proof que administrará la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de plantillas</td> 
      <td> <p> Si los flujos de trabajo automatizados de su organización están organizados en grupos, puede seleccionar el nombre del grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Crear grupos de plantillas de flujo de trabajo automatizado</a> más adelante en este artículo para obtener más información.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zona horaria de plantilla </td> 
      <td> <p>La zona horaria predeterminada para la plantilla es la que utiliza. Si la zona horaria de los creadores y revisores de prueba que utilizarán la plantilla es diferente, puede cambiarla aquí para asegurarse de que los plazos de las fases se establezcan en los momentos adecuados para esos usuarios. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>Seleccione las actividades de fase que desee que estén disponibles para los que crean pruebas con la plantilla. </p> <p><b>ADVERTENCIA</b>: Si no selecciona las opciones Añadir una fase y Añadir personas a las fases, ni el propietario de la plantilla ni el propietario de ninguna prueba que utilice esta plantilla podrán añadir una fase o compartir la prueba.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Flujo de trabajo** , cambie el nombre de cualquier etapa y expanda su configuración ![](assets/arrow-button.png) para realizar los cambios necesarios:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Plazo calculado a partir de</td> 
      <td> <p>Especifique cómo desea calcular la fecha límite:</p> 
       <ul> 
        <li> <p><strong>Plazo calculado a partir de la creación de pruebas</strong>: en el <strong>Establecer la fecha límite de la fase</strong> , seleccione el número de días laborables que desee añadir a la fecha de creación de la prueba para establecer automáticamente una fecha límite en la prueba.</p> </li> 
        <li><strong>Plazo calculado desde la activación de la fase</strong>: en el <strong>Establecer la fecha límite de la fase</strong> , seleccione el número de días laborables que desee añadir a la fecha de activación de la fase para establecer automáticamente una fecha límite en la prueba.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activar fase</td> 
      <td> <p>Especifique si la fase se activa automática o manualmente. Para la primera fase, puede seleccionar <strong>Al crear la prueba</strong>, <strong>En una fecha y hora específicas</strong>, o <strong>Manualmente</strong>.</p> <p>Las demás opciones estarán disponibles cuando añada una segunda fase, ya que es necesario seleccionar una fase principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear fase</td> 
      <td>Especifique si desea permitir que la fase se bloquee para comentarios. Las opciones son bloquear una etapa manual o automáticamente, ya sea cuando comience la siguiente etapa o cuando se tomen todas las decisiones en la etapa principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisión</td> 
      <td>Finaliza la fase la primera vez que uno de los responsables de la toma de decisiones presenta su decisión. Para obtener más información, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuración de revisión en Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacidad</td> 
      <td>Oculta los comentarios y decisiones de a las personas que no se agregan al escenario o que no son supervisores o superiores en la cuenta. Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminación de fase</td> 
      <td>Convierte la fase en obligatoria.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Más <img src="assets/more-icon.png"></td> 
      <td>Agregar revisores a la fase o eliminar la fase.<p>Si cada una de las pruebas se envía a las mismas personas en una fase concreta, puede especificar sus nombres aquí nombre para que no tenga que agregarlos cada vez que cree una prueba. Escriba y seleccione el nombre de un usuario que desee añadir a la fase y, a continuación, añada su <strong>Rol</strong> en la prueba y <strong>Alertas de correo electrónico</strong> la configuración que desee para el usuario. Para obtener información sobre las funciones de revisión, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configurar funciones de corrección predeterminadas</a>. Para obtener información sobre las alertas de prueba por correo electrónico, consulte la sección <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configurar valores predeterminados de prueba para un usuario</a> en el artículo <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configuración de notificaciones por correo electrónico en Workfront Proof</a>.</p><p>Puede agregar tantos usuarios como desee a una fase</p><p>Sugerencia: Puede arrastrar y soltar nombres de revisores entre fases en el diagrama de fases. Las fases disponibles se resaltan en azul.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Repita el paso para cualquier otra etapa que desee agregar a la plantilla.

   En la parte superior del **Flujo de trabajo** , puede ver un diagrama del flujo de trabajo automatizado que está configurando. A medida que vaya añadiendo fases, estas aparecerán en el diagrama con líneas que muestran las dependencias entre ellas. Puede hacer clic en un escenario del diagrama para ver la configuración de dicho escenario.

   Si no necesita ver el diagrama, puede hacer clic en **Ocultar diagrama**.

1. En el **Compartido con** , si desea eliminar un usuario, haga clic en el botón Más ![](assets/more-icon.png) a la derecha, y luego haga clic en **Eliminar**.

## Crear grupos de plantillas de flujo de trabajo automatizado {#create-automated-workflow-template-groups}

Como administrador de Workfront, puede ver y administrar todas las plantillas de flujo de trabajo automatizado de la cuenta de su organización. Puede resultar útil organizar las plantillas en grupos.

Para crear un grupo de plantillas de flujo de trabajo automatizado:

{{step1-to-proofing}}

1. Clic **Flujos de trabajo** en el panel izquierdo.
1. En el **Flujo de trabajo** pestaña, haga clic en **Nuevo** > **Nuevo grupo de plantillas**.
1. Escriba un nombre descriptivo para el nuevo grupo de plantillas y pulse **Entrar**.

Puede mover las plantillas entre grupos arrastrándolas y soltándolas.

## Administrar plantillas de flujo de trabajo automatizado

{{step1-to-proofing}}

1. En el panel izquierdo de Workfront Proof, haga clic en **Flujos de trabajo**.
1. En el **Flujos de trabajo** que aparezca, realice una de las acciones siguientes:

   * Añadir una plantilla nueva
   * Agregar un nuevo grupo de plantillas
   * Eliminar uno o varios grupos de plantillas
   * Acceso a los detalles de una plantilla
   * Arrastrar una plantilla a otro grupo de plantillas
