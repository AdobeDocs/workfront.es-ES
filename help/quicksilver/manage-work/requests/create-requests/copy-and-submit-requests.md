---
title: Copiar y enviar solicitudes
description: Cuando envía solicitudes similares con frecuencia, puede copiar una solicitud enviada existente. En este caso, puede copiar una solicitud existente, realizar cambios mínimos en ella y volver a enviarla como una solicitud nueva.
author: Lisa
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 4ec3732d547cb3976c1376cbd0cf86b44b0e691b
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 99%

---

# Copiar y enviar solicitudes

Cuando envía solicitudes similares con frecuencia, puede copiar una solicitud enviada existente. En este caso, puede copiar una solicitud existente, realizar cambios mínimos en ella y volver a enviarla como una solicitud nueva.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p><b>NOTA</b>

Si no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso para añadir solicitudes a una cola de solicitudes</p> <p>Ver permisos superiores en la solicitud existente</p> <p>Para obtener información sobre cómo configurar una cola de solicitudes, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: colaborador o superior</p>
   O
   <p>Actual: solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  </td> 
  </tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Acceso para añadir solicitudes a una cola de solicitudes</p> <p>Ver permisos superiores en la solicitud existente</p> <p>Para obtener información sobre cómo configurar una cola de solicitudes, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe tener una solicitud que usted o alguien de su organización haya enviado anteriormente para poder copiarla y volver a enviarla. Si la solicitud pertenece a otra persona, debe tener al menos acceso a la Vista para poder copiarla y enviarla como nueva.

## Consideraciones sobre cómo copiar y enviar solicitudes como nuevas

* Solo puede copiar y enviar solicitudes enviadas. No puede copiar solicitudes redactadas.
* Puede copiar y enviar solicitudes que haya enviado originalmente, o solicitudes que otros hayan enviado siempre que tenga acceso al menos a Vista.
* Siempre tiene permiso de acceso para copiar y enviar una copia de sus propias solicitudes, a menos que alguien le quite estos permisos.
* El acceso para copiar y enviar solicitudes enviadas originalmente por otros podría concederse automáticamente a personas de la misma compañía cuando el creador de la cola de solicitudes habilite **Las personas de la misma compañía heredarán los mismos permisos para todas las solicitudes** en las áreas Detalles de cola o Editar proyecto. Deshabilitar esta configuración solo permite que el solicitante original vea sus propias solicitudes.

  Para obtener más información, consulte los siguientes artículos:

   * [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md)

* Puede actualizar la copia de la solicitud original antes de volver a enviarla como una solicitud nueva.
* Si se producen los siguientes cambios después de enviar la solicitud original, ya no podrá copiarla y volver a enviarla:

   * Se eliminó la cola de solicitudes.
   * Se eliminó el tema de la cola.

     >[!TIP]
     >
     >Si el tema de la cola era el único en la cola de solicitudes, aún puede copiar y enviar la solicitud y se guardará en la propia cola.

   * La cola de solicitudes ya no se publica como cola de solicitudes de ayuda. Para obtener más información, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Si la cola de solicitudes no tiene ningún tema en cola y la solicitud original se envió antes de enero de 2022.

   * El estado del proyecto asociado a la cola de solicitudes ya no es Actual.

* Puede copiar y enviar una copia de una solicitud convertida si esta se ha conservado en el proceso de conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >La solicitud copiada no está vinculada a un objeto de resolución.

## Copiar y enviar solicitudes

{{step1-to-requests}}

1. (Condicional) Si la sección Enviados no se muestra de forma predeterminada, haga clic en **Enviados** en el panel izquierdo.

   >[!TIP]
   >
   >   Es posible que Workfront o el administrador de grupos personalicen la plantilla de diseño y eliminen áreas del menú principal o del panel izquierdo del entorno. En este caso, es posible que no estén a su disposición.

1. Busque la solicitud que desea copiar y enviar como nueva y realice una de las siguientes acciones:

   * Selecciónela y haga clic en **Copiar** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) en la esquina superior izquierda de la lista Solicitudes enviadas.

   >[!TIP]
   >
   > Si no ha seleccionado una solicitud primero, el icono Copiar aparece atenuado.

   * Haga clic en el menú **Más** ![](assets/more-icon.png) que se encuentra a la derecha del nombre de la solicitud, a continuación haga clic en **Copiar y enviar como nuevo**

     O

     Haga clic con el botón derecho en la solicitud seleccionada, a continuación haga clic en **Copiar y enviar como nuevo**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Cuando no tiene acceso para crear problemas, recibe la advertencia de que el administrador le ha restringido la creación de solicitudes.

