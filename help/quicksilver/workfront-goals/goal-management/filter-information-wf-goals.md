---
product-previous: workfront-goals
navigation-topic: goal-management
title: Filtrar información en Adobe Workfront Goals
description: Puede ver las metas que usted o cualquier otro usuario haya añadido en Adobe Workfront Goals. Para obtener información sobre la creación de metas, consulte Crear metas en Adobe Workfront Goals. Cuando visualice las metas, puede filtrar la información en Workfront Goals para ver solo las metas que sean importantes para usted.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 88%

---

# Filtrar información en Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Puede ver las metas que usted o cualquier otro usuario haya añadido en Adobe Workfront Goals. Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md). Cuando visualice las metas, puede filtrar la información en Workfront Goals para ver solo las metas que sean importantes para usted.

## Requisitos de acceso

>[!NOTE]
>
>Su empresa puede optar por seguir utilizando los objetivos de Adobe Workfront si compró este paquete anteriormente. Debe hablar con el representante de su cuenta para obtener más detalles.
>
>Adobe Workfront Goals ya no se puede adquirir.

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>paquete de Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront</td>
 <td>
 <p>Colaborador o superior</p>
<p>Solicitud o superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuración de nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Ver o permisos superiores a los objetivos para verlos</p>
  <p>Administrar permisos para los objetivos y editarlos</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores del sistema, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
  <p>Or</p>
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Información general sobre los filtros en Workfront Goals

>[!NOTE]
>
>Para encontrar y centrarse de forma eficaz en las metas correctas, le recomendamos que utilice filtros en Workfront Goals.  Estos le permiten mostrar la información correcta antes de empezar a administrar las metas que son importantes para usted. De forma predeterminada, Workfront Goals muestra todas las metas del sistema.

Puede buscar y filtrar por metas en las siguientes secciones del área Metas en Workfront:

* Lista de metas
* Gráficos
* Alineación de metas

