---
product-area: projects
navigation-topic: manage-issues
title: Mover problemas
description: Puede mover problemas entre proyectos y tareas.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 89%

---

# Mover problemas

<!--Audited: 12/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Puede mover problemas entre los siguientes objetos:

* De un proyecto a otro
* De una tarea a otra tarea del mismo proyecto o de otro proyecto
* De una tarea al proyecto o a otro proyecto
* De un proyecto a una tarea del mismo proyecto o a una tarea de otro proyecto

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo:</p> 
   <ul><li>Colaborador o superior</li>
   <li>Ligero o superior para mover problemas en la sección Problemas de un proyecto</li></ul>
   <p>Actual:</p>
   <ul>
   <li><p>Solicitud o superior</p></li>
   <li><p>Revise o aumente la licencia para mover problemas en la sección Problemas de un proyecto.</p></li></ul>   
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a proyectos y tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para el problema</p> <p>Permisos de aportación para el elemento al que está moviendo el problema con la posibilidad de Añadir problemas.</td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre cómo mover problemas

Tenga en cuenta lo siguiente al mover problemas que contienen documentos o están asociados a una cola de solicitudes:

* El administrador del sistema o del grupo puede impedir que se muevan los problemas que tienen horas registradas, según la configuración de la preferencia Permitir a los usuarios mover tareas y problemas con horas registradas en el área Configuración. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* **Cuando un problema está asociado con una cola de solicitudes:** cuando mueve un problema a otro objeto y el problema está asociado con una cola de solicitudes, el problema movido ya no se asocia con la cola original desde la que se originó el primer problema.
* **Cuando se adjunta un documento al problema:** cuando se mueve un problema a otro objeto y el problema tiene un documento adjunto, el documento, sus versiones y revisiones también se mueven al nuevo problema. Las aprobaciones asociadas con el documento no se mueven.
* **Cuando un problema está vinculado a un documento o a una carpeta:** cuando mueve un problema que tiene documentos o carpetas vinculados a un servicio de terceros como Google Drive, los vínculos a los documentos se mueven con el problema.

## Desplazamiento de problemas a una lista

Puede mover uno o varios problemas de una lista de problemas o de un informe de problemas.

1. Vaya al proyecto que contiene el problema o problemas que desea mover.

   O

   Vaya a un informe de problema.

1. Si seleccionó ir a un proyecto, haga clic en **Problemas** en el panel izquierdo.
1. Seleccione el problema o problemas que desee mover, haga clic en el **menú Más** en la parte superior de la lista de problemas y luego haga clic en **Mover a**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continúe moviendo los problemas, tal como se describe en la sección [Mover un solo problema](#move-a-single-issue) a partir del paso 2.

## Desplazamiento de un solo problema {#move-a-single-issue}

Puede mover un problema al verlo.

### Desplazamiento de un solo problema

1. Vaya a un problema que desee mover, haga clic en el menú **Más** ![](assets/more-icon.png) que se encuentra a la derecha del nombre del problema y, a continuación, haga clic en **Mover a**.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   Se muestra el cuadro **Mover problema**.

   ![](assets/move-issue-box-nwe-350x280.png)

1. En la sección **Seleccionar proyecto de destino**, especifique el nombre del proyecto al que desea mover los problemas. El nombre del proyecto actual se muestra de forma predeterminada.

   >[!TIP]
   >
   >En la lista solo se muestran 100 proyectos.

1. (Condicional) Haga clic en **Solicitar acceso** si no cuenta con acceso para mover problemas al proyecto.
1. (Condicional) Continúe moviendo el problema en el proyecto de destino seleccionado sin solicitar acceso si tiene acceso para añadir problemas a una de las tareas del proyecto de destino.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Se muestran mensajes similares si el proyecto seleccionado está pendiente de aprobación, completado o inactivo, cuando el administrador de Workfront impide añadir problemas a estos proyectos. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) En la sección **Opciones**, anule la selección de cualquiera de los elementos enumerados en la tabla siguiente para eliminarlos del problema que se movió. Todas las opciones están seleccionadas de forma predeterminada.

   >[!IMPORTANT]
   >
   >Si se anula la selección de elementos en la lista Opciones, se pierden datos. La información del problema existente se eliminará y no se podrá recuperar.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td>Anule la selección de esta opción para eliminar toda la información del problema al moverlo a su nueva ubicación. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td>Elimina los usuarios, funciones o equipos asignados al problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>Elimina el porcentaje completado, si lo hay, del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documentos</p></td> 
      <td> <p>Elimina todo lo que hay en la pestaña de documentos, incluidas las versiones de los documentos, los documentos vinculados y las carpetas.

   <b>NOTA</b>

   Si decide que los documentos no se muevan con el problema, los documentos se eliminarán y se enviarán a la papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y se restaurarán en el problema movido.

   Si el problema se elimina después de haberlo movido, los documentos restaurados se colocarán en el área Documentos de la página del usuario del administrador que los restaura.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td>Elimina las entidades con las que se comparte el problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actualizaciones</td> 
      <td>Elimina los comentarios de la sección Actualizaciones del problema.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Opcional) En la sección **Seleccionar tarea**, seleccione la tarea a la que desea mover el problema.
1. Haga clic en **Mover problema** o en **Mover problemas**, si ha seleccionado varios problemas en una lista.

   Los problemas movidos se añaden al proyecto especificado.




