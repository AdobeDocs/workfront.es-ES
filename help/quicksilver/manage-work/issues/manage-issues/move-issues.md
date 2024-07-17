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
source-wordcount: '881'
ht-degree: 1%

---

# Mover problemas

Puede mover problemas entre los siguientes objetos:

* De un proyecto a otro
* De una tarea a otra tarea del mismo proyecto o de otro proyecto
* De una tarea al proyecto o a otro proyecto
* De un proyecto a una tarea del mismo proyecto o a una tarea de otro proyecto

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Revise o aumente la licencia para mover problemas en la sección Problemas de un proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a Proyectos y tareas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas de su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acceso a los problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el problema</p> <p>Permisos de Contribute para el elemento al que está moviendo el problema con la capacidad de Agregar problemas.</p> <p> Para obtener información sobre la concesión de permisos a los problemas, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre cómo solicitar permisos adicionales, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Consideraciones sobre cómo mover problemas

Tenga en cuenta lo siguiente al mover problemas que contienen documentos o están asociados a una cola de solicitudes:

* **Cuando un problema está asociado con una cola de solicitudes:** Cuando mueve un problema a otro objeto y el problema está asociado con una cola de solicitudes, el problema movido ya no está asociado con la cola original desde la que se originó el primer problema.
* **Cuando se adjunta un documento al problema:** Cuando se mueve un problema a otro objeto y el problema tiene un documento adjunto, el documento, sus versiones y revisiones también se mueven al nuevo problema. Las aprobaciones asociadas con el documento no se mueven.
* **Cuando un problema está vinculado a un documento o a una carpeta:** Cuando mueve un problema que tiene documentos o carpetas vinculados a un servicio de terceros como Google Drive, los vínculos a los documentos se mueven con el problema.

## Mover problemas a una lista

Puede mover uno o varios problemas de una lista de problemas o de un informe de problemas.

1. Vaya al proyecto que contiene el problema o problemas que desea mover.

   O

   Vaya a un informe de problemas.

1. Si seleccionó ir a un proyecto, haga clic en **Problemas** en el panel izquierdo.
1. Seleccione el problema o problemas que desee mover, haga clic en el **menú Más** en la parte superior de la lista de problemas y luego haga clic en **Mover a**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continúe moviendo el problema, como se describe en la sección [Mover un solo problema](#move-a-single-issue) a partir del paso 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Mover un solo problema {#move-a-single-issue}

Puede mover un problema al verlo.

### Mover un solo problema en el entorno de vista previa

1. Vaya a un problema que desee copiar, haga clic en el menú **Más** ![](assets/more-icon.png)situado a la derecha del nombre del problema y, a continuación, seleccione **Mover** a.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   Se muestra el cuadro **Mover problema**.

   ![](assets/move-issue-box-nwe-350x280.png)

1. En la sección **Seleccionar proyecto de destino**, especifique el nombre del proyecto al que desea mover los problemas. El nombre del proyecto actual se muestra de forma predeterminada.

   >[!TIP]
   >
   >En la lista solo se muestran 100 proyectos.

1. (Condicional) Haga clic en **solicitar acceso** si no cuenta con acceso para mover problemas al proyecto.
1. (Condicional) Continúe moviendo el problema en el proyecto de destino seleccionado sin solicitar acceso si tiene acceso para agregar problemas a una de las tareas del proyecto de destino.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Se muestran mensajes similares si el proyecto seleccionado está en aprobación pendiente, completado o muerto, cuando el administrador de Workfront impide añadir problemas a estos proyectos. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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
      <td>Quita usuarios, roles o equipos asignados al problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>Elimina el porcentaje completado, si lo hay, del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documentos</p></td> 
      <td> <p>Quita todo lo que hay en la ficha de documentos, incluidas las versiones de los documentos, los documentos vinculados y las carpetas.

   <b>NOTA</b>

   Si decide que los documentos no se muevan con el problema, los documentos se eliminarán y se enviarán a la papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y se restaurarán en el problema movido.

   Si el problema se elimina después de moverlo, los documentos restaurados se colocarán en el área Documentos de la página del usuario del administrador que los restaura.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td>Elimina las entidades con las que se comparte el problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actualizaciones</td> 
      <td>Quita los comentarios de la sección Actualizaciones del problema.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Opcional) En la sección **Seleccionar tarea**, seleccione la tarea a la que desea mover el problema.
1. Haga clic en **Mover problema** o en **Mover problemas**, si ha seleccionado varios problemas en una lista.

   Los problemas movidos se agregan al proyecto especificado.




