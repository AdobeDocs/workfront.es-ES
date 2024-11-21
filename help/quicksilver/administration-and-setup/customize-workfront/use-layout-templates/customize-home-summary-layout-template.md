---
title: Personalización del panel de resumen mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puede usar una plantilla de diseño para configurar lo que ven los usuarios cuando hacen clic en una tarea o un problema en el resumen. Cada configuración que realice siguiendo los pasos siguientes afecta al panel Resumen. Estas personalizaciones no se aplican al panel Resumen del documento.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 8880891c0f5fd8fecad6c2f58136d36a943105ae
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 2%

---

# Personalización del panel Resumen mediante una plantilla de diseño

<!--Audited: 11/2024-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Puede usar una plantilla de diseño para configurar lo que los usuarios ven en el panel de resumen cuando hacen clic en una tarea o un problema. Cada configuración que realice siguiendo los pasos siguientes afecta al panel Resumen. Estas personalizaciones no se aplican al panel Resumen del documento.

Puede configurar lo siguiente:

* Qué campos se muestran para una tarea o un problema en el área de Detalles y en qué orden
* Si se muestran las actualizaciones, la hora registrada, los documentos adjuntos y las marcas de tiempo de una tarea o un problema seleccionados

También puede personalizar los campos que ven los usuarios en el área de Inicio cuando hacen clic en una aprobación de proyecto, aprobación de documento o aprobación de versión de documento asignada a ellos.

Para obtener información sobre el Panel de resumen, consulte [Resumen general](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, vea [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, vea [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Nuevo: estándar</p>
  <p> Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalización del panel Resumen mediante una plantilla de diseño

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Haga clic en la flecha abajo ![](assets/dropdown-arrow.png) bajo **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Panel de resumen**.

1. En la lista que aparece debajo, haga clic en el tipo de objeto para el que desea personalizar el Panel de resumen.

   La tabla siguiente explica lo que se puede personalizar para cada objeto

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tareas</td> 
      <td> <p>En una lista de tareas, esta configuración afecta al panel de resumen que aparece a la derecha de la página cuando un usuario selecciona una tarea y luego hace clic en el icono Abrir resumen <img src="assets/summary-panel-icon.png">.</p>

   <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemas</td> 
      <td><p>En una lista de problemas, esta configuración afecta al panel de resumen que se muestra en el lado derecho de la página cuando un usuario selecciona un problema y luego hace clic en el icono Abrir resumen <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proyectos</td> 
      <td><ul><li><p>En Inicio, cuando un usuario hace clic en una aprobación de proyecto asignada a él, su configuración para esta configuración afecta al área a la derecha de la aprobación.</p>
      <p><b>IMPORTANTE:</b> </p><p>Esta función está en desuso. Cualquier cambio que realice en esta área está relacionado con una función que Workfront ha eliminado. Esta opción se eliminará de Workfront con una actualización de mantenimiento posterior.</p></li>
      <li><span class="preview"><p>Esta área se ha eliminado del entorno de vista previa.</p></li></span></ul> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td>
     <ul><li><p>En Inicio, cuando un usuario hace clic en una aprobación de documento asignada a él, su configuración para esta configuración afecta al área a la derecha de la aprobación.</p>
      <p><b>IMPORTANTE:</b> </p><p> Esta función está en desuso. Cualquier cambio que realice en esta área está relacionado con una función que Workfront ha eliminado. Esta opción se eliminará de Workfront con una actualización de mantenimiento posterior.</p></li>
      <li><span class="preview"><p>Esta área se ha eliminado del entorno de vista previa.</p></li></span></ul>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versiones de documento</td> 
      <td><ul><li><p>En Inicio, cuando un usuario hace clic en una aprobación asignada a él para una versión concreta de un documento, la configuración de esta opción afecta al área a la derecha de la aprobación.</p>
      <p><p><b>IMPORTANTE:</b></p> Esta función está en desuso. Cualquier cambio que realice en esta área está relacionado con una función que Workfront ha eliminado. Esta opción se eliminará de Workfront con una actualización de mantenimiento posterior.</p></li>
      <li><span class="preview"><p>Esta área se ha eliminado del entorno de vista previa.</p></li></span></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Si una tarea no está asignada, el usuario asignado a la plantilla de diseño no verá las personalizaciones de campo en el Resumen.

1. (Condicional) Si hizo clic en Tareas o Problemas en el paso anterior, seleccione la categoría de tarea o problema que desee personalizar.

   <span class="preview">![](assets/choose-cat-cstmz-nwe-adobe-branding.png)</span>

1. (Condicional) Si aparece el menú desplegable **Establecer botón de acción principal** (si selecciona **Tareas** o **Problemas** en la lista de la izquierda), haga clic en la acción principal (**Listo** o **Estado**) que desee que esté disponible para los usuarios en el Panel de resumen cuando vean una tarea o un problema.

   <span class="preview">![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)</span>

1. Agregue ![](assets/add-item-plus-in-circle-blue.png) u oculte ![](assets/close-or-hide---x.png) campos para el tipo de objeto seleccionado.

   <span class="preview">![](assets/lt-home-add-hide-fields-adobe-branding.png)</span>

1. Repita los pasos del 3 al 6 para personalizar el Panel de resumen para cualquier otro tipo de objeto.
1. Haga clic en **Configuración global**, cerca de la esquina inferior izquierda, y luego habilite o deshabilite cualquiera de las siguientes opciones relacionadas con los objetos de Adobe Workfront en el Resumen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostrar actualizaciones de trabajo</td> 
      <td>Muestra las actualizaciones realizadas sobre una tarea o un problema seleccionados en el Panel de resumen. Esto incluye tanto las actualizaciones del sistema como las realizadas por un usuario. Los usuarios aún pueden filtrar las actualizaciones del sistema, tal como se describe en <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Habilitar o deshabilitar las actualizaciones del sistema</a> en <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabajo de actualización</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Registrar tiempo de trabajo</td> 
      <td>Muestra la opción Registrar tiempo de trabajo cuando se selecciona una tarea o un problema, lo que permite a los usuarios registrar el tiempo en los elementos de trabajo directamente desde las áreas Inicio y Resumen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver documentos asociados con el trabajo</td> 
      <td>Muestra un área Documentos en el Panel de resumen cuando se selecciona una tarea o un problema, donde se enumeran los documentos adjuntos a la tarea o al problema. Los usuarios pueden hacer clic en los documentos para verlos en una ventana de vista previa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar marca de tiempo</td> 
      <td>Oculta las marcas de tiempo de los siguientes campos de fecha en el Panel de resumen:
       <ul>
        <li>Fecha planificada de finalización</li>
        <li>Fecha de confirmación</li>
        <li>Fecha de envío</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

Para obtener más información acerca de las plantillas de diseño, vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
