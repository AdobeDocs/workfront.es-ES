---
title: Creación de objetos de Workfront mediante automatizaciones de registros de Planning de Adobe Workfront
description: Puede configurar automatizaciones en Workfront Planning para que, cuando se activen, creen objetos en Workfront.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 11%

---

# Creación de objetos mediante automatizaciones de registros de Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Puede configurar automatizaciones en Adobe Workfront Planning que, cuando estén activadas, creen objetos en Workfront o Workfront Planning.

Puede configurar y activar la automatización en la página del registro. El objeto que se crea se conecta al registro de Planning y se coloca en el campo especificado en la automatización.

Por ejemplo, puede crear una automatización que tome una campaña de Workfront Planning y cree un proyecto en Workfront para rastrear el progreso de esa campaña. El proyecto estaría conectado a la campaña de Workfront Planning.

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

* El nuevo nombre de objeto o registro es el mismo que el nombre de registro a partir del cual se crea.
* Si el registro para el que utiliza la automatización ya tiene objetos del mismo tipo conectados en el campo que seleccione para agregar nuevos objetos, los nuevos objetos se agregan al campo de conexión y los objetos existentes también permanecen conectados.

## Configuración de una automatización en Workfront Planning

Debe configurar una automatización en Workfront Planning para poder utilizarla para crear objetos.

{{step1-to-planning}}

1. Haga clic en una tarjeta de tipo de registro y, a continuación, haga clic en el nombre de un registro.

   Se abre la página de tipo de registro.
1. Haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Administrar automatizaciones**.

   Se abre la lista de automatizaciones disponibles.

1. Haga clic en **Nueva automatización** en la esquina superior derecha de la pantalla. Se abre el cuadro **Nueva automatización**.
1. Actualice los campos siguientes:

   * Reemplace **automatización sin título** por el texto que desea que aparezca en el botón de automatización. Los usuarios harán clic en este botón al utilizar la automatización para crear un objeto de Workfront.
   * **Descripción**: agregue una descripción para identificar el propósito de la automatización.

1. En la página de detalles de la automatización, actualice los campos siguientes en la sección **Déclencheur**:

   * **Déclencheur**: seleccione la acción que almacenará en déclencheur la automatización. Por ejemplo, seleccione **clic en botón**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Actualice los campos siguientes en la sección **Acciones**:
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
      * **Campo conectado donde se crea el registro**: Este es el campo conectado donde se mostrará el nuevo registro. Este campo es obligatorio.
      * **Campo de asignación**: seleccione campos del tipo de registro para el que se creó la automatización para asignarlos a los campos del tipo de registro conectado.
      * **Para el campo de registro conectado**: seleccione los campos del registro conectado que corresponderán a los campos del tipo de registro para el que cree la automatización.
1. (Opcional y condicional) Si no tiene un campo de conexión para un tipo de objeto de Workfront, haga clic en el icono **Crear un campo de conexión** ![](assets/create-a-connection-field-icon.png) para agregar un campo.
1. (Opcional y condicional) Si seleccionó agregar un registro, haga clic en **Agregar** en el área de **Asignar campos** para agregar y asignar campos adicionales y, a continuación, seleccione un campo en **Transferir de** y un campo en **Transferir a** para indicar qué campo del registro seleccionado originalmente debe mostrarse en qué campo del registro conectado.
1. Haga clic en **Guardar**.

   La automatización aparece en la lista de automatizaciones y está disponible para su uso en registros.
1. (Opcional) Para editar, deshabilitar o eliminar una automatización, haga lo siguiente:

   En la lista de automatizaciones, pase el ratón sobre el nombre de una automatización guardada, haga clic en el menú **Más** ![](assets/more-menu.png) y, a continuación, elija una de las siguientes opciones:

   * **Editar**: actualice la información y configure los campos en la automatización.
   * **Deshabilitar**: la automatización no se mostrará como una opción en la barra de herramientas de la vista de tabla de los registros y los usuarios ya no podrán utilizarla para crear registros u objetos. Para que vuelva a estar disponible, vuelva a hacer clic en el menú **Más** ![](assets/more-menu.png) y, a continuación, haga clic en **Activar**.
   * **Eliminar**: la automatización se ha eliminado y no se puede recuperar. Los registros que se han creado con la automatización permanecen conectados al registro seleccionado originalmente.

## Utilice una automatización de Workfront Planning para crear un objeto

1. En Workfront Planning, abra la página de tipo de registro que contiene los registros que desea utilizar para crear objetos de Workfront.
1. Abra la vista de tabla.
1. Seleccione uno o varios registros.

   Aparece una barra azul en la parte inferior de la tabla con botones adicionales, incluidos los botones de automatización.
1. Haga clic en el botón de automatización cerca de la esquina inferior derecha de la pantalla.

   ![Botón de automatización](assets/automation-custom-button.png)

   El nuevo objeto se muestra en el campo conectado indicado en la configuración del botón de automatización.

   >[!NOTE]
   >
   >Se recomienda comprobar que el objeto se ha creado y conectado según lo esperado.

1. (Opcional) Haga clic en el nuevo objeto del campo conectado. Se abrirá la página del objeto y podrá realizar cambios adicionales en el nuevo objeto.

<!--you might need to add something about notifications and emails?!-->
