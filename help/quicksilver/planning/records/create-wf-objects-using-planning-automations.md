---
title: Creación de objetos de Workfront mediante automatizaciones de registros de Planning de Adobe Workfront
description: Puede configurar automatizaciones en Adobe Workfront Planning que, cuando estén activadas, creen objetos en Workfront o registros en Workfront Planning. Los objetos y registros creados se conectan automáticamente a los registros existentes de Planning.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 10%

---

# Creación de objetos mediante automatizaciones de registros de Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Puede configurar automatizaciones en Adobe Workfront Planning que, cuando estén activadas, creen objetos en Workfront o registren Workfront Planning. Los objetos o registros creados se vinculan automáticamente a los registros desde los que activa la automatización.

Puede configurar y activar la automatización en la página del registro en Workfront Planning. El objeto conectado que se crea se coloca en el campo conectado del tipo de registro desde el que se ejecuta la automatización.

Por ejemplo, puede crear una automatización que tome una campaña de Workfront Planning y cree un proyecto en Workfront para rastrear el progreso de esa campaña. El proyecto estaría conectado a la campaña de Workfront Planning en el campo Proyecto conectado de la campaña.

Para obtener más información sobre los registros conectados, consulte [Información general sobre los registros conectados](/help/quicksilver/planning/records/connected-records-overview.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td> Estándar
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p> 
   <p>Edite el acceso en Workfront para los tipos de objeto que desea crear (proyectos, portafolios, programas). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Administre los permisos del espacio de trabajo al que desee agregar registros. </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   <p>Administre permisos a objetos Workfront (portafolios) para agregar objetos secundarios (proyectos).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>Todos los usuarios, incluidos los administradores de Workfront, deben tener asignada una plantilla de diseño que incluya el área de Planning en el menú principal </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Consideraciones sobre la creación de objetos y registros mediante una automatización

* El nuevo nombre de objeto o registro es el mismo que el nombre de registro a partir del cual se crea. <!--take this out when they add the field mapping - no longer just the name of the original record-->
* Los objetos nuevos no anulan los existentes en el mismo campo.
* La automatización crea objetos adicionales solo en los campos de tipo de conexión Varios a varios o Uno a varios.

## Configuración de una automatización en Workfront Planning

Debe configurar una automatización para un tipo de registro en Workfront Planning para poder utilizarlo para crear objetos.

{{step1-to-planning}}

1. Haga clic en una tarjeta de tipo de registro y, a continuación, haga clic en el nombre de un registro.

   Se abre la página de tipo de registro.
1. Haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Administrar automatizaciones**.

   Se abre la lista de automatizaciones disponibles.

1. Haga clic en **Nueva automatización** en la esquina superior derecha de la pantalla. Se abre el cuadro **Nueva automatización**.
1. Actualice los campos siguientes:

   * Reemplace **automatización sin título** por el texto que desea que aparezca en el botón de automatización. Los usuarios harán clic en este botón cuando utilicen la automatización para crear un objeto de Workfront o un registro de Planning.
   * **Descripción**: agregue una descripción para identificar el propósito de la automatización.
1. Haga clic en **Guardar**.
Se abre la página de detalles de automatización.

1. En la página de detalles de la automatización, actualice los campos siguientes en la sección **Déclencheur**:

   * **Déclencheur**: seleccione la acción que almacenará en déclencheur la automatización. Por ejemplo, seleccione **clic en botón**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Actualice los campos siguientes en la sección **Acciones**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Tipo de objeto**: seleccione el objeto que desea que cree la automatización. Este campo es obligatorio.

     Puede crear los siguientes objetos a partir de los registros de Workfront Planning:

      * Proyecto
      * Portafolio
      * Programa
      * Grupo
      * Registro
1. (Condicional) Según el tipo de objeto que desee crear, actualice los campos siguientes:

   * **Proyecto**:
      * **Campo conectado donde se crea el objeto**: Este es el campo conectado donde se mostrará el nuevo proyecto. Este campo es obligatorio
      * **Plantilla a partir de la cual crear el proyecto**: seleccione una plantilla de proyecto que Workfront utilizará para crear el proyecto.
   * **Portfolio**:
      * **Campo conectado donde se crea el objeto**: Este es el campo conectado donde se mostrará el nuevo portafolio. Este campo es obligatorio.
      * **Formulario personalizado para adjuntar al nuevo portafolio**: seleccione un formulario personalizado para adjuntarlo al nuevo portafolio. Debe crear un formulario personalizado de portafolio para poder seleccionarlo.
   * **Programa**:
      * **Campo conectado donde se crea el objeto**: Este es el campo conectado donde se mostrará el nuevo programa. Este campo es obligatorio.
      * **Portafolio de programas**: seleccione un portafolio donde se agregará el nuevo programa. Este campo es obligatorio.
      * 
         * **Formulario personalizado para adjuntar al nuevo programa**: seleccione un formulario personalizado para adjuntarlo al nuevo programa. Debe crear un formulario personalizado de programa para poder seleccionarlo.
   * **Grupo**:
      * **Campo conectado donde se crea el objeto**: Este es el campo conectado donde se mostrará el nuevo grupo. Este campo es obligatorio.
      * **Formulario personalizado para adjuntar al nuevo grupo**: seleccione un formulario personalizado para adjuntarlo al nuevo programa. Debe crear un formulario personalizado de programa para poder seleccionarlo.
   * **Registro**:
      * **Tipo de registro conectado**: seleccione el tipo de registro que desea crear.
      * **Campo conectado donde se crea el registro**: Este es el campo conectado donde se mostrará el nuevo registro. Este campo es obligatorio. <!--this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label-->
      * **Asignar campos**
         * **Transferir de**: seleccione campos del tipo de registro para el que se creó la automatización para asignarlos a los campos del tipo de registro conectado.
      * **Transferir a**: seleccione campos del registro recién creado que se rellenarán con información del registro desde el que está ejecutando la automatización.
1. (Opcional y condicional) Si seleccionó crear un registro, haga clic en **Agregar campos** para asignar campos de búsqueda adicionales de un registro a otro.
1. (Opcional y condicional) Si no tiene un campo de conexión para un tipo de objeto de Workfront, haga clic en el icono **Crear un campo de conexión** ![](assets/create-a-connection-field-icon.png) para agregar un campo.
1. Haga clic en **Guardar** en la esquina superior derecha de la página de detalles de automatización.

   La automatización se muestra en la lista de automatizaciones y está disponible para su uso en registros.
1. (Opcional) Para editar, deshabilitar o eliminar una automatización, haga lo siguiente:

   1. En la lista de automatizaciones, pase el ratón sobre el nombre de una automatización guardada y luego haga clic en el menú **Más** ![](assets/more-menu.png).

   1. Haga clic en **Editar** para actualizar la información y configurar los campos de la automatización.
   1. Haga clic en **Deshabilitar** para quitar la automatización de la vista de tabla e impedir que los usuarios la usen para crear registros u objetos. Para que vuelva a estar disponible, vuelva a hacer clic en el menú **Más** ![](assets/more-menu.png) y, a continuación, haga clic en **Activar**.
   1. Haga clic en **Eliminar** para eliminar la automatización. Una automatización eliminada no se puede recuperar. Los registros que se han creado con la automatización permanecen conectados al registro seleccionado originalmente.

## Utilice una automatización de Workfront Planning para crear un objeto o un registro

1. En Workfront Planning, abra la página de tipo de registro que contiene los registros que desea utilizar para crear objetos de Workfront o registros de Planning.
1. Abra la vista de tabla.
1. Seleccione uno o varios registros.

   Aparece una barra azul en la parte inferior de la tabla con botones adicionales, incluidos los botones de automatización.
1. Haga clic en el botón de automatización cerca de la esquina inferior derecha de la pantalla.

   ![Botón de automatización](assets/automation-custom-button.png)

   Si la automatización ha creado correctamente un objeto o un registro, aparece un mensaje de confirmación en la parte inferior de la pantalla.

   El nuevo objeto se muestra en el campo conectado indicado en la configuración del botón de automatización. Es posible que tenga que actualizar la página antes de ver el nuevo objeto.

   >[!NOTE]
   >
   >Se recomienda comprobar que el objeto se ha creado y conectado según lo esperado.

1. (Opcional) Haga clic en el nuevo objeto del campo conectado. Se abrirá la página del objeto y podrá realizar cambios adicionales en el nuevo objeto.

<!--you might need to add something about notifications and emails?!-->
