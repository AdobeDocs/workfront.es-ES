---
product-area: requests
navigation-topic: create-requests
title: Crear y enviar solicitudes de Adobe Workfront
description: El trabajo planificado se representa en Adobe Workfront mediante proyectos y tareas. Sin embargo, puede trabajar en un entorno en el que el trabajo no planificado (en forma de solicitudes aleatorias) pueda entrar en cualquier momento. Workfront proporciona un flujo de trabajo para acomodar este tipo de entorno mediante el uso de colas de solicitud.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: b40ade1f1d7a9b81c654a274c5e8c872bf74b180
workflow-type: tm+mt
source-wordcount: '2337'
ht-degree: 2%

---

# Crear y enviar solicitudes de Adobe Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE:&nbsp;If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

El trabajo planificado se representa en Adobe Workfront mediante proyectos y tareas. Sin embargo, puede trabajar en un entorno en el que el trabajo no planificado (en forma de solicitudes aleatorias) pueda entrar en cualquier momento. Workfront proporciona un flujo de trabajo para acomodar este tipo de entorno mediante el uso de colas de solicitud. 

Después de crear una solicitud en una cola de solicitud, puede asignarla para que se complete o puede convertirla en una tarea o un proyecto.\
Para obtener más información sobre la conversión de problemas en una tarea o proyecto, consulte el artículo [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Puede crear una solicitud de las siguientes maneras:

* Desde cero, tal como se describe en este artículo.
* De borradores. Para obtener más información, consulte [Crear solicitudes a partir de borradores](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* A partir de una solicitud existente, copiando y enviando una copia. Para obtener más información, consulte [Copiar y enviar solicitudes](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Requisitos de acceso

<!--drafted for P&P - replace table: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos para utilizar colas de solicitud

Como administrador de Workfront, debe crear colas de solicitud y ponerlas a disposición de los usuarios antes de que puedan utilizar esta funcionalidad. Un usuario con una licencia de Planificador y con acceso de edición a Proyectos y permisos de gestión de un proyecto específico también puede crear colas de solicitud. 

Para obtener información sobre cómo crear colas de solicitudes, consulte el artículo [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Debe crear los siguientes componentes de una cola de solicitud:

* Un proyecto en estado actual, publicado como una cola de solicitud de ayuda.
* Temas de colas.\
   Para obtener más información, consulte el artículo [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Reglas de enrutamiento.\
   Para obtener más información, consulte el artículo [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Opcional) Grupos de temas.\
   Para obtener más información, consulte el artículo [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Opcional) Solicite un formulario personalizado.\
   Para obtener más información, consulte el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (Opcional) Proceso de aprobación de solicitudes.\
   Para obtener más información, consulte el artículo [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Crear solicitudes y generar borradores en la aplicación web de Workfront

Cuando se crea una solicitud en la aplicación web de Workfront, Workfront la guarda como borrador antes de enviarla. Workfront crea un borrador en cuanto selecciona la cola de solicitudes y comienza a introducir información para él.

Puede continuar enviando la solicitud, o puede completar toda la información disponible y salir de ella para terminarla más tarde. Workfront guarda la solicitud redactada que inició en la carpeta Borradores .

>[!IMPORTANT]
>
>Tenga en cuenta lo siguiente al trabajar con borradores:
>
>* Workfront no crea borradores de solicitudes cuando las envía desde una aplicación de terceros, como enviarlas por correo electrónico a Workfront o crearlas con cualquier otra aplicación. Cuando envía una solicitud desde fuera de la aplicación web de Workfront, la solicitud se guarda en la sección Enviado .
>* Si cambia la estructura de una cola de solicitudes, ya no puede acceder a los borradores existentes. Por ejemplo, si se elimina un tema de cola o se agrega un grupo de temas, ya no se puede acceder a los borradores guardados.
>


Para obtener información sobre la creación de solicitudes a partir de borradores existentes, consulte [Crear solicitudes a partir de borradores](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Para obtener información sobre la eliminación de borradores de solicitud, consulte también [Eliminar un borrador de solicitud](../../../manage-work/requests/create-requests/delete-request-draft.md).

Para crear una solicitud en la aplicación web de Workfront: 

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. Haga clic en  **Solicitudes** y haga clic en **Nueva solicitud** en la esquina superior derecha de la página.

   >[!TIP]
   >
   >* Puede acceder a la opción Nueva solicitud desde cualquier sección del área Solicitudes .
   >* La opción Nueva solicitud aparece atenuada cuando no tiene acceso para crear problemas.


1. (Condicional) Haga clic dentro del **Tipo de solicitud** y realice una de las siguientes acciones:

   * En el **Rutas recientes** , seleccione una ruta que haya utilizado recientemente para abrir una cola de solicitudes. Una ruta incluye la cola de solicitudes, los grupos de temas y el tema de la cola al que ha enviado recientemente. Las tres últimas rutas se muestran de forma predeterminada.

      >[!NOTE]
      >
      >Workfront guarda una ruta únicamente cuando se ha enviado una solicitud. No crea rutas para solicitudes redactadas.

      ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * En el **Solicitar colas** seleccione una cola de solicitudes.
   * Escriba una palabra clave que pertenezca a una ruta previamente accedida para buscar una cola de solicitudes.

      Por ejemplo, si tiene una cola de solicitud denominada &quot;Asistencia técnica&quot; con un grupo de temas denominado &quot;Ubicación&quot; y un tema de cola denominado &quot;Remoto&quot;, puede escribir &quot;remoto&quot; y se mostrarán todas las colas de solicitud que contengan &quot;remoto&quot; en cualquier elemento de su ruta.

      >[!TIP]
      >
      >Cuando se escribe un nombre que contiene un carácter especial, se muestra la cola de solicitudes, el tema de la cola o el grupo de temas, incluso cuando se omite escribir el carácter.

      ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

      La lista de colas de solicitud disponibles y rutas recientes se actualiza dinámicamente para incluir solo las rutas que contienen la palabra clave que está resaltada en los resultados.

      Los resultados de la búsqueda se muestran en las siguientes áreas:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Colas de solicitudes</td> 
        <td>Solicitar colas que contienen la palabra clave en su nombre</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Solicitar rutas</td> 
        <td> <p>Rutas (que incluyen colas de solicitud, grupos de temas, temas de cola) que contienen la palabra clave en cualquiera de los nombres de sus elementos</p> </td> 
       </tr> 
      </tbody> 
     </table>
   >[!TIP]
   >
   >* Las 200 primeras colas de solicitudes se muestran de forma predeterminada, en orden alfabético.
   >* El nombre de la cola de solicitudes es el nombre del proyecto que se ha publicado como cola de solicitud de ayuda.
   >* La descripción del proyecto configurado como la cola de solicitudes seleccionada se muestra a la derecha del nombre de la cola de solicitudes.

   >   
   >Para obtener más información sobre cómo publicar un proyecto como cola de solicitud de ayuda, consulte el artículo [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. En el **Nueva solicitud** realice una de las siguientes acciones:

   * (Condicional) Seleccione un borrador disponible del mensaje de notificación que se muestra en el campo Tipo de solicitud .

      Esta área se muestra únicamente si ha guardado borradores antes de enviarlos.

      Los tres borradores más recientes de tres temas de cola diferentes se muestran de forma predeterminada.

      ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Comience a introducir una nueva solicitud en la cola seleccionada.

      Un nuevo borrador se guarda automáticamente en la sección Borradores después de que empiece a introducir información para la nueva solicitud y asigne un nombre a la solicitud en el campo Asunto.

1. (Opcional) Si la cola de solicitud incluye grupos de temas, seleccione el nombre del grupo de temas en el primer campo desplegable. De lo contrario, seleccione un tema de cola.

   >[!TIP]
   Cuando pasa el ratón sobre un grupo de temas o un tema de cola, se muestra el campo Descripción a la derecha. Contiene información adicional sobre el tema de grupo de temas o de cola.
   ![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >

   Puede tener hasta 10 niveles de grupos de temas integrados en la cola de solicitudes.\
   Para obtener más información sobre cómo crear grupos de temas, consulte el artículo [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obtener más información sobre la creación de temas de cola, consulte el artículo [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   Si ha seleccionado un borrador o una ruta anterior, los grupos de temas y los temas de la cola ya están seleccionados. Si es necesario, puede seleccionar otra.

1. Según los campos que habilitó el administrador de Workfront en la variable **Nuevos campos de problema** de la sección **Detalles de cola** en el proyecto, puede encontrar cualquiera de los campos siguientes al enviar una nueva solicitud:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Asunto</strong> </td> 
      <td>Especifique un nombre para la solicitud. Se trata de un campo obligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td>Especifique una descripción para la solicitud.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dirección URL</strong> </td> 
      <td> <p>Especifique una dirección URL que esté relacionada con la solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad</strong> </td> 
      <td> <p>Especifique una prioridad para la solicitud. La prioridad debe definir la velocidad con la que cree que se debe resolver esta solicitud. Las opciones predeterminadas son: </p> 
       <ul> 
        <li>Ninguno</li> 
        <li>Bajo </li> 
        <li>Normal</li> 
        <li>Alto</li> 
        <li>Urgente</li> 
       </ul> <p>El administrador del sistema puede modificar los nombres de las prioridades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gravedad</strong> </td> 
      <td> <p>Especifique una gravedad para la solicitud. La gravedad debe definir el impacto que esta solicitud tiene en su trabajo si no se resuelve a tiempo. Las opciones predeterminadas son:</p> 
       <ul> 
        <li>Cosmético</li> 
        <li>Causa confusión</li> 
        <li>Error con solución</li> 
        <li>Error sin solución</li> 
        <li>Error fatal</li> 
       </ul> <p>El administrador del sistema puede modificar los nombres de gravedad.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contacto primario</strong> </td> 
      <td>El Contacto Principal de una solicitud le toma por defecto, ya que usted es la persona de punto para abordar cualquier pregunta relacionada con la solicitud. Sin embargo, puede cambiarlo a cualquier otro usuario de Workfront.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Asignaciones</strong> </td> 
      <td> <p><span>Especifique el nombre de un usuario, función de trabajo o equipo activo al que se debe asignar la solicitud.</span> </p> <p>Solo puede especificar un equipo.</p>

   <p> Según cómo se haya configurado la cola de solicitudes, es posible que solo pueda asignar uno o dos tipos de recurso a la solicitud, en lugar de los tres (por ejemplo, puede que solo pueda asignar la solicitud a los usuarios).</p>

   <p>Si una regla de enrutamiento también está asociada a la cola de solicitudes y enruta automáticamente la solicitud a un tipo diferente de recurso (por ejemplo, un equipo), la solicitud se asigna tanto a la entidad que especifique manualmente al enviar la solicitud (usuarios) como al recurso especificado en la regla de enrutamiento (el equipo). </p>

   <p> Para obtener más información, consulte los siguientes artículos:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Crear reglas de enrutamiento</a> <br> </p> </li> 
      </ul> </p>

   <p><span>Se recomienda utilizar reglas de enrutamiento para las colas de solicitud de modo que se puedan enrutar automáticamente a los recursos adecuados.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Horas planificadas</strong> </td> 
      <td> <p>Calcule cuántas horas tardaría esta solicitud en completarse.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha planificada de inicio</strong> </td> 
      <td> <p>Especifique la fecha en la que se debe iniciar el trabajo en esta solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha planificada de finalización</strong> </td> 
      <td>Especifique la fecha en la que desea que se resuelva esta solicitud.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estado</strong> </td> 
      <td>El estado predeterminado de una nueva solicitud es "Nuevo". Es posible que el administrador del sistema haya cambiado el nombre de este estado. También puede cambiar el estado a otra cosa desde este menú desplegable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Agregue documentos a la solicitud. </p> <p> Dependiendo de cómo se haya configurado la cola de solicitudes, la sección Documentos podría mostrarse antes o después de los campos personalizados. </p> <p>Los documentos que se cargan en Workfront se almacenan durante 24 horas en una solicitud redactada. Después, debe volver a adjuntarlas cuando vuelva a editar y envíe el borrador. Los documentos vinculados desde otras unidades se guardan en el borrador de forma permanente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Si el administrador de Workfront ha asociado un formulario personalizado con la cola de solicitud o con el tema de cola, especifique los campos dentro del formulario personalizado.\
   Los formularios personalizados son diferentes para cada instancia de Workfront. 
1. (Opcional y condicional) En cualquier momento durante la introducción de la solicitud, haga clic en [!UICONTROL **Descartar borrador**] si desea eliminar el borrador que se crea automáticamente. Esto elimina el borrador que no se puede recuperar. Aparece un mensaje de confirmación para confirmar que está eliminando el borrador.

1. (Opcional) Haga clic en [!UICONTROL **Deshacer**] en el mensaje de confirmación si desea revertir la acción y mantener el borrador.

1. Realice una de las siguientes acciones:

   * Haga clic en **Submit** si está listo para enviar la solicitud. La solicitud se guarda en la sección Enviado . En función de la regla de enrutamiento de la cola de solicitud, esta solicitud puede enrutarse a un proyecto diferente al designado como cola de solicitud. Para obtener información sobre las reglas de enrutamiento, consulte [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      O

      Haga clic en **Cerrar** si no estás listo para enviarlo y puedes volver y terminarlo más tarde. La solicitud se guarda en la sección Borradores y estará disponible la próxima vez que envíe una solicitud para esta cola de solicitudes.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)
   Al enviar la solicitud, el borrador se elimina automáticamente y no se puede restaurar.

   Para obtener información sobre cómo abordar las solicitudes entrantes, consulte el artículo [Administrar solicitudes de trabajo y equipo](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Para obtener información sobre la localización de solicitudes enviadas o redactadas, consulte también [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Crear solicitudes fuera de Workfront

Puede compartir un vínculo directo a una cola de solicitudes al enviar una nueva solicitud e incrustarla en otras aplicaciones. Los usuarios que accedan a este vínculo desde la web o desde otras aplicaciones también deben iniciar sesión con una cuenta de Workfront activa para poder acceder a esta cola y enviarle solicitudes. Para obtener más información, consulte [Compartir un vínculo a una cola de solicitudes](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Crear solicitudes enviando correos electrónicos a Workfront

Si la cola de solicitud está habilitada para recibir solicitudes por correo electrónico, puede enviar las solicitudes por correo electrónico directamente al correo electrónico asociado con la cola de solicitud.

El texto del cuerpo del correo electrónico se agrega como descripción de la solicitud.

>[!NOTE]
El formato del HTML se elimina cuando la solicitud entra en Workfront, pero las firmas y el contenido de los subprocesos de respuesta existente no se eliminan y aparecen en la descripción de la solicitud.

Para obtener información sobre cómo habilitar una cola de solicitud para recibir solicitudes por correo electrónico, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitud](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Crear solicitudes con el cliente de Outlook

Puede enviar solicitudes mediante el cliente de Outlook. Puede crear una solicitud nueva o convertir un correo electrónico en una solicitud. 

Para obtener información sobre el envío de solicitudes mediante el cliente de Outlook, consulte el artículo [Crear una solicitud de Adobe Workfront a partir de un correo electrónico de Outlook](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Crear solicitudes utilizando la aplicación móvil de Workfront

Puede enviar solicitudes mediante la aplicación móvil en su smartphone. Puede crear una nueva solicitud y enviarla a las colas de solicitud a las que tiene acceso para ver en la aplicación web. 

Para obtener información sobre el envío de solicitudes a través de la aplicación móvil, consulte la [Solicitudes](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests) en los artículos:

* [Adobe Workfront para Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)
* [Adobe Workfront para iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)

## Crear solicitudes de otras aplicaciones

Puede enviar solicitudes mediante cualquier aplicación que se haya integrado con Workfront: 

* Puede crear una integración personalizada entre Workfront y otra aplicación que le permita enviar solicitudes a Workfront desde la otra aplicación.\
   Para obtener más información sobre las integraciones personalizadas de Workfront, consulte el artículo [Integraciones de Adobe Workfront](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* Puede enviar solicitudes desde Salesforce si ha instalado la aplicación de Workfront para Salesforce.\
   Para obtener información sobre el envío de solicitudes de Salesforce mediante la aplicación Workfront para Salesforce, consulte el artículo [Envío de solicitudes de Adobe Workfront desde objetos de Salesforce](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## Localizar solicitudes enviadas

Para obtener información sobre la localización de solicitudes enviadas o redactadas, consulte [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
