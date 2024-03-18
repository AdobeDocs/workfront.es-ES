---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de placas Adobe Workfront
description: Puede utilizar el conector de tableros de Adobe Workfront para automatizar los procesos en los tableros de Workfront y conectarlo a aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
source-git-commit: 074bcf15c61f9c0c75cebf774b15baf7fe383f35
workflow-type: tm+mt
source-wordcount: '2118'
ht-degree: 1%

---

# [!DNL Adobe Workfront] Módulos de tableros

>[!NOTE]
>
>Este conector está actualmente en versión beta.

Los tableros de Adobe Workfront son herramientas flexibles que permiten la colaboración en equipo al proporcionar acceso a un tablero compartido que contiene columnas y tarjetas.

Puede utilizar los módulos de Tableros de Adobe Workfront para leer o actualizar registros, realizar una llamada de API a la API de Tableros de Workfront o almacenar en déclencheur un escenario cuando se produzca una acción en un tablero.

Para obtener información general sobre los tableros de Workfront, consulte [Información general de tableros](/help/quicksilver/agile/boards-overview.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>
  <td> <p>Cualquiera</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td>
   <td> <p>Nuevo: estándar</p><p>O</p><p>Actual: [!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).
Módulos de tableros de Adobe Workfront y sus campos

## Requisitos previos

Debe tener configurado un tablero en Adobe Workfront para poder conectarse a él.

## Creación de una conexión a los paneles de Workfront

>[!NOTE]
>
>Puede utilizar una conexión de Workfront para conectarse a los tableros de Workfront o puede crear una conexión de tableros de Workfront independiente.

Para crear una conexión de Workfront Boards:

1. En cualquier [!DNL Adobe Workfront Boards] , haga clic en **[!UICONTROL Añadir]** situado junto al cuadro Conexión.

1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
          <td>
            <p>Escriba un nombre para esta conexión.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Entorno]</td>
          <td>Seleccione si desea conectarse a un entorno de producción o de no producción.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo]</td>
          <td>Seleccione si le importa conectarse a una cuenta de servicio o a una cuenta personal.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de cliente]<p>(Opcional)</p></td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Secreto de cliente]<p>(Opcional)</p></td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL Secreto de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL URL de autenticación]<p>(Opcional)</p></td>
          <td>Introduzca la dirección URL que utilizará su instancia de Workfront para autenticar esta conexión. <p>El valor predeterminado es <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Prefijo de host]</td>
          <td>Introduzca el prefijo de host.<p>El valor predeterminado es <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## Módulos de tableros de Adobe Workfront y sus campos

Al configurar los módulos de Tableros de Workfront, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, pueden mostrarse campos adicionales de Tableros de Workfront, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [tarjetas](#cards)
* [Tableros](#boards)
* [Columnas](#columns)
* [Etiquetas](#tags)
* [Otro](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### tarjetas

* [Añadir elemento de lista de comprobación](#add-checklist-item)
* [Agregar subtarea](#add-subtask)
* [Crear una tarjeta](#create-a-card)
* [Mover una tarjeta](#move-a-card)
* [Leer una tarjeta](#read-a-card)
* [Actualizar una tarjeta](#update-a-card)

#### Añadir elemento de lista de comprobación

Este módulo de acción agrega un elemento de lista de comprobación a la tarjeta especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de tarjeta]</td> 
   <td>Introduzca o asigne el ID de la tarjeta a la que desea agregar un elemento de lista de comprobación.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elementos de lista de comprobación]</td> 
   <td>Para cada elemento de la lista de comprobación que desee agregar, haga clic en Agregar elemento, escriba el nombre del elemento de la lista de comprobación y seleccione si el elemento se ha completado.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Agregar subtarea

Este módulo de acción agrega una subtarea a una tarjeta en los paneles. La tarjeta debe ser una tarjeta conectada. La subtarea también se agrega a la tarea de Workfront que representa la tarjeta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tarjeta principal]</td> 
   <td>Introduzca o asigne el ID de la tarjeta a la que desea agregar una subtarea.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero que contiene la tarjeta a la que desea agregar una subtarea.<p>Puede encontrar el ID del tablero en la URL cuando visualice el tablero en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre]</td> 
   <td>Escriba o asigne un nombre para la nueva subtarea.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Crear una tarjeta

Este módulo de acción crea una nueva tarjeta en un tablero de Workfront.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero al que desea agregar una tarjeta.<p>Puede encontrar el ID del tablero en la URL cuando visualice el tablero en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de columna]</td> 
   <td>Introduzca o asigne el ID de la columna a la que desea agregar una subtarea.<p>Puede encontrar el ID de la etiqueta en la información que devuelve el módulo Leer un tablero.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre]</td> 
   <td>Escriba o asigne un nombre para la nueva tarjeta.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Mover una tarjeta

Este módulo de acción mueve una tarjeta a una columna diferente en el mismo tablero.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de tarjeta]</td> 
   <td>Introduzca o asigne el ID de la tarjeta que desea mover.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero que contiene la tarjeta que desea mover.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de columna de destino]</td> 
   <td>Introduzca o asigne el ID de la columna a la que desea mover la tarjeta.<p>Puede encontrar el ID de la etiqueta en la información que devuelve el módulo Leer un tablero.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To index]</td> 
   <td>Introduzca o asigne la posición que desea que tenga la tarjeta en la nueva columna.<p>Posición superior de la columna en el índice 0.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Leer una tarjeta

Este módulo de acción recupera información sobre una tarjeta específica.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de tarjeta]</td> 
   <td>Introduzca o asigne el ID de la tarjeta que desea leer.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Actualizar una tarjeta

Este módulo de acción actualiza la información de una tarjeta especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de tarjeta]</td> 
   <td>Introduzca o asigne el ID de la tarjeta que desea actualizar.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero que contiene la tarjeta que desea actualizar.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre]</td> 
   <td>Escriba o asigne un nombre nuevo para la tarjeta.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de tarjeta]</td> 
   <td>Escriba o asigne una nueva descripción para la tarjeta/\.</p></td> 
  </tr> 
 </tbody> 
