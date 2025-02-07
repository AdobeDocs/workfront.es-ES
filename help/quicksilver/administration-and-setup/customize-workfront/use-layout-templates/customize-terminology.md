---
title: Personalizar la terminología de la interfaz de usuario con una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para cambiar las etiquetas de algunos objetos que aparecen en Workfront y que coincidan con los términos utilizados en su organización.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 95%

---

# Personalizar la terminología de la interfaz de usuario con una plantilla de diseño

Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para cambiar las etiquetas de algunos objetos que aparecen en Workfront y que coincidan con los términos utilizados en su organización.

Después de guardar una plantilla de diseño en la que ha cambiado la terminología, cerrar la sesión de Workfront y volver a iniciarla, las etiquetas que ha cambiado aparecen donde aparecerían las etiquetas predeterminadas en la mayoría de las áreas de Workfront:

* Menú principal
* Todas las áreas accesibles desde el menú principal
* Todas las fichas
* Todos los menús
* Generador de informes y elementos de creación de informes (vistas, filtros y agrupaciones)
* Botones Guardar
* Archivos exportados
* Correos electrónicos
* Aplicaciones móviles

>[!NOTE]
>
>* El área Complemento de Outlook no muestra las etiquetas personalizadas.
>* Pueden aparecer problemas gramaticales y de otro tipo al personalizar las etiquetas. Por ejemplo, si cambia “Problema” a “Solicitud”, puede haber lugares en la IU donde vea la frase “Un solicitud”. Para obtener más información, consulte [Implicaciones de la personalización de nombres de objeto](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) en el artículo [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Para obtener más información sobre las plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obtener más información sobre las plantillas de diseño para grupos, consulte [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, consulte [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
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

## Personalizar la terminología de interfaz de usuario

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en **Establecer terminología** cerca de la esquina superior derecha de la página.
1. Realice una de las siguientes acciones:

   * Para utilizar un término alternativo proporcionado por Workfront, haga clic en la flecha abajo ![Flecha abajo](assets/dropdown-arrow.png) junto a la etiqueta y, a continuación, haga clic en la etiqueta alternativa que desee en la lista desplegable.

     >[!NOTE]
     >
     >Las etiquetas alternativas que se proporcionan en las listas desplegables son compatibles con las versiones de Workfront localizadas en idiomas distintos al inglés.

   * Para proporcionar su propia alternativa personalizada para la etiqueta mostrada para un objeto, haga clic en **Establecer nombre personalizado** a la derecha de la etiqueta y, a continuación, escriba las formas en **singular** y **plural** del término personalizado. Puede hacer clic en **Restablecer** si cambia de opinión.

     Puede personalizar los siguientes nombres de objeto:

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Objetos de Workfront</p></td>
        <td>
          <p>Portafolio</p>
          <p>Programa</p>
          <p>Proyecto</p>
          <p>Tarea</p>
          <p>Problema</p>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Actividad</p>
         </ul></td>
        <td><p>Para obtener más información sobre estos objetos, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprender los objetos en Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objetos de Workfront Goals</p></td>
        <td>
         <ul>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Actividad</p>
         </ul></td>
        <td><p>Estos objetos requieren una licencia adicional. Para obtener más información, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Información general sobre Adobe Workfront Goals</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Objetos del planificador de escenarios de Workfront</p></td>
        <td>
         <ul>
          <p>Iniciativa</p>
          <p>Escenario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Estos objetos requieren una licencia adicional. Para obtener más información, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Introducción al planificador de escenarios</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Cuando haya finalizado, haga clic en **Listo**.

   >[!TIP]
   >
   >Después de hacer clic en Listo (e incluso después de guardar la plantilla de diseño), siempre puede volver a la configuración Establecer terminología y hacer clic en Restablecer junto a cualquier término personalizado para devolverlo a su estado predeterminado.

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

1. Para ver los cambios terminológicos:

   1. Cierre la sesión y vuelva a iniciarla en Workfront.
   1. Cierre todas las pestañas del explorador que haya abierto para su entorno de Workfront.

   >[!IMPORTANT]
   >
   >Esto también es necesario para todas las personas que hayan utilizado la plantilla de diseño antes de realizar los cambios terminológicos.

Para obtener más información sobre las plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
