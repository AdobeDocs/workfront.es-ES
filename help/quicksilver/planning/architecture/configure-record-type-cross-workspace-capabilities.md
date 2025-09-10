---
title: Configuración de funciones de espacio de trabajo cruzado para el tipo de registro
description: Puede habilitar un tipo de registro para que se agregue a otro espacio de trabajo o para que se conecte desde otro espacio de trabajo.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 7%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Configuración de funciones entre espacios de trabajo para tipos de registros

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Las siguientes son funciones de varios espacios de trabajo de los tipos de registro:

* Puede designar un tipo de registro como centralizado. Los usuarios pueden agregar tipos de registros centralizados a otros espacios de trabajo que pueden administrar.
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
Y
<li><p>Paquete Planning Plus</p></li></ul>
O
<ul><li><p>Cualquier paquete de flujo de trabajo</p> </li>
Y
<li><p>Planificación del paquete de Prime o Ultimate</p></li></ul>
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
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

## Configuración de tipos de registros centralizados

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

Como administrador de espacio de trabajo, puede configurar un tipo de registro para que sea un tipo de registro centralizado. Se puede añadir un tipo de registro centralizado a otros espacios de trabajo.

Un gestor de espacio de trabajo puede añadir un tipo de registro centralizado a un espacio de trabajo que gestione. También se agregan los campos originales del tipo de registro.

Los usuarios pueden agregar registros a un tipo de registro centralizado desde cualquier espacio de trabajo para el que tengan permisos de contribución y donde se agregue el tipo de registro centralizado, incluido su espacio de trabajo original. Pueden ver registros del espacio de trabajo para el que solo tienen permisos de visualización.

Para obtener más información, vea [Información general sobre los tipos de registros centralizados](/help/quicksilver/planning/architecture/centralized-record-types-overview.md)

Para configurar la adición de un tipo de registro como tipo de registro centralizado:

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del tipo de registro.
1. Haga clic en **Editar**.

   ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   >[!TIP]
   >
   >Si un tipo de registro ya se ha designado como tipo de registro centralizado y se ha añadido a otros espacios de trabajo, la opción Editar aparece atenuada.

1. En el cuadro **Editar tipo de registro**, seleccione la ficha **Configuración avanzada**.
1. Habilite la opción **Permitir agregar este tipo de registro a otros espacios de trabajo**.

   ![Editar la configuración avanzada del tipo de registro con Agregar a otros espacios de trabajo habilita](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Después de agregar un tipo de registro centralizado a otro espacio de trabajo, esta configuración ya no se puede deshabilitar.

1. En el campo **Seleccione quién puede agregar este tipo de registro a los espacios de trabajo que administra**, agregue las entidades que desee permitir para agregar este tipo de registro a los espacios de trabajo que administra.

   Su nombre se añade automáticamente en el campo.

   Puede agregar usuarios individuales o grupos, equipos, roles o empresas a cuyos usuarios desee permitir que agreguen este tipo de registro a los espacios de trabajo que administran.

   Debe designar al menos una entidad (usuario, equipo, grupo, función o compañía) para poder habilitar esta configuración.

   Puede editar este campo después de guardar el tipo de registro.

1. (Opcional) Elimine su nombre del campo **Seleccione quién puede agregar este tipo de registro a los espacios de trabajo que administran**.

1. Haga clic en **Guardar**.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para que las personas designadas lo añadan a otro espacio de trabajo.

   >[!NOTE]
   >
   >Sólo se puede editar el aspecto y la configuración del tipo de registro y sus campos originales desde el espacio de trabajo original.

   * La tarjeta de tipo de registro muestra un icono centralizado ![Icono de tipo de registro centralizado](assets/global-icon.png) para indicar que el tipo de registro está disponible para agregarse a otros espacios de trabajo.
   * Un campo **Workspace** generado por el sistema se agrega a la vista de tabla del tipo de registro y los detalles de sus registros.

     El campo Workspace muestra el espacio de trabajo desde el que se crea cada registro.

     Este campo es de solo lectura y no se puede eliminar.
1. (Opcional) Vaya a otro espacio de trabajo y cree un tipo de registro utilizando un tipo de registro existente. Seleccione el tipo de registro que ha activado en los pasos anteriores.

   Para obtener más información, vea [Agregar tipos de registros existentes](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

## Configurar tipos de registros conectables

<!--this is a UI term; don't change the title of this section-->

Puede configurar un tipo de registro para que se conecte desde otros espacios de trabajo al crear o editar el tipo de registro.

Para configurar un tipo de registro al que conectarse desde otros espacios de trabajo al editar el tipo de registro:

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro; a continuación, haga clic en **Editar**
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Editar**.

   ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. En el cuadro **Editar tipo de registro**, seleccione la ficha **Configuración avanzada**.
1. Habilite la opción **Permitir la conexión a este tipo de registro en otros espacios de trabajo**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Editar pestaña de configuración avanzada de tipo de registro con la conexión habilitada desde otros espacios de trabajo](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Cuando está habilitado, el tipo de registro es accesible y se puede conectar a desde otros espacios de trabajo.

1. Elija desde qué espacios de trabajo se puede acceder al tipo de registro. Elija entre las siguientes opciones:

   * **En todo el sistema**: los usuarios pueden conectarse a este tipo de registro desde todos los espacios de trabajo donde tengan permisos de administración.
   * **Espacios de trabajo específicos**: agregue los nombres de los espacios de trabajo a los que los administradores de espacios de trabajo pueden conectarse para este tipo de registro.
1. Haga clic en **Guardar**.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para conectarse desde los espacios de trabajo designados.
   * La tarjeta de tipo de registro muestra un icono de conexión entre espacios de trabajo ![icono de conexión entre espacios de trabajo](assets/connect-from-other-workspaces-icon.png) para indicar que el tipo de registro está disponible para conectarse desde cualquier espacio de trabajo que haya designado en su configuración.

   El tipo de registro está disponible para conectarse a desde los espacios de trabajo designados.
1. (Opcional) Vaya a otro espacio de trabajo y añada una conexión al tipo de registro que ha activado para la conectividad entre espacios de trabajo en los pasos anteriores.

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).









