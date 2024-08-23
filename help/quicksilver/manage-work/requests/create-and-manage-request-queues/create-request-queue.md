---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear una cola de solicitudes
description: Puede configurar una Cola de solicitudes en la que los usuarios puedan introducir solicitudes ocasionales que no estén planificadas para trabajar en un proyecto. Por ejemplo, se puede configurar una cola de solicitudes del servicio de asistencia para capturar todas las solicitudes de usuarios que llegan a un departamento de TI.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '2653'
ht-degree: 2%

---


# Crear una cola de solicitudes

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

Puede configurar una Cola de solicitudes en la que los usuarios puedan introducir solicitudes ocasionales que no estén planificadas para trabajar en un proyecto. Por ejemplo, se puede configurar una cola de solicitudes del servicio de asistencia para capturar todas las solicitudes de usuarios que llegan a un departamento de TI.

Este artículo describe cómo crear una cola de solicitudes en la que los usuarios pueden enviar solicitudes. Para obtener información sobre cómo enviar una nueva solicitud a una cola de solicitudes, consulte [Copiar y enviar solicitudes](../create-requests/copy-and-submit-requests.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Nueva licencia: Standard </p>
   O
   <p>Licencia actual: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administración de permisos del proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--old access levels: 
You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b></p> 
   
   <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator
-->

## Resumen de colas de solicitudes

Una cola de solicitudes se configura como un proyecto. Cuando designa el proyecto como una cola de solicitudes, se puede acceder a la cola desde el área de solicitudes de Adobe Workfront. Al personalizar la cola de solicitudes, también está personalizando el formulario que los usuarios rellenan cuando envían las solicitudes.

Este artículo describe cómo crear una cola de solicitudes a partir de un proyecto existente. Sin embargo, para generar coherencia en el proceso de admisión de solicitudes o para agregarle varias capas con fines de creación de informes y mejorar la administración, también puede configurar componentes básicos adicionales de una cola de solicitudes que se describen en la siguiente tabla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Detalles de cola</td> 
   <td> <p>Debe configurar un proyecto como cola de solicitudes en el área Detalles de la cola. Este paso es obligatorio. </p> <p>Para obtener más información, consulte la sección <a href="#create-a-request-queue" class="MCXref xref">Crear una cola de solicitudes</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Grupos de temas</td> 
   <td> <p>Son menús adicionales que clasifican las solicitudes en función de funciones comunes. Por ejemplo, para una cola de solicitudes de TI, es posible que desee tener grupos de temas "in situ" y "remoto". </p> <p>Para obtener más información, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Crear grupos de temas</a>. </p> <p>Esto es opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Temas de colas</td> 
   <td> <p>Son menús adicionales que clasifican solicitudes que pertenecen al mismo grupo de temas en función de características comunes. Un grupo de temas puede contener varios temas de colas. </p> <p>Por ejemplo, el grupo de temas "En el sitio" para la cola de solicitudes de TI puede contener los temas de colas "Hardware", "Software" y "Red". </p> <p>Para obtener más información, vea <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crear temas de colas</a>. </p> <p>Esto es opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reglas de enrutamiento</td> 
   <td> <p>Permiten dirigir cada solicitud a un usuario, rol, equipo o proyecto. </p> <p>Para obtener más información, vea <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Crear reglas de enrutamiento</a>. </p> <p>Esto es opcional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crear una cola de solicitudes

Al configurar un proyecto como Cola de solicitudes, el estado del proyecto debe ser Actual para que se muestre en el área Solicitudes de Workfront.

>[!TIP]
>
>Es posible que el administrador de su Workfront o de su grupo le asigne una plantilla de diseño personalizada que no incluya algunas de las secciones descritas en los pasos siguientes.


Para crear una cola de solicitudes:

1. Vaya al proyecto que desee configurar como cola de solicitudes.
1. (Opcional) Haga clic en **Detalles del proyecto** en el panel izquierdo y agregue una **Descripción** al proyecto en el área **Información general**. Esta información se muestra en todas las solicitudes nuevas.
1. Haga clic en **Detalles de cola** en el panel izquierdo. Es posible que tengas que hacer clic en **Mostrar más** y luego en **Detalles de la cola**.

   Se abrirá la sección Detalles de la cola.

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Especifique la siguiente información:

   * **Publish como cola de solicitud de ayuda:** Seleccione esta opción para identificar este proyecto como cola de solicitud. Todos los problemas entrantes se consideran solicitudes.\
     Cuando esta opción no está seleccionada, el proyecto se comporta como un proyecto estándar en Workfront y todos los problemas entrantes son problemas.

   * **Quién puede agregar solicitudes a esta cola:** Seleccione qué usuarios tienen acceso para agregar solicitudes a esta cola. Puede permitir que los siguientes grupos de personas vean la cola de solicitudes en su área de solicitudes de la barra de navegación global cuando agreguen una nueva solicitud:

     | Quién puede introducir solicitudes | Descripción |
     |---|---|
     | Cualquiera | Cualquier usuario de Workfront con una cuenta activa puede ver esta cola de solicitudes y agregarle solicitudes |
     | Personas con acceso de visualización en este proyecto | Los usuarios con permisos de Vista en el proyecto pueden ver y agregar solicitudes a esta cola |
     | Personas en la compañía de este proyecto | Los usuarios que pertenecen a la compañía asociada con este proyecto pueden ver y agregar solicitudes a esta cola. Si hay una empresa asociada al proyecto, el nombre de la empresa se muestra entre paréntesis después de esta configuración. |
     | Personas en el grupo de este proyecto | Los usuarios que pertenecen al grupo asociado a este proyecto pueden ver y agregar solicitudes a esta cola. Si hay un grupo asociado con el proyecto, el nombre del grupo se muestra entre paréntesis después de esta configuración, en fuente gris. |

     {style="table-layout:auto"}

   * **Compartir con estos vínculos:** Las siguientes opciones permiten proporcionar acceso directo a la cola de solicitudes y a los formularios asociados a ella a usuarios que no sean de Workfront o a usuarios de Workfront que usen una página externa. Para obtener información acerca de cómo incrustar una cola de solicitudes en un panel como página externa, vea [Incrustar una cola de solicitudes en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Los usuarios ya deben tener derechos de acceso a la cola de solicitudes para obtener acceso directo. El uso de cualquiera de las opciones descritas aquí no concede acceso automáticamente a los usuarios.

     >[!TIP]
     >
     >Los usuarios deben iniciar sesión en Workfront antes de obtener acceso a la cola de solicitudes cuando acceden a la página Cola de solicitudes desde otra aplicación.

      * **URL de acceso directo:** Cuando un usuario accede a esta URL desde un explorador, se le redirige directamente a la sección Nueva solicitud del área Solicitudes y se selecciona esta solicitud de forma predeterminada para ellos.

        ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >Puede mostrar una cola de solicitudes en un panel como una página externa. En este caso, la cola de solicitudes está preseleccionada, pero puede seleccionar cualquier otra cola de solicitudes del campo Tipo de solicitud. Los usuarios de pueden cambiar el Tipo de solicitud. También se muestran los componentes de navegación de las solicitudes.

      * **Código incrustado:** Utilice este código de HTML para incrustar el formulario de cola de solicitudes como un iframe en cualquier página de HTML.\
        Si los usuarios no están autenticados en Workfront cuando ven la página donde está incrustado el código, se muestra el cuadro de diálogo de inicio de sesión de Workfront. Cuando los usuarios inician sesión, se muestra el formulario Cola de solicitudes.

        >[!NOTE]
        >
        >Al mostrar una Cola de solicitudes en un iframe, solo se muestra el formulario de solicitud, el nombre de la solicitud aparece preseleccionado y atenuado. El usuario no puede cambiar el tipo de solicitud. Los componentes de navegación del área de Solicitudes no se muestran.

        Para que el formulario de cola de solicitudes se muestre al utilizar este código incrustado, debe habilitar la configuración &quot;Permitir incrustación de Workfront en un iframe&quot; en la configuración del sistema. Para obtener más información sobre cómo habilitar la incrustación de Workfront en un iframe, consulte [Configurar las preferencias de seguridad del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Si esta configuración no está habilitada, el iframe se muestra en blanco.

        Puede ajustar varios aspectos de cómo se muestra el formulario incrustado de la siguiente manera:

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
           <td> <p>Modifique los atributos "anchura" y "altura".</p> <p>De forma predeterminada, la anchura es "500" y la altura es "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Dirigir a los usuarios a un tema de cola o grupo de temas específico</p> </td> 
           <td> <p>Añada el parámetro "path" a la dirección URL src. Puede encontrar el parámetro de ruta navegando hasta el tema de la cola o el grupo de temas deseado en el formulario no incrustado e inspeccionando la dirección URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostrar y permitir a los usuarios cambiar la lista desplegable de grupo de temas preconfigurada</p> </td> 
           <td> <p>Use el parámetro "path" agregando el parámetro <code>showPreSelectedOptions=true</code> a <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detectar cuándo se ha enviado el formulario</p> </td> 
           <td> <p>Agregue un detector de eventos "message" a la ventana de su página web y verifique si <code>event.data.type</code> es <code>requestSubmitted</code>. <code>event.data.newIssueID</code> se establecerá en el ID del problema creado.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Tipos de solicitud:** Seleccione entre las opciones predeterminadas siguientes.

     El administrador de Workfront puede cambiar el nombre de los tipos de solicitud predeterminados. Para obtener más información sobre cómo cambiar el nombre de los tipos de solicitud, consulte [Personalizar tipos de problemas predeterminados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Informe de errores
      * Solicitud de cambio
      * Problema
      * Solicitud

        Este campo es obligatorio y debe seleccionar al menos una opción.

     >[!NOTE]
     >
     >Los tipos de solicitud se muestran como una selección en el área Solicitudes sólo si el tipo de solicitud está seleccionado en las páginas Detalles de Cola y Tema de Cola. Para obtener información acerca de cómo configurar el área Detalles de cola de un proyecto, vea [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Cada tipo seleccionado aquí estará disponible en el formulario (puede seleccionar más de uno). Seleccionar más de un tipo puede ayudar a organizar las solicitudes que se reciben.\
     Por ejemplo, si utiliza el formulario en una cola de solicitudes para un proyecto de TI, pueden aparecer en la cola los siguientes tipos de solicitudes: hardware, software, correcciones de errores y problemas.

   * **Duración predeterminada:** La duración predeterminada es el tiempo que normalmente se tarda en completar un problema. Esto se convierte en el valor predeterminado para todos los problemas entrantes y se puede modificar manualmente. La duración suele establecerse en horas, días o semanas. La duración predeterminada de un problema es la misma que las horas planificadas para el mismo. La fecha planificada de finalización del problema se calcula según este campo.\
     El valor predeterminado para la duración del problema es de 1 día u 8 horas. Si el administrador de Workfront establece las horas típicas por día laborable en menos de 8 horas, la duración predeterminada de los problemas sigue siendo de 8 horas. Por ejemplo, si el valor de Horas habituales por día laborable es de 7 horas, el valor de Duración predeterminada para los problemas es de 1,14 días u 8 horas. Para obtener más información acerca de cómo configurar el sistema Horas típicas por día laborable, vea la sección &quot;Cálculos de escala de tiempo&quot; en el artículo [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Las personas de la misma compañía heredarán los mismos permisos para todas las solicitudes.:** Cuando se seleccionan, todas las solicitudes enviadas a la cola son visibles para los usuarios de la misma compañía. Los usuarios pueden ver estas solicitudes en la sección Todas las solicitudes , ubicada dentro del área Solicitudes. En el momento en que esta configuración está habilitada o deshabilitada, afecta a todas las solicitudes futuras; no afecta de forma retroactiva a la información.
   * **Cuando alguien realiza una solicitud, conceder automáticamente:** Cuando un usuario realiza una solicitud a la cola de solicitudes, se concede automáticamente al usuario el nivel de permiso que usted elija para esa solicitud. Seleccione entre los siguientes niveles de permisos:

      * **Ver acceso**
      * **Acceso a Contribute**. Esta es la selección predeterminada.
      * **Administrar acceso**

     Para obtener información acerca del modelo de permisos de Workfront, vea [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Al establecer permisos aquí se ahorra tiempo, en lugar de tener que conceder permisos para cada solicitud entrante individual. Elegir esta opción afecta a todas las solicitudes futuras, pero no tiene un impacto retroactivo en las solicitudes existentes.

   * **Aprobación predeterminada**: asocie un proceso de aprobación con esta cola de solicitudes. En este menú desplegable solo están visibles los procesos de aprobación de problemas. Todos los problemas enviados a esta cola se asociarán con este proceso de aprobación. El administrador de Workfront debe definir los procesos de aprobación en el nivel de sistema antes de poder asociarlos a colas de solicitudes. Los usuarios con acceso administrativo a los procesos de aprobación también pueden crear procesos de aprobación específicos del grupo.

     >[!IMPORTANT]
     >
     >Si el grupo del proyecto cambia, el proceso de aprobación específico del grupo adjunto a los problemas existentes se convierte en un proceso de aprobación de un solo uso. Para obtener más información acerca de cómo afectan los cambios en el grupo del proyecto o los cambios en el proceso de aprobación a la configuración de aprobación, vea [Cómo afectan los cambios en el grupo y el proceso de aprobación a los procesos de aprobación asignados](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Si tiene varios temas de colas asociados a una cola de solicitudes, le recomendamos que asocie procesos de aprobación a los temas de colas. Para obtener más información acerca de cómo crear temas de colas, vea [Crear temas de colas](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Tenga en cuenta lo siguiente al agregar procesos de aprobación a las colas de solicitud:

      * En la lista solo se muestran los procesos de aprobación activos.
      * Los procesos de aprobación de todo el sistema y específicos del grupo se muestran en la lista. Un proceso de aprobación asociado a un grupo que no sea el del proyecto no se muestra en la lista.

   * **Ruta predeterminada**: asocie una regla de enrutamiento con esta cola de solicitudes. Utilice Reglas de enrutamiento para asignar automáticamente los nuevos problemas enviados a una cola de solicitudes al recurso correcto (usuario, rol o equipo) y al proyecto correcto. Todos los problemas enviados a esta cola se asociarán con esta regla de enrutamiento. Debe configurar las reglas de enrutamiento para que se muestren en la sección Detalles de cola y para poder asociarlas a la cola de solicitudes.\
     Si tiene varios temas de colas asociados a una cola de solicitudes, le recomendamos que asocie las reglas de enrutamiento a los temas de colas. Para obtener más información acerca de la creación de reglas de enrutamiento, vea [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nuevos campos de problema:** En la sección **Mostrar los siguientes campos seleccionados a todos los usuarios**, seleccione los campos que desee que estén visibles para todos los usuarios que envíen una solicitud al proyecto o que agreguen un problema al proyecto o a las tareas.

     >[!TIP]
     >
     >Nuevos campos de problema seleccionados en la sección Detalles de cola también están asociados con cualquier problema nuevo agregado al proyecto <!--this is confusing: or to the tasks in the Issues section-->.

     Al habilitar cualquiera de los campos Asignado a, Rol de trabajo o Equipo, siempre se les cambia el nombre a Asignaciones en el formulario de solicitud, pero solo puede especificar el tipo de asignación seleccionada aquí.

     >[!NOTE]
     >
     >Si ha seleccionado Asignado a en el área Detalles de Cola, solo puede introducir usuarios en el campo Asignaciones del formulario de solicitud. En este caso, no puede introducir funciones ni un equipo.

   * **Documentos**: si selecciona mostrar la sección Documentos en el nuevo formulario de solicitud, seleccione dónde se debe colocar la sección de carga de documentos. Seleccione una de las siguientes opciones:

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
        <td> <p><span>Se muestra la sección Documentos entre los campos de Workfront y los campos personalizados del formulario de solicitud.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Mostrar todos los campos seleccionados y no seleccionados a:** Seleccione a qué usuarios desea ver todos los campos del nuevo formulario de solicitud. Las siguientes opciones controlan el acceso a los campos del formulario.

     | Qué usuarios pueden ver todos los campos del formulario de solicitud | Descripción |
     |---|---| 
     | Todos los usuarios (licencias de planificación) | Todos los usuarios que tengan una licencia de planificación pueden ver los campos seleccionados y los no seleccionados. |
     | Personas con acceso de visualización en este proyecto (licencia de planificación) | Los usuarios con una licencia de planificación que también tengan derechos de visualización sobre este proyecto pueden ver los campos seleccionados y los no seleccionados. El resto de los usuarios que pueden enviar solicitudes a este proyecto pueden ver solo los campos seleccionados. |
     | Ningún usuario | Ningún usuario puede ver los campos no seleccionados. Todos los usuarios que pueden enviar solicitudes a este proyecto solo pueden ver los campos seleccionados. |

   * **Forms personalizado**: seleccione un formulario personalizado para asociarlo a la cola de solicitudes. En este menú desplegable solo está disponible la opción Problema con Forms personalizado. Todos los problemas enviados a la cola de solicitudes tendrán los formularios seleccionados asociados a ellos. Debe crear formularios personalizados de problema antes de poder verlos mostrados en la sección Detalles de la cola.
Si tiene varios temas de la cola asociados a una cola de solicitudes, le recomendamos que asocie formularios personalizados a los temas de la cola en su lugar. Para obtener más información sobre la creación de subsecciones para la cola de solicitudes, consulte [Crear temas de colas](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![](assets/custom-forms-on-queue-details.png)

     Si tiene varios formularios personalizados asociados a la cola de solicitudes, arrastre y suelte los formularios para ordenarlos en el orden deseado, en la sección **Reordenar Forms**.

     >[!TIP]
     >
     >Los formularios personalizados agregados a la sección Detalles de cola también están asociados con cualquier problema nuevo agregado al proyecto <!--this is confusiong: or the tasks in the Issues  section-->.

1. Siga seleccionando información para la configuración en el área **Configuración de la cola de correo electrónico**, para permitir que los usuarios envíen solicitudes por correo electrónico al proyecto de cola de solicitudes.

   Para obtener más información, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitudes](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Haga clic en **Guardar**.\
   El proyecto se ha configurado para ser una cola de solicitudes y los usuarios ahora pueden agregarle solicitudes.

1. (Opcional) Para mejorar la funcionalidad de la cola de solicitudes, cree subsecciones adicionales para la cola, así como reglas para redirigir las solicitudes entrantes al equipo, usuario asignado o proyecto correcto.

   * Para obtener información acerca de cómo crear subsecciones para la cola de solicitudes, vea los artículos [Crear temas de colas](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) y [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Para obtener información sobre cómo enrutar las solicitudes al usuario asignado, al equipo y al proyecto adecuados, consulte [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
