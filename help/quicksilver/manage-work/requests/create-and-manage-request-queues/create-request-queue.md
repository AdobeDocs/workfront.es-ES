---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear una cola de solicitud
description: Puede configurar una cola de solicitud en la que los usuarios puedan introducir solicitudes ocasionales que no estén planificadas para trabajar en un proyecto.
author: Alina
feature: Work Management
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '2545'
ht-degree: 2%

---

# Crear una cola de solicitud

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

Puede configurar una cola de solicitud en la que los usuarios puedan introducir solicitudes ocasionales que no estén planificadas para trabajar en un proyecto. Por ejemplo, se puede configurar una cola de solicitudes del servicio de asistencia para capturar todas las solicitudes de los usuarios que llegan a un departamento de TI.

## Requisitos de acceso

<!--drafted for P&P: replace the table below with this:

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
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administrar permisos para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront

## Resumen de las colas de solicitud

La cola de solicitudes se configura como proyecto. Cuando se designa el proyecto como cola de solicitud, se puede acceder a la cola desde el área Solicitudes de Adobe Workfront. Al personalizar la cola de solicitud, también se personaliza el formulario que los usuarios rellenan cuando envían las solicitudes.

En este artículo se describe cómo crear una cola de solicitudes a partir de un proyecto existente. Sin embargo, para crear coherencia en el proceso de admisión de solicitudes o para agregarle varias capas con fines de creación de informes y una mejor administración, también puede configurar componentes básicos adicionales de una cola de solicitudes que se describen en la siguiente tabla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Detalles de cola</td> 
   <td> <p>Debe configurar un proyecto como una cola de solicitud en el área Detalles de la cola . Este paso es obligatorio. </p> <p>Para obtener más información, consulte la <a href="#create-a-request-queue" class="MCXref xref">Crear una cola de solicitud</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Grupos de temas</td> 
   <td> <p>Son menús adicionales que clasifican las solicitudes en función de características comunes. Por ejemplo, para una cola de solicitud de TI, es posible que desee tener grupos de temas "en el sitio" y "remotos". </p> <p>Para obtener más información, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Crear grupos de temas</a>. </p> <p>Esto es opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Temas de colas</td> 
   <td> <p>Son menús adicionales que clasifican solicitudes que pertenecen al mismo grupo de temas en función de características comunes. Un grupo de temas puede contener varios temas de cola. </p> <p>Por ejemplo, el grupo de temas "En el sitio" para la cola de solicitud de TI puede contener los temas de cola "Hardware", "Software" y "Red". </p> <p>Para obtener más información, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crear temas de cola</a>. </p> <p>Esto es opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reglas de enrutamiento</td> 
   <td> <p>Permiten dirigir cada solicitud a un usuario, función de trabajo, equipo o a un proyecto. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Crear reglas de enrutamiento</a>. </p> <p>Esto es opcional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crear una cola de solicitud

Cuando configura un proyecto como cola de solicitud, el estado del proyecto debe ser Actual para que se muestre en el área Solicitudes de Workfront.

Para crear una cola de solicitud:

