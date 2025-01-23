---
title: Crear objetos de Workfront desde Workfront Planning
description: Puede crear tipos de objetos de Workfront a medida que los conecta desde otros registros en Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 9db8ea3f26dd7e8b4c8aa52fb9902832db7a6a5c
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 11%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Creación de objetos de Workfront desde Workfront Planning

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede crear los siguientes tipos de objetos de Workfront desde Workfront Planning:

* Proyectos
* Portafolios

Puede crear proyectos y portafolios de Workfront desde Workfront Planning cuando conecte un registro de Workfront Planning con un proyecto o portafolio.

>[!IMPORTANT]
>
>* Solo puede crear proyectos y portafolios en Workfront al conectarlos desde un registro.
>
>* No se pueden crear programas, grupos ni compañías al conectarlos desde un registro en Workfront Planning.
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

Para obtener información acerca de cómo conectar registros de Planning con objetos de Workfront, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

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
   <p>Editar el acceso en Workfront para los tipos de objeto que desea crear (proyectos y portafolios) al conectar los registros a ellos. </p>  
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

## Requisitos previos para crear objetos de Workfront al conectarlos con registros de Workfront Planning

Debe tener lo siguiente para poder agregar nuevos proyectos o portafolios conectándolos desde registros existentes:

* Tipos de registro conectados a proyectos o portafolios de Workfront. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
* Registros. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
* El acceso y los permisos correctos en Workfront Planning y Workfront, tal como se describe en la sección [Requisitos de acceso](#access-requirements) de este artículo.

## Crear proyectos al conectarlos con registros de Workfront Planning

Para crear proyectos al conectarlos desde otros registros:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los proyectos de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   Puede conectar proyectos desde un campo de conexión en las siguientes áreas de Workfront Planning:

   * La vista de tabla de un tipo de registro
   * Página de detalles o cuadro de vista previa de un registro

1. (Condicional) Si no encuentra un proyecto al intentar agregarlo desde el campo de registro conectado de otro registro, agregue un nombre y, a continuación, haga clic en **+ Agregar**. El botón **+ Agregar** va seguido del nombre del tipo de objeto al que se está conectando. Por ejemplo, &quot;Agregar proyecto&quot;, al agregar un nuevo proyecto a una campaña existente. El botón Agregar también va seguido del nombre del proyecto que ha escrito.

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">Se abre el cuadro **Crear proyecto**.</span>

1. <span class="preview">(Opcional) Actualice **nombre del proyecto**. De forma predeterminada, el nombre del proyecto se debe a lo que agregó como elemento de búsqueda al conectarlo desde el registro. </span>
1. <span class="preview">(Opcional) Seleccione una **plantilla de proyecto**. Si no selecciona ninguna plantilla, Workfront crea un proyecto en blanco sin tareas. </span>
1. <span class="preview">Haga Clic En **Crear**. </span>
1. <span class="preview">(Condicional) Si seleccionó crear un proyecto a partir de una plantilla, siga los pasos del artículo [Crear un proyecto con una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) para finalizar la adición del proyecto.</span>

   El nuevo proyecto se crea y se agrega al campo conectado del registro seleccionado.

1. (Opcional) Haga clic en el nombre del nuevo proyecto de Workfront Planning para abrir la página del proyecto en Workfront y realizar actualizaciones adicionales en el proyecto.

## Cree portafolios al conectarlos con registros de Workfront Planning

Para crear portafolios al conectarlos desde otros registros:

1. Vaya a la página de detalles de un registro o a la tabla del tipo de registro y comience a conectar los registros de Workfront Planning con los portafolios de Workfront, tal como se describe en el artículo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   Puede conectar portafolios desde un campo de conexión en las siguientes áreas de Workfront Planning:

   * La vista de tabla de un tipo de registro
   * Página de detalles o cuadro de vista previa de un registro

1. (Condicional) Si no encuentra un portafolio al intentar agregarlo desde el campo de registro conectado de otro registro, agregue un nombre y, a continuación, haga clic en **+ Agregar**. El botón **+ Agregar** va seguido del nombre del tipo de objeto al que se está conectando. Por ejemplo, &quot;Agregar portafolio&quot;, al agregar un nuevo portafolio a una campaña existente. El botón Agregar también va seguido del nombre del portafolio que ha escrito.

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   El portafolio se crea y se agrega al campo de conexión del registro seleccionado.

1. (Opcional) Haga clic en el nombre del nuevo portafolio de Workfront Planning para abrir la página del portafolio en Workfront y realizar actualizaciones adicionales en el portafolio.
