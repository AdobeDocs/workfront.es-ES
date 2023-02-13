---
title: Copiar y enviar solicitudes
description: Copiar y enviar solicitudes
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# Copiar y enviar solicitudes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is NWE only - hard code it in classic articles!)</p>
-->

Cuando envía solicitudes similares con frecuencia, puede copiar una solicitud enviada existente. En este caso, puede copiar una solicitud existente, realizar cambios mínimos en ella y volver a enviarla como una solicitud nueva.

## Requisitos de acceso

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
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
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso para agregar solicitudes a una cola de solicitudes</p> <p>Ver o permisos superiores en la solicitud existente</p> <p>Para obtener información sobre la configuración de una cola de solicitudes, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe tener una solicitud que usted u otra persona de su organización hayan enviado anteriormente para poder copiarla y volver a enviarla. Si la solicitud pertenece a otra persona, debe tener al menos acceso a Ver para poder copiarla y enviarla como nueva.

## Consideraciones sobre cómo copiar y enviar solicitudes como nuevas

* Solo puede copiar y enviar solicitudes enviadas. No se pueden copiar solicitudes redactadas.
* Puede copiar y enviar solicitudes que haya enviado originalmente, o solicitudes que otros hayan enviado y que usted tenga acceso al menos a Ver.
* Siempre tiene acceso para copiar y enviar una copia de sus propias solicitudes, a menos que alguien haya eliminado sus permisos.
* El acceso para copiar y enviar solicitudes enviadas originalmente por otros puede otorgarse automáticamente a personas de la misma empresa cuando el creador de la cola de solicitudes habilita la variable **Los usuarios de la misma empresa heredarán los mismos permisos para todas las solicitudes** en las áreas Detalles de cola o Editar proyecto . Deshabilitar esta configuración permite que solo el solicitante original vea sus propias solicitudes.

   Para obtener más información, consulte los siguientes artículos:

   * [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md)

* Puede actualizar la copia de la solicitud original antes de volver a enviarla como una nueva solicitud.
* Si se producen los cambios siguientes después de enviar la solicitud original, ya no se puede copiar y volver a enviarla:

   * Se eliminó la cola de solicitudes.
   * Se eliminó el tema de la cola.

      >[!TIP]
      >
      >Si el tema de la cola era el único de la cola de solicitudes, aún puede copiar y enviar la solicitud y se guardará en la propia cola de solicitudes.

   * La cola de solicitudes ya no se publica como cola de solicitud de ayuda. Para obtener más información, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Si la cola de solicitudes no tiene tema en cola y la solicitud original se envió antes de enero de 2022.

   * El estado del proyecto asociado con la cola de solicitudes ya no es actual.

* Puede copiar y enviar una copia de una solicitud convertida si la solicitud se ha conservado en el proceso de conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   >[!TIP]
   >
   >La solicitud copiada no está vinculada a un objeto de resolución.

## Copiar y enviar solicitudes

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Solicitudes**.
1. (Condicional) Si la sección Enviado no se muestra de forma predeterminada, haga clic en **Enviado** en el panel izquierdo.
1. Busque la solicitud que desea copiar y enviar como nueva y realice una de las siguientes acciones:

   * Selecciónelo y haga clic en el botón **Copiar y enviar como nuevo** icono ![](assets/copy-and-submit-as-new-requests-area-nwe.png) en la esquina superior izquierda de la lista de solicitudes enviadas.
   * Haga clic en el **Más** menú ![](assets/more-icon.png) a la derecha del nombre de la solicitud y haga clic en **Copiar y enviar como nuevo**

      O

      Haga clic con el botón derecho en la solicitud seleccionada y, a continuación, haga clic en **Copiar y enviar como nuevo**.

      ![](assets/request-selected-more-menu-options-nwe-350x191.png)

      >[!TIP]
      >
      >Cuando no tiene acceso para crear problemas, recibe una advertencia que indica que el administrador ha restringido la creación de solicitudes.

1. (Opcional) Actualice la siguiente información, si es necesario:

   * **Tipo de solicitud**: la cola de solicitudes donde se guarda la solicitud copiada. De forma predeterminada, la solicitud copiada se guarda en la cola de solicitudes de la solicitud original.
   * **Grupos de temas** y **Temas de cola**, si están seleccionados. Los nombres o grupos de temas y los temas de la cola se personalizan según el entorno. De forma predeterminada, la solicitud copiada se guarda en los grupos de temas y en los temas de cola de la solicitud original.

      >[!TIP]
      >
      >Si la ruta cambia de la ruta de la solicitud original, el creador de la cola de solicitudes modificó la cola.

