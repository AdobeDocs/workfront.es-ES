---
title: Personalización de la terminología de la interfaz de usuario mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para cambiar las etiquetas de algunos objetos que aparecen en Workfront y que coincidan con los términos utilizados en su organización.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 2%

---

# Personalización de la terminología de la interfaz de usuario mediante una plantilla de diseño

Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para cambiar las etiquetas de algunos objetos que aparecen en Workfront y que coincidan con los términos utilizados en su organización.

Después de guardar una plantilla de diseño en la que ha cambiado la terminología, cerrar la sesión de Workfront y volver a iniciarla, las etiquetas que ha cambiado aparecen donde aparecerían las etiquetas predeterminadas en la mayoría de las áreas de Workfront:

* Menú principal
* Todas las áreas accesibles desde el menú principal
* Todas las pestañas
* Todos los menús
* Report Builder y elementos de informes (vistas, filtros y agrupaciones)
* Botones Guardar
* Archivos exportados
* Correos electrónicos
* Aplicaciones móviles

>[!NOTE]
>
>* El área Complemento de Outlook no muestra las etiquetas personalizadas.
>* Puede encontrar problemas gramaticales y de otro tipo al personalizar las etiquetas. Por ejemplo, si cambia &quot;Problema&quot; a &quot;Solicitud&quot;, puede haber lugares en la interfaz de usuario donde vea la frase &quot;Una solicitud&quot;. Para obtener más información, vea [Implicaciones de la personalización de nombres de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) en el artículo [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Para obtener más información acerca de las plantillas de diseño, vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Personalización de la terminología de interfaz de usuario

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en **Establecer terminología** cerca de la esquina superior derecha de la página.
1. Realice una de las siguientes acciones:

   * Para utilizar un término alternativo proporcionado por Workfront, haga clic en la flecha hacia abajo ![](assets/dropdown-arrow.png) junto a la etiqueta y, a continuación, haga clic en la etiqueta alternativa que desee en la lista desplegable.

     >[!NOTE]
     >
     >Las etiquetas alternativas que se proporcionan en las listas desplegables son compatibles con las versiones de Workfront localizadas en idiomas distintos del inglés.

   * Para proporcionar su propia alternativa personalizada para la etiqueta mostrada para un objeto, haga clic en **Establecer nombre personalizado** a la derecha de la etiqueta y, a continuación, escriba los formularios **Singular** y **Plural** del término personalizado. Puedes hacer clic en **Restablecer** si cambias de opinión.

     Puede personalizar los siguientes nombres de objeto:

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Objetos Workfront</p></td>
        <td>
          <p>Portafolio</p>
          <p>Programar</p>
          <p>Proyecto</p>
          <p>Tarea</p>
          <p>Problema</p>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Actividad</p>
         </ul></td>
        <td><p>Para obtener más información acerca de estos objetos, vea <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprender los objetos en Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objetos Workfront Goals</p></td>
        <td>
         <ul>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Actividad</p>
         </ul></td>
        <td><p>Estos objetos requieren una licencia adicional. Para obtener más información, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Información general sobre los objetivos de Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Objetos del planificador de escenarios Workfront</p></td>
        <td>
         <ul>
          <p>Iniciativa</p>
          <p>Escenario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Estos objetos requieren una licencia adicional. Para obtener más información, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Introducción al Scenario Planner</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Cuando termine, haga clic en **Listo**.

   >[!TIP]
   >
   >Después de hacer clic en Listo (e incluso después de guardar la plantilla de diseño), siempre puede volver a la configuración Definir terminología y hacer clic en Restablecer junto a cualquier término personalizado para devolverlo a su estado predeterminado.

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

1. Para ver los cambios terminológicos:

   1. Cierre la sesión y vuelva a iniciarla en Workfront.
   1. Cierre todas las pestañas del explorador que haya abierto para su entorno de Workfront.

   >[!IMPORTANT]
   >
   >Esto también es necesario para todos los que hayan utilizado la plantilla de diseño antes de realizar los cambios terminológicos.

Para obtener más información acerca de las plantillas de diseño, vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
