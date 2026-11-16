---
title: Habilitar un Workspace de Workfront Planning en GenStudio for Performance Marketing
description: Puede hacer que un espacio de trabajo de Adobe Workfront Planning esté disponible en GenStudio for Performance Marketing cuando tenga acceso a ambas aplicaciones.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 5%
---
# Habilitar un espacio de trabajo de Workfront Planning en GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

Si su empresa también compra Adobe GenStudio for Performance Marketing y usted es cliente de Adobe Workfront Planning, el espacio de trabajo de GenStudio también está disponible en Workfront Planning.

Si ya tiene un espacio de trabajo de Planning en Workfront Planning, puede habilitarlo para GenStudio for Performance Marketing en lugar de volver a crear los mismos datos desde él en GenStudio.

Al habilitar un espacio de trabajo, se vincula a un proyecto de Adobe Cloud Storage y se asignan sus tipos de registros y campos al espacio de trabajo de GenStudio. Una vez completada la configuración, puede abrir los registros del espacio de trabajo en GenStudio.

Debe tener lo siguiente:

* Acceso a Workfront Planning y GenStudio for Performance Marketing.
* Un proyecto de Adobe Cloud Storage para vincular al espacio de trabajo. Un administrador de organización puede crear uno en Adobe Admin Console.

  Para obtener más información, consulte [Administrar almacenamiento de Adobe](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->

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
<p>Cualquier Workfront o flujo de trabajo y cualquier paquete de Planning</p> 
O
<p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p>

</td> 
   <tr> 
<td> 
   <p> Productos adicionales</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Configuración de Adobe Admin Console</p> </td> 
   <td> 
   <p> Debe crear proyectos de Adobe Storage Cloud en Adobe Admin Console </p>

<p>Para obtener más información, consulte <a href="https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies">Administrar proyectos</a>

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar de planificación</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Configuración del nivel de acceso de Adobe Workfront</p></td> 
   <td> <p>Debe agregar un flujo de trabajo y un tipo de licencia de Planning al nivel de acceso de Workfront cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Funciones de usuario de Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Cualquier función de usuario de GenStudio si necesita acceder a Campañas, Productos y Personas</li>
   <li>GenStudio System Manager si necesita acceder a las activaciones <!--and Events--></li></ul>
   Para obtener más información, consulte <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funciones de usuario y permisos</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  
   <p>En Workfront Planning: </p>
   <ul>
   <li><p>Administración de permisos en el espacio de trabajo <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>En Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> Crear permisos en Adobe GenStudio for Performance Marketing para crear elementos</p></li></ul>
   </td>  
</tbody> 
</table>

Para obtener información sobre el acceso a Adobe Workfront Planning, consulte [Información general sobre el acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Para obtener más información sobre Adobe GenStudio for Performance Marketing, consulte [Guía del usuario de Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/home).

+++ 

## Habilitar un espacio de trabajo de Workfront Planning en GenStudio

1. En Workfront Planning, abra el espacio de trabajo que desee habilitar.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del área de trabajo y, a continuación, haga clic en **Habilitar GenStudio**.

   El cuadro **Hacer que el espacio de trabajo GenStudio** esté habilitado se abre con los siguientes pasos:

   1. **Proyecto ACPC**: Seleccione el **Proyecto ACPC** (proyecto de Adobe Cloud Storage) que desea sincronizar con este espacio de trabajo y, a continuación, haga clic en **Siguiente**. Los usuarios acceden al espacio de trabajo en GenStudio a través de este proyecto.

      ![Habilitar GenStudio en el espacio de trabajo - Paso del proyecto ACPC](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Tipos de registros**: asigne los tipos de registros del área de trabajo a los seis tipos de registros que requiere GenStudio:

      * Campañas
      * Productos
      * Personas
      * Canales
      * Regiones
      * Activaciones

      Para cada uno, abra la lista y seleccione el tipo de registro de Planning correspondiente, o bien seleccione **Agregar nuevo** para crearlo y luego haga clic en **Siguiente**.

      ![Habilitar GenStudio en el espacio de trabajo - Paso de tipos de registro](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Campos**: Asigne los campos para cada tipo de registro. Utilice las pestañas de la parte superior del cuadro de diálogo para desplazarse entre los tipos de registro. Para cada campo, seleccione el campo Planning correspondiente o seleccione **Agregar nuevo** para crear un campo.

      Repita la configuración del campo para todos los tipos de registros.

      ![Habilitar GenStudio en el espacio de trabajo - Paso Campos](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Revise y corrija cualquier advertencia.

      Por ejemplo, un nuevo campo puede convertirse en el campo principal del tipo de registro o se cambia el nombre de un alias de campo que ya está en uso (si ya tiene un campo denominado &quot;Regiones&quot;, el importado puede convertirse en &quot;Regiones 2&quot;).

      Al asignar un campo **Status** se agregan las opciones necesarias.

   1. Haga clic en **Publicar**.

      Aparecerá un mensaje de confirmación cuando el espacio de trabajo esté activado. Los tipos de registros asignados se marcan en el espacio de trabajo.

      Los tipos de registro asignados para que sean accesibles desde GenStudio tienen un nuevo icono **Adobe** en sus tarjetas.

      ![Tipo de registro de campañas con icono de Adobe](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Abra GenStudio, seleccione **Campañas** y luego haga clic en el **proyecto ACPC** que configuró originalmente para esta configuración en la esquina inferior izquierda de la pantalla. Revise los campos y tipos de registro importados.

   >[!TIP]
   >
   >Solo verá los registros que permita la pertenencia al proyecto de Adobe Cloud Storage.