1. (Opcional) Actualice cualquier información de la solicitud copiada. Según los campos que habilite el creador de la cola de solicitudes en la variable **Nuevos campos de problema** de la sección **Detalles de cola** en el proyecto, puede encontrar cualquiera de los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Asunto</strong> </td> 
      <td>Muestra el nombre de la solicitud original. Actualícelo, si es necesario. De lo contrario, Workfront asigna un nombre a la solicitud copiada <b>Copia de &lt;name of="" original="" request=""&gt;</b>. Se trata de un campo obligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td>Muestra la descripción de la solicitud original. Actualícelo, si es necesario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dirección URL</strong> </td> 
      <td> <p>Muestra la dirección URL de la solicitud original. Actualícelo, si es necesario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad</strong> </td> 
      <td> <p>Especifique la prioridad de la solicitud. La prioridad debe definir la velocidad con la que cree que se debe resolver esta solicitud. Las opciones predeterminadas son:</p> 
       <ul> 
        <li>Ninguno</li> 
        <li>Bajo</li> 
        <li>Normal</li> 
        <li>Alto</li> 
        <li>Urgente</li> 
       </ul> <p>El administrador de Workfront puede modificar los nombres de las prioridades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gravedad</strong> </td> 
      <td> <p>Especifique la gravedad de la solicitud. La gravedad debe definir el impacto que esta solicitud tiene en su trabajo si no se resuelve a tiempo. Las opciones predeterminadas son:</p> 
       <ul> 
        <li>Cosmético</li> 
        <li>Causa confusión</li> 
        <li>Error con solución</li> 
        <li>Error sin solución</li> 
        <li>Error fatal</li> 
       </ul> <p>El administrador de Workfront puede modificar los nombres de gravedad.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contacto primario</strong> </td> 
      <td>El Contacto Principal de una solicitud le toma por defecto, ya que usted es la persona de punto para abordar cualquier pregunta relacionada con la solicitud. Sin embargo, puede cambiarlo a cualquier otro usuario de Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Asignaciones</strong></span> </td> 
      <td> <p>Indique el nombre de un usuario, función de trabajo o equipo activo al que se debe asignar la solicitud. </p> <p> Puede especificar más de un usuario, función de trabajo o equipo. </p> <p>Según la configuración de la cola de solicitudes, es posible que solo pueda asignar la solicitud a uno o dos tipos de recursos, en lugar de a los tres. </p> <p>Se recomienda utilizar reglas de enrutamiento para las colas de solicitud de modo que se puedan enrutar automáticamente a los recursos adecuados. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Según cómo se haya configurado la cola de solicitudes, es posible que solo pueda asignar un tipo de recurso a la solicitud (por ejemplo, usuarios). Si una regla de enrutamiento también está asociada a la cola de solicitudes y enruta automáticamente la solicitud a un tipo diferente de recurso (por ejemplo, un equipo), la solicitud se asigna tanto a la entidad que especifique manualmente al enviar la solicitud (usuarios) como al recurso especificado en la regla de enrutamiento (el equipo).</p> <p style="font-weight: normal;">Para obtener más información, consulte los siguientes artículos:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Crear reglas de enrutamiento</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Horas planificadas</strong> </td> 
      <td> <p>Calcule cuántas horas tardaría esta solicitud en completarse.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha planificada de inicio</strong> </td> 
      <td> <p>La fecha en la que se debe iniciar el trabajo en esta solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha planificada de finalización</strong> </td> 
      <td>La fecha en la que desea que se resuelva esta solicitud.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estado</strong> </td> 
      <td>El estado predeterminado de una nueva solicitud es "Nuevo". Es posible que el administrador de Workfront haya cambiado el nombre de este estado. También puede cambiar el estado a otra cosa desde este menú desplegable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Agregue documentos a la solicitud. Los documentos adjuntos a la solicitud original no se transfieren a la solicitud copiada.</p> <p><b>SUGERENCIA</b>

   Dependiendo de cómo se haya configurado la cola de solicitudes, la sección Documentos podría mostrarse antes o después de los campos personalizados.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Opcional) Actualice la información en los formularios personalizados adjuntos, si es necesario.

   >[!TIP]
   >
   >* Todos los formularios personalizados adjuntos a la solicitud original y los valores incluidos en los campos personalizados se transfieren a la solicitud copiada. Esto incluye campos que contienen lógica.
   >* No se pueden quitar formularios personalizados de la solicitud copiada.


1. Haga clic en **Submit**.

   La solicitud copiada se envía como una nueva solicitud en la cola de solicitudes especificada.
