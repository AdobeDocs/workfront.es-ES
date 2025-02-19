---
title: Creación de objetos de Workfront mediante automatizaciones de registros de Planning de Adobe Workfront
description: Puede configurar automatizaciones en Adobe Workfront Planning que, cuando estén activadas, creen objetos en Workfront o registros en Workfront Planning. Los objetos y registros creados se conectan automáticamente a los registros existentes de Planning. En este artículo se describe cómo administrar las automatizaciones, incluido cómo editarlas, deshabilitarlas, eliminarlas y almacenarlas en déclencheur para crear objetos y registros.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 966c2a2b0159c89a41d4502fb0eb0e318f3e5ba9
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 9%

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

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Puede configurar automatizaciones en Adobe Workfront Planning que, cuando estén activadas, creen objetos en Workfront o registros en Workfront Planning cuando se activen desde un registro de Planning. Los objetos o registros creados se conectan automáticamente a los registros desde los que activa la automatización.

Puede configurar y activar la automatización en la página del tipo de registro en Workfront Planning. El objeto conectado que se crea se coloca en el campo conectado del tipo de registro desde el que se ejecuta la automatización.

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
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

* El nuevo nombre de objeto o registro es el mismo que el nombre de registro a partir del cual se crea.
* Los nuevos objetos o registros no anulan los existentes en el mismo campo. Al activar la misma automatización varias veces para los mismos registros, se agregan los nuevos objetos o registros en el mismo campo conectado del registro original, además de los creados anteriormente.
* La automatización agrega objetos adicionales solo en los campos de tipo de conexión Varios a varios o Uno a varios. En todos los demás casos, la automatización crea el objeto, pero no lo conecta al registro original desde el que se activa la automatización.

## Configuración de una automatización en Workfront Planning

Debe configurar una automatización para un tipo de registro en Workfront Planning para poder utilizarlo para crear objetos.

{{step1-to-planning}}

1. Haga clic en una tarjeta de tipo de registro y, a continuación, haga clic en el nombre de un registro.

   Se abre la página de tipo de registro.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que hay a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Administrar automatizaciones**.

   Se abre la lista de automatizaciones disponibles para el tipo de registro seleccionado.

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

     >[!TIP]
     >
     >Una vez guardada la automatización, ya no se puede cambiar el tipo de objeto en este campo.

1. (Condicional) Según el tipo de objeto que desee crear, actualice los campos siguientes:


   * **Proyecto**:
      * **Campo conectado donde se crea el objeto**: Este es el campo conectado donde se mostrará el nuevo proyecto. Este campo es obligatorio.
      * **Plantilla a partir de la cual crear el proyecto**: seleccione una plantilla de proyecto que Workfront utilizará para crear el proyecto.
   * **Portfolio**:
      * **Campo conectado donde se crea el objeto**: Este es el campo conectado donde se mostrará el nuevo portafolio. Este campo es obligatorio.
      * **Formulario personalizado para adjuntar al nuevo portafolio**: seleccione un formulario personalizado para adjuntarlo al nuevo portafolio. Debe crear un formulario personalizado de portafolio para poder seleccionarlo.
   * **Programa**:
      * **Campo conectado donde se crea el objeto**: Este es el campo conectado donde se mostrará el nuevo programa. Este campo es obligatorio.
      * **Portafolio de programas**: seleccione un portafolio donde se agregará el nuevo programa. Este campo es obligatorio.
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
1. (Opcional y condicional) Si no tiene un campo de conexión para un tipo de objeto de Workfront, haga clic en el icono **Crear un campo de conexión** ![Crear un campo de conexión](assets/create-a-connection-field-icon.png) para agregar un campo.

   El nuevo campo se crea automáticamente y se denomina **Conectado &lt; nombre de objeto de Workfront >**. Por ejemplo, cuando se crea un campo conectado a un portafolio para el registro, se denomina &quot;Portafolio conectado&quot;.

1. Haga clic en **Guardar** en la esquina superior derecha de la página de detalles de automatización.

   La automatización se muestra en la lista de automatizaciones y está disponible para su uso en registros.
1. (Opcional) Para editar, deshabilitar o eliminar una automatización, haga lo siguiente:

   1. En la lista de automatizaciones, pase el ratón sobre el nombre de una automatización guardada y luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png).

   1. Haga clic en **Editar** para actualizar la información y configurar los campos de la automatización.
   1. Haga clic en **Deshabilitar** para quitar la automatización de la vista de tabla e impedir que los usuarios la usen para crear registros u objetos. Para que vuelva a estar disponible, vuelve a hacer clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haz clic en **Activar**.
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


<!--****************************************FUTURE ARTICLE AFTER THE RELEASE TO PREVIEW ON FEBRUARY 20:*****************************************************  

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same record adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 

(************hide this for now: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. ***************)

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. *************update this step with a list of all possible triggers; right now only Button click is available*********

1. Update the following fields in the **Actions** section: **********submitted bugs for these fields - see if they need changing here***********
   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Select one of the following actions: 

      * Create group
      * Create program
      * Create portfolio
      * Create project
      * Create record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the action selected in this field.

1. (Conditional) Depending on what action you selected, update the following fields:

   * **Create project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Project template**: Select a project template that Workfront will use to create the project.  
   * **Create portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Create program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create record**: 
      * **Record type**: Select the record type you want to create. 

      The **Settings** sub-section displays. Update the following fields in the **Settings** sub-section: 

      * **Field on the connected record type where the current record will show**: This is the connected field on the record type selected for the action where the current record will display. 
      
      For example, if you are creating an automation for campaigns to connect Product records from, this is the connected field on the Product record type where the campaigns will display, after the products are created using the automation. 
      
      This is a required field. 
      
      ******submitted a change in functionality and UI text for this - revise?? *******
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 

      >[!TIP]
      >
      >The field types from the original record type must match the field types from the newly created record type.

1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Conditional) If you selected to create a record and there are no connection fields between the original record type and the record type selected in the **Actions** area, click the question mark icon to the right of the **Field on the connected record type where the current record will show** field, then click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   The new field is automatically created for the record type you selected in the **Actions** area, and named **Connected Record**. 
   
   A connected field for the selected record type is also created on the original record type from where you are configuring the automation. 
1. (Optional and conditional) If you selected to create a Workfront object and don't have a connection field for the selected Workfront object type, click the question mark icon to the right of the **Connected field where the < Workfront object type name > is created** field, and click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.

## Manage existing automations

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. (Optional) To edit, disable, or delete an automation, do one of the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.

      >[!TIP]
      >
      >   You cannot change the action you originally selected for an automation. 
   

   1. Click **Disable** to remove the automation from the record's table view and prevent users from using it to create records or objects. 

   Records that have been created using a disabled automation remain connected to the record originally selected.
   
   To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. 
   
   Records that have been created using a deleted automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the automation you want to use to automatically create and connect records or objects. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   The following things occur: 

   * A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   * The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   * The record you are triggering the automation from is added to the connected field of the new record.

   >[!NOTE]
   >
   >We recommend checking that the objects or records were created and the connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

***********you might need to add something about notifications and emails?!*************

-->