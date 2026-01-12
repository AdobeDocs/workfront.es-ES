---
title: Configuración de funciones de varios espacios de trabajo para tipos de registro
description: Puede habilitar un tipo de registro para que se agregue a otro espacio de trabajo o para que se conecte desde otro espacio de trabajo en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 895fcc9e8bfc6ef21e82ae6dab4c370b0e267cad
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 5%

---


<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTICLE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->

# Configuración de funciones entre espacios de trabajo para tipos de registros

<!--this article is linked to the UI in the Advanced settings/ Cross-workspace settings tab - do not delete or change the URL-->

{{planning-important-intro}}

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Puede configurar los tipos de registros para que funcionen en varios espacios de trabajo en Adobe Workfront Planning.

Puede designar un tipo de registro como uno de los siguientes:

* <span class="preview">**Un tipo de registro global**: los usuarios pueden agregar tipos de registro global a otros espacios de trabajo que puedan administrar.</span>
* **Un tipo de registro conectable**: los usuarios pueden conectarse a este tipo de registro desde otros espacios de trabajo.

Primero debe definir las capacidades de un tipo de registro entre espacios de trabajo para que los administradores de espacios de trabajo puedan agregarlo o conectarlo desde otros espacios de trabajo.

Las funciones entre espacios de trabajo de un tipo de registro se definen al crear o editar un tipo de registro.

Para obtener más información, consulte uno de los siguientes artículos:

* [Crear tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)
* [Editar tipos de registro](/help/quicksilver/planning/architecture/edit-record-types.md)

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
<p>Para configurar tipos de registros conectables: </p>
<ul> 
<li><p>Cualquier paquete Workfront y cualquier paquete Planning</p></li>
O
<li>Cualquier flujo de trabajo y un paquete de Planning Prime o Ultimate</p></li></ul>

<div class="preview">
<p>Para configurar tipos de registros globales:</p>

<ul> 
<li><p>Cualquier paquete Workfront y un paquete Planning Plus</p></li>
O
<li><p>Cualquier flujo de trabajo y un paquete de Planning Prime o Ultimate</p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p>

</div> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Workflow Prime or Ultimate package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> -->

<div class="preview">

## Configuración de tipos de registros globales

<!--this is a UI term; don't change the title of this section-->

Como administrador de espacio de trabajo, puede configurar un tipo de registro para que sea un tipo de registro global. Se puede agregar un tipo de registro global a otros espacios de trabajo.

Un administrador del espacio de trabajo puede agregar un tipo de registro global a un espacio de trabajo que administre. Los campos originales del tipo de registro también se añaden al espacio de trabajo secundario.

Los usuarios pueden agregar registros a un tipo de registro global desde cualquier espacio de trabajo en el que tengan permisos de contribución y en el que se agregue el tipo de registro global, incluido su espacio de trabajo original. Pueden ver registros de espacios de trabajo a los que solo tienen permisos de visualización.

