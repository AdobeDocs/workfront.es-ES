---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurar [!DNL Adobe Workfront for Jira]
description: Puede utilizar [!DNL Adobe Workfront for Jira] para integrar sus sistemas [!DNL Jira] y [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '2454'
ht-degree: 95%

---

# Configurar [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Jira no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Jira.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Jira, consulte [Módulos de software de Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Puede utilizar [!DNL Adobe Workfront for Jira] para integrar sus sistemas [!DNL Jira] y [!DNL Workfront].

Después de instalar el complemento, puede definir flujos de trabajo que creen problemas de [!DNL Jira] automáticamente cuando se creen elementos de trabajo de [!DNL Workfront]. Los elementos de ambas aplicaciones se vinculan y parte de su información se actualiza automáticamente en ambos sistemas.

Todos los usuarios de [!DNL Workfront] y [!DNL Jira] pueden beneficiarse de esta integración. Solo necesitan una licencia para el sistema en el que más trabajan, y no para ambos sistemas.

Este complemento está disponible para las versiones de [!UICONTROL Server] y [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) del software [!DNL Jira].

Para obtener una lista de versiones de [!DNL Jira] que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) en el [!DNL Atlassian Marketplace].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en Jira y Workfront para dedicarlas a esta integración, en lugar de utilizar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de poder configurar [!DNL Workfront for Jira], debe:

