---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurar [!DNL Adobe Workfront for Jira]
description: Puede utilizar [!DNL Adobe Workfront for Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 4ade799ff735183f83f045e7eaa876961d266208
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Jira]

Puede utilizar [!DNL Adobe Workfront for Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.

Después de instalar el complemento, puede definir los flujos de trabajo que crean [!DNL Jira] problemas automáticamente al [!DNL Workfront] los elementos de trabajo se crean. Los elementos de ambas aplicaciones se vinculan y parte de su información se actualiza automáticamente en ambos sistemas.

Todos los usuarios en [!DNL Workfront] y [!DNL Jira] puede beneficiarse de esta integración. Solo necesitan una licencia para el sistema en el que más trabajan, y no para ambos sistemas.

Este complemento está disponible tanto para [!UICONTROL Servidor] y [!UICONTROL OnDemand] (o [!UICONTROL Nube]) versiones de [!DNL Jira] Software.

Para obtener una lista de [!DNL Jira] versiones que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) en el [!DNL Atlassian Marketplace].

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] [plan]*</td> 
   <td><p>Nuevo plan: Cualquiera</p>
       <p>o</p>
       <p>Plan actual: [!UICONTROL Pro] o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td><p>Nuevo plan: [!UICONTROL Standard] </p>
       <p>o</p> 
       <p>Plan actual: [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Le recomendamos que cree cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de utilizar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser un [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de poder configurar [!DNL Workfront for Jira], debe:

* Instalar [!DNL Workfront for Jira].
Para obtener instrucciones sobre la instalación [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurar [!DNL Workfront for Jira]

Al configurar [!DNL Workfront for Jira], puede:

* Definir los déclencheur que se crearán [!DNL Jira] elementos cuando [!DNL Workfront] se crean los elementos.
* Especifique qué campos deben sincronizarse entre los elementos vinculados entre [!DNL Jira] y [!DNL Workfront].

>[!NOTE]
>
>* Después de configurar [!DNL Workfront for Jira] en su [!DNL Jira] entorno, todos [!DNL Jira] los usuarios ven un [!DNL Workfront] panel derecho en todo [!DNL Jira] elementos. El panel contiene información sobre los elementos que pueden estar vinculados a [!DNL Workfront] o especifica que no [!DNL Workfront] los elementos están vinculados a [!DNL Jira] elementos.
>* Al usar el [!DNL Jira Server] instalación, solo los problemas asociados con los proyectos identificados como déclencheur para la integración de Workfront muestran el panel Workfront. Para obtener más información sobre la configuración de déclencheur para [!DNL Workfront to Jira] flujo de trabajo, consulte [Configurar déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Para configurar [!DNL Workfront for Jira]:

1. Iniciar sesión en [!DNL Jira] as a [!DNL Jira] administrador.
1. Clic **[!UICONTROL Configuración]** en el principal [!DNL Jira] menú.
1. Clic **[!UICONTROL Complementos]**, luego haga clic en **[!UICONTROL Administración de complementos]**.

1. Expanda el **[!DNL Workfront]** complemento de.
1. Clic **[!UICONTROL Configurar]**.
1. Siga las indicaciones para iniciar sesión en [!DNL Workfront].

   >[!NOTE]
   >
   >El usuario debe tener un válido `apiKey` in [!UICONTROL Workfront] para crear una conexión correcta.

   Debe iniciar sesión en [!DNL Workfront] as a [!DNL Workfront] para continuar con la configuración.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] se conecta a [!DNL Jira] uso de OAuth 2.0, un estándar utilizado por la mayoría de las integraciones basadas en la web para la autenticación y autorización de usuarios.
   >* Cuando se le pida que introduzca el dominio de su [!DNL Workfront] , escríbalo con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.
   >* La autenticación mejorada no está disponible hasta que [!DNL Workfront] El administrador lo habilita para esta integración.

1. En Jira, seleccione la **[!UICONTROL Déclencheur]** para configurar la creación automática de [!DNL Jira] elementos como nuevos [!DNL Workfront] se crean los elementos.

   Para obtener más información sobre la configuración de déclencheur para que Workfront [!DNL Jira] flujo de trabajo, consulte [Configurar déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Seleccione el **[!UICONTROL Configurar]** para configurar la sincronización de campos entre campos vinculados [!DNL Jira] y [!DNL Workfront] elementos.

   Para obtener más información sobre la configuración de la sincronización de campos entre [!DNL Jira] y [!DNL Workfront], consulte [Configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Después de definir los déclencheur y la sincronización de campos entre las dos aplicaciones, cualquier [!DNL Workfront] Un usuario que puede crear tareas o problemas podría poner en déclencheur la creación de un elemento en [!DNL Jira]. El usuario puede crear un elemento si los criterios del elemento que crea coinciden con los déclencheur de [!DNL Jira], incluso si el usuario no tiene un [!DNL Jira] licencia. Además, cualquier [!DNL Jira] el usuario puede empezar a trabajar inmediatamente en el [!DNL Jira] y sus actualizaciones son visibles en [!DNL Workfront], sin que tengan un [!DNL Workfront] licencia. Cualquier actualización en [!DNL Workfront] también son visibles en la [!DNL Jira] elementos.

1. (Opcional) Seleccione la **[!UICONTROL Registro de actividad]** para revisar los errores que se hayan producido durante la integración.

   Para obtener más información sobre [!UICONTROL Registro de actividad], consulte [Ver el [!DNL Jira] [!UICONTROL Registro de actividad]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurar déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]

Como el [!DNL Jira] administrador del sistema, puede definir déclencheur que creen problemas automáticamente en [!DNL Jira] cuando un elemento entre [!DNL Workfront] cumple determinados criterios.

>[!NOTE]
>
>La integración puede tardar hasta 10 minutos en crear nuevos problemas en [!DNL Jira].

Tenga en cuenta lo siguiente al configurar y activar la creación de [!DNL Jira] elementos como [!DNL Workfront] se crean los elementos:

* La integración es unidireccional: solo puede almacenar en déclencheur los elementos que cree en [!DNL Workfront] que se creará automáticamente en [!DNL Jira]. No se pueden almacenar en déclencheur los elementos creados en [!DNL Jira] para que se cree automáticamente en [!DNL Workfront].
* No hay límite en cuanto a la cantidad de déclencheur que puede tener.
* Si un elemento que crea en [!DNL Workfront] coincide con más de un déclencheur, solo se crea un elemento en [!DNL Jira]. El elemento se crea en [!DNL Jira] según el primer déclencheur (en el orden en que se hayan definido en [!DNL Jira]). El resto de déclencheur se ignoran.
* Solo un elemento en [!DNL Workfront] se puede vincular a un elemento en Jira. Nunca se puede vincular uno [!DNL Workfront] elemento a varios [!DNL Jira] problemas, o uno [!DNL Jira] problema a varios [!DNL Workfront] elementos.

Para configurar déclencheur para crear elementos automáticamente en [!DNL Jira]:

1. Iniciar sesión en [!DNL Jira] como administrador del sistema.
1. Clic **[!UICONTROL Configuración]** en el principal [!DNL Jira] menú.
1. Clic **[!UICONTROL Complementos]**, entonces **[!UICONTROL Administración de complementos]**.
1. Expanda el **[!DNL Workfront]** complemento de.
1. Clic **[!UICONTROL Configurar]**.
1. Iniciar sesión en [!DNL Workfront] como administrador del sistema.

   El **[!UICONTROL Déclencheur]** está seleccionada de forma predeterminada en Jira.

1. Clic **[!UICONTROL Añadir déclencheur]** para añadir un nuevo déclencheur.
1. En el **[!UICONTROL equipo/usuario/función de Workfront]** , especifique el nombre de un campo [!DNL Workfront] equipo, usuario o función del puesto y, a continuación, haga clic en para seleccionarlo cuando se muestre en la lista.

   >[!NOTE]
   >
   >No puede tener varios déclencheur para el mismo equipo, usuario o rol.

   Cuando alguien crea una tarea o un problema y lo asigna a una de estas entidades, se crea automáticamente un problema en [!DNL [!DNL Jira]].

1. En el **[!UICONTROL [!DNL Jira]proyecto]** , empiece a escribir el nombre de un [!DNL Jira] proyecto y, a continuación, haga clic en para seleccionarlo cuando se muestre en la lista.

   Si la variable [!DNL Jira] Se crea el problema y se coloca en el proyecto que eligió aquí.

1. Seleccione un **I[!UICONTROL tipo de problema]** en el menú desplegable.

   Indica el tipo de problema que se crea en [!DNL Jira] cuando se cumplan las condiciones de este déclencheur, en función de la configuración de ese proyecto específico en [!DNL Jira].

1. Haga clic en **[!UICONTROL Guardar]**.

   Con esta configuración, cada vez que [!DNL Workfront] Si el usuario crea un elemento que coincide con los déclencheur especificados, se crea un nuevo problema en [!DNL Jira].

## Configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos

Como el [!DNL Jira] administrador, puede definir qué campos deben sincronizarse automáticamente en los elementos vinculados entre [!DNL Workfront] y Jira. Algunos campos se pueden sincronizar desde el [!DNL Workfront] a la [!DNL Jira] y otros se sincronizan de Jira a Workfront.

Para definir qué campos deben sincronizarse automáticamente en los elementos vinculados entre las dos aplicaciones:

1. Iniciar sesión en [!DNL Jira] como administrador de Jira.
1. Clic **[!UICONTROL Configuración]** en el principal [!DNL Jira] menú.
1. Clic **[!UICONTROL Complementos]**, entonces **[!UICONTROL Administración de complementos]**.
1. Expanda el **[!DNL Workfront]** complemento de.
1. Clic **[!UICONTROL Configurar]**.
1. Iniciar sesión en [!DNL Workfront] como administrador de Workfront.
1. En Jira, haga clic en **[!UICONTROL Configurar]** pestaña.
1. En el **[!UICONTROL Sincronizar desde Workfront a Jira]** , seleccione los campos que desea actualizar en [!DNL Jira] cuando se actualizan en Workfront.

   1. Seleccione cualquiera de las siguientes frecuencias con las que se sincronizan los campos:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Al Crear]</td>
              <td>Los campos que especifique se sincronizan entre el Workfront vinculado y [!DNL Jira] elementos cuando el elemento se crea en Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Siempre]</td>
              <td>Los campos que especifique se sincronizan entre el Workfront vinculado y [!DNL Jira] elementos cuando los campos se actualizan en Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Nunca]</td>
              <td>Los campos que especifique nunca se sincronizan entre los campos vinculados [!DNL Workfront] y [!DNL Jira] elementos. No hay ninguna indicación en [!DNL Jira] que el campo se ha actualizado en [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Seleccione cualquiera de las siguientes opciones para sincronizar los campos [!DNL Workfront] hasta [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Nombre]</td>
         <td><p>El nombre de una tarea o un problema en [!DNL Workfront] se convierte en el nombre del problema al que está vinculado [!DNL Jira].</p><p>Nota: Cuando se crean nuevos elementos en [!DNL Jira] automáticamente, la variable [!DNL Workfront] El nombre siempre se actualiza en [!DNL Jira] elemento, independientemente de si este campo está habilitado aquí o no. Cuando un [!DNL Jira] el elemento está vinculado manualmente a [!DNL Workfront] elemento, el nombre del [!DNL Workfront] sólo actualizaciones de elementos en [!DNL Jira] al seleccionar <strong>Siempre</strong> sincronice este campo. Para obtener más información sobre cómo vincular elementos de forma manual o automática, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descripción]</td>
         <td>La descripción de una tarea o un problema en [!DNL Workfront] se convierte en la descripción del problema al que está vinculado en [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documentos</td>
         <td><p>Documentos adjuntos a una tarea o a un problema en [!DNL Workfront] también se adjuntan al problema al que está vinculado en Jira. Nuevas versiones de documento de [!DNL Workfront] se añaden como documentos independientes a Jira y se anexan con <i>_v&lt;version number=""&gt;</i> para indicar la versión numerada en Workfront. </p><p>Por ejemplo, si el nombre de un documento en [!DNL Workfront] es <strong>Anuncio principal</strong>, y se le añade una nueva versión en [!DNL Workfront], la nueva versión se transfiere a [!DNL Jira] como documento nuevo con el nombre <strong>Ad_v2 principal</strong>.</p><p>Importante: <p>Tenga en cuenta lo siguiente al sincronizar documentos:</p>
           <ul>
            <li><p>Los documentos de más de 5 MB no se sincronizan. Si falla la sincronización de un documento porque es demasiado grande, se registra un error en el registro de actividades. </p><p>Para obtener más información sobre el registro de actividades, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Ver el registro de actividades de Jira</a>.</p></li>
            <li><p>Los documentos vinculados a tareas y problemas de servidores externos no se transfieren al [!DNL Jira] elementos. Solo los documentos cargados directamente en la tarea o el problema en [!DNL Workfront] se transfieren al problema vinculado en [!DNL Jira].</p></li>
            <li><p>Para crear una prueba a partir de un documento, debe generarla en [!DNL Workfront]. </p><p>Para obtener más información sobre la generación de una prueba, consulte <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Crear una prueba para un documento existente </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Creación de una prueba para un documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Fecha planificada de finalización]</td>
         <td><p>[!UICONTROL Fecha planificada de finalización] de una tarea o un problema en [!DNL Workfront] se convierte en el [!UICONTROL Fecha de vencimiento] del problema al que está vinculado [!DNL Jira].</p><p>Nota: Asegúrese de que muestra <strong>[!UICONTROL Fecha de vencimiento]</strong> el [!DNL Jira] problemas, para que este valor se sincronice.</p></td>
        </tr>
       </tbody>
      </table>

1. En el **[!UICONTROL Sincronizar desde [!DNL Jira] hasta[!DNL Workfront]]** , seleccione los campos que desea actualizar en [!DNL Workfront] cuando se actualizan en [!DNL Jira].

   1. Seleccione cualquiera de las siguientes frecuencias con las que se sincronizan los campos:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Siempre]</td>
         <td>Los campos que especifique siempre se sincronizan entre los campos vinculados [!DNL Workfront] y [!DNL Jira] elementos al actualizar los campos en [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nunca]</td>
         <td><p>Los campos que especifique nunca se sincronizan entre los campos vinculados [!DNL Workfront] y [!DNL Jira] elementos. No hay ninguna indicación en [!DNL Workfront] que el campo se ha actualizado en [!DNL Jira]. </p><p>Nota: Cuando selecciona Nunca, [!DNL Workfront] Los campos de aún se pueden actualizar manualmente desde [!DNL Jira] en la izquierda [!DNL Workfront] panel de la [!DNL Jira] problema. Estas actualizaciones solo aparecen en [!DNL Workfront] elementos en [!DNL Jira] y [!DNL Workfront] y no en [!DNL Jira] elementos.</p></td>
        </tr>
       </tbody>
      </table>

   1. Seleccione para sincronizar cualquiera de los siguientes campos de [!DNL Jira] hasta [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Estado]</td>
         <td>[!UICONTROL Estado] de un problema en [!DNL Jira] se convierte en el [!UICONTROL Status] de la tarea o el problema al que está vinculado [!DNL Workfront].<br>Para obtener más información acerca de [!DNL Workfront] estados, consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creación o edición de un estado</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Asignado]</td>
         <td><p>[!UICONTROL Asignado] de un problema en [!DNL Jira] se convierte en el [!UICONTROL usuario asignado] de la tarea o problema al que está vinculado [!DNL Workfront].</p><p>Importante: Cuando asigna un elemento en [!DNL Jira] a un usuario que no tiene un [!DNL Workfront] cuenta, la integración crea un nuevo usuario activo en [!DNL Workfront] solo cuando <strong>Crear automáticamente un usuario en [!DNL Workfront] si la variable [!DNL Jira] el usuario no tiene un [!DNL Workfront] account</strong> se establece en <strong>[!UICONTROL Siempre]</strong>. Este usuario no ocupa un [!DNL Workfront] licencia. Los usuarios activos pueden ser asignados a elementos de trabajo en [!DNL Workfront], pero no se puede incluir en las actualizaciones. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Archivos adjuntos]</td>
         <td>Archivos adjuntos de un problema en [!DNL Jira] también están adjuntos a la tarea o problema al que están vinculados en [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comentarios]</td>
         <td><p>Un comentario en una [!DNL Jira] Este problema también se publica en el [!DNL Workfront] en el área de [!UICONTROL Updates]. Por el contrario, un comentario publicado en el área de [!UICONTROL Updates] para un [!DNL Workfront] la tarea o el problema se sincroniza con [!DNL Jira]Flujo de comentarios nativo de para el problema vinculado. </p><p>Se establece en <strong>[!UICONTROL Siempre]</strong> de forma predeterminada. Si selecciona <strong>[!UICONTROL Nunca]</strong> aquí, todavía puede publicar comentarios manualmente sobre un elemento vinculado en [!DNL Workfront] o en [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. En el **[!UICONTROL OTROS]** , seleccione qué campos adicionales deben actualizarse entre los elementos vinculados.

   1. Seleccione una opción para determinar si los campos especificados **[!UICONTROL Siempre]** o **[!UICONTROL Nunca]** actualizar en [!DNL Jira] o [!DNL Workfront] cuando se modifiquen.

   1. Seleccione entre los siguientes campos y actualizaciones:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar [!DNL Workfront] Datos personalizados en el panel derecho de [!DNL Jira]]</td>
         <td><p>Muestra el [!DNL Workfront] Datos personalizados de un elemento en [!DNL Workfront] panel derecho.</p><p>Nota: Las secciones de formulario personalizado se muestran en la variable [!DNL Workfront] panel derecho con el nivel de acceso del [!DNL Workfront] Administrador del sistema.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar [!DNL Workfront] Prioridad en el panel derecho de [!DNL Jira]]</td>
         <td>Muestra el [!DNL Workfront] Prioridad de un elemento en [!DNL Workfront] panel derecho.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Agregar una actualización en [!DNL Workfront] Actualiza la pestaña acerca de los cambios de Fecha de vencimiento en [!DNL Jira]]</td>
         <td>Agrega un comentario en la ficha [!UICONTROL Update] del [!DNL Workfront] cuando cambie la [!UICONTROL Fecha de vencimiento] en el elemento vinculado [!DNL Jira] elemento.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Crear automáticamente un usuario en [!DNL Workfront] si la variable [!DNL Jira] el usuario no tiene un [!DNL Workfront] account]</td>
         <td><p>Existen los siguientes escenarios:</p>
          <ul>
           <li>Al seleccionar <strong>[!UICONTROL Siempre]</strong>, la integración se habilita para crear un nuevo usuario de Workfront cada vez que se crea un [!DNL Jira] usuario sin [!DNL Workfront] realiza las siguientes acciones en un recurso vinculado [!DNL Jira] problema:
            <ul>
             <li>Se ha asignado a un [!DNL Jira] problema</li>
             <li><p>Registra el tiempo en un [!DNL Jira] problema</p><p>Este nuevo usuario no ocupa un [!DNL Workfront] licencia. El valor predeterminado es Siempre. El usuario ha creado de este modo en [!DNL Workfront] tiene "[!UICONTROL Jira]" agregado a su nombre.</p></li>
            </ul></li>
           <li>Al seleccionar <strong>[!UICONTROL Nunca]</strong>Sin embargo, suceden las siguientes cosas:
            <ul>
             <li>No es posible ver ninguna [!DNL Jira] asignaciones en el [!DNL Workfront] elementos. En este caso, solo las asignaciones realizadas en [!DNL Workfront] mostrar en la [!DNL Workfront] elementos.</li>
             <li>La hora registrada en un vínculo [!DNL Jira] Problema de un usuario sin [!DNL Workfront] La cuenta de no se transfiere automáticamente al vínculo de [!DNL Workfront] elemento. Todavía puede registrar tiempo en el [!DNL Workfront] elemento en el panel derecho del [!DNL Jira] problema.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Haga clic en **[!UICONTROL Guardar]**.

   Ahora, cada vez que un usuario actualiza cualquiera de los campos especificados en esta configuración en un elemento de [!DNL Jira] o [!DNL Workfront], el elemento vinculado en la otra aplicación también se actualiza.

