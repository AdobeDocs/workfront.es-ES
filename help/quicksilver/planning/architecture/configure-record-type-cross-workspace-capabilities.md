---
title: Configuración de funciones de espacio de trabajo cruzado para el tipo de registro
description: Puede habilitar un tipo de registro para que se agregue a otro espacio de trabajo o para que se conecte desde otro espacio de trabajo.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 943c26efa6f6351abf885dbc5f3aa09c0b0fab05
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 12%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# Configuración de funciones entre espacios de trabajo para tipos de registros

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Puede designar un tipo de registro para que se añada a otro espacio de trabajo o para que se conecte desde otro espacio de trabajo, en Adobe Workfront Planning.

Primero debe definir las capacidades de un tipo de registro entre espacios de trabajo para que los administradores de espacios de trabajo puedan conectarlo o importarlo a otros espacios de trabajo.

Las funciones entre espacios de trabajo de un tipo de registro se definen al crear o editar un tipo de registro.

Para obtener más información, consulte uno de los siguientes artículos:

* [Crear tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)
* [Editar tipos de registro](/help/quicksilver/planning/architecture/edit-record-types.md)

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuración de la adición de un tipo de registro a otros espacios de trabajo

Como administrador de espacio de trabajo, puede configurar un tipo de registro para que se agregue a otros espacios de trabajo al crear o editar un tipo de registro.

Al configurar la adición de un tipo de registro a otros espacios de trabajo, un administrador de espacios de trabajo puede importar el tipo de registro y toda su información a uno de los espacios de trabajo que administra.

Para configurar la adición de un tipo de registro a otro espacio de trabajo al editar el tipo de registro:

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro y, a continuación, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) situado a la derecha del nombre del tipo de registro.
1. Haga clic en **Editar**.

   ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. En el cuadro **Editar tipo de registro**, seleccione la ficha **Configuración avanzada**.
1. Habilite la opción **Permitir agregar este tipo de registro a otros espacios de trabajo**.

   ![Editar la configuración avanzada del tipo de registro con Agregar a otros espacios de trabajo habilita](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. En el campo **Seleccione quién puede agregar este tipo de registro a los espacios de trabajo que administra**, agregue los usuarios a los que desea permitir que agreguen este tipo de registro a los espacios de trabajo que administran.

   Su nombre se añade automáticamente en el campo.

   Puede agregar usuarios individuales o grupos, equipos, roles o empresas a cuyos usuarios desee permitir que agreguen este tipo de registro a los espacios de trabajo que administran.

   Puede editar este campo después de guardar el tipo de registro.
1. (Opcional) Elimine su nombre del campo **Seleccione quién puede agregar este tipo de registro a los espacios de trabajo que administran**.

1. Haga clic en **Guardar**.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para que las personas designadas lo añadan a otro espacio de trabajo.

   >[!NOTE]
   >
   >Sólo se puede editar el tipo de registro y sus campos desde el espacio de trabajo original.

   * La tarjeta de tipo de registro muestra un icono global ![icono de tipo de registro global](assets/global-icon.png) para indicar que el tipo de registro está disponible para agregarse a cualquier área de trabajo cuyo administrador haya designado en la configuración.
   * Se agrega un campo **Workspace** generado por el sistema al tipo de registro.

     El campo Workspace muestra el espacio de trabajo desde el que se ha creado cada registro.

     Este campo es de solo lectura y no se puede eliminar.

## Configurar la conexión a un tipo de registro desde otros espacios de trabajo

Puede configurar un tipo de registro al que conectarse desde otros espacios de trabajo al crear o editar el tipo de registro.

Para configurar un tipo de registro al que conectarse desde otros espacios de trabajo al editar el tipo de registro:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registro desee editar.

   Se abre la página del espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en el menú **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro; a continuación, haga clic en **Editar**
O
   * Haga clic en una tarjeta de tipo de registro para abrir la página de tipo de registro, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Editar**.

   ![Más opciones de menú de la tarjeta de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. En el cuadro **Editar tipo de registro**, seleccione la ficha **Configuración avanzada**.
1. Habilite la opción **Permitir la conexión a este tipo de registro en otros espacios de trabajo**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Editar pestaña de configuración avanzada de tipo de registro con la conexión habilitada desde otros espacios de trabajo](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Cuando está habilitado, el tipo de registro es accesible y se puede conectar desde otros espacios de trabajo.

1. Elija desde qué espacios de trabajo se puede acceder al tipo de registro. Elija entre las siguientes opciones:

   * **En todo el sistema**: los usuarios pueden conectarse a este tipo de registro desde todos los espacios de trabajo donde tengan permisos de administración.
   * **Espacios de trabajo específicos**: agregue los nombres de los espacios de trabajo a los que los administradores de espacios de trabajo pueden conectarse para este tipo de registro.
1. Haga clic en **Editar**.

   Ocurren lo siguiente:

   * El tipo de registro y sus campos ya están disponibles para conectarse desde los espacios de trabajo designados.
   * La tarjeta de tipo de registro muestra un icono de conexión entre espacios de trabajo ![icono de conexión entre espacios de trabajo](assets/connect-from-other-workspaces-icon.png) para indicar que el tipo de registro está disponible para conectarse desde cualquier espacio de trabajo que haya designado en su configuración.

   El tipo de registro está disponible para conectarse desde los espacios de trabajo designados.