* Instalar [!DNL Workfront for Jira].
Para obtener instrucciones sobre la instalación de [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurar [!DNL Workfront for Jira]

Si configura [!DNL Workfront for Jira], podrá:

* Defina los activadores que crearán elementos de [!DNL Jira] cuando se creen elementos de [!DNL Workfront].
* Especifique qué campos deben sincronizarse entre los elementos vinculados entre [!DNL Jira] y [!DNL Workfront].

>[!NOTE]
>
>* Después de configurar [!DNL Workfront for Jira] en su entorno de [!DNL Jira], todos los usuarios de [!DNL Jira] verán un panel derecho de [!DNL Workfront] en todos los elementos de [!DNL Jira]. El panel contiene información sobre los elementos que podrían vincularse desde [!DNL Workfront] o especifica que no hay elementos de [!DNL Workfront] vinculados a elementos de [!DNL Jira].
>* Al utilizar la instalación de [!DNL Jira Server], solo se muestran en el panel Workfront los problemas asociados con los proyectos identificados como activadores para la integración de Workfront. Para obtener más información acerca de la configuración de activadores para el flujo de trabajo de [!DNL Workfront to Jira], consulte [Configuración de activadores para vincular automáticamente elementos entre  [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Para configurar [!DNL Workfront for Jira]:

1. Inicie sesión en [!DNL Jira] como administrador de [!DNL Jira].
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haga clic en **[!UICONTROL Complementos]** y luego haga clic en **[!UICONTROL Administrar complementos]**.

1. Expanda el complemento de **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Siga las indicaciones para iniciar sesión en [!DNL Workfront].

   >[!NOTE]
   >
   >El usuario debe tener un(a) `apiKey` válido(a) en [!UICONTROL Workfront] para crear una conexión correcta.

   Debe iniciar sesión en [!DNL Workfront] como administrador de [!DNL Workfront] para continuar con la configuración.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] se conecta a [!DNL Jira] mediante OAuth 2.0, un estándar utilizado por la mayoría de las integraciones basadas en la web para la autenticación y autorización de usuarios.
   >* Cuando se le pida que introduzca el dominio de su cuenta de [!DNL Workfront], escríbalo con este formato: *eldominiodesucompañía.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.
   >* La autenticación mejorada no está disponible hasta que un administrador de [!DNL Workfront] la habilite para esta integración.

1. En Jira, seleccione la pestaña **[!UICONTROL Activadores]** para configurar la creación automática de [!DNL Jira] elementos a medida que se creen elementos nuevos de [!DNL Workfront].

   Para obtener más información sobre la configuración de activadores para el flujo de trabajo de Workfront a [!DNL Jira], consulte [Configuración de activadores para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Seleccione la ficha **[!UICONTROL Configuración]** para configurar la sincronización de campos entre los elementos vinculados [!DNL Jira] y [!DNL Workfront].

   Para obtener más información acerca de cómo configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront], consulte [Configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Después de definir los activadores y la sincronización de campos entre las dos aplicaciones, cualquier usuario de [!DNL Workfront] que pueda crear tareas o problemas podría crear un activador para la creación de un elemento en [!DNL Jira]. El usuario puede crear un elemento si los criterios del elemento que crea coinciden con los activadores de [!DNL Jira], aunque el usuario no tenga una licencia de [!DNL Jira]. Además, cualquier usuario de [!DNL Jira] puede empezar a trabajar inmediatamente en el elemento de [!DNL Jira] y sus actualizaciones son visibles en [!DNL Workfront], sin que tenga una licencia de [!DNL Workfront]. Cualquier actualización de [!DNL Workfront] también está visible en los elementos de [!DNL Jira].

1. (Opcional) Seleccione la ficha **[!UICONTROL Registro de actividad]** para revisar los errores que puedan haberse producido durante la integración.

   Para obtener más información sobre el [!UICONTROL Registro de actividad], consulte [Ver el [!DNL Jira] [!UICONTROL registro de actividad]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurar activadores para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]

Como administrador del sistema de [!DNL Jira], puede definir activadores que creen problemas automáticamente en [!DNL Jira] cuando un elemento de [!DNL Workfront] cumpla determinados criterios.

>[!NOTE]
>
>La integración podría tardar hasta 10 minutos en crear nuevos problemas en [!DNL Jira].

Tenga en cuenta lo siguiente al configurar y activar la creación de elementos de [!DNL Jira] a medida que se crean elementos de [!DNL Workfront]:

* La integración es unidireccional: solo puede crear elementos de activadores que cree en [!DNL Workfront] para que se creen automáticamente en [!DNL Jira]. No se pueden activar elementos creados en [!DNL Jira] para que se creen automáticamente en [!DNL Workfront].
* No hay límite en cuanto a la cantidad de activadores que puede tener.
* Si un elemento que crea en [!DNL Workfront] coincide con más de uno de los activadores, solo se creará un elemento en [!DNL Jira]. El elemento se crea en [!DNL Jira] según el primer activador (en el orden en que se definieron en [!DNL Jira]). El resto de activadores se ignoran.
* Solo un elemento de [!DNL Workfront] se puede vincular a un elemento de Jira. Nunca puede vincular un elemento de [!DNL Workfront] a varios problemas de [!DNL Jira], ni un problema de [!DNL Jira] a varios elementos de [!DNL Workfront].

Para configurar activadores para crear automáticamente elementos en [!DNL Jira]:

1. Inicie sesión en [!DNL Jira] como administrador del sistema.
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haga clic en **[!UICONTROL Complementos]** y luego en **[!UICONTROL Administrar complementos]**.
1. Expanda el complemento de **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Inicie sesión en [!DNL Workfront] como administrador del sistema.

   La pestaña **[!UICONTROL Activadores]** está seleccionada de forma predeterminada en Jira.

1. Haga clic en **[!UICONTROL Añadir activador]** para añadir un activador nuevo.
1. En el campo **[!UICONTROL equipo/usuario/función de Workfront]**, especifique el nombre de un equipo, usuario o función de [!DNL Workfront] y, a continuación, haga clic para seleccionarlo cuando se muestre en la lista.

   >[!NOTE]
   >
   >No puede tener varios activadores para el mismo equipo, usuario o función.

   Cuando alguien crea una tarea o un problema y lo asigna a una de estas entidades, se crea automáticamente un problema en [!DNL [!DNL Jira]].

1. En el campo proyecto de **[!UICONTROL [!DNL Jira]]**, empiece a escribir el nombre de un proyecto de [!DNL Jira] y, a continuación, haga clic en para seleccionarlo cuando se muestre en la lista.

   Cuando se crea el problema de [!DNL Jira], se coloca en el proyecto que eligió aquí.

1. Seleccione un **[!UICONTROL Tipo de problema]** en el menú desplegable.

   Indica el tipo de problema que se crea en [!DNL Jira] cuando se cumplen las condiciones de este activador, en función de la configuración de ese proyecto específico en [!DNL Jira].

1. Haga clic en **[!UICONTROL Guardar]**.

   Con esta configuración, cada vez que un usuario de [!DNL Workfront] crea un elemento que coincide con los activadores especificados, se crea un nuevo problema en [!DNL Jira].

## Configurar la sincronización de campos entre elementos de [!DNL Jira] y [!DNL Workfront]

Como administrador de [!DNL Jira], puede definir qué campos se deben sincronizar automáticamente en los elementos vinculados entre [!DNL Workfront] y Jira. Algunos campos se pueden sincronizar desde [!DNL Workfront] al elemento de [!DNL Jira], mientras que otros se sincronizan desde Jira a Workfront.

Para definir qué campos deben sincronizarse automáticamente en los elementos vinculados entre las dos aplicaciones:

1. Inicie sesión en [!DNL Jira] como administrador de Jira.
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haga clic en **[!UICONTROL Complementos]** y luego en **[!UICONTROL Administrar complementos]**.
1. Expanda el complemento de **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Inicie sesión en [!DNL Workfront] como administrador de Workfront.
1. En Jira, haga clic en la pestaña **[!UICONTROL Configuración]**.
1. En la sección **[!UICONTROL Sincronizar de Workfront a Jira]**, seleccione los campos que desee actualizar en [!DNL Jira] cuando se actualicen en Workfront.

   1. Seleccione cualquiera de las siguientes frecuencias con las que se sincronizan los campos:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>Los campos que especifique se sincronizan entre los elementos vinculados de Workfront y [!DNL Jira] cuando el elemento se crea en Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>Los campos que especifique se sincronizan entre los elementos vinculados de Workfront y [!DNL Jira] cuando los campos se actualizan en Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>Los campos que especifique nunca se sincronizan entre los elementos vinculados [!DNL Workfront] y [!DNL Jira]. No hay ninguna indicación en [!DNL Jira] de que el campo se haya actualizado en [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Seleccione cualquiera de las siguientes opciones para sincronizar los campos de [!DNL Workfront] a [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>El nombre de una tarea o un problema de [!DNL Workfront] se convierte en el nombre del problema al que está vinculado en [!DNL Jira].</p><p>Nota:Cuando se crean nuevos elementos en [!DNL Jira] automáticamente, el nombre de [!DNL Workfront] siempre se actualiza en el elemento de [!DNL Jira], independientemente de si este campo está habilitado aquí o no. Cuando un elemento de [!DNL Jira] se vincula manualmente a un elemento de [!DNL Workfront], el nombre del elemento de [!DNL Workfront] solo se actualiza en [!DNL Jira] cuando selecciona <strong>Sincronizar siempre</strong> este campo.Para obtener más información sobre la vinculación de elementos manual o automática, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Vinculación de elementos entre [!DNL Adobe Workfront] y [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>La descripción de una tarea o un problema en [!DNL Workfront] se convierte en la descripción del problema al que está vinculado en [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documentos</td>
         <td><p>Los documentos adjuntos a una tarea o a un problema en [!DNL Workfront] también se adjuntan al problema al que está vinculado en Jira. Las nuevas versiones de [!DNL Workfront] se añaden como documentos independientes a Jira y se anexan con <i>_v&lt;número de versión&gt;</i> para indicar la versión numerada en Workfront. </p><p>Por ejemplo, si el nombre de un documento de [!DNL Workfront] es <strong>Anuncio principal</strong> y le añade una nueva versión en [!DNL Workfront], la nueva versión se transfiere a [!DNL Jira] como un documento nuevo con el nombre <strong>Anuncio principal_v2</strong>.</p><p>Importante: <p>Tenga en cuenta lo siguiente al sincronizar documentos:</p>
           <ul>
            <li><p>Los documentos de más de 5 MB no se sincronizan. Si falla la sincronización de un documento porque es demasiado grande, se registra un error en el registro de actividades. </p><p>Para obtener más información sobre el registro de actividad, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Ver el registro de actividad de Jira</a>.</p></li>
            <li><p>Los documentos vinculados a tareas y problemas de servidores externos no se transfieren a los elementos de [!DNL Jira]. Solo los documentos cargados directamente en la tarea o el problema de [!DNL Workfront] se transfieren al problema vinculado en [!DNL Jira].</p></li>
            <li><p>Para crear una prueba a partir de un documento, debe generar la prueba en [!DNL Workfront]. </p><p>Para obtener más información sobre cómo generar una prueba, consulte <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Crear una prueba para un documento existente </a>en <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Crear una prueba para un documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>La [!UICONTROL Planned Completion Date] de una tarea o un problema en [!DNL Workfront] se convierte en la [!UICONTROL Due Date] del problema al que está vinculado en [!DNL Jira].</p><p>Nota: Asegúrese de mostrar <strong>[!UICONTROL Due Date]</strong> en los problemas de [!DNL Jira] para que este valor se sincronice.</p></td>
        </tr>
       </tbody>
      </table>

1. En la sección **[!UICONTROL Sincronizar de [!DNL Jira] a[!DNL Workfront]]**, seleccione los campos que desea actualizar en [!DNL Workfront] cuando se actualicen en [!DNL Jira].

   1. Seleccione cualquiera de las siguientes frecuencias con las que se sincronizan los campos:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>Los campos que especifique siempre se sincronizan entre los elementos vinculados de [!DNL Workfront] y [!DNL Jira] cuando los campos se actualizan en [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>Los campos que especifique nunca se sincronizan entre los elementos vinculados de [!DNL Workfront] y [!DNL Jira]. No hay ninguna indicación en [!DNL Workfront] de que el campo se haya actualizado en [!DNL Jira]. </p><p>Nota: cuando selecciona Nunca, los campos de [!DNL Workfront] aún se pueden actualizar manualmente desde [!DNL Jira] en el panel izquierdo de [!DNL Workfront] del problema de [!DNL Jira]. Estas actualizaciones aparecen solamente en elementos de [!DNL Workfront] en [!DNL Jira] y [!DNL Workfront], y no en elementos de [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

   1. Seleccione sincronizar cualquiera de los siguientes campos de [!DNL Jira] a [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>El [!UICONTROL Status] de un problema en [!DNL Jira] se convierte en el [!UICONTROL Status] de la tarea o problema al que está vinculado en [!DNL Workfront].<br>Para obtener más información acerca de los estados de [!DNL Workfront], consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>El [!UICONTROL Assignee] de un problema en [!DNL Jira] se convierte en el [!UICONTROL Assignee] de la tarea o problema al que está vinculado en [!DNL Workfront].</p><p>Importante: Cuando se asigna un elemento de [!DNL Jira] a un usuario que no tiene una cuenta de [!DNL Workfront], la integración crea un nuevo usuario activo en [!DNL Workfront] solo cuando <strong>Crea automáticamente un usuario en [!DNL Workfront] si el usuario de [!DNL Jira] no tiene una cuenta de [!DNL Workfront]</strong> se establece en <strong>[!UICONTROL Always]</strong>. Este usuario no ocupa una licencia de [!DNL Workfront].Los usuarios activos se pueden asignar a elementos de trabajo en [!DNL Workfront], pero no se pueden incluir en las actualizaciones. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Los archivos adjuntos de un problema en [!DNL Jira] también se adjuntan a la tarea o problema al que está vinculado en [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>También se publicó un comentario sobre un problema de [!DNL Jira] en el elemento de [!DNL Workfront] vinculado en el área de [!UICONTROL Updates]. Por el contrario, un comentario publicado en el área de [!UICONTROL Updates] para una tarea o un problema de [!DNL Workfront] se sincroniza con el flujo de comentarios nativo de [!DNL Jira] para el problema vinculado. </p><p>De forma predeterminada, se establece en <strong>[!UICONTROL Always]</strong>. Si selecciona <strong>[!UICONTROL Never]</strong> aquí, aún puede publicar comentarios manualmente sobre un elemento vinculado en [!DNL Workfront] o en [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. En la sección **[!UICONTROL OTHER]**, seleccione qué campos adicionales deben actualizarse entre los elementos vinculados.

   1. Seleccione una opción para determinar si los campos que especifique **[!UICONTROL Siempre]** o **[!UICONTROL Nunca]** se actualizan en [!DNL Jira] o [!DNL Workfront] cuando se modifican.

   1. Seleccione entre los siguientes campos y actualizaciones:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Custom Data in the right panel in [!DNL Jira]]</td>
         <td><p>Muestra los datos personalizados de [!DNL Workfront] de un elemento en el panel derecho de [!DNL Workfront].</p><p>Nota: Las secciones de formulario personalizado se muestran en el panel derecho de [!DNL Workfront] con el nivel de acceso del administrador del sistema [!DNL Workfront].</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Priority in the right panel in [!DNL Jira]]</td>
         <td>Muestra la prioridad de [!DNL Workfront] de un elemento en el panel derecho de [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Updates tab about Due Date changes in [!DNL Jira]]</td>
         <td>Se añade un comentario en la ficha [!UICONTROL Update] del elemento de [!DNL Workfront] cuando la [!UICONTROL Due Date] cambia en el elemento vinculado de [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] if the [!DNL Jira] user does not have a [!DNL Workfront] account]</td>
         <td><p>Se dan los siguientes escenarios:</p>
          <ul>
           <li>Al seleccionar <strong>[!UICONTROL Always]</strong>, habilita la integración para crear un nuevo usuario de Workfront cada vez que un usuario de [!DNL Jira] sin una cuenta de [!DNL Workfront] realice las siguientes acciones en un problema de [!DNL Jira] vinculado:
            <ul>
             <li>Se ha asignado a un problema de [!DNL Jira]</li>
             <li><p>Registra el tiempo en un problema de [!DNL Jira]</p><p>Este nuevo usuario no ocupa una licencia de [!DNL Workfront]. El valor predeterminado es Siempre. El usuario creado de esta manera en [!DNL Workfront] tiene “[!UICONTROL Jira]" añadido a su nombre.</p></li>
            </ul></li>
           <li>Cuando selecciona <strong>[!UICONTROL Never]</strong>, sucede lo siguiente:
            <ul>
             <li>No puede ver ninguna asignación de [!DNL Jira] en los elementos de [!DNL Workfront]. En este caso, solo se muestran las asignaciones realizadas en [!DNL Workfront] en los elementos de [!DNL Workfront].</li>
             <li>El tiempo que un usuario sin cuenta de [!DNL Workfront] ha registrado en un problema de [!DNL Jira] vinculado no se transfiere automáticamente al elemento de [!DNL Workfront] vinculado. Todavía puede registrar tiempo en el elemento [!DNL Workfront] del panel derecho del problema de [!DNL Jira].</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Haga clic en **[!UICONTROL Guardar]**.

   Ahora, cada vez que un usuario actualiza cualquiera de los campos especificados en esta configuración en un elemento de [!DNL Jira] o [!DNL Workfront], también se actualiza el elemento vinculado en la otra aplicación.

## Resolución de problemas

### No se pueden crear elementos en [!DNL Jira] porque los campos del activador están marcados como “[!UICONTROL No se encontraron]”

#### Problema

Cuando se produce un error con la aplicación [!DNL Workfront for Jira], [!DNL Workfront] deshabilita los activadores para evitar mayores complicaciones. Cuando estos activadores están deshabilitados, se muestran como “[!UICONTROL No se pudo encontrar]”.

#### Solución

Busque el error que deshabilitó los activadores. Puede encontrar el error en el [!DNL Workfront for Jira] Registro de actividad de .

La causa más común de este comportamiento es el error “[!UICONTROL No se puede establecer el campo duedate. No aparece en la pantalla adecuada o es desconocido]”.

Este error significa que está intentando sincronizar la “[!UICONTROL Fecha planificada de finalización]” de [!DNL Workfront] a [!DNL Jira]. Para ello, debe asegurarse de que los objetos de [!DNL Jira] tengan un campo denominado “[!UICONTROL Fecha de vencimiento]”. Si no tiene este campo, [!DNL Workfront] no puede sincronizar la fecha planificada de finalización de [!DNL Workfront] y deshabilita los activadores.

Para resolver este error, intente una de las siguientes acciones:

* Pida al administrador de [!DNL Jira] que actualice los objetos de [!DNL Jira] afectados para asegurarse de que tengan un campo de fecha de vencimiento.
* Deshabilite la sincronización de la fecha planificada de finalización de [!DNL Workfront] en la página [!UICONTROL Configuración] de Workfront.
