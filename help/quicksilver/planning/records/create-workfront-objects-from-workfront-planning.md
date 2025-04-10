---
title: Crear objetos de Workfront desde Workfront Planning
description: Puede crear tipos de objetos de Workfront a medida que los conecta desde otros registros en Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 88b8443525043a0710dfc6f93739e54f2e78a569
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 10%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Cree objetos de Workfront desde Workfront Planning a medida que los conecta a registros

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede crear objetos de Adobe Workfront desde Workfront Planning de las siguientes maneras:

* Al conectar objetos de Workfront desde registros de Planning

  En este artículo se describe cómo crear objetos de Workfront desde Workfront Planning a medida que se conectan desde registros de Planning.
* Cuando se utilizan automatizaciones desde la página de un registro.

  Para obtener información acerca de cómo crear objetos de Workfront mediante automatizaciones, vea [Crear objetos mediante automatizaciones de registros de Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Puede crear los siguientes tipos de objetos de Workfront desde Workfront Planning cuando conecte un registro de Workfront Planning con los siguientes tipos de objetos de Workfront:

* Proyectos
* Portafolios
* Programas

>[!IMPORTANT]
>
>* Solo puede crear proyectos, portafolios y programas en Workfront al conectarlos desde un registro.
>
>* No se pueden crear grupos o empresas al conectarlos desde un registro en Workfront Planning.
>

Puede conectar proyectos, portafolios y programas desde un campo de conexión en las siguientes áreas de Workfront Planning:

* La vista de tabla de un tipo de registro
* La página Detalles o el cuadro de vista previa de un registro
* La ficha Conexiones de un registro

Para obtener información acerca de cómo conectar registros de Planning con objetos de Workfront, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
   <p>Edite el acceso en Workfront para los tipos de objeto que desea crear (proyectos, programas y portafolios) a medida que conecta los registros a ellos. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Administre permisos en el área de trabajo <!--<span class="preview">and record type</span>--> donde desee agregar registros. </p>  
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

## Requisitos previos para crear objetos de Workfront al conectarlos con registros de Workfront Planning

Debe tener lo siguiente para poder agregar nuevos proyectos o portafolios conectándolos desde registros existentes:

* Tipos de registro conectados a proyectos, portafolios o programas de Workfront. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
* Registros. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
* El acceso y los permisos correctos en Workfront Planning y Workfront, tal como se describe en la sección [Requisitos de acceso](#access-requirements) de este artículo.

## Cree proyectos a medida que los conecte con registros de Workfront Planning

Para crear proyectos al conectarlos desde otros registros:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los proyectos de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

1. (Condicional) Haga clic en **Agregar proyecto**
O
Empiece a escribir el nombre de un proyecto y haga clic en **Agregar proyecto** si no lo encuentra.

   Si no encuentra un proyecto al intentar agregarlo desde el campo de registro conectado de otro registro, agregue un nombre y haga clic en **Agregar proyecto**. El botón Agregar va seguido del nombre del proyecto que ha escrito.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![Agregar proyecto al conectarlo desde un campo de conexión](assets/add-project-when-connecting-it-from-connection-field.png)

   Se abre el cuadro **Crear proyecto**.

1. (Opcional) Actualice **Nombre del proyecto**. De forma predeterminada, el nombre del proyecto se debe a lo que agregó como elemento de búsqueda al conectarlo desde el registro.
1. (Opcional) Seleccione una **plantilla de proyecto**. Si no selecciona ninguna plantilla, Workfront crea un proyecto en blanco sin tareas.
1. Haga clic en **Crear**.
1. (Condicional) Si seleccionó crear un proyecto a partir de una plantilla, siga los pasos del artículo [Crear un proyecto con una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) para finalizar la adición del proyecto.

   El nuevo proyecto se crea y se agrega al campo conectado del registro seleccionado.

1. (Opcional) Haga clic en el nombre del nuevo proyecto de Workfront Planning para abrir la página del proyecto en Workfront y realizar actualizaciones adicionales en el proyecto.

## Cree portafolios a medida que los conecta con registros de Workfront Planning

Para crear portafolios a medida que los conecta desde registros de Planning:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los portafolios de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. (Condicional) Haga clic en **Agregar portafolio**

   O

   Empiece a escribir el nombre de un portafolio y, a continuación, haga clic en **Agregar portafolio** si no lo encuentra.—> Si no encuentra un portafolio al intentar agregarlo desde el campo de registro conectado de otro registro, agregue un nombre y haga clic en **Agregar portafolio**. El botón Agregar también va seguido del nombre del portafolio que ha escrito.

   ![Agregar portafolio al conectarlo desde un campo de conexión](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   El portafolio se crea y se agrega al campo de conexión del registro seleccionado.

1. (Opcional) Haga clic en el nombre del nuevo portafolio de Workfront Planning para abrir la página del portafolio en Workfront y realizar actualizaciones adicionales en el portafolio.

## Cree programas a medida que los conecte con registros de Workfront Planning

Para crear programas a medida que los conecta desde registros de Planning:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los portafolios de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."-->

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

