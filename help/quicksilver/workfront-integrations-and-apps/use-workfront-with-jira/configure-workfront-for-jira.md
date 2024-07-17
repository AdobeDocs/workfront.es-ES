---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurar  [!DNL Adobe Workfront for Jira]
description: Puedes usar [!DNL Adobe Workfront for Jira] para integrar tus [!DNL Jira] sistemas y [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2384'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->

Puede usar [!DNL Adobe Workfront for Jira] para integrar sus sistemas [!DNL Jira] y [!DNL Workfront].

Después de instalar el complemento, puede definir flujos de trabajo que creen [!DNL Jira] problemas automáticamente cuando se creen [!DNL Workfront] elementos de trabajo. Los elementos de ambas aplicaciones se vinculan y parte de su información se actualiza automáticamente en ambos sistemas.

Todos los usuarios de [!DNL Workfront] y [!DNL Jira] pueden beneficiarse de esta integración. Solo necesitan una licencia para el sistema en el que más trabajan, y no para ambos sistemas.

Este complemento está disponible para las versiones de [!UICONTROL Server] y [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) del software [!DNL Jira].

Para obtener una lista de [!DNL Jira] versiones que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) en [!DNL Atlassian Marketplace].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] [plan]</td> 
   <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: [!UICONTROL Pro] o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard] </p>
       <p>o</p> 
       <p>Actual: [!UICONTROL plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarlas a esta integración, en lugar de usar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder configurar [!DNL Workfront for Jira], debe:

* Instalar [!DNL Workfront for Jira].
Para obtener instrucciones sobre la instalación de [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurar [!DNL Workfront for Jira]

Si configura [!DNL Workfront for Jira], podrá:

* Defina los déclencheur que crearán [!DNL Jira] elementos cuando se creen [!DNL Workfront] elementos.
* Especifique qué campos deben sincronizarse entre los elementos vinculados entre [!DNL Jira] y [!DNL Workfront].

>[!NOTE]
>
>* Después de configurar [!DNL Workfront for Jira] en su entorno [!DNL Jira], todos los usuarios de [!DNL Jira] verán un panel derecho de [!DNL Workfront] en todos los elementos de [!DNL Jira]. El panel contiene información sobre los elementos que podrían vincularse desde [!DNL Workfront] o especifica que no hay elementos [!DNL Workfront] vinculados a [!DNL Jira] elementos.
>* Al utilizar la instalación de [!DNL Jira Server], solo se muestran en el panel Workfront los problemas asociados con los proyectos identificados como déclencheur para la integración de Workfront. Para obtener más información acerca de la configuración de déclencheur para el flujo de trabajo [!DNL Workfront to Jira], consulte [Configuración de déclencheur para vincular automáticamente elementos entre  [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Para configurar [!DNL Workfront for Jira]:

1. Inicie sesión en [!DNL Jira] como administrador de [!DNL Jira].
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haz clic en **[!UICONTROL Complementos]** y luego haz clic en **[!UICONTROL Administrar complementos]**.

1. Expanda el complemento **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Siga las indicaciones para iniciar sesión en [!DNL Workfront].

   >[!NOTE]
   >
   >El usuario debe tener un(a) `apiKey` válido(a) en [!UICONTROL Workfront] para crear una conexión correcta.

   Debe iniciar sesión en [!DNL Workfront] como administrador de [!DNL Workfront] para continuar con la configuración.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] se conecta a [!DNL Jira] mediante OAuth 2.0, un estándar utilizado por la mayoría de las integraciones basadas en la web para la autenticación y autorización de usuarios.
   >* Cuando se le pida que introduzca el dominio de su cuenta de [!DNL Workfront], escríbalo con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.
   >* La autenticación mejorada no está disponible hasta que un administrador de [!DNL Workfront] la habilite para esta integración.

1. En Jira, seleccione la ficha **[!UICONTROL Déclencheur]** para configurar la creación automática de [!DNL Jira] elementos a medida que se creen [!DNL Workfront] elementos nuevos.

   Para obtener más información sobre la configuración de déclencheur para el flujo de trabajo de Workfront a [!DNL Jira], consulte [Configuración de déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Seleccione la ficha **[!UICONTROL Setup]** para configurar la sincronización de campos entre los elementos vinculados [!DNL Jira] y [!DNL Workfront].

   Para obtener más información acerca de cómo configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront], vea [Configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Después de definir los déclencheur y la sincronización de campos entre las dos aplicaciones, cualquier usuario de [!DNL Workfront] que pueda crear tareas o problemas podría crear un déclencheur para la creación de un elemento en [!DNL Jira]. El usuario puede crear un elemento si los criterios del elemento que crea coinciden con los déclencheur de [!DNL Jira], aunque el usuario no tenga una licencia de [!DNL Jira]. Además, cualquier usuario de [!DNL Jira] puede empezar a trabajar inmediatamente en el elemento [!DNL Jira] y sus actualizaciones son visibles en [!DNL Workfront], sin que tenga una licencia de [!DNL Workfront]. Cualquier actualización de [!DNL Workfront] también está visible en los [!DNL Jira] elementos.

1. (Opcional) Seleccione la pestaña **[!UICONTROL Registro de actividad]** para revisar los errores que puedan haberse producido durante la integración.

   Para obtener más información sobre [!UICONTROL Registro de actividad], consulte [Ver el [!DNL Jira] [!UICONTROL Registro de actividad]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurar déclencheur para vincular automáticamente elementos entre [!DNL Jira] y [!DNL Workfront]

Como administrador del sistema de [!DNL Jira], puede definir déclencheur que crearían problemas automáticamente en [!DNL Jira] cuando un elemento de [!DNL Workfront] cumpla determinados criterios.

>[!NOTE]
>
>La integración podría tardar hasta 10 minutos en crear nuevos problemas en [!DNL Jira].

Tenga en cuenta lo siguiente al configurar y activar la creación de [!DNL Jira] elementos a medida que se crean [!DNL Workfront] elementos:

* La integración es unidireccional: solo puede crear elementos de déclencheur que cree en [!DNL Workfront] para que se creen automáticamente en [!DNL Jira]. No puede almacenar en déclencheur elementos que cree en [!DNL Jira] para que se creen automáticamente en [!DNL Workfront].
* No hay límite en cuanto a la cantidad de déclencheur que puede tener.
* Si un elemento que crea en [!DNL Workfront] coincide con más de uno de los déclencheur, sólo se creará un elemento en [!DNL Jira]. El elemento se crea en [!DNL Jira] según el primer déclencheur (en el orden en que se definieron en [!DNL Jira]). El resto de déclencheur se ignoran.
* Solo un elemento de [!DNL Workfront] se puede vincular a un elemento de Jira. Nunca puede vincular un elemento de [!DNL Workfront] a varios problemas de [!DNL Jira], ni un problema de [!DNL Jira] a varios elementos de [!DNL Workfront].

Para configurar déclencheur para crear automáticamente elementos en [!DNL Jira]:

1. Inicie sesión en [!DNL Jira] como administrador del sistema.
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haz clic en **[!UICONTROL Complementos]** y luego en **[!UICONTROL Administrar complementos]**.
1. Expanda el complemento **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Inicie sesión en [!DNL Workfront] como administrador del sistema.

   La ficha **[!UICONTROL Déclencheur]** está seleccionada de forma predeterminada en Jira.

1. Haga clic en **[!UICONTROL Agregar déclencheur]** para agregar un déclencheur nuevo.
1. En el campo **[!UICONTROL equipo/usuario/función de Workfront]**, especifique el nombre de un equipo, usuario o función de trabajo de [!DNL Workfront] y, a continuación, haga clic en para seleccionarlo cuando se muestre en la lista.

   >[!NOTE]
   >
   >No puede tener varios déclencheur para el mismo equipo, usuario o rol.

   Cuando alguien crea una tarea o un problema y lo asigna a una de estas entidades, se crea automáticamente un problema en [!DNL [!DNL Jira]].

1. En el campo **[!UICONTROL [!DNL Jira]proyecto]**, empiece a escribir el nombre de un proyecto [!DNL Jira] y, a continuación, haga clic en para seleccionarlo cuando se muestre en la lista.

   Cuando se crea el problema [!DNL Jira], se coloca en el proyecto que eligió aquí.

1. Seleccione un **I[!UICONTROL tipo de problema]** en el menú desplegable.

   Indica el tipo de problema que se crea en [!DNL Jira] cuando se cumplen las condiciones de este déclencheur, en función de la configuración de ese proyecto específico en [!DNL Jira].

1. Haga clic en **[!UICONTROL Guardar]**.

   Con esta configuración, cada vez que un usuario de [!DNL Workfront] crea un elemento que coincide con los déclencheur especificados, se crea un nuevo problema en [!DNL Jira].

## Configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] elementos

Como administrador de [!DNL Jira], puede definir qué campos se deben sincronizar automáticamente en los elementos vinculados entre [!DNL Workfront] y Jira. Algunos campos se pueden sincronizar desde [!DNL Workfront] al elemento [!DNL Jira], mientras que otros se sincronizan desde Jira a Workfront.

Para definir qué campos deben sincronizarse automáticamente en los elementos vinculados entre las dos aplicaciones:

1. Inicie sesión en [!DNL Jira] como administrador de Jira.
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haz clic en **[!UICONTROL Complementos]** y luego en **[!UICONTROL Administrar complementos]**.
1. Expanda el complemento **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Inicie sesión en [!DNL Workfront] como administrador de Workfront.
1. En Jira, haga clic en la ficha **[!UICONTROL Configuración]**.
1. En la sección **[!UICONTROL Sincronizar de Workfront a Jira]**, seleccione los campos que desee actualizar en [!DNL Jira] cuando se actualicen en Workfront.

   1. Seleccione cualquiera de las siguientes frecuencias con las que se sincronizan los campos:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Al Crear]</td>
              <td>Los campos que especifique se sincronizan entre los elementos vinculados de Workfront y [!DNL Jira] cuando el elemento se crea en Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Siempre]</td>
              <td>Los campos que especifique se sincronizan entre los elementos vinculados de Workfront y [!DNL Jira] cuando los campos se actualizan en Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Nunca]</td>
              <td>Los campos que especifique nunca se sincronizan entre los elementos vinculados [!DNL Workfront] y [!DNL Jira]. No hay ninguna indicación en [!DNL Jira] de que el campo se haya actualizado en [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Seleccione cualquiera de las siguientes opciones para sincronizar los campos de [!DNL Workfront] a [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Nombre]</td>
         <td><p>El nombre de una tarea o un problema de [!DNL Workfront] se convierte en el nombre del problema al que está vinculado en [!DNL Jira].</p><p>Nota: Cuando se crean nuevos elementos en [!DNL Jira] automáticamente, el nombre de [!DNL Workfront] siempre se actualiza en el elemento [!DNL Jira], independientemente de si este campo está habilitado aquí o no. Cuando un elemento de [!DNL Jira] se vincula manualmente a un elemento de [!DNL Workfront], el nombre del elemento de [!DNL Workfront] solo se actualiza en [!DNL Jira] cuando selecciona <strong>Sincronizar siempre</strong> este campo. Para obtener más información sobre cómo vincular elementos de forma manual o automática, vea <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descripción]</td>
         <td>La descripción de una tarea o un problema en [!DNL Workfront] se convierte en la descripción del problema al que está vinculado en [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documentos</td>
         <td><p>Los documentos adjuntos a una tarea o a un problema en [!DNL Workfront] también se adjuntan al problema al que está vinculado en Jira. Las nuevas versiones de [!DNL Workfront] se agregan como documentos independientes a Jira y se anexan con <i>_v&lt;número de versión&gt;</i> para indicar la versión numerada en Workfront. </p><p>Por ejemplo, si el nombre de un documento de [!DNL Workfront] es <strong>Anuncio principal</strong> y le agrega una nueva versión en [!DNL Workfront], la nueva versión se transfiere a [!DNL Jira] como un documento nuevo con el nombre <strong>Anuncio principal_v2</strong>.</p><p>Importante: <p>Tenga en cuenta lo siguiente al sincronizar documentos:</p>
           <ul>
            <li><p>Los documentos de más de 5 MB no se sincronizan. Si falla la sincronización de un documento porque es demasiado grande, se registra un error en el registro de actividades. </p><p>Para obtener más información sobre el registro de actividad, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Ver el registro de actividad de Jira</a>.</p></li>
            <li><p>Los documentos vinculados a tareas y problemas de servidores externos no se transfieren a los [!DNL Jira] elementos. Solo los documentos cargados directamente en la tarea o el problema de [!DNL Workfront] se transfieren al problema vinculado en [!DNL Jira].</p></li>
            <li><p>Para crear una revisión a partir de un documento, debe generar la revisión en [!DNL Workfront]. </p><p>Para obtener más información sobre cómo generar una revisión, consulte <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Crear una revisión para un documento existente </a>en <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Crear una revisión para un documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Fecha planificada de finalización]</td>
         <td><p>La [!UICONTROL Fecha planificada de finalización] de una tarea o un problema en [!DNL Workfront] se convierte en la [!UICONTROL Fecha de vencimiento] del problema al que está vinculado en [!DNL Jira].</p><p>Nota: Asegúrese de mostrar <strong>[!UICONTROL Fecha de vencimiento]</strong> en [!DNL Jira] problemas para que este valor se sincronice.</p></td>
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
         <td role="rowheader">[!UICONTROL Siempre]</td>
         <td>Los campos que especifique siempre se sincronizan entre los elementos vinculados [!DNL Workfront] y [!DNL Jira] cuando los campos se actualizan en [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nunca]</td>
         <td><p>Los campos que especifique nunca se sincronizan entre los elementos vinculados [!DNL Workfront] y [!DNL Jira]. No hay ninguna indicación en [!DNL Workfront] de que el campo se haya actualizado en [!DNL Jira]. </p><p>Nota: cuando selecciona Nunca, [!DNL Workfront] campos aún se pueden actualizar manualmente desde [!DNL Jira] en el panel izquierdo [!DNL Workfront] del problema [!DNL Jira]. Estas actualizaciones aparecen solamente en [!DNL Workfront] elementos de [!DNL Jira] y [!DNL Workfront], y no en [!DNL Jira] elementos.</p></td>
        </tr>
       </tbody>
      </table>

   1. Seleccione sincronizar cualquiera de los siguientes campos de [!DNL Jira] a [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Estado]</td>
         <td>El [!UICONTROL Estado] de un problema en [!DNL Jira] se convierte en el [!UICONTROL Estado] de la tarea o problema al que está vinculado en [!DNL Workfront].<br>Para obtener más información acerca de [!DNL Workfront] estados, vea <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Asignado]</td>
         <td><p>El [!UICONTROL asignado] de un problema en [!DNL Jira] se convierte en el [!UICONTROL asignado] de la tarea o problema al que está vinculado en [!DNL Workfront].</p><p>Importante: Cuando asigna un elemento de [!DNL Jira] a un usuario que no tiene una cuenta de [!DNL Workfront], la integración crea un nuevo usuario activo en [!DNL Workfront] solo cuando <strong>Crea automáticamente un usuario en [!DNL Workfront] si el usuario de [!DNL Jira] no tiene una cuenta de [!DNL Workfront]</strong> se establece en <strong>[!UICONTROL Always]</strong>. Este usuario no ocupa una licencia de [!DNL Workfront]. Los usuarios activos se pueden asignar a elementos de trabajo en [!DNL Workfront], pero no se pueden incluir en las actualizaciones. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Archivos adjuntos]</td>
         <td>Los archivos adjuntos de un problema en [!DNL Jira] también se adjuntan a la tarea o problema al que está vinculado en [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comentarios]</td>
         <td><p>También se publicó un comentario sobre un problema de [!DNL Jira] en el elemento [!DNL Workfront] vinculado en el área de [!UICONTROL Updates]. Por el contrario, un comentario publicado en el área de [!UICONTROL Updates] para una tarea o un problema de [!DNL Workfront] se sincroniza con el flujo de comentarios nativo de [!DNL Jira] para el problema vinculado. </p><p>De forma predeterminada, se establece en <strong>[!UICONTROL Always]</strong>. Si selecciona <strong>[!UICONTROL Never]</strong> aquí, aún puede publicar comentarios manualmente sobre un elemento vinculado en [!DNL Workfront] o en [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. En la sección **[!UICONTROL OTHER]**, seleccione qué campos adicionales deben actualizarse entre los elementos vinculados.

   1. Seleccione una opción para determinar si los campos que especifica **[!UICONTROL Siempre]** o **[!UICONTROL Nunca]** se actualizan en [!DNL Jira] o [!DNL Workfront] cuando se modifican.

   1. Seleccione entre los siguientes campos y actualizaciones:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar [!DNL Workfront] datos personalizados en el panel derecho de [!DNL Jira]]</td>
         <td><p>Muestra los datos personalizados [!DNL Workfront] de un elemento en el panel derecho [!DNL Workfront].</p><p>Nota: Las secciones de formulario personalizado se muestran en el panel derecho de [!DNL Workfront] con el nivel de acceso del administrador del sistema [!DNL Workfront].</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar prioridad [!DNL Workfront] en el panel derecho de [!DNL Jira]]</td>
         <td>Muestra la prioridad [!DNL Workfront] de un elemento en el panel derecho [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Agregar una actualización en la ficha [!DNL Workfront] actualizaciones acerca de los cambios de fecha de vencimiento en [!DNL Jira]]</td>
         <td>Agrega un comentario en la ficha [!UICONTROL Actualización] del elemento [!DNL Workfront] cuando [!UICONTROL Fecha de vencimiento] cambia en el elemento [!DNL Jira] vinculado.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Crear automáticamente un usuario en [!DNL Workfront] si el usuario [!DNL Jira] no tiene una cuenta de [!DNL Workfront]]</td>
         <td><p>Existen los siguientes escenarios:</p>
          <ul>
           <li>Al seleccionar <strong>[!UICONTROL Always]</strong>, habilita la integración para crear un nuevo usuario de Workfront cada vez que un usuario de [!DNL Jira] sin una cuenta de [!DNL Workfront] realice las siguientes acciones en un problema de [!DNL Jira] vinculado:
            <ul>
             <li>Se ha asignado a un problema [!DNL Jira]</li>
             <li><p>Registra el tiempo en un problema de [!DNL Jira]</p><p>Este nuevo usuario no ocupa una licencia de [!DNL Workfront]. El valor predeterminado es Siempre. El usuario creado de esta manera en [!DNL Workfront] tiene "[!UICONTROL Jira]" agregado a su nombre.</p></li>
            </ul></li>
           <li>Cuando selecciona <strong>[!UICONTROL Nunca]</strong>, suceden las siguientes cosas:
            <ul>
             <li>No puede ver ninguna asignación de [!DNL Jira] en los elementos de [!DNL Workfront]. En este caso, solo se muestran las asignaciones realizadas en [!DNL Workfront] en los [!DNL Workfront] elementos.</li>
             <li>El tiempo que un usuario sin cuenta de [!DNL Workfront] ha registrado en un problema de [!DNL Jira] vinculado no se transfiere automáticamente al elemento de [!DNL Workfront] vinculado. Todavía puede registrar tiempo en el elemento [!DNL Workfront] del panel derecho del problema [!DNL Jira].</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Haga clic en **[!UICONTROL Guardar]**.

   Ahora, cada vez que un usuario actualiza cualquiera de los campos especificados en esta configuración en un elemento de [!DNL Jira] o [!DNL Workfront], también se actualiza el elemento vinculado en la otra aplicación.