</table>

### Tableros

* [Crear un tablero](#create-a-board)
* [Leer un tablero](#read-a-board)

#### Crear un tablero

Este módulo de acción crea un tablero en Workfront. Puede especificar el tipo de tablero que desea crear.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de tablero]</td> 
   <td>Introduzca o asigne un nombre para el nuevo tablero.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo]</td> 
   <td>Seleccione el tipo de tablero que desea crear.</td> 
  </tr> 
 </tbody> 
</table>

#### Leer un tablero

Este módulo de acción devuelve información sobre un único tablero, como las tarjetas, columnas, etiquetas y miembros del tablero.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero para el que desea recuperar información.<p>Puede encontrar el ID del tablero en la URL cuando visualice el tablero en Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

### Columnas

#### Creación de una columna

Este módulo de acción crea una nueva columna en el tablero especificado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero al que desea agregar una columna.<p>Puede encontrar el ID del tablero en la URL cuando visualice el tablero en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de columna]</td> 
   <td>Introduzca o asigne un nombre para la nueva columna.</td> 
  </tr> 
 </tbody> 
</table>

### Etiquetas

* [Añadir una etiqueta a una tarjeta](#add-card-tag)
* [Creación de una etiqueta](#create-a-tag)

#### Añadir una etiqueta a una tarjeta

Este módulo de acción agrega una etiqueta a una tarjeta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de tarjeta]</td> 
   <td>Introduzca o asigne el ID de la tarjeta a la que desee agregar una etiqueta.<p>Puede encontrar el ID de la tarjeta en la dirección URL cuando la visualice en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero que contiene la tarjeta a la que desea agregar una etiqueta.<p>Puede encontrar el ID del tablero en la URL cuando visualice el tablero en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de etiqueta]</td> 
   <td>Introduzca o asigne el ID de la etiqueta que desee añadir.<p>Puede encontrar el ID de la etiqueta en la información que devuelve el módulo Leer un tablero.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Creación de una etiqueta

Este módulo de acción crea una etiqueta nueva y le asigna un color.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Id. de tablero]</td> 
   <td>Introduzca o asigne el ID del tablero para el que desea crear una etiqueta.<p>Puede encontrar el ID del tablero en la URL cuando visualice el tablero en Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de etiqueta]</td> 
   <td>Introduzca o asigne un nombre para la nueva etiqueta.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color de etiqueta]</td> 
   <td>Seleccione el color de esta etiqueta.</td> 
  </tr> 
 </tbody> 
</table>

### Otro

#### Realizar una llamada de API personalizada

Este módulo de acción realiza una llamada personalizada a la API de Workfront Boards.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
      <td> <p>Puede utilizar una conexión existente de Workfront para conectarse a los tableros de Workfront o puede utilizar una conexión específica de los tableros de Workfront. </p><p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Creación de una conexión a los paneles de Workfront</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Introduzca una ruta relativa a<code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p><p>Para la mayoría de las llamadas de tableros, el método es POST. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Determina el tipo de contenido de la solicitud.</p> <p>Por ejemplo,<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>En los paneles de Workfront, esta sección suele dejarse vacía.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de Graphql incrustado de JSON </p> <p>Ejemplo:</p><p>En este ejemplo se actualiza un nombre de columna. Puede incluir la variable <code>boardId</code> y <code>columnId</code> como GUID codificados o asignados desde un módulo anterior.<p><pre>{

  &quot;query&quot;: &quot;mutation { updateColumn(boardId: \&quot;\&quot;, columnId: \&quot;\&quot;, updateColumnInput: { name: \&quot;\&quot; }) { id name }}&quot;

}</pre><p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