Para obtener más información, vea [Información general sobre los tipos de registros entre espacios de trabajo](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

Para configurar un tipo de registro como global:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee configurar como globales.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro. <!--add new screen shot without Share for now-->

     ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del tipo de registro.
1. Haga clic en **Editar** o en **Configuración**.

   >[!TIP]
   >
   >Cuando se agrega un tipo de registro a otro espacio de trabajo, se muestra como un tipo de registro global en ese espacio de trabajo. En este caso, las opciones Editar y Configuración aparecen atenuadas.

1. (Condicional) Si hizo clic en **Editar**, en el cuadro **Editar tipo de registro**, haga clic en la ficha **Configuración entre espacios de trabajo**

   O bien, si hizo clic en **Configuración**, haga clic en la sección **Configuración del área de trabajo cruzada** en el panel izquierdo.
1. Habilite la opción **Permitir agregar este tipo de registro a otros espacios de trabajo**.

   ![Editar la configuración del tipo de registro entre espacios de trabajo con Agregar a otros espacios de trabajo habilitados](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Después de agregar un tipo de registro global a otro espacio de trabajo, esta configuración ya no se puede deshabilitar.

1. En el campo **Seleccione quién puede agregar este tipo de registro a los espacios de trabajo que administra**, agregue las entidades que desee permitir para agregar este tipo de registro a los espacios de trabajo que administra.

   Su nombre se añade automáticamente en el campo.

   Puede agregar usuarios individuales, grupos, equipos, funciones del puesto o empresas a cuyos usuarios desee permitir que agreguen este tipo de registro a los espacios de trabajo que administran.

   Puede editar este campo después de guardar el tipo de registro.

1. (Opcional) Elimine su nombre del campo **Seleccione quién puede agregar este tipo de registro a los espacios de trabajo que administran**.

   >[!TIP]
   >
   >Debe designar al menos una entidad (usuario, equipo, grupo, función o compañía) para poder habilitar esta configuración.

1. (Condicional) Haga clic en **Guardar** en el cuadro **Editar tipo de registro** o haga clic en la flecha hacia atrás a la izquierda de **Configuración** en el encabezado de la página para guardar los cambios.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para que las personas designadas lo añadan a otro espacio de trabajo.

   >[!NOTE]
   >
   >Sólo se puede editar el aspecto y la configuración del tipo de registro y sus campos originales desde el espacio de trabajo original.

   * La tarjeta de tipo de registro muestra un icono **tipo de registro global** ![icono de tipo de registro global](assets/global-icon.png) para indicar que el tipo de registro está disponible para agregarse a otros espacios de trabajo.
   * Un campo **Workspace** generado por el sistema se agrega a la vista de tabla del tipo de registro y los detalles de sus registros.

     El campo Workspace muestra el espacio de trabajo desde el que se crea cada registro.

     Este campo es de solo lectura y no se puede eliminar.
1. (Opcional) Vaya a otro espacio de trabajo y cree un tipo de registro utilizando un tipo de registro existente. Seleccione el tipo de registro que ha activado en los pasos anteriores.

   Para obtener más información, vea [Agregar tipos de registros existentes desde otro área de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   El tipo de registro agregado de un tipo de registro global en el área de trabajo secundaria también muestra un icono de **tipo de registro global** ![icono de tipo de registro global](assets/global-icon.png).
1. (Opcional) Vuelva al espacio de trabajo original donde creó el tipo de registro global y edite el tipo de registro siguiendo los pasos del 1 al 4 anteriores a <!--ensure this stays accurate-->
1. (Opcional) Revise la lista de espacios de trabajo donde se ha agregado el registro global en la sección **Espacios de trabajo donde se usa este tipo de registro**. El propietario del espacio de trabajo también aparece junto al nombre del espacio de trabajo.

   ![Espacios de trabajo donde se usa este tipo de registro](assets/workspaces-where-this-record-type-is-used.png)
1. (Opcional) Haga clic en el nombre de uno de los espacios de trabajo enumerados en la sección **Espacios de trabajo donde se usa este tipo de registro** para abrir ese espacio de trabajo.

</div>

## Configurar tipos de registros conectables

<!--this is a UI term; don't change the title of this section-->

Puede configurar un tipo de registro para que se conecte desde otros espacios de trabajo al crear o editar el tipo de registro.

La configuración de un tipo de registro para que sea conectable difiere según el entorno que elija para la configuración.

### Configurar tipos de registros conectables en el entorno de producción

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee configurar como conectables.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro

     ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Editar**.

1. Haga clic en la ficha **Configuración avanzada**.

1. Habilite la opción **Permitir la conexión a este tipo de registro desde otros espacios de trabajo**.

   ![Editar ficha de configuración avanzada de registro con la conexión habilitada desde otros espacios de trabajo](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Cuando está habilitado, el tipo de registro se vuelve conectable y se puede acceder a él desde otros espacios de trabajo.

1. Elija desde qué espacios de trabajo se puede acceder al tipo de registro. Elija entre las siguientes opciones:

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **En todo el sistema**: los usuarios pueden conectarse a este tipo de registro desde todos los espacios de trabajo donde tengan permisos de administración.
   * **Espacios de trabajo específicos**: en el menú desplegable, agregue los nombres de los espacios de trabajo donde los administradores de espacios de trabajo pueden conectarse a este tipo de registro.
1. (Condicional) Haga clic en **Guardar** en el cuadro **Editar tipo de registro** para guardar los cambios.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para conectarse desde los espacios de trabajo designados.
   * La tarjeta de tipo de registro muestra un icono de tipo de registro conectable ![Icono de tipo de registro conectable](assets/connect-from-other-workspaces-icon.png) para indicar que el tipo de registro está disponible para conectarse desde cualquier área de trabajo designada en su configuración.

1. (Opcional) Vaya a otro espacio de trabajo y añada una conexión al tipo de registro que ha activado para la conectividad entre espacios de trabajo en los pasos anteriores.

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

<div class="preview">

### Configuración de tipos de registros conectables en el entorno de vista previa

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee configurar como conectables.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro

     ![Más opciones de menú de la tarjeta de tipo de registro con Configuración](assets/more-menu-options-from-record-type-card-with-settings-link.png)

   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del tipo de registro.
1. Haga clic en **Editar** o en **Configuración**.

1. (Condicional) Si hizo clic en **Editar**, en el cuadro **Editar tipo de registro**, haga clic en la ficha **Configuración entre espacios de trabajo**

   O bien, si hizo clic en **Configuración**, haga clic en la sección **Configuración del área de trabajo cruzada** en el panel izquierdo.

1. Habilite la opción **Permitir la conexión a este tipo de registro en otros espacios de trabajo**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   <!-- add new screen shot with new tab name-->

   ![Editar tipo de registro en la ficha Configuración entre espacios de trabajo con la conexión habilitada desde otros espacios de trabajo](assets/edit-record-type-box-cross-workspace-settings-connectable-record-type-enabled.png)

   Cuando está habilitado, el tipo de registro es accesible y se puede conectar a desde otros espacios de trabajo.

1. Elija desde qué espacios de trabajo se puede acceder al tipo de registro. Elija entre las siguientes opciones:

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **Todos los espacios de trabajo**: los usuarios pueden conectarse a este tipo de registro desde todos los espacios de trabajo en los que tengan permisos de administración.
   * **Espacios de trabajo específicos**: en el menú desplegable, agregue los nombres de los espacios de trabajo donde los administradores de espacios de trabajo pueden conectarse a este tipo de registro.
1. (Condicional) Haga clic en **Guardar** en el cuadro **Editar tipo de registro** o haga clic en la flecha hacia atrás a la izquierda de **Configuración** en el encabezado de la página para guardar los cambios.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para conectarse desde los espacios de trabajo designados.
   * La tarjeta de tipo de registro muestra un icono de tipo de registro conectable ![Icono de tipo de registro conectable](assets/connect-from-other-workspaces-icon.png) para indicar que el tipo de registro está disponible para conectarse desde cualquier área de trabajo designada en su configuración.

1. (Opcional) Vaya a otro espacio de trabajo y añada una conexión al tipo de registro que ha activado para la conectividad entre espacios de trabajo en los pasos anteriores.

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

</div>









