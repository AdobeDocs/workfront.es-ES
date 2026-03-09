---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear proyecto de Forms de admisión
description: Puede utilizar formularios de entrada de proyectos para simplificar el proceso de creación de proyectos en Workfront
author: Alina
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 5%

---

# Crear formularios de entrada de proyecto

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Los formularios de entrada de proyecto son un tipo de formulario de solicitud que permite a los usuarios solicitar proyectos. Los proyectos se crean a partir del formulario, sin necesidad de crear un proyecto a partir de un problema enviado.

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
   <td> 
   <p>Nueva licencia: estándar </p>
   O
   <p>Licencia actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront para crear formularios de entrada de proyectos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Otros productos</td> 
   <td> <p>Su organización debe haber adquirido Workfront Planning para utilizar funciones de Planning como las automatizaciones.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Capacidades y limitaciones de Project Intake Forms

### Competencias

Los formularios de entrada del proyecto incluyen las siguientes capacidades:

#### Automatizaciones de Workfront Planning

Los formularios de entrada de proyectos de Workfront admiten Workfront Planning Automations para configurar las propiedades específicas del proyecto creadas.

Para obtener más información sobre las automatizaciones de Planning, consulte [Configuración de automatizaciones de Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Configuración de aprobación

Los formularios de entrada de proyecto incluyen la capacidad de configurar aprobadores para las solicitudes enviadas.

### Limitaciones

#### Tipos de campo admitidos

Forms de admisión de proyectos puede incluir campos de cualquier formulario personalizado con el tipo de objeto Proyecto.

Los siguientes tipos de campo no son compatibles actualmente con Project Intake Forms:

* Sección
* Fórmula
* Resumen
* Resumen de línea única
* Conexión de planificación
* Referencias de campos nativos a los que se hace referencia en los campos nativos de Project, que son de sólo lectura (por ejemplo, `workRequiredExpression`)

#### Solicitando experiencia

Los formularios de admisión de proyectos solo se pueden utilizar con la nueva experiencia solicitante.

Para obtener información sobre la nueva experiencia de solicitud, consulte [Crear y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

#### Uso compartido

Los formularios de admisión del proyecto no admiten el uso compartido público. Las opciones de uso compartido incluyen:

* **Cualquiera**: cualquier persona del sistema puede usar el formulario para enviar una solicitud de proyecto.
* **Usuarios especificados**: puede seleccionar qué usuarios específicos tienen acceso al formulario de solicitud de proyecto.

## Creación de un formulario de entrada de proyecto

{{step1-to-requests}}

1. Habilite **Cambiar a una nueva configuración de experiencia**, en la esquina superior derecha de la pantalla.
1. Haga clic en **Formularios de solicitud** en la esquina superior derecha de la pantalla.

   >[!NOTE]
   >
   >Dado que solo los administradores de Workfront pueden crear formularios de entrada, el botón Solicitar formularios solo está visible para los administradores.

   Aparecerá una lista de los formularios de solicitud disponibles actualmente. Esto incluye formularios de solicitud de Workfront Planning.

1. Haga clic en **Nuevo formulario de solicitud** en la esquina superior derecha de la pantalla.
1. Introduzca un nombre para el formulario de solicitud. De manera predeterminada, el nombre del formulario es **Formulario sin título**.
1. Seleccione el tipo de objeto **Proyecto** cerca de la parte superior de la lista desplegable. Actualmente, este es el único tipo de proyecto de Workfront disponible. Otros elementos de la lista pertenecen a Workfront Planning.
1. (Opcional) Agregue una **Descripción** para el formulario de solicitud.
1. Haga clic en **Crear**. El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.

   El generador de formularios de entrada de proyecto se abre en la pestaña Formulario.

   El formulario de admisión contiene la siguiente información de forma predeterminada:

   * **Sección predeterminada**: Este es el salto de sección predeterminado que Workfront aplica al formulario de solicitud. Todos los campos de registro se muestran en el área **Sección predeterminada**.
   * Campo **Asunto**: Campo que identificará la solicitud en Workfront. La configuración y el valor del campo Subject no se pueden editar.
   * Todos los campos asociados con los proyectos.

     Los campos contenidos en el formulario de solicitud serán visibles para todos los que envíen una solicitud de proyecto.

1. Para añadir campos al formulario, haga clic en el tipo de campo en el panel de navegación izquierdo y, a continuación, seleccione el campo.
1. (Opcional) Para quitar un campo, pase el ratón sobre el campo del formulario que quiera quitar y luego haga clic en el icono **x** para quitarlo.
1. (Opcional) Para quitar la **sección predeterminada** del formulario, haga lo siguiente:

   1. Elimine todos los campos de la sección predeterminada.
   1. Haga clic en la ficha **Elementos de contenido**, agregue una nueva sección y, a continuación, agregue un nombre para la sección.
   1. Agregue campos a la nueva sección.
   1. Haga clic en el icono **x** para quitar la **sección predeterminada**.
1. Haga clic en cualquier campo y, a continuación, utilice los controles del panel derecho del formulario para definir su tamaño o cualquiera de las siguientes informaciones:

   * **Etiqueta**: este es el nombre del campo tal como aparecerá en el formulario de solicitud. Esto no cambia el nombre del campo de registro.
   * **Instrucciones**: Agregue más información sobre el campo.
   * **Crear un campo obligatorio**: cuando se selecciona, el campo debe tener un valor. De lo contrario, el formulario no se podrá enviar.
   * **Agregar lógica**: defina qué condiciones deben cumplirse para que el campo se muestre o se oculte.

   >[!TIP]
   >
   >   El tipo de campo de cada campo se muestra en la parte superior del panel derecho, después de seleccionar el campo en el formulario.
   >     

1. (Opcional) Haga clic en la pestaña **Elementos de contenido** de la parte izquierda del formulario y agregue cualquiera de los siguientes elementos:

   * **Texto descriptivo**
   * **Salto de sección**

   Para obtener más información sobre cómo crear un formulario personalizado, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en la ficha **Automatizaciones** de la izquierda del formulario y, a continuación, siga uno de estos procedimientos:

   * Seleccione una plantilla de proyecto
   * Adjuntar cualquier formulario personalizado
   * Definir el propietario de un proyecto
   * Agregar el proyecto a un portafolio o programa

   Cualquier selección que realice aquí se aplicará a los proyectos creados a partir de este formulario de entrada.

1. (Opcional) Haga clic en **Vista previa** para ver cómo se mostrará el formulario para otros usuarios cuando lo usen para enviar un nuevo registro.

1. (Opcional) Haga clic en la ficha **Configuración** y, a continuación, agregue al menos un usuario o equipo&lt; al campo **Aprobadores** para aprobar nuevas solicitudes para este formulario de admisión.

   * Al asociar un formulario de entrada a los aprobadores, cualquier nueva solicitud debe ser aprobada primero por todos los aprobadores antes de que genere un proyecto.
   * Puede agregar uno o varios aprobadores a un formulario de entrada.
   * Si al menos un aprobador rechaza la solicitud, esta se rechaza y el proyecto no se crea.
   * Todos los aprobadores deben tomar una decisión antes de aprobar o rechazar un proyecto.
   * Si un equipo se establece como aprobador, solo se requiere una decisión del equipo.

     Para obtener más información sobre cómo agregar aprobaciones a los formularios de solicitud, consulte [Agregar aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Opcional) Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del formulario en el encabezado y, a continuación, haga clic en **Editar** para actualizar el nombre del formulario.

1. Haga clic en **Publicar** para publicar el formulario y obtener un vínculo único para él.

   Ocurren lo siguiente:

   * Se ha quitado el botón **Publicar**.
   * Se agrega el botón **Cancelar publicación** al formulario. Si hace clic en él, se impedirá el acceso al formulario.
   * Se agrega un botón **Compartir** al formulario.
   * El formulario está disponible en el área de Solicitudes del menú principal de Workfront.

1. Haga clic en **Compartir** para compartir el formulario con otros usuarios.
1. Haga clic en la flecha que señala a la izquierda del nombre del formulario en el encabezado para cerrar el formulario.

   Se abre la vista de tabla **Formularios de solicitud** y se agrega el formulario.

1. (Opcional) Pase el ratón sobre el nombre de un formulario de solicitud en la vista de tabla, luego haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del formulario y haga clic en una de las siguientes opciones:

   * **Editar formulario**: haga clic aquí para editar más información en el formulario.
   * **Cancelar publicación**: haga clic aquí para cancelar la publicación del formulario que lo quita del área de solicitudes en Workfront.
   * **Compartir**: haga clic aquí para modificar quién tiene acceso al formulario.
   * **Copiar vínculo**: haga clic aquí para copiar rápidamente el vínculo del formulario de solicitud sin abrir el formulario.
   * **Eliminar**: haga clic aquí para eliminar el formulario. No se eliminan todas las solicitudes y registros agregados mediante el formulario. El formulario no se puede recuperar.

   >[!NOTE]
   >
   >Puede identificar los formularios de entrada de proyecto en la vista de tabla porque muestran &quot;Proyecto&quot; en la columna Tipo de objeto.

1. Haga clic en la flecha que señala a la izquierda de **Formularios de solicitud** en el encabezado para cerrar la tabla de Formularios de solicitud.

