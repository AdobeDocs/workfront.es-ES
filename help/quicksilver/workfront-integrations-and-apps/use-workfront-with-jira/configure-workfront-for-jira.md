---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurar [!DNL Adobe Workfront for Jira]
description: Puede usar [!DNL Adobe Workfront for Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Jira]

Puede usar [!DNL Adobe Workfront for Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.

Después de instalar el complemento, puede definir los flujos de trabajo que crean [!DNL Jira] se emite automáticamente cuando [!DNL Workfront] se crean elementos de trabajo. Los elementos de ambas aplicaciones se vinculan y parte de su información se actualiza automáticamente en ambos sistemas.

Todos los usuarios de [!DNL Workfront] y [!DNL Jira] puede beneficiarse de esta integración. Sólo necesitan una licencia para el sistema en el que funcionan más y no para ambos sistemas.

Este complemento está disponible tanto para la variable [!UICONTROL Servidor] y [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) versiones de [!DNL Jira] Software.

Para obtener una lista de [!DNL Jira] versiones que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) en el [!DNL Atlassian Marketplace].

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] información general sobre licencias</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de usar las existentes que se podrían adjuntar a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de configurar [!DNL Workfront for Jira], debe

* Instalar [!DNL Workfront for Jira]\
   Para obtener instrucciones sobre la instalación [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurar [!DNL Workfront for Jira]

Configurando [!DNL Workfront for Jira] puede:

* Definir déclencheur que se crearán [!DNL Jira] elementos cuando [!DNL Workfront] se crean.
* Especificar qué campos deben sincronizarse entre elementos vinculados entre [!DNL Jira] y [!DNL Workfront].

>[!NOTE]
>
>* Después de configurar [!DNL Workfront for Jira] en su [!DNL Jira] entorno, todo [!DNL Jira] los usuarios ven un [!DNL Workfront] panel derecho en todo [!DNL Jira] elementos. El panel contiene información sobre los elementos que se pueden vincular desde [!DNL Workfront] o especifica que no [!DNL Workfront] los elementos están vinculados a [!DNL Jira] elementos.
>* Al usar la variable [!DNL Jira Server] , solo los problemas asociados con proyectos identificados como déclencheur para la integración de Workfront se muestran en el panel de Workfront. Para obtener más información sobre la configuración de déclencheur para la variable [!DNL Workfront to Jira] flujo de trabajo, consulte [Configuración de déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




Para configurar [!DNL Workfront for Jira]:

1. Iniciar sesión [!DNL Jira] como [!DNL Jira] administrador.
1. Haga clic en **[!UICONTROL Configuración]** en el [!DNL Jira] para abrir el Navegador.
1. Haga clic en **[!UICONTROL Complementos]** y haga clic en **[!UICONTROL Administrar complementos]**.

1. Expanda el **[!DNL Workfront]** complemento.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Siga las indicaciones para iniciar sesión en [!DNL Workfront].

   >[!NOTE]
   >
   >[!UICONTROL Workfront] conecta con [!DNL Jira] con OAuth 2.0, un estándar utilizado por la mayoría de las integraciones basadas en web para la autenticación y autorización de usuarios.

   Debe iniciar sesión en [!DNL Workfront] como [!DNL Workfront] para continuar con la configuración.

   >[!NOTE]
   >
   >* Cuando se le pida que introduzca el dominio de su [!DNL Workfront] cuenta, escríbala con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de la empresa suele ser el nombre de la empresa.
   >* La autenticación mejorada no está disponible hasta que se [!DNL Workfront] el administrador lo habilita para esta integración.



1. Seleccione el **[!UICONTROL Déclencheur]** para configurar la creación automática de [!DNL Jira] elementos como nuevos [!DNL Workfront] se crean.

   Para obtener más información sobre la configuración de déclencheur para Workfront en [!DNL Jira] flujo de trabajo, consulte [Configuración de déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Seleccione el **[!UICONTROL Configuración]** para configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] elementos.

   Para obtener más información sobre la configuración de la sincronización de campos entre [!DNL Jira] y [!DNL Workfront], consulte [Configuración de la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Después de definir los déclencheur y la sincronización de campos entre las dos aplicaciones, cualquier [!DNL Workfront] el usuario que puede crear tareas o problemas puede potencialmente almacenar en déclencheur la creación de un elemento en [!DNL Jira]. El usuario puede crear un elemento si los criterios del elemento que crea coinciden con los déclencheur de [!DNL Jira], aunque el usuario no tenga un [!DNL Jira] licencia. Además, cualquier [!DNL Jira] el usuario puede empezar a trabajar inmediatamente en [!DNL Jira] y sus actualizaciones se pueden ver en [!DNL Workfront], sin que tengan un [!DNL Workfront] licencia. Cualquier actualización en [!DNL Workfront] también están visibles en la variable [!DNL Jira] elementos.

1. (Opcional) Seleccione el **[!UICONTROL Registro de actividades]** para revisar los errores que puedan haberse producido durante la integración.

   Para obtener más información sobre la variable [!UICONTROL Registro de actividades], consulte [Consulte la [!DNL Jira] [!UICONTROL Registro de actividades]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configuración de déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]

Como [!DNL Jira] administrador del sistema, puede definir déclencheur que creen problemas automáticamente en [!DNL Jira] cuando un elemento de [!DNL Workfront] cumple ciertos criterios.

>[!NOTE]
>
>La integración podría tardar hasta 10 minutos en crear nuevos problemas en [!DNL Jira].

Tenga en cuenta lo siguiente al configurar la activación de la creación de [!DNL Jira] elementos como [!DNL Workfront] los elementos se crean:

* La integración es unidireccional: Solo se pueden almacenar en déclencheur los elementos creados en [!DNL Workfront] para crearse automáticamente en [!DNL Jira]. No se pueden almacenar en déclencheur los elementos creados en [!DNL Jira] para crearse automáticamente en [!DNL Workfront].
* No hay límite para la cantidad de déclencheur que se pueden tener.
* Si un elemento se crea en [!DNL Workfront] coincide con más de uno de los déclencheur, solo se crea un elemento en [!DNL Jira]. El elemento se crea en [!DNL Jira] según el primer déclencheur (en el orden en que se han definido en [!DNL Jira]). Todos los demás déclencheur se ignoran.
* Solo un elemento de [!DNL Workfront] se puede vincular a un elemento en Jira. Nunca se puede vincular una [!DNL Workfront] elemento a varios [!DNL Jira] problemas o uno [!DNL Jira] problema con varios [!DNL Workfront] elementos.

Para configurar déclencheur para la creación automática de elementos en [!DNL Jira]:

1. Iniciar sesión [!DNL Jira] como administrador del sistema.
1. Haga clic en **[!UICONTROL Configuración]** en el [!DNL Jira] para abrir el Navegador.
1. Haga clic en **[!UICONTROL Complementos]**, luego **[!UICONTROL Administrar complementos]**.

1. Expanda el **[!DNL Workfront]** complemento.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Iniciar sesión en [!DNL Workfront] como administrador del sistema.

   La variable **[!UICONTROL Déclencheur]** está seleccionada de forma predeterminada.

1. Haga clic en **[!UICONTROL Agregar déclencheur]** para agregar un nuevo déclencheur.
1. En el **[!UICONTROL Equipo/usuario/función de Workfront]** , especifique el nombre de una [!DNL Workfront] equipo, usuario o función de trabajo, haga clic en para seleccionarlo cuando aparezca en la lista.

   >[!NOTE]
   >
   >No puede tener varios déclencheur para el mismo equipo, usuario o función.

   Cuando alguien crea una tarea o un problema y la asigna a una de estas entidades, se crea automáticamente un problema en [!DNL [!DNL Jira]].

1. En el **[!UICONTROL [!DNL Jira]proyecto]** , empiece a escribir el nombre de una [!DNL Jira] y, a continuación, haga clic en para seleccionarlo cuando aparezca en la lista.

   Cuando la variable [!DNL Jira] se crea, se coloca en el proyecto que especifique aquí.

1. Seleccione un **I[!UICONTROL Tipo de problema]** en el menú desplegable.

   Esto indica el tipo de problema creado en [!DNL Jira] cuando se cumplan las condiciones de este déclencheur, en función de la configuración de ese proyecto específico en [!DNL Jira].

1. Haga clic en **[!UICONTROL Guardar]**.

   Con esta configuración, cada vez que se [!DNL Workfront] El usuario crea un elemento que coincide con los déclencheur especificados, se crea un nuevo problema en [!DNL Jira].

## Configuración de la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos

Como [!DNL Jira] administrador, puede definir qué campos deben sincronizarse automáticamente en los elementos vinculados entre [!DNL Workfront] y Jira. Ciertos campos se pueden sincronizar desde la [!DNL Workfront] a [!DNL Jira] y otros se sincronizan de Jira a Workfront.

Para definir qué campos deben sincronizarse automáticamente en elementos vinculados entre las dos aplicaciones:

1. Iniciar sesión [!DNL Jira] como administrador de Jira.
1. Haga clic en **[!UICONTROL Configuración]** en el [!DNL Jira] para abrir el Navegador.
1. Haga clic en **[!UICONTROL Complementos]**, luego **[!UICONTROL Administrar complementos]**.

1. Expanda el **[!DNL Workfront]** complemento.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Iniciar sesión en [!DNL Workfront] como administrador de Workfront.
1. Haga clic en el **[!UICONTROL Configuración]** pestaña .

1. En el **[!UICONTROL Sincronizar de Jira a Workfront]** seleccione los campos que desea actualizar en [!DNL Jira] cuando se actualizan en Workfront.

   1. Seleccione cualquiera de las siguientes frecuencias con las que se sincronizan los campos:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>Los campos que especifique se sincronizan entre el Workfront vinculado y [!DNL Jira] elementos cuando el elemento se crea en Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Siempre]</td>
              <td>Los campos que especifique se sincronizan entre el Workfront vinculado y [!DNL Jira] cuando los campos se actualizan en Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Nunca]</td>
              <td>Los campos especificados no se sincronizan nunca entre los vinculados [!DNL Workfront] y [!DNL Jira] elementos. No hay indicación en [!DNL Jira] que el campo se actualizó en [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Seleccione para sincronizar cualquiera de los campos siguientes desde [!DNL Workfront] a [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>El nombre de una tarea o un problema en [!DNL Workfront] se convierte en el nombre del problema en el que está vinculado [!DNL Jira].</p><p>Nota: Cuando se crean nuevos elementos en [!DNL Jira] automáticamente, la variable [!DNL Workfront] El nombre siempre se actualiza en la variable [!DNL Jira] , independientemente de si este campo está activado aquí o no. Cuando [!DNL Jira] el elemento está vinculado manualmente a un [!DNL Workfront] elemento, el nombre del [!DNL Workfront] solo actualizaciones de elementos en [!DNL Jira] cuando seleccione <strong>Siempre</strong> sincronice este campo. Para obtener más información sobre cómo vincular elementos de forma manual o automática, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descripción]</td>
         <td>La descripción de una tarea o un problema en [!DNL Workfront] se convierte en la descripción del problema en el que está vinculado [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documentos</td>
         <td><p>Documentos adjuntos a una tarea o un problema en [!DNL Workfront] también se adjuntan al asunto al que está vinculado en Jira. Nuevas versiones de documentos de [!DNL Workfront] se añaden como documentos separados a Jira y se añaden con <i>_v&lt;version number=""&gt;</i> para indicar la versión numerada en Workfront. </p><p>Por ejemplo, si el nombre de un documento de [!DNL Workfront] es <strong>Publicidad principal</strong>y le agregará una nueva versión en [!DNL Workfront], la nueva versión se transfiere a [!DNL Jira] como un nuevo documento con el nombre <strong>Anuncio principal_v2</strong>.</p><p>Importante: <p>Tenga en cuenta lo siguiente al sincronizar documentos:</p>
           <ul>
            <li><p>Los documentos de más de 5 MB no se sincronizan. Si falla la sincronización de documentos porque el documento es demasiado grande, se registra un error en el registro de actividades, </p><p>Para obtener más información sobre el registro de actividades, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Ver el registro de actividades de Jira</a>.</p></li>
            <li><p>Los documentos vinculados a tareas y problemas de servidores externos no se transfieren al [!DNL Jira] elementos. Solo los documentos cargados directamente en la tarea o el problema en [!DNL Workfront] se transfieren a la emisión vinculada en [!DNL Jira].</p></li>
            <li><p>Para crear una prueba a partir de un documento, debe generar la prueba en [!DNL Workfront]. </p><p>Para obtener más información sobre la generación de una prueba, consulte <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">Crear una prueba para un documento existente </a>en <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Crear una prueba para un documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Fecha de finalización prevista]</td>
         <td><p>La [!UICONTROL Fecha de finalización planeada] de una tarea o un problema en [!DNL Workfront] se convierte en la [!UICONTROL Fecha de vencimiento] del problema con el que está vinculado [!DNL Jira].</p><p>Nota: Asegúrese de que se muestra <strong>[!UICONTROL Fecha de vencimiento]</strong> en [!DNL Jira] problemas, para que este valor se sincronice.</p></td>
        </tr>
       </tbody>
      </table>

1. En el **[!UICONTROL Sincronizar desde [!DNL Jira] a[!DNL Workfront]]** seleccione los campos que desea actualizar en [!DNL Workfront] cuando se actualizan en [!DNL Jira].

   1. Seleccione cualquiera de las siguientes frecuencias con las que se sincronizan los campos:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Siempre]</td>
         <td>Los campos que especifique siempre se sincronizan entre los campos vinculados [!DNL Workfront] y [!DNL Jira] elementos cuando los campos se actualizan en [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nunca]</td>
         <td><p>Los campos especificados no se sincronizan nunca entre los vinculados [!DNL Workfront] y [!DNL Jira] elementos. No hay indicación en [!DNL Workfront] que el campo se actualizó en [!DNL Jira]. </p><p>Nota: Cuando selecciona Nunca, [!DNL Workfront] los campos se pueden actualizar manualmente desde [!DNL Jira] a la izquierda [!DNL Workfront] del panel [!DNL Jira] problema. Estas actualizaciones solo aparecen en [!DNL Workfront] elementos en [!DNL Jira] y [!DNL Workfront] y no en [!DNL Jira] elementos.</p></td>
        </tr>
       </tbody>
      </table>

   1. Seleccione para sincronizar cualquiera de los campos siguientes desde [!DNL Jira] a [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>El [!UICONTROL Status] de un problema en [!DNL Jira] se convierte en el [!UICONTROL Status] de la tarea o problema con el que está vinculado [!DNL Workfront].<br>Para obtener más información, consulte [!DNL Workfront] estados, consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>El [!UICONTROL Assignee] de un problema en [!DNL Jira] se convierte en el [!UICONTROL Assignee] de la tarea o problema con el que está vinculado [!DNL Workfront].</p><p>Importante: Al asignar un artículo en [!DNL Jira] a un usuario que no tiene un [!DNL Workfront] cuenta, la integración crea un nuevo usuario activo en [!DNL Workfront] solo cuando la variable <strong>Crear automáticamente un usuario en [!DNL Workfront] si la variable [!DNL Jira] el usuario no tiene un [!DNL Workfront] account</strong> está configurado como <strong>[!UICONTROL Siempre]</strong>. Este usuario no ocupa un [!DNL Workfront] licencia. Los usuarios activos pueden asignarse a elementos de trabajo en [!DNL Workfront], pero no se puede incluir en las actualizaciones. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Archivos adjuntos de un problema en [!DNL Jira] también se adjuntan a la tarea o al problema en el que está vinculada [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comentarios]</td>
         <td><p>Un comentario en un [!DNL Jira] el problema también se publica en el vínculo [!DNL Workfront] elemento del área [!UICONTROL Actualizaciones]. Por el contrario, un comentario publicado en el área [!UICONTROL Actualizaciones] para un [!DNL Workfront] sincronizar tareas o problemas con [!DNL Jira]del flujo de comentarios nativo de para el problema vinculado. </p><p>Esto se configura como <strong>[!UICONTROL Siempre]</strong> de forma predeterminada. Si selecciona <strong>[!UICONTROL Nunca]</strong> aquí puede seguir publicando comentarios manualmente en un elemento vinculado desde [!DNL Workfront] o [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. En el **[!UICONTROL OTROS]** seleccione qué campos adicionales deben actualizarse entre los elementos vinculados.

   1. Seleccione una opción para determinar si los campos especificados **[!UICONTROL Siempre]** o **[!UICONTROL Nunca]** actualizar en [!DNL Jira] o [!DNL Workfront] cuando se modifican.

   1. Seleccione entre los siguientes campos y actualizaciones:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Datos personalizados en el panel derecho de [!DNL Jira]]</td>
         <td><p>Muestra el [!DNL Workfront] Datos personalizados de un elemento de la sección [!DNL Workfront] panel derecho.</p><p>Nota: Las secciones Formulario personalizado se muestran en la sección [!DNL Workfront] panel derecho con el nivel de acceso de la variable [!DNL Workfront] Administrador del sistema.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Prioridad en el panel derecho de [!DNL Jira]]</td>
         <td>Muestra el [!DNL Workfront] Prioridad de un elemento de la sección [!DNL Workfront] panel derecho.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Agregue una actualización en la [!DNL Workfront] Pestaña Actualizaciones sobre los cambios de Fecha de vencimiento en [!DNL Jira]]</td>
         <td>Añade un comentario en la pestaña [!UICONTROL Update] de [!DNL Workfront] elemento en el que [!UICONTROL Fecha de vencimiento] cambia en [!DNL Jira] elemento.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Crear automáticamente un usuario en [!DNL Workfront] si la variable [!DNL Jira] el usuario no tiene un [!DNL Workfront] account]</td>
         <td><p>Existen los siguientes escenarios:</p>
          <ul>
           <li>Al seleccionar <strong>[!UICONTROL Siempre]</strong> habilita la integración para crear un nuevo usuario de Workfront cada vez que se [!DNL Jira] usuario sin [!DNL Workfront] La cuenta realiza las siguientes acciones en un vínculo [!DNL Jira] problema:
            <ul>
             <li>Se asigna a un [!DNL Jira] problema</li>
             <li><p>Registra la hora a [!DNL Jira] problema</p><p>Este nuevo usuario no ocupa un [!DNL Workfront] licencia. La configuración predeterminada es Siempre. El usuario ha creado este modo en [!DNL Workfront] tiene "[!UICONTROL Jira]" añadido a su nombre.</p></li>
            </ul></li>
           <li>Al seleccionar <strong>[!UICONTROL Nunca]</strong>, suceden las siguientes cosas:
            <ul>
             <li>No puede ver ninguna [!DNL Jira] asignaciones en la variable [!DNL Workfront] elementos. En este caso, solo las asignaciones realizadas en [!DNL Workfront] en la [!DNL Workfront] elementos.</li>
             <li>El tiempo registrado en un vínculo [!DNL Jira] problema de un usuario sin [!DNL Workfront] la cuenta no se transfiere automáticamente al [!DNL Workfront] elemento. Aún puede iniciar sesión en el [!DNL Workfront] elemento en el panel derecho del [!DNL Jira] problema.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Haga clic en **[!UICONTROL Guardar]**.

   Ahora, cada vez que un usuario actualiza cualquiera de los campos especificados en esta configuración en un elemento de [!DNL Jira] o [!DNL Workfront], el elemento vinculado en la otra aplicación también se actualiza.