## Resolución de problemas

### Los elementos no se pueden crear en [!DNL Jira] debido a los campos de déclencheur marcados con &quot;[!UICONTROL No se pudo encontrar]&quot;

#### Problema

Cuando se produce un error con la variable [!DNL Workfront for Jira] aplicación, [!DNL Workfront] deshabilita los déclencheur para prevenir complicaciones adicionales. Cuando estos déclencheur están desactivados, se muestran como &quot;[!UICONTROL No se pudo encontrar].&quot;

#### Solución

Busque el error que deshabilitó las déclencheur. Puede encontrar el error en la [!DNL Workfront for Jira] [!UICONTROL Registro de actividad].

La causa más común de este comportamiento es el error &quot;[!UICONTROL No se puede establecer el campo &#39;duedate&#39;. No aparece en la pantalla adecuada o es desconocido.]&quot;

Este error significa que está intentando sincronizar el &quot;[!UICONTROL Fecha planificada de finalización]&quot; de [!DNL Workfront] hasta [!DNL Jira]. Para ello, debe asegurarse de que su [!DNL Jira] Los objetos de tienen un campo llamado &quot;[!UICONTROL Fecha de vencimiento].&quot; Si no tiene este campo, [!DNL Workfront] no puede sincronizar la fecha planificada de finalización desde [!DNL Workfront] y deshabilita las déclencheur.

Para resolver este error, intente una de las siguientes acciones:

* Pregunte a su [!DNL Jira] para actualizar el afectado [!DNL Jira] para asegurarse de que tienen un campo de fecha de vencimiento.
* Desactivar la sincronización de [!DNL Workfront]Fecha planificada de finalización de en Workfront [!UICONTROL Configurar] página.
