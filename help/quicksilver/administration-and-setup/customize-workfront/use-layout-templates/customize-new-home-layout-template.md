---
title: Personalizar una nueva página de inicio con una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puede utilizar una plantilla de diseño para configurar lo que ven los usuarios cuando abren una nueva página de inicio.
author: Nolan
feature: System Setup and Administration
role: Admin
source-git-commit: 6e4e6ba8f960f11aeb824d29b4bbf1d75532747b
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 1%

---

# Personalizar una nueva página de inicio con una plantilla de diseño

Puede utilizar una plantilla de diseño para configurar lo que ven los usuarios cuando abren una nueva página de inicio.

Puede configurar lo siguiente:

* Los widgets que se muestran en el espacio de trabajo de forma predeterminada y su diseño en la página
* Qué fondo se selecciona
* Configuración de widgets específicos, incluidos los filtros y grupos disponibles para los widgets Mis proyectos, Mis tareas y Mis problemas, así como sus valores predeterminados

>[!IMPORTANT]
>
>Las opciones de plantilla de diseño de administrador descritas en esta página anulan las opciones de personalización de los usuarios individuales.
>
>Cuando se guardan los cambios realizados en una plantilla de diseño, se cambiará la nueva página de inicio de los usuarios para que coincida con la plantilla y las selecciones de widgets existentes se colocarán en la parte inferior de la página. Aunque el usuario puede cambiar la posición de los widgets seleccionados por el administrador y cambiar su tamaño, no se pueden eliminar.

Para obtener información sobre la nueva página Inicio, consulte [Introducción a la nueva página de inicio](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

Para obtener información sobre la creación de plantillas de diseño, consulte [Creación y administración de plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información sobre plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información sobre cómo asignar una plantilla de diseño a los usuarios, consulte [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar una nueva página de inicio con una plantilla de diseño

1. Empiece a trabajar en una plantilla de diseño como se describe en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Haga clic en la flecha hacia abajo ![](assets/dropdown-arrow.png) bajo **Personalizar lo que ven los usuarios**, luego haga clic en **Espacio de trabajo principal**.

1. En las pestañas que aparecen a la derecha, haga clic en **Diseño y diseño** para elegir y organizar los widgets y el fondo, o **Configuración del widget** para administrar la configuración de widgets individuales como filtros y grupos disponibles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Diseño y disposición</td> 
      <td>
      <p>Seleccione los widgets que estarán presentes en los espacios de trabajo de los usuarios, su posición y elija un fondo. Tenga en cuenta que, aunque los usuarios no pueden eliminar los widgets seleccionados, pueden moverlos y cambiarles el tamaño libremente, así como agregar widgets adicionales.</p>
      <p>Esta pestaña funciona esencialmente como un pequeño espacio de trabajo nuevo en Inicio; como tal, se puede personalizar según los pasos descritos en <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Agregar, editar o quitar widgets en la nueva página de inicio</a>. Seleccione los widgets y organice el espacio de trabajo tal como desea que aparezca para los usuarios.</p>
      <p>Para cambiar el fondo, siga los pasos que aparecen debajo de <b>Personalización de fondo</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Introducción a la nueva página de inicio</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración del widget</td> 
      <td>
      <p>Cambie la configuración de los widgets individuales. Actualmente, solo se admiten tres widgets:</p>
      <ul>
        <li>Mis proyectos</li>
        <li>Mis tareas</li>
        <li>Mis problemas</li>
      </ul>
      <p>Una vez que haya seleccionado el widget que desea editar, las opciones disponibles se mostrarán a la derecha. Estas opciones incluyen <b>Filtros</b>, <b>Columnas</b>, y <b>Grupos</b>. Puede:</p>
      <ul>
        <li><b>Seleccione los filtros, columnas o grupos que estarán disponibles para los usuarios:</b><p>Marque la casilla junto a todas las opciones de la lista que desee que los usuarios puedan utilizar. Las opciones no seleccionadas no aparecerán para los usuarios.</li></p>
        <li><b>Establezca un filtro o un grupo predeterminado para el widget:</b><p>Pase el ratón sobre una opción y aparecerá un botón que le permitirá establecer esa opción como predeterminada para los usuarios. El valor predeterminado actual tendrá un distintivo predeterminado azul a su derecha.</li></p>
        <li><b>Agregue un filtro, una columna o un grupo existentes a la lista de opciones disponibles:</b><p>Haga clic en el botón del signo más situado en la parte inferior de cada lista para agregar una opción a esa lista. Tenga en cuenta que solo los filtros, campos (para columnas) o grupos existentes se pueden agregar de esta manera.</li></p>
      </ul>
      </td> 
     </tr>
    </tbody> 
   </table>

>[!IMPORTANT]
>
>Si establece un filtro o una agrupación predeterminados para un widget específico mediante una plantilla de diseño, es posible que no surta efecto inmediatamente debido a las preferencias de usuario existentes. Para aplicar el nuevo filtro o agrupación inmediatamente, es posible que usted o el usuario tengan que restablecer sus preferencias de usuario añadiendo &quot;/resetUser&quot; al final de su URL.

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar** en la esquina inferior izquierda.