## Resolución de problemas

### Los elementos no se pueden crear en [!DNL Jira] debido a los campos de déclencheur marcados &quot;[!UICONTROL No se pudo encontrar]&quot;

#### Problema

Cuando se produce un error con nuestra [!DNL Workfront for Jira] aplicación, [!DNL Workfront] deshabilita los déclencheur para evitar complicaciones adicionales. Cuando esos déclencheur están desactivados, se muestran como &quot;[!UICONTROL No se pudo encontrar]&quot;.

#### Solución

Busque el error que desactivó las déclencheur. Puede encontrar el error en el [!DNL Workfront for Jira] &quot;[!UICONTROL Registro de actividades]&quot;.

La causa más común de este comportamiento es el error &quot;[!UICONTROL No se puede establecer el campo &quot;duplicado&quot;. No está en la pantalla adecuada o es desconocido.]&quot;

Este error significa que está intentando sincronizar el[!UICONTROL Fecha de finalización planeada]&quot; de [!DNL Workfront] a [!DNL Jira]. Para ello, debe asegurarse de que su [!DNL Jira] los objetos tienen un campo llamado &quot;[!UICONTROL Fecha de vencimiento]&quot;. Si no tienen este campo, [!DNL Workfront] no puede sincronizar la fecha de finalización prevista a partir de [!DNL Workfront] y deshabilita sus déclencheur.

Para resolver este error, pruebe uno de los siguientes métodos:

* Pregunte a su [!DNL Jira] para actualizar el [!DNL Jira] para garantizar que tengan un campo de fecha de vencimiento.
* Desactivar la sincronización de [!DNL Workfront]La fecha de finalización prevista en Workfront &quot;[!UICONTROL Configuración]&quot;
