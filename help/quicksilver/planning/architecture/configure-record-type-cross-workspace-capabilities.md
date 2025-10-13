---
title: Configuración de funciones de varios espacios de trabajo para tipos de registro
description: Puede habilitar un tipo de registro para que se agregue a otro espacio de trabajo o para que se conecte desde otro espacio de trabajo.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '1230'
ht-degree: 5%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTILE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->


<!--this article is linked to the UI - do not delete or change the URL-->

<!--THIS MIGHT ALREADY BE ADDED TO THE "OVERVIEW" ARTICLE, BUT CHECK: add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Configuración de funciones entre espacios de trabajo para tipos de registros

<!--this is linked to the UI in the info icon when you enable a record to be either global or connectable-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Puede configurar los tipos de registros para que funcionen en varios espacios de trabajo.

Las siguientes son funciones de varios espacios de trabajo de los tipos de registro:

* Puede designar un tipo de registro como global. Los usuarios pueden agregar tipos de registros globales a otros espacios de trabajo que puedan administrar.
* Puede designar un tipo de registro como conectable. Los usuarios pueden conectarse a este tipo de registro desde otros espacios de trabajo.

Primero debe definir las capacidades de un tipo de registro entre espacios de trabajo para que los administradores de espacios de trabajo puedan conectarlo desde o agregarlo a otros espacios de trabajo.

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
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Cualquier paquete de Workfront</p></li>
<p>Y</p>
<li><p>Cualquier paquete de Planning para crear tipos de registros conectables</p></li>
<li><p>Paquete de Planning Plus para crear tipos de registros globales</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Configuración de tipos de registros globales

<!--this is a UI term; don't change the title of this section-->

Como administrador de espacio de trabajo, puede configurar un tipo de registro para que sea un tipo de registro global. Se puede agregar un tipo de registro global a otros espacios de trabajo.

Un administrador del espacio de trabajo puede agregar un tipo de registro global a un espacio de trabajo que administre. También se agregan los campos originales del tipo de registro.

Los usuarios pueden agregar registros a un tipo de registro global desde cualquier espacio de trabajo para el que tengan permisos de contribución y donde se agregue el tipo de registro global, incluido su espacio de trabajo original. Pueden ver registros del espacio de trabajo para el que solo tienen permisos de visualización.

Para obtener más información, vea [Información general sobre los tipos de registros entre espacios de trabajo](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

Para configurar un tipo de registro como global:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee configurar como globales.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro

     ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del tipo de registro.
1. Haga clic en **Editar** o en **Configuración**.

   >[!TIP]
   >
   >Cuando se agrega un tipo de registro a otro espacio de trabajo, se muestra como un tipo de registro global en ese espacio de trabajo. En este caso, las opciones Editar y Configuración aparecen atenuadas.

1. (Condicional) Si hizo clic en **Editar**, en el cuadro **Editar tipo de registro**, haga clic en la ficha **Configuración entre espacios de trabajo**

   O bien, si hizo clic en **Configuración**, vaya a la sección **Configuración del área de trabajo cruzada** en el panel izquierdo.
1. Habilite la opción **Permitir agregar este tipo de registro a otros espacios de trabajo**.

   ![Editar la configuración del tipo de registro entre espacios de trabajo con Agregar a otros espacios de trabajo habilitados](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Después de agregar un tipo de registro global a otro espacio de trabajo, esta configuración ya no se puede deshabilitar.

1. En el campo **Seleccione quién puede agregar este tipo de registro a los espacios de trabajo que administra**, agregue las entidades que desee permitir para agregar este tipo de registro a los espacios de trabajo que administra.

   Su nombre se añade automáticamente en el campo.

   Puede agregar usuarios individuales o grupos, equipos, roles o empresas a cuyos usuarios desee permitir que agreguen este tipo de registro a los espacios de trabajo que administran.

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

   * La tarjeta de tipo de registro muestra un icono global ![icono de tipo de registro global](assets/global-icon.png) para indicar que el tipo de registro está disponible para agregarse a otros espacios de trabajo.
   * Un campo **Workspace** generado por el sistema se agrega a la vista de tabla del tipo de registro y los detalles de sus registros.

     El campo Workspace muestra el espacio de trabajo desde el que se crea cada registro.

     Este campo es de solo lectura y no se puede eliminar.
1. (Opcional) Vaya a otro espacio de trabajo y cree un tipo de registro utilizando un tipo de registro existente. Seleccione el tipo de registro que ha activado en los pasos anteriores.

   Para obtener más información, vea [Agregar tipos de registros existentes desde otro área de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Configurar tipos de registros conectables

<!--this is a UI term; don't change the title of this section-->

Puede configurar un tipo de registro para que se conecte desde otros espacios de trabajo al crear o editar el tipo de registro.

Para configurar un tipo de registro como conectable:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee configurar como conectables.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro

     ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del tipo de registro.
1. Haga clic en **Editar** o en **Configuración**.

1. (Condicional) Si hizo clic en **Editar**, en el cuadro **Editar tipo de registro**, haga clic en la ficha **Configuración entre espacios de trabajo**

   O bien, si hizo clic en **Configuración**, vaya a la sección **Configuración del área de trabajo cruzada** en el panel izquierdo.

1. Habilite la opción **Permitir la conexión a este tipo de registro en otros espacios de trabajo**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Editar tipo de registro en la ficha Configuración entre espacios de trabajo con la conexión habilitada desde otros espacios de trabajo](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Cuando está habilitado, el tipo de registro es accesible y se puede conectar a desde otros espacios de trabajo.

1. Elija desde qué espacios de trabajo se puede acceder al tipo de registro. Elija entre las siguientes opciones:

   * **En todo el sistema**: los usuarios pueden conectarse a este tipo de registro desde todos los espacios de trabajo donde tengan permisos de administración.
   * **Espacios de trabajo específicos**: agregue los nombres de los espacios de trabajo a los que los administradores de espacios de trabajo pueden conectarse para este tipo de registro.
1. (Condicional) Haga clic en **Guardar** en el cuadro **Editar tipo de registro** o haga clic en la flecha hacia atrás a la izquierda de **Configuración** en el encabezado de la página para guardar los cambios.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para conectarse desde los espacios de trabajo designados.
   * La tarjeta de tipo de registro muestra un icono de conexión entre espacios de trabajo ![icono de conexión entre espacios de trabajo](assets/connect-from-other-workspaces-icon.png) para indicar que el tipo de registro está disponible para conectarse desde cualquier espacio de trabajo que haya designado en su configuración.

   El tipo de registro está disponible para conectarse a desde los espacios de trabajo designados.
1. (Opcional) Vaya a otro espacio de trabajo y añada una conexión al tipo de registro que ha activado para la conectividad entre espacios de trabajo en los pasos anteriores.

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).