1. (Opcional) Actualice la siguiente información, si es necesario:

   * **Tipo de solicitud**: la cola de solicitudes donde se ha guardado la solicitud copiada. De forma predeterminada, la solicitud copiada se guarda en la cola de solicitudes de la solicitud original.
   * **Grupos de temas** y **Temas de colas**, si están seleccionados. Los nombres o los grupos de temas y los temas de colas se personalizan según el entorno. De forma predeterminada, la solicitud copiada se guarda en los grupos de temas y en los temas de cola de la solicitud original.

     >[!TIP]
     >
     >Si la ruta cambia de la ruta de la solicitud original, el creador de la cola de solicitudes modificó la cola.

1. (Opcional) Actualice la información de la solicitud copiada. Según los campos que el creador de la cola de solicitudes habilitó en la sección **Nuevos campos de problema** de la subpestaña **Detalles de la cola** del proyecto, podría encontrar cualquiera de los siguientes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Asunto</strong> </td> 
      <td>Muestra el nombre de la solicitud original. Actualícelo si es necesario.De lo contrario, Workfront denomina a la solicitud copiada <b>Copia de &lt;Nombre de la solicitud original&gt;</b>. Este campo es obligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td>Muestra la descripción de la solicitud original. Actualícelo si es necesario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Muestra la dirección URL de la solicitud original. Actualícelo si es necesario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad</strong> </td> 
      <td> <p>Especifique la prioridad de la solicitud. La prioridad debe definir la rapidez con la que cree que se debe resolver esta solicitud. Las opciones predeterminadas son las siguientes:</p> 
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
      <td> <p>Especifique la gravedad de la solicitud. La gravedad debe definir el impacto que esta solicitud tiene en su trabajo en caso de que no se resuelva a tiempo. Las opciones predeterminadas son las siguientes:</p> 
       <ul> 
        <li>Cosmético</li> 
        <li>Causa confusión</li> 
        <li>Error con solución</li> 
        <li>Error sin solución</li> 
        <li>Error fatal</li> 
       </ul> <p>El administrador de Workfront puede modificar los nombres de las gravedades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contacto principal</strong> </td> 
      <td>El contacto principal de una solicitud es de forma predeterminada usted, ya que es la persona indicada para responder a cualquier pregunta relacionada con la solicitud. Sin embargo, puede cambiarlo por cualquier otro usuario de Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Asignaciones</strong></span> </td> 
      <td> <p>Indique el nombre de un usuario, una función o un equipo activo al que se debe asignar la solicitud. </p> <p> Puede especificar más de un usuario, una función o un equipo. </p> <p>Según la configuración de la cola de solicitudes, es posible que solo pueda asignar la solicitud a uno o dos tipos de recursos, en lugar de a los tres. </p> <p>Se recomienda utilizar reglas de enrutamiento para las colas de solicitudes, de modo que se puedan enrutar automáticamente a los recursos adecuados. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Según la configuración de la cola de solicitudes, es posible que solo pueda asignar un tipo de recurso a la solicitud (por ejemplo, usuarios). Si una regla de enrutamiento también está asociada a la cola de solicitudes y enruta automáticamente la solicitud a un tipo diferente de recurso (por ejemplo, un equipo), la solicitud se asigna tanto a la entidad que especifique manualmente al enviar la solicitud (usuarios) como al recurso especificado en la regla de enrutamiento (el equipo).</p> <p style="font-weight: normal;">Para obtener más información, consulte los siguientes artículos:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Crear reglas de enrutamiento</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Horas planificadas</strong> </td> 
      <td> <p>Calcule cuántas horas tardaría esta solicitud en completarse.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha planificada de inicio</strong> </td> 
      <td> <p>La fecha en la que debería comenzar el trabajo en esta solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha planificada de finalización</strong> </td> 
      <td>La fecha en la que desea que se resuelva esta solicitud.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estado</strong> </td> 
      <td>El estado predeterminado de una nueva solicitud es "Nuevo". Es posible que el administrador de Workfront haya cambiado el nombre de este estado. También puede cambiar el estado a otro en este menú desplegable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Añada documentos a su solicitud. Los documentos adjuntos a la solicitud original no se transfieren a la solicitud copiada.</p> <p><b>Sugerencia</b>

   Según la configuración de la cola de solicitudes, la sección Documentos podría mostrarse antes o después de los campos personalizados.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Opcional) Actualice la información de los formularios personalizados adjuntos si es necesario.

   >[!TIP]
   >
   >* Todos los formularios personalizados adjuntos a la solicitud original y los valores incluidos en los campos personalizados se transfieren a la solicitud copiada. Esto incluye campos que contienen lógica.
   >* No se pueden eliminar los formularios personalizados de la solicitud copiada.

1. Haga clic en **Enviar**.

   La solicitud copiada se envía como una nueva solicitud en la cola de solicitudes especificada.
