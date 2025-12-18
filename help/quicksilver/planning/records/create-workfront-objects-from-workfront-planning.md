---
title: Cree objetos de Workfront desde Workfront Planning a medida que los conecta a registros
description: Puede crear tipos de objetos de Workfront a medida que los conecta desde otros registros en Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 57592455c61f0ddd14f6d2bcc033b58a8cdc7028
workflow-type: tm+mt
source-wordcount: '1267'
ht-degree: 5%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Cree objetos de Workfront desde Workfront Planning a medida que los conecta a registros

<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede crear objetos de Adobe Workfront desde Workfront Planning de las siguientes maneras:

* Al conectar objetos de Workfront desde registros de Planning

  En este artículo se describe cómo crear objetos de Workfront desde Workfront Planning a medida que se conectan desde registros de Planning.
* Cuando se utilizan automatizaciones desde la página de un registro.

  Para obtener información acerca de cómo crear objetos de Workfront mediante automatizaciones, vea [Crear objetos mediante automatizaciones de registros de Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

>[!IMPORTANT]
>
>Puede crear los siguientes objetos de Workfront desde Workfront Planning cuando los conecte con registros de Planning:
>
>* Proyectos
>* Portafolios
>* Programas
>
>Puede conectar los siguientes objetos de Workfront con registros de Planning, pero no puede crearlos en el proceso de conexión:
>
>* Grupos
>* Compañías
>

Tenga en cuenta lo siguiente al conectar y crear objetos de Workfront con registros de Workfront Planning:

* Puede conectar proyectos, portafolios, programas, grupos y empresas de Workfront desde un campo de conexión desde las siguientes áreas de Workfront Planning:

   * La vista de tabla de un tipo de registro
   * La página Detalles o el cuadro de vista previa de un registro
   * La ficha Conexiones de un registro

* Puede crear proyectos desde las siguientes áreas de Workfront Planning:

   * La vista de tabla de un tipo de registro
   * El área Detalles de un registro en el campo de conexión
   * La página Registro conectado de un registro

* Puede crear portafolios y programas desde las siguientes áreas de Workfront Planning:

   * La vista de tabla de un tipo de registro
   * El área Detalles de un registro en el campo de conexión

Para obtener información acerca de cómo conectar registros de Planning con objetos de Workfront, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p> <p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td>

<tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p> 
   <p>Acceso de edición con acceso a Crear objetos en Workfront para los tipos de objeto que desea crear (proyectos, portafolios, programas). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Conceda permisos de contribución o superiores al espacio de trabajo y tipo de registro donde desee agregar registros. </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   <p>Administre permisos a objetos Workfront (portafolios) para agregar objetos secundarios (proyectos).</p>
   </td> 
  </tr>   
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
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
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  -->


## Requisitos previos para crear objetos de Workfront al conectarlos con registros de Workfront Planning

Debe tener lo siguiente para poder agregar nuevos proyectos o portafolios conectándolos desde registros existentes:

* Tipos de registro conectados a proyectos, portafolios o programas de Workfront. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
* Registros para los tipos de registros conectados a objetos de Workfront. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
* El acceso y los permisos correctos en Workfront Planning y Workfront, tal como se describe en la sección [Requisitos de acceso](#access-requirements) de este artículo.

## Cree proyectos a medida que los conecte con registros de Workfront Planning

Puede crear proyectos a medida que los conecta con registros en Workfront Planning en las siguientes áreas de Workfront Planning:

* La vista de tabla de un tipo de registro o el área Detalles de un registro en el campo de conexión
* La página Registro conectado de un registro, en el área Detalles de un registro

### Crear proyectos desde el área Detalles de un registro o desde la vista de tabla de un tipo de registro

Para crear proyectos al conectarlos desde otros registros:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los proyectos de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

1. (Condicional) Haga clic en **Agregar proyecto**
O
Empiece a escribir el nombre de un proyecto y haga clic en **Agregar proyecto** si no lo encuentra. El botón Agregar va seguido del nombre del proyecto que ha escrito.

   ![Agregar proyecto al conectarlo desde un campo de conexión](assets/add-project-when-connecting-it-from-connection-field.png)

   Se abre el cuadro **Crear proyecto**.

1. (Opcional) Actualice **Nombre del proyecto**. De forma predeterminada, el nombre del proyecto se debe a lo que agregó como elemento de búsqueda al conectarlo desde el registro.
1. (Opcional) Seleccione una **plantilla de proyecto**. Si no selecciona ninguna plantilla, Workfront crea un proyecto en blanco sin tareas.
1. Haga clic en **Crear**.
1. (Condicional) Si seleccionó crear un proyecto a partir de una plantilla, siga los pasos del artículo [Crear un proyecto con una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) para finalizar la adición del proyecto.

   El nuevo proyecto se crea y se agrega al campo conectado del registro seleccionado.

1. (Opcional) Haga clic en el nombre del nuevo proyecto de Workfront Planning para abrir la página del proyecto en Workfront y realizar actualizaciones adicionales en el proyecto.

### Crear proyectos desde la página Registros conectados de un registro

1. Conecte el tipo de objeto Project con un tipo de registro de Workfront Planning en la vista de tabla.

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Haga clic en el nombre de un registro en cualquier vista. Se abrirá el cuadro de vista previa de detalles.

1. Agregue una **página Registros conectados** para los proyectos.

   Para obtener más información, consulte la sección &quot;Agregar una página de registros conectados a un registro&quot; en el artículo [Administrar el diseño de la página del registro](/help/quicksilver/planning/records/manage-the-record-page.md).

   La página Registros conectados se muestra en la vista de tabla. Los proyectos conectados se muestran en la tabla.

   ![Vista de tabla de proyectos en la página de registros conectados](assets/projects-connected-records-page-table.png)

1. Haga clic en **Nueva fila** en la tabla de proyectos para agregar un proyecto.

   Solo puede agregar un proyecto en blanco en esta área. No se puede agregar un proyecto mediante una plantilla.
1. (Opcional) Haga clic en el nombre del proyecto en la vista de tabla para abrir el proyecto en Workfront y agregar más información.

## Cree portafolios a medida que los conecta con registros de Workfront Planning

Puede crear portafolios desde la vista de tabla de un tipo de registro o desde la página Detalles de un registro.

Para crear portafolios a medida que los conecta desde registros de Planning:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los portafolios de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

1. (Condicional) Haga clic en **Agregar portafolio**

   O

   Empiece a escribir el nombre de un portafolio y, a continuación, haga clic en **Agregar portafolio** si no lo encuentra. El botón Agregar va seguido del nombre del portafolio que ha escrito.

   ![Agregar portafolio al conectarlo desde un campo de conexión](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   El portafolio se crea y se agrega al campo de conexión del registro seleccionado.

1. (Opcional) Haga clic en el nombre del nuevo portafolio de Workfront Planning para abrir la página del portafolio en Workfront y realizar actualizaciones adicionales en el portafolio.

## Cree programas a medida que los conecte con registros de Workfront Planning

Puede crear programas desde la vista de tabla de un tipo de registro o desde la página Detalles de un registro.

Para crear programas a medida que los conecta desde registros de Planning:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los portafolios de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

1. Haga clic en **Agregar programa**

   O

   Empiece a escribir el nombre de un programa y, a continuación, haga clic en **Agregar programa** si no lo encuentra. El botón Agregar va seguido del nombre del programa que ha escrito.

   ![Agregar programa de Workfront al conectarlo desde el campo de conexión](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   Se abre la casilla **Crear programa**.

1. Actualice **Nombre de programa**. Este campo es obligatorio.
1. Elija un **Portfolio** en la lista desplegable o empiece a escribir el nombre de un portafolio y, a continuación, selecciónelo cuando se muestre en la lista. Este campo es obligatorio.
1. Haga clic en **Crear**.

   El programa se crea y se agrega al campo de conexión del registro seleccionado.

1. (Opcional) Haga clic en el nombre del nuevo programa de Workfront Planning para abrir la página del programa en Workfront y realizar actualizaciones adicionales.