Para obtener información acerca de las secciones del área Metas, consulte [Información general sobre las secciones de Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>Puede configurar filtros para una sección y que se mantengan al pasar a otra sección de Workfront Goals.

Tenga en cuenta lo siguiente al trabajar con filtros en Workfront Goals:

* Puede crear y aplicar un filtro sin guardarlo, o bien puede guardar un filtro para reutilizarlo más adelante.

  Se dan los siguientes escenarios:

   * Al guardar un filtro, este se convierte en el filtro predeterminado cada vez que inicia sesión en Workfront Goals.
   * Cuando aplique un filtro sin guardarlo, puede volver a las listas originales al actualizar la página.

* Solo puede ver y aplicar los filtros que ha creado. Los filtros creados por otros usuarios solo se muestran para esos usuarios.
* No puede compartir filtros que haya creado con otros usuarios.

## Aplicación de un filtro rápido en Workfront Goals

Puede utilizar un filtro rápido en una lista de metas para que le ayude a localizar únicamente los elementos que son importantes para usted. Los filtros rápidos no se pueden guardar ni son persistentes. Workfront borra los resultados de un filtro rápido al actualizar la página.

Para obtener más información, consulte [Aplicar el filtro rápido a una lista](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Creación y aplicación de un filtro en Workfront Goals

El proceso de creación de filtros es el mismo para cualquier sección de Workfront Goals.

Puede crear un filtro desde cero o editar uno de los filtros integrados.

1. Vaya a Workfront Goals.

   Para obtener información sobre cómo acceder a Workfront Goals, consulte [Acceso y apertura de metas en Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   De forma predeterminada, se muestra la sección Lista de metas.

1. Haga clic en **Filtro** en la esquina superior derecha de la lista.

   ![Icono de filtro](assets/filter-icon-and-label.png)

   De manera predeterminada, Workfront aplica el filtro **Todos** que muestra todas las metas del sistema.

   >[!TIP]
   >
   >No se puede editar ni eliminar el filtro Todos.

1. Realice una de las siguientes acciones:

   * Haga clic en cualquiera de los siguientes filtros predefinidos para mostrar las metas solo para los siguientes propietarios:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>Todas</td> 
        <td> <p>Todas las metas del sistema, independientemente de quién los haya creado, cuál sea su periodo de vigencia o quién sea su propietario. Este es el filtro predeterminado y no se puede editar. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Personal</td> 
        <td>Las metas de las que es propietario.</td> 
       </tr> 
       <tr> 
        <td>Mis equipos</td> 
        <td> <p>Las metas para las que cualquiera de sus equipos está seleccionado como propietario. </p> <p><b>Sugerencia</b>

     No se muestran metas cuando no se le ha asignado ningún equipo. </p> </td>
     </tr> 
       <tr> 
        <td>Mis grupos</td> 
        <td>Las metas para las que cualquiera de sus grupos está seleccionado como propietario. </td> 
       </tr> 
       <tr> 
        <td>Compañía</td> 
        <td> <p>Las metas asociadas con su organización. </p> <p><b>SUGERENCIA</b>
        <p>En Adobe Workfront Goals, el filtro Compañía muestra las metas para las que su organización está seleccionada como propietaria. </p> <p>No puede buscar compañías utilizando este campo. De forma predeterminada, solo está seleccionada la organización que es la propietaria de la instancia de Workfront. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Pase el ratón sobre el nombre de un filtro, luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) junto a su nombre para personalizarlo y agregar nombres específicos de usuarios, equipos, grupos o el nombre de su organización, y después selecciónelo cuando aparezca en la lista.

   * Haga clic en **Nuevo filtro** para crear un nuevo filtro y, a continuación, seleccione entre las siguientes opciones para personalizar el nuevo filtro:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Periodo</td> 
        <td>Seleccione un período de tiempo en el menú desplegable. Puede seleccionar varios períodos de tiempo. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Estado</td> 
        <td> <p>Seleccione un estado en el menú desplegable de las siguientes opciones:</p> 
         <ul> 
          <li> <p>Activo</p> </li> 
          <li> <p>Borrador</p> </li> 
          <li> <p>Inactivo</p> </li> 
          <li> <p>Cerrado</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Progreso</td> 
        <td> <p>Seleccione un progreso en el menú desplegable de las siguientes opciones: </p> 
         <ul> 
          <li> <p>Con problemas</p> </li> 
          <li> <p>En riesgo</p> </li> 
          <li> <p>Bien encaminado</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Propietario</td> 
        <td> <p>Empiece a escribir el nombre de un propietario y, a continuación, selecciónelo cuando aparezca en la lista. </p> <p>Puede escribir los nombres de los usuarios, equipos, grupos o el nombre de su organización, o bien puede seleccionar entre las opciones predefinidas. </p> <p>Las siguientes opciones de filtro predefinidas siempre hacen referencia al usuario que ha iniciado sesión actualmente: </p> 
         <ul> 
          <li> <p><strong>Yo</strong>: muestra las metas de las que usted es propietario.</p> </li> 
          <li> <p><strong>Mi equipo local</strong> y <strong>Todos mis equipos</strong>: muestra las metas en las que su equipo local o cualquiera de sus equipos han sido designados como propietarios. </p> <p>Sugerencia: No se muestran metas cuando no se le ha asignado ningún equipo. </p> </li> 
          <li> <p><strong>Mi grupo de inicio</strong> y <strong>Todos mis grupos</strong>: muestra las metas en las que su grupo de inicio o cualquiera de sus grupos están designados como propietarios.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Opcional) Haga clic en **Restablecer** en la esquina inferior derecha del cuadro de filtro para borrar todos los campos que ha seleccionado y empiece a crear el filtro desde cero.
1. (Opcional) Haga clic en **Aplicar** para aplicar el filtro sin guardarlo.

   El filtro se muestra en el área **Sin guardar** del generador de filtros como **Nuevo filtro**.

   No se puede cambiar el nombre de un filtro sin guardar.

   Los filtros que no se hayan guardado se eliminarán del área Metas la próxima vez que cierre la sesión de Workfront y vuelva a iniciarla.

   >[!TIP]
   >
   >Solo se puede tener un nuevo filtro sin guardar a la vez.

1. Haga clic en **Guardar** para guardar el filtro y utilizarlo más adelante, luego agregue un nombre para el filtro en el campo **Agregar nombre de filtro** y haga clic en **Listo**.

   Esto guardará el filtro en la sección **Guardado** del generador de filtros. Este filtro se podrá utilizar en el futuro.

   El último filtro guardado y aplicado se muestra de forma predeterminada la próxima vez que se vuelve a iniciar sesión en Workfront

1. (Opcional) Haga clic en la **flecha hacia la izquierda** junto a **Nuevo filtro** para salir del generador de filtros y volver a la lista de filtros.
1. (Opcional) Pase el puntero por encima de un filtro personalizado, haga clic en el menú **Más**, a continuación, haga clic en **Eliminar** y luego en **Eliminar**. Esto elimina el filtro y no se puede recuperar.

   >[!TIP]
   >
   >No puede eliminar ninguno de los filtros predefinidos.

1. Haga clic en el **icono X** en la esquina superior derecha del generador de filtros para cerrarlo.

   El nombre del filtro aplicado actualmente se muestra a la derecha del icono Filtro, en la esquina superior derecha de la lista de metas.

   La lista de metas se filtra según los criterios de filtro.

1. (Opcional y condicional) Cuando visualice las metas en la sección Alineación de metas, haga clic en **Muéstrelas** si desea ver las metas filtradas.

   ![Mostrarles el vínculo de los elementos filtrados](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   El nombre del filtro aparece resaltado en amarillo para indicar que se está ignorando.

   ![Filtrar contorno amarillo](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Opcional y condicional) Haga clic en **Volver a aplicar el filtro** para aplicar el filtro y omitir los elementos mostrados en el paso anterior.


