---
product-area: projects
navigation-topic: manage-issues
title: Mover problemas
description: Puede mover problemas entre proyectos y tareas.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# Mover problemas

Puede mover problemas entre los siguientes objetos:

* De un proyecto a otro
* De una tarea a otra tarea en el mismo proyecto o en otro proyecto
* De una tarea al proyecto o a otro proyecto
* De un proyecto a una tarea del mismo proyecto o a una tarea de otro proyecto

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Revise o obtenga una licencia superior para mover problemas en la sección Problemas de un proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Ver o acceder más a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas en el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concesión de acceso a problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el problema</p> <p>Permisos de Contribute para el elemento en el que está moviendo el problema con la capacidad de agregar problemas.</p> <p> Para obtener información sobre la concesión de permisos a problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre la solicitud de permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre problemas de movimiento

Tenga en cuenta lo siguiente cuando mueva problemas que contengan documentos o que estén asociados a una cola de solicitudes:

* **Cuando un problema está asociado con una cola de solicitudes:** Cuando se mueve un problema a otro objeto y el problema está asociado con una cola de solicitudes, el problema movido ya no está asociado con la cola original desde la que se originó el primer problema.
* **Cuando se adjunta un documento al problema:** Cuando se mueve un problema a otro objeto y el problema tiene un documento adjunto, el documento, sus versiones y pruebas también pasan al nuevo problema. Las aprobaciones asociadas al documento no se mueven.
* **Cuando un problema está vinculado a un documento o a una carpeta:** Cuando se mueve un problema que tiene documentos o carpetas vinculados a un servicio de terceros como Google Drive, los vínculos a los documentos se mueven con el problema.

## Mover problemas en una lista

Puede mover uno o varios problemas de una lista de problemas o de un informe de problemas.

1. Vaya al proyecto que contenga el problema o los problemas que desee mover.

   O

   Vaya a un informe de problemas.

1. Si seleccionó ir a un proyecto, haga clic en **Problemas** en el panel izquierdo.
1. Seleccione el problema o los problemas que desea mover y haga clic en el botón **Más menú** en la parte superior de la lista de problemas, haga clic en **Mover a**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continúe moviendo el problema, tal como se describe en la sección [Mover un solo problema](#move-a-single-issue) a partir del paso 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Mover un solo problema {#move-a-single-issue}

Puede mover un problema al verlo.

### Mover un solo problema en el entorno de vista previa

1. Vaya a un problema que desee copiar y haga clic en el botón **Más** menú ![](assets/more-icon.png)a la derecha del nombre del problema y, a continuación, seleccione **Mover** a.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   La variable **Mover problema** se muestra.

   ![](assets/move-issue-box-nwe-350x280.png)

1. En el **Seleccionar proyecto de destino** , especifique el nombre del proyecto al que desea mover los problemas. El nombre del proyecto actual se muestra de forma predeterminada.

   >[!TIP]
   >
   >En la lista solo se muestran 100 proyectos.

1. (Condicional) Haga clic en **acceso de solicitud** si no tiene acceso para mover problemas al proyecto.
1. (Condicional) Continúe moviendo el problema en el proyecto de destino seleccionado sin solicitar acceso si tiene acceso para agregar problemas a una de las tareas del proyecto de destino.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Se muestran mensajes similares si el proyecto seleccionado está pendiente de aprobación, completado o muerto, cuando el administrador de Workfront evita agregar problemas a estos proyectos. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) En la **Opciones** , desmarque cualquiera de los elementos enumerados en la tabla siguiente para eliminarlos del problema que se ha movido. Todas las opciones están seleccionadas de forma predeterminada.

   >[!IMPORTANT]
   >
   >Al anular la selección de elementos en la lista Opciones, se pierden datos. La información del problema existente se eliminará y no se podrá recuperar.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td>Anule la selección de esta opción para eliminar toda la información del problema al moverla a su nueva ubicación. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td>Elimina los usuarios, las funciones de trabajo o los equipos que están asignados al problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>Elimina el porcentaje completado, si lo hay, del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documentos</p></td> 
      <td> <p>Quita todo lo que aparece en la ficha documentos, incluidas las versiones de documentos, los documentos vinculados y las carpetas.

   <b>NOTA</b>

   Si opta por no mover los documentos con el problema, los documentos se eliminarán y se colocarán en la Papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y restaurarlos en el problema movido.

   Si el problema se elimina después de moverlo, los documentos restaurados se colocarán en el área Documentos de la página de usuario del administrador que los restaura.
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


1. (Opcional) En la **Seleccionar tarea** , seleccione la tarea a la que desea mover el problema.
1. Haga clic en **Mover problema** o **Mover problemas**, si ha seleccionado varios problemas en una lista.

   Los problemas movidos se añaden al proyecto especificado.