## Resolución de problemas

### No se pueden crear elementos en [!DNL Jira] debido a campos de déclencheur marcados como &quot;[!UICONTROL No se encontraron]&quot;

#### Problema

Cuando se produce un error con la aplicación [!DNL Workfront for Jira], [!DNL Workfront] deshabilita los déclencheur para evitar complicaciones adicionales. Cuando estos déclencheur están deshabilitados, se muestran como &quot;[!UICONTROL No se pudo encontrar]&quot;.

#### Solución

Busque el error que deshabilitó las déclencheur. Puede encontrar el error en [!DNL Workfront for Jira] [!UICONTROL Registro de actividad].

La causa más común de este comportamiento es el error &quot;[!UICONTROL No se puede establecer el campo &#39;duedate&#39;. No aparece en la pantalla adecuada o es desconocido.]&quot;

Este error significa que está intentando sincronizar la &quot;[!UICONTROL Fecha planificada de finalización]&quot; de [!DNL Workfront] a [!DNL Jira]. Para ello, debe asegurarse de que los objetos de [!DNL Jira] tengan un campo denominado &quot;[!UICONTROL Fecha de vencimiento]&quot;. Si no tiene este campo, [!DNL Workfront] no puede sincronizar la fecha planificada de finalización de [!DNL Workfront] y deshabilita las déclencheur.

Para resolver este error, intente una de las siguientes acciones:

* Pida al administrador de [!DNL Jira] que actualice los objetos [!DNL Jira] afectados para asegurarse de que tengan un campo de fecha de vencimiento.
* Deshabilite la sincronización de la fecha planificada de finalización de [!DNL Workfront] en la página [!UICONTROL Configuración] de Workfront.
