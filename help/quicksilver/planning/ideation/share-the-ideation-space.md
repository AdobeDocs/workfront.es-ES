---
title: Compartir un espacio de ideas con otros usuarios
description: Adobe Workfront Planning ahora ofrece una capacidad adicional para idear antes de iniciar sus campañas. Aproveche el poder de la IA para crear y colaborar en ideas con otros antes de que se conviertan en registros de planificación.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 6%

---


# Compartir un espacio de ideación con otros usuarios

<!--add to TOC and miniTOC-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible como parte del programa **Beta** del espacio de ideación. </span>

<span class="preview">Para obtener más información, consulte [Introducción al espacio de ideación para Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

<!--ome of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article-->

Los permisos de registros de Workfront Planning se transfieren al espacio de ideación de un registro.

Además, puede conceder a otros usuarios permisos para utilizar el espacio de ideación y agregarle ideas.

Tenga en cuenta lo siguiente:

* Los creadores de ideaciones siempre tienen permisos de edición en sus propias ideaciones.

* Debe tener permisos de editor en un espacio de ideación para crear informes y exportarlos a otras aplicaciones.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
<ul> 
<li><p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p></li>
O
<li><p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Productos adicionales</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workflow</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> 
   <ul>
   <li><p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   </li>
   <li><p>La configuración Deshabilitar espacio de ideación en su nivel de acceso debe estar deseleccionada</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Permisos de contribución o superiores al espacio de trabajo y tipo de registro donde desee agregar registros </p>
      <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
      <p>Ver permisos de objetos de Workfront para agregarlos a informes <!--not sure if this is available--></p>
      <p>Permisos de editor en el espacio de ideación para crear informes</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Funciones de usuario de Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Cualquier función de usuario de GenStudio para acceder a campañas, productos y personas</li>
   <li>GenStudio System Manager para acceder a las activaciones <!--and Events--></li></ul>
   Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funciones de usuario y permisos</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Compartir un espacio de ideación

1. Acceda al espacio de ideación de un registro de Planning.

   Para obtener más información, consulte uno de los siguientes artículos:

   * [Creación de registros de Planning a partir de informes del espacio de ideación](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
   * [Creación de informes en el espacio de ideación](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. Haga clic en **Compartir** en la esquina superior derecha y, a continuación, haga clic en el icono de **Configuración** ![Icono de configuración](assets/setting-icon.png) en la esquina superior derecha del cuadro **Compartir documento**.
1. En la lista Quién tiene acceso, elija una de las siguientes opciones:

   * **Solo las personas invitadas pueden tener acceso**

     Debe agregar usuarios individuales al espacio de ideación y darles un nivel de permiso.
   * **Todos los usuarios de &lt; entorno de Workfront de su compañía > pueden realizar comentarios**

     Todas las personas de la organización que tengan un flujo de trabajo y una licencia de Planning en su nivel de acceso pueden encontrar la idea y realizar comentarios al respecto.
   * **Cualquier persona que tenga el vínculo puede hacer comentarios**

     Cualquier persona que comparta un vínculo a la idea puede realizar comentarios sobre él, incluidas las personas externas a la organización.

1. Haga clic en **Copiar vínculo** para generar un vínculo a la idea y compartirlo con otros usuarios. El vínculo se añadirá al portapapeles.
1. Haga clic en la flecha hacia atrás del cuadro Configuración para volver al uso compartido.
1. (Condicional) Si ha seleccionado compartir el espacio de ideas con personas específicas, empiece a escribir su nombre o dirección de correo electrónico y, a continuación, seleccione uno de los siguientes niveles de permisos:

   | Permiso del espacio de ideación | Competencias |
   |---|---|
   | **Editor** | Puede editar, descargar y compartir el espacio de ideación |
   | **Comentarista** | Puede ver el espacio de ideación y realizar comentarios en él |
   | **Visor** | Puede ver el espacio de ideación |

1. (Opcional) Incluya un mensaje con su asignación y luego haga clic en **Invitar**.

   Los usuarios invitados reciben una notificación por correo electrónico sobre su asignación de permisos.

1. Haga clic en el icono **X** para cerrar el cuadro **Compartir documento**.











