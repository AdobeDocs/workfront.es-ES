---
title: Personalización de la terminología de la interfaz de usuario mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para cambiar las etiquetas de algunos objetos que aparecen en Workfront y que coinciden con los términos utilizados en su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# Personalización de la terminología de la interfaz de usuario mediante una plantilla de diseño

Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para cambiar las etiquetas de algunos objetos que aparecen en Workfront y que coinciden con los términos utilizados en su organización.

Después de guardar una plantilla de diseño en la que cambió la terminología, cerrar la sesión de Workfront y volver a entrar, las etiquetas que ha cambiado aparecen donde aparecerían las etiquetas predeterminadas en la mayoría de las áreas de Workfront:

* Menú principal
* Todas las áreas a las que se accede desde el menú principal
* Todas las pestañas
* Todos los menús
* Report Builder y elementos de informes (vistas, filtros y agrupaciones)
* Botones Guardar
* Archivos exportados
* Correos electrónicos
* Aplicaciones móviles

>[!NOTE]
>
>* El área del complemento de Outlook no muestra las etiquetas personalizadas.
>* Puede encontrar problemas gramaticales y de otro tipo al personalizar etiquetas. Por ejemplo, si cambia &quot;Problema&quot; a &quot;Solicitud&quot;, es posible que haya lugares en la interfaz de usuario donde vea la frase &quot;Solicitud&quot;. Para obtener más información, consulte [Implicaciones de personalizar nombres de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


Para obtener información sobre plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acceso

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
   <td> <p>Para realizar estos pasos a nivel de sistema, necesita el nivel de acceso del administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de dicho grupo.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalización de la terminología de la interfaz de usuario

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en **Definir terminología** cerca de la esquina superior derecha de la página.
1. Realice una de las siguientes acciones:

   * Para utilizar un término alternativo proporcionado por Workfront, haga clic en la flecha hacia abajo  ![](assets/dropdown-arrow.png) junto a la etiqueta y, a continuación, haga clic en la etiqueta alternativa que desee en la lista desplegable.

      >[!NOTE]
      >
      >Las etiquetas alternativas que se proporcionan en las listas desplegables son compatibles con las versiones de Workfront localizadas para idiomas que no sean el inglés.

   * Para proporcionar su propia alternativa personalizada para la etiqueta mostrada para un objeto, haga clic en **Definir nombre personalizado** a la derecha de la etiqueta, luego escriba la **Singular** y **Plural** formas del término personalizado. Puede hacer clic en **Restablecer** si cambias de opinión.

      Puede personalizar los nombres de objeto siguientes:

      <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Objetos de Workfront</p></td>
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
        <td><p>Para obtener más información sobre estos objetos, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objetos de objetivos de Workfront</p></td>
        <td>
         <ul>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Actividad</p>
         </ul></td>
        <td><p>Estos objetos requieren una licencia adicional. Para obtener más información, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Información general sobre los objetivos de Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Objetos del planificador de escenario de Workfront</p></td>
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

1. Cuando haya terminado, haga clic en **Listo**.

   >[!TIP]
   >
   >Después de hacer clic en Finalizado (e incluso después de guardar la plantilla de diseño), siempre puede volver a la configuración de Definir terminología y hacer clic en Restablecer junto a cualquier término personalizado para devolverlo a su estado predeterminado.

1. Continúe personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

1. Para ver los cambios terminológicos:

   1. Cierre la sesión y vuelva a iniciarla en Workfront.
   1. Cierre todas las fichas del explorador que haya abierto para su entorno de Workfront.

   >[!IMPORTANT]
   >
   >Esto también es necesario para cualquier usuario que haya utilizado la plantilla de diseño antes de realizar cambios en la terminología.

Para obtener más información sobre las plantillas de diseño, consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
