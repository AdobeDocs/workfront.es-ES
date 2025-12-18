---
product-area: requests
navigation-topic: create-requests
title: Creación y envío de solicitudes
description: En Adobe Workfront, el trabajo planificado se representa mediante proyectos y tareas. Sin embargo, es posible que se trabaje en un entorno en el que el trabajo no planificado (en forma de solicitudes aleatorias) pueda llegar en cualquier momento. Workfront proporciona un flujo de trabajo para dar cabida a este tipo de entorno mediante el uso de colas de solicitudes.
author: Becky
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: 684f7fc62fe341a59b1b7f7ae6c7118a5e511513
workflow-type: tm+mt
source-wordcount: '2546'
ht-degree: 82%

---

# Creación y envío de solicitudes

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->


En Adobe Workfront, el trabajo planificado se representa mediante proyectos y tareas. Sin embargo, es posible que se trabaje en un entorno en el que el trabajo no planificado, en forma de solicitudes, pueda llegar en cualquier momento. Workfront proporciona un flujo de trabajo para dar cabida a este tipo de entorno mediante el uso de colas de solicitudes.

Después de crear una solicitud en una cola de solicitudes, puede asignarla para que se complete o puede convertirla en una tarea o un proyecto.\
Para obtener más información sobre la conversión de problemas en una tarea o proyecto, consulte el artículo [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Puede crear una solicitud de Workfront de las siguientes maneras:

* Desde cero como se describe en este artículo.
* A partir de borradores. Para obtener más información, consulte [Crear solicitudes a partir de borradores](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* A partir de una solicitud existente, copiando y enviando una copia. Para obtener más información, consulte [Copiar y enviar solicitudes](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

Puede crear una solicitud de Workfront Planning desde cero para crear registros en Workfront Planning de las siguientes maneras:

* Desde un vínculo a un formulario de solicitud de Workfront Planning.

* Desde un formulario de solicitud de Workfront Planning en el área de solicitudes de Workfront.

  Su organización debe adquirir un paquete de Workfront Planning. Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Producto</td> 
   <td> <ul><li>Adobe Workfront</li><li>Debe tener Adobe Workfront Planning para ver solicitudes de Planning o formularios de solicitud</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos para utilizar colas de solicitudes

La persona con la función de administrador de Workfront debe crear colas de solicitudes y ponerlas a disposición de los usuarios para que puedan utilizar esta funcionalidad. Un usuario con licencia de Planificador y con acceso de edición a proyectos y permisos de administración para un proyecto específico también puede crear colas de solicitudes.

Para obtener información sobre la creación de colas de solicitudes, consulte el artículo [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Una persona con la función de administrador de Workfront debe crear los siguientes componentes de una cola de solicitudes:

* Un proyecto en estado Actual, publicado como cola de solicitudes de ayuda.
* Temas de colas.\
  Para obtener más información, consulte el artículo [Crear temas de colas](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Reglas de enrutamiento\
  Para obtener más información, consulte el artículo [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Opcional) Grupos de temas.\
  Para obtener más información, consulte el artículo [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Opcional) Formulario personalizado de solicitud.\
  Para obtener más información, consulte el artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* (Opcional) Proceso de aprobación de la solicitud.\
  Para obtener más información, consulte el artículo [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Crear solicitudes y generar borradores en la aplicación web de Workfront

Al crear una solicitud en la aplicación web de Workfront, Workfront la guarda como borrador antes de enviarla. Workfront crea un borrador en cuanto se selecciona la cola de solicitudes y se empieza a introducir información sobre esta.

Puede seguir enviando la solicitud o puede completar toda la información que tenga disponible y salir de ella para terminarla más tarde. Workfront guarda el borrador de la solicitud que inició en la carpeta Borradores <span class="preview"> o en la lista de solicitudes.</span>

>[!IMPORTANT]
>
>Tenga en cuenta lo siguiente al trabajar con borradores:
>
>* Workfront no crea solicitudes de borrador cuando las envía desde una aplicación de terceros, como cuando las envía por correo electrónico a Workfront o las crea con cualquier otra aplicación. Cuando envía una solicitud desde fuera de la aplicación web de Workfront, se guarda en la sección Enviada.
>* Si la estructura de una cola de solicitudes cambia, ya no se puede acceder a los borradores existentes. Por ejemplo, si se quita un tema de la cola o se añade un grupo de temas, los borradores guardados ya no estarán accesibles.
>

Para obtener información sobre la creación de solicitudes a partir de borradores existentes, consulte [Crear solicitudes a partir de borradores](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Para obtener información sobre la eliminación de borradores de solicitud, consulte también [Eliminar un borrador de solicitud](../../../manage-work/requests/create-requests/delete-request-draft.md).

Para crear una solicitud en la aplicación web de Workfront:

{{step1-to-requests}}

1. (Opcional y condicional) Seleccione la opción **Cambiar a una nueva experiencia** en la parte superior derecha de la pantalla.

1. Haga clic en **Nueva solicitud** en la esquina superior derecha de la página.

   >[!TIP]
   >
   >* Puede acceder a la opción Nueva solicitud desde cualquier sección del área Solicitudes.
   >* La opción Nueva solicitud se atenúa cuando no tiene acceso para crear problemas.

   Se abre el cuadro **Nueva solicitud**.

1. (Condicional) Si ha cambiado a la nueva experiencia, seleccione una de las rutas o formularios de la cola de solicitudes de Workfront o haga clic en la barra de búsqueda.

   Al hacer clic en la barra de búsqueda, aparece una lista desplegable que muestra primero las colas y los formularios utilizados más recientemente. Seleccione uno de la lista o empiece a escribir y seleccione la cola o el formulario cuando aparezca.

   >[!NOTE]
   >
   >Considere lo siguiente con respecto a la nueva experiencia solicitante:
   >* La lista incluye tanto las colas de solicitud de Workfront como los formularios de solicitud de Workfront Planning.
   >* Puede filtrar la lista por tipo de objeto.
   >* <span class="preview">En la nueva experiencia de solicitud, los borradores se encuentran en la misma lista que las solicitudes enviadas</span>.

1. (Condicional) Si ha cambiado a la nueva experiencia, seleccione los grupos de temas y los temas de la cola y continúe actualizando el formulario.

   De lo contrario, haga clic dentro del campo **Tipo de solicitud** y realice una de las siguientes acciones:

   * En la sección **Rutas recientes**, seleccione una que haya utilizado recientemente para abrir una cola de solicitudes. Una ruta de acceso incluye la cola de solicitudes, los grupos de temas y el tema de la cola que se ha enviado recientemente. Las tres últimas rutas se muestran de forma predeterminada.

     >[!NOTE]
     >
     >Workfront guarda una ruta solo cuando realmente se le ha enviado una solicitud. No crea rutas para las solicitudes en borrador.

     ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * En la sección **Colas de solicitudes**, seleccione una cola de solicitudes.
   * Introduzca una palabra clave que pertenezca a una ruta a la que se haya accedido anteriormente para buscar una cola de solicitudes.

     Por ejemplo, si tiene una cola de solicitudes llamada “Servicio de asistencia” con un grupo de temas llamado “Ubicación” y un tema de colas llamado “Remoto”, puede escribir “remoto” y se mostrarán todas las colas de solicitudes que contengan “remoto” en cualquier elemento de su ruta.

     >[!TIP]
     >
     >Cuando se escribe un nombre que contiene un carácter especial, la cola de solicitudes, el tema de la cola o el grupo de temas se muestran incluso cuando se omite escribir el carácter.

     ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     La lista de colas de solicitud disponibles y las rutas recientes se actualiza dinámicamente para incluir solo las rutas que contienen la palabra clave resaltada en los resultados.

     Los resultados de la búsqueda se muestran en las siguientes áreas:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Colas de solicitudes</td> 
        <td>Colas de solicitudes que contienen la palabra clave en su nombre</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Solicitar rutas</td> 
        <td> <p>Rutas (que incluyen colas de solicitudes, grupos de temas y temas de cola) que contienen la palabra clave en cualquiera de los nombres de sus elementos</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* Las 200 primeras colas de solicitudes se muestran de forma predeterminada en orden alfabético.
   >* El nombre de la cola de solicitudes es el nombre del proyecto que se ha publicado como cola de solicitudes de ayuda.
   >* La descripción del proyecto configurado como cola de solicitudes seleccionada se muestra a la derecha del nombre de la cola de solicitudes.
   >   
   >Para obtener más información sobre la publicación de un proyecto como cola de solicitudes de ayuda, consulte el artículo [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. En el formulario **Nueva solicitud**, realice una de las siguientes acciones:

   * (Condicional) Seleccione un borrador disponible en el mensaje de notificación que se muestra en el campo Tipo de solicitud.

     Esta área solo se muestra si ha guardado borradores antes sin enviarlos.

     Los tres borradores más recientes de tres temas de cola diferentes se muestran de forma predeterminada.

     ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Comience a introducir una nueva solicitud en la cola seleccionada.

     Se guardará un nuevo borrador automáticamente en la sección Borradores después de que empiece a introducir información para la nueva solicitud y asigne un nombre a la solicitud en el campo Asunto.

1. (Opcional) Si la cola de solicitudes incluye grupos de temas, seleccione el nombre del grupo de temas en el primer campo desplegable. De lo contrario, seleccione un tema de la cola.

   >[!TIP]
   >
   >Al pasar el puntero por encima de un grupo de temas o un tema de la cola, el campo Descripción aparece a la derecha. Contiene información adicional sobre el grupo de temas o el tema de la cola.
   >
   >
   >![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)
   >

   Puede tener hasta 10 niveles de grupos de temas integrados en la cola de solicitudes.\
   Para obtener más información sobre la creación de grupos de temas, consulte el artículo [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obtener más información sobre la creación de temas de la cola, consulte el artículo [Crear temas de la cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   >
   >Si ha seleccionado un borrador o una ruta anterior, los grupos de temas y los temas de la cola ya están seleccionados. Puede seleccionar otro diferente, si es necesario.

1. Según los campos que haya habilitado la persona con rol de administrador de Workfront en la sección **Nuevos campos de problema** de la subpestaña **Detalles de la cola** del proyecto, podría encontrar cualquiera de los siguientes campos al enviar una nueva solicitud:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Asunto</strong> </td> 
      <td>Especifique un nombre para la solicitud. Este campo es obligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td>Especifique una descripción para la solicitud.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Especifique una dirección URL que pueda estar relacionada con la solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad</strong> </td> 
      <td> <p>Especifique una prioridad para la solicitud. La prioridad debe definir la rapidez con la que cree que se debe resolver esta solicitud. Las opciones predeterminadas son: </p> 
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
      <td> <p>Especifique una gravedad para la solicitud. La gravedad debe definir el impacto que esta solicitud tiene en su trabajo en caso de que no se resuelva a tiempo. Las opciones predeterminadas son:</p> 
       <ul> 
        <li>Cosmético</li> 
        <li>Causa confusión</li> 
        <li>Error con solución</li> 
        <li>Error sin solución</li> 
        <li>Error fatal</li> 
       </ul> <p>El administrador del sistema puede modificar los nombres de las gravedades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contacto principal</strong> </td> 
      <td>El contacto principal de una solicitud es de forma predeterminada usted, ya que es la persona indicada para responder a cualquier pregunta relacionada con la solicitud. Sin embargo, puede cambiarlo por cualquier otro usuario de Workfront.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Asignaciones</strong> </td> 
      <td> <p><span>Especifique el nombre de un usuario activo, función o equipo al que se debe asignar la solicitud.</span> </p> <p>Solo puede especificar un equipo.</p>

   <p> Según la configuración de la cola de solicitudes, es posible que solo pueda asignar uno o dos tipos de recursos a la solicitud, en lugar de los tres (por ejemplo, puede que solo pueda asignar la solicitud a los usuarios).</p>

   <p>Si una regla de enrutamiento también está asociada a la cola de solicitudes y enruta automáticamente la solicitud a un tipo diferente de recurso (por ejemplo, un equipo), la solicitud se asigna tanto a la entidad que especifique manualmente al enviar la solicitud (usuarios) como al recurso especificado en la regla de enrutamiento (el equipo). </p>

   <p> Para obtener más información, consulte los siguientes artículos:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Crear reglas de enrutamiento</a> <br> </p> </li> 
      </ul> </p>

   <p><span>Recomendamos utilizar reglas de enrutamiento para las colas de solicitudes de modo que se puedan enrutar automáticamente a los recursos apropiados.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Horas planificadas</strong> </td> 
      <td> <p>Calcule cuántas horas tardaría esta solicitud en completarse.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha de inicio planificada</strong> </td> 
      <td> <p>Especifique la fecha en la que debe comenzar el trabajo en esta solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha planificada de finalización</strong> </td> 
      <td>Especifique la fecha en la que desea que se resuelva esta solicitud.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estado</strong> </td> 
      <td>El estado predeterminado de una nueva solicitud es "Nuevo". Es posible que el administrador del sistema haya cambiado el nombre de este estado. También puede cambiar el estado a otro en este menú desplegable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Añada documentos a su solicitud. </p> <p> Según la configuración de la cola de solicitudes, la sección Documentos podría mostrarse antes o después de los campos personalizados. </p> <p>Los documentos que se cargan en Workfront se almacenan durante 24 horas en un borrador de solicitud. Después, debe volver a adjuntarlos cuando vuelva a editar y enviar el borrador. Los documentos vinculados desde otras unidades se guardan en el borrador de forma permanente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Si el administrador de Workfront ha asociado un formulario personalizado a la cola de solicitudes o al tema de la cola, especifique los campos dentro del formulario personalizado.\
   Los formularios personalizados son diferentes para cada instancia de Workfront.
1. (Opcional y condicional) En cualquier momento mientras escribe la solicitud, haga clic en [!UICONTROL **Descartar borrador**] si desea eliminar el borrador que se crea automáticamente. Esto elimina el borrador que no se puede recuperar. Se mostrará un mensaje de confirmación para confirmar que lo está eliminando.

1. (Opcional) Haga clic en [!UICONTROL **Deshacer**] en el mensaje de confirmación si desea revertir la acción y conservarlo.

1. Realice una de las siguientes acciones:

   * Haga clic en **Enviar** si está listo para enviar la solicitud. La solicitud se guarda en la sección Enviada. En función de la regla de enrutamiento de la cola de solicitudes, esta solicitud puede redirigirse a un proyecto diferente al designado como cola de solicitudes. Para obtener información acerca de las reglas de enrutamiento, consulte [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     O

     Haga clic en **Cerrar** si no estás listo para enviarlo y puede volver y terminarlo más adelante. La solicitud se guardará en la sección Borradores y estará disponible la próxima vez que envíe una solicitud para esta cola de solicitudes.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   Al enviar la solicitud, el borrador se eliminará automáticamente y no se podrá restaurar.

   Las solicitudes enviadas se enumeran en la sección **Enviadas** del área de solicitudes. Si está usando la nueva experiencia, las solicitudes enviadas por Workfront se mostrarán en la ficha **Workfront** del área de Solicitudes.

   Para obtener información acerca de cómo direccionar las solicitudes de entrada, consulte el artículo [Administración de solicitudes de trabajo y equipo](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Para obtener información sobre cómo buscar solicitudes enviadas o en borrador, consulte también [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Creación de solicitudes desde fuera de Workfront

Puede compartir un vínculo directo a una cola de solicitudes cuando envíe una nueva solicitud e incrustarla en otras aplicaciones. Los usuarios que acceden a este vínculo desde la web o desde otras aplicaciones también deben iniciar sesión con una cuenta activa de Workfront para poder acceder a esta cola y enviar solicitudes a la misma. Para obtener más información, consulte [Compartir un vínculo a una cola de solicitudes](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Creación de solicitudes por correo electrónico en Workfront

Si la cola de solicitudes está habilitada para recibir solicitudes por correo electrónico, puede enviarlas por correo electrónico directamente a la dirección de correo electrónico asociada a la cola.

El texto del cuerpo del correo electrónico se añade como descripción de la solicitud.

>[!NOTE]
>
>El formato de HTML se elimina cuando la solicitud entra en Workfront, pero las firmas y el contenido del hilo Responder a existente no se eliminan y aparecen en la descripción de la solicitud.

Para obtener información acerca de cómo habilitar una cola de solicitudes para recibir solicitudes por correo electrónico, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitudes](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Creación de solicitudes con la aplicación móvil de Workfront

Puede enviar solicitudes mediante la aplicación móvil en su smartphone. Puede crear una nueva solicitud y enviarla a las colas de solicitudes a las que tiene acceso de visualización en la aplicación web.

Para obtener información sobre el envío de solicitudes a través de la aplicación móvil, consulte la sección Solicitudes en los artículos:

* [Adobe Workfront para Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests)
* [Adobe Workfront para iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## Creación de solicitudes desde otras aplicaciones

Puede enviar solicitudes utilizando cualquier aplicación que se haya integrado con Workfront:

* Puede crear una integración personalizada entre Workfront y otra aplicación que le permita enviar solicitudes a Workfront desde la otra aplicación.\
  Para obtener más información acerca de las integraciones de Workfront personalizadas, consulte el artículo [Integraciones de Adobe Workfront](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

## Creación de solicitudes mediante un formulario de solicitud de Workfront Planning

Puede agregar una solicitud de Workfront Planning mediante un formulario de solicitud de Planning. Si agrega solicitudes de Workfront Planning, puede crear registros de Planning si el formulario de solicitud está aprobado o si no requiere aprobación.

Su organización debe adquirir un paquete de Workfront Planning para poder enviar solicitudes de Planning.

Para obtener más información, consulte los siguientes artículos:

* [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* [Envíe solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Localizar solicitudes enviadas

Para obtener información sobre cómo localizar solicitudes enviadas o en borrador, consulte [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