1. Vaya al proyecto que desea configurar como cola de solicitud.
1. (Opcional) Haga clic en **Detalles del proyecto** en el panel izquierdo y añada una **Descripción** al proyecto en el **Información general** . Esta información se muestra en todas las solicitudes nuevas.
1. Haga clic en **Detalles de cola** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**, luego **Detalles de cola**.

   Se abre la sección Detalles de la cola .

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Especifique la siguiente información:

   * **Publicar como cola de solicitud de ayuda:** Seleccione esta opción para identificar este proyecto como una cola de solicitudes. Todos los problemas entrantes se consideran solicitudes.\
      Cuando no se selecciona esta opción, el proyecto se comporta como un proyecto estándar en Workfront y todos los problemas entrantes son problemas.

   * **Quién puede agregar solicitudes a esta cola:** Seleccione a qué usuarios tienen acceso para añadir solicitudes a esta cola. Puede permitir que los siguientes grupos de personas vean la cola de solicitud en el área Solicitudes de la barra de navegación global:

      | Cualquiera | Cualquier usuario de Workfront con una cuenta activa puede ver esta cola de solicitudes y agregarle solicitudes |
      |---|---|
      | Personas con acceso de visualización en este proyecto | Los usuarios con permisos de visualización del proyecto pueden ver y agregar solicitudes a esta cola |
      | Personas en la compañía de este proyecto | Los usuarios que pertenezcan a la empresa asociada con este proyecto podrán ver y agregar solicitudes a esta cola. Si hay una empresa asociada al proyecto, el nombre de la empresa aparece entre paréntesis después de esta configuración. |
      | Personas en el grupo de este proyecto | Los usuarios que pertenezcan al grupo asociado con este proyecto podrán ver y agregar solicitudes a esta cola. Si hay un grupo asociado al proyecto, el nombre del grupo se muestra entre paréntesis después de esta configuración. |

      {style="table-layout:auto"}

   * **Comparta con estos vínculos:** Las siguientes opciones permiten proporcionar acceso directo a la cola de solicitud y a los formularios asociados a ella a usuarios fuera de Workfront o a usuarios de Workfront que utilicen una página externa. Para obtener información sobre la incrustación de una cola de solicitudes en un panel como página externa, consulte [Incrustar una cola de solicitudes en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

      Los usuarios ya deben tener derechos de acceso a la cola de solicitud para obtener acceso directo. El uso de cualquiera de las opciones descritas aquí no concede automáticamente acceso a los usuarios.

      >[!TIP]
      >
      >Los usuarios deben iniciar sesión primero en Workfront antes de obtener acceso a la cola de solicitudes cuando acceden a la página Cola de solicitudes desde otra aplicación.

      * **Dirección URL de acceso directo:** Cuando un usuario accede a esta dirección URL desde un explorador, se dirige al usuario directamente a la sección Nueva solicitud del área Solicitudes y esta solicitud está seleccionada de forma predeterminada para ellos.

         ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

         >[!NOTE]
         >
         >Puede mostrar una cola de solicitud en un panel como página externa. En este caso, la cola de solicitud está preseleccionada, pero puede seleccionar cualquier otra cola de solicitud del campo Tipo de solicitud . los usuarios pueden cambiar el tipo de solicitud. También se muestran los componentes de navegación de las solicitudes.

      * **Código incrustado:** Utilice este código de HTML para incrustar el formulario de cola de solicitudes como iframe en cualquier página de HTML.\
         Si los usuarios no están autenticados en Workfront cuando ven la página donde está incrustado el código, se muestra el cuadro de diálogo de inicio de sesión de Workfront . Una vez que los usuarios inician sesión, se muestra el formulario Cola de solicitud .

         ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

         >[!NOTE]
         Cuando se muestra una cola de solicitud en un iframe, solo se muestra el formulario de solicitud, el nombre de la solicitud se preselecciona y se atenúa. El usuario no puede cambiar el tipo de solicitud. Los componentes de navegación del área Solicitudes no se muestran.

         Para que se muestre el formulario de la cola de solicitudes al utilizar este código incrustado, debe habilitar la configuración &quot;Permitir incrustación de Workfront en un iframe&quot; en la configuración del sistema. Para obtener más información sobre cómo habilitar la incrustación de Workfront en un iframe, consulte [Configuración de las preferencias de seguridad del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Si esta configuración no está activada, el iframe se muestra en blanco.

         Puede ajustar varios aspectos de cómo se muestra el formulario incrustado, de la siguiente manera:

         <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funcionalidad</strong> </p> </th> 
           <th> <p><strong>Solución</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Ajustar el tamaño del marco</p> </td> 
           <td> <p>Modifique los atributos "width" y "height".</p> <p>De forma predeterminada, la anchura es "500" y la altura es "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Dirigir a los usuarios a un tema de cola o grupo de temas específico</p> </td> 
           <td> <p>Agregue el parámetro "ruta" a la dirección URL src. Para encontrar el parámetro de ruta, vaya al tema de cola o al grupo de temas deseados en el formulario no incrustado e inspeccione la dirección URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostrar y permitir que los usuarios cambien la lista desplegable Grupo de temas preconfigurado</p> </td> 
           <td> <p>Utilice el parámetro "path" añadiendo la variable <code>showPreSelectedOptions=true</code> para <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detectar cuándo se ha enviado el formulario</p> </td> 
           <td> <p>Añada un detector de eventos "message" a la ventana de la página web y compruebe si <code>event.data.type</code> es <code>requestSubmitted</code>. <code>event.data.newIssueID</code> se establecerá en el ID del problema creado.</p> </td> 
          </tr> 
         </tbody> 
        </table>
   * **Tipos de solicitud:** Seleccione entre las opciones predeterminadas que aparecen a continuación.

      El administrador de Workfront puede cambiar el nombre de los tipos de solicitud predeterminados. Para obtener más información sobre el cambio de nombre de los tipos de solicitud, consulte [Personalización de tipos de problemas predeterminados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Cambiar orden
      * Problema
      * Solicitudes
      * Riesgo

         Se trata de un campo obligatorio y debe seleccionar al menos una opción.
      >[!NOTE]
      Los tipos de solicitud se muestran como una selección en el área Solicitudes solo si el tipo de solicitud está seleccionado en las páginas Detalles de la cola y Tema de la cola. Para obtener información sobre la configuración del área Detalles de cola de un proyecto, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Cada tipo seleccionado aquí estará disponible en el formulario (puede seleccionar más de uno). Seleccionar más de un tipo puede ayudar a organizar varias solicitudes que llegan.\
      Por ejemplo, si está utilizando el formulario en una cola de solicitudes para un proyecto de TI, los siguientes tipos de solicitud pueden llegar a la cola: hardware, software, correcciones de errores y problemas.

   * **Duración predeterminada:** La duración predeterminada es el período de tiempo que normalmente se tarda en completar un problema. Se convierte en el valor predeterminado para todos los problemas entrantes y se puede modificar manualmente. La duración se suele establecer en horas, días o semanas. La duración predeterminada de un problema es la misma que las horas planificadas para el problema. La Fecha de finalización planeada de la emisión calcula en función de este campo.\
      La duración predeterminada del problema es de 1 día u 8 horas. Si el administrador de Workfront establece el valor de Horas típicas por día laboral en menos de 8 horas, la duración predeterminada para los problemas es de 8 horas. Por ejemplo, si la opción Horas típicas por día de trabajo está establecida en 7 horas, la duración predeterminada para los problemas es de 1,14 días u 8 horas. Para obtener más información sobre cómo configurar el sistema Horario típico por día laboral, consulte la sección &quot;Cálculos de línea de tiempo&quot; en el artículo [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Las personas de la misma compañía heredarán los mismos permisos en todas las solicitudes.:** Cuando se selecciona, todas las solicitudes enviadas a la cola son visibles para los usuarios de la misma empresa. Los usuarios pueden ver estas solicitudes en la sección Todas las solicitudes , ubicada dentro del área Solicitudes . Cuando esta configuración está habilitada o deshabilitada, afecta a todas las solicitudes futuras; no afecta retroactivamente a la información.
   * **Cuando alguien realice una solicitud, conceda automáticamente:** Cuando un usuario realiza una solicitud a la cola de solicitudes, se le concede automáticamente el nivel de permiso que elija para esa solicitud. Seleccione entre los siguientes niveles de permisos:\
      **- Vista**

      **- Aportar**
      **- Administrar**

      Para obtener información sobre el modelo de permisos de Workfront, consulte [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
      Configurar los permisos aquí ahorra tiempo, en lugar de tener que conceder permisos para cada solicitud entrante individual. La selección de esta opción afecta a todas las solicitudes futuras, pero no afecta retroactivamente a las solicitudes existentes.

   * **Aprobación predeterminada**: Asocie un proceso de aprobación a esta cola de solicitudes. En este menú desplegable solo están visibles los procesos de aprobación de problemas. Todos los problemas enviados a esta cola se asociarán con este proceso de aprobación. El administrador de Workfront debe definir los procesos de aprobación a nivel del sistema antes de poder asociarlos a las colas de solicitud. Los usuarios con acceso administrativo a procesos de aprobación también pueden crear procesos de aprobación específicos del grupo.

      >[!IMPORTANT]
      Si el grupo del proyecto cambia, el proceso de aprobación específico del grupo asociado a problemas existentes se convierte en un proceso de aprobación de un solo uso. Para obtener más información sobre cómo los cambios en el grupo del proyecto o en el proceso de aprobación afectan a la configuración de aprobación, consulte [Efecto de los cambios en el grupo y el proceso de aprobación en los procesos de aprobación asignados](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

      Si tiene varios temas de cola asociados con una cola de solicitud, se recomienda asociar los procesos de aprobación con los temas de la cola. Para obtener más información sobre la creación de temas de cola, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Tenga en cuenta lo siguiente al agregar procesos de aprobación para solicitar colas:

      * En la lista solo se muestran los procesos de aprobación activos.
      * En la lista se muestran los procesos de aprobación de todo el sistema y de grupos específicos. Un proceso de aprobación asociado a un grupo que no sea el del proyecto no se muestra en la lista.
   * **Ruta predeterminada**: Asocie una regla de enrutamiento con esta cola de solicitudes. Utilice las reglas de enrutamiento para asignar automáticamente nuevos problemas enviados a una cola de solicitud al recurso correcto (usuario, función de trabajo o equipo) y al proyecto correcto. Todos los problemas enviados a esta cola se asociarán con esta regla de enrutamiento. Debe configurar las reglas de enrutamiento para poder asociarlas a la cola de solicitudes.\
      Si tiene varios temas de cola asociados con una cola de solicitud, se recomienda asociar las reglas de enrutamiento con los temas de la cola. Para obtener más información sobre la creación de reglas de enrutamiento, consulte [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nuevos campos de problema:** En la sección Show the following selected fields to all users , seleccione los campos que desee que sean visibles para todos los usuarios que envíen una solicitud al proyecto o que añadan un problema al proyecto o a las tareas.

      >[!TIP]
      Los nuevos campos de problema seleccionados en la sección Detalles de cola también están asociados a cualquier problema nuevo que se agregue al proyecto o a las tareas de la sección Problemas .

      Cuando se activa cualquiera de los campos Asignado a, Función de trabajo o Equipo, siempre se cambia el nombre a Asignaciones en el formulario de solicitud, pero solo se puede especificar el tipo de asignación seleccionada aquí.

      **Ejemplo:** Si ha seleccionado Asignado a en el área Detalles de la Cola , solo puede introducir usuarios en el campo Asignaciones del formulario de solicitud. En este caso, no puede introducir funciones de trabajo ni un equipo.

   * **Documentos**: Si selecciona mostrar la sección Documentos en el nuevo formulario de solicitud, seleccione dónde debe colocarse la sección Carga de documento. Seleccione una de las siguientes opciones:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Después de formularios personalizados</td> 
        <td><span>La sección Documentos se muestra en la parte inferior del formulario de solicitud.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Antes de formularios personalizados</td> 
        <td> <p><span>La sección Documents aparece entre los campos de Workfront y los campos personalizados del formulario de solicitud.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

      ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Mostrar todos los campos seleccionados y no seleccionados a:** Seleccione los usuarios que desea que vean todos los campos del formulario. Las siguientes opciones controlan el acceso a los campos del formulario.

      | Todos los usuarios (Planificar licencias) | Todos los usuarios que tengan una licencia de Plan pueden ver los campos seleccionados, así como los no seleccionados. |
      |---|---|
      | Personas con acceso de visualización en este proyecto (licencia de planificación) | Los usuarios con una licencia Plan que también tengan derechos de Vista para este proyecto pueden ver los campos seleccionados, así como los campos no seleccionados. El resto de los usuarios que pueden enviar solicitudes a este proyecto pueden ver solo los campos seleccionados. |
      | Ningún usuario | Ningún usuario puede ver los campos no seleccionados. Todos los usuarios que pueden enviar solicitudes a este proyecto solo pueden ver los campos seleccionados. |

      {style="table-layout:auto"}

   * **Forms personalizado**: Seleccione un formulario personalizado para asociarlo a la cola de solicitud. Solo se puede seleccionar Forms personalizado de problemas en este menú desplegable. Todos los problemas enviados a la cola de solicitud tendrán los formularios seleccionados asociados a ellos.\
      Si tiene varios temas de cola asociados con una cola de solicitud, le recomendamos que asocie formularios personalizados con los temas de la cola. Para obtener más información sobre la creación de subsecciones para la cola de solicitud, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Si tiene varios formularios personalizados asociados a la cola de solicitud, arrastre y suelte los formularios para ordenarlos en el orden deseado, en el **Reordenar Forms** para obtener más información.

      >[!TIP]
      Los formularios personalizados que se agregan a la sección Detalles de cola también están asociados a cualquier problema nuevo que se agregue al proyecto o a las tareas de la sección Problemas .

   * **Permitir que los problemas se añadan por correo electrónico:** Seleccione esta opción para permitir que las solicitudes se envíen por correo electrónico.\
      Para obtener más información, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitud](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).




1. Haga clic en **Guardar**.\
   El proyecto se ha configurado para ser una cola de solicitud y los usuarios ahora pueden agregarle solicitudes.

1. (Opcional) Para mejorar la funcionalidad Cola de solicitudes , cree subsecciones adicionales para la cola, así como reglas para enrutar las solicitudes entrantes al equipo, el usuario asignado o el proyecto correctos.

   Para obtener información sobre la creación de subsecciones para la cola de solicitud, consulte los artículos [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) y [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).\
   Para obtener información sobre el enrutamiento de las solicitudes al usuario asignado, equipo y proyecto adecuado, consulte [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
