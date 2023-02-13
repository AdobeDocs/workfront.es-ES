---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos Trello
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan Trello, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5039'
ht-degree: 0%

---

# [!UICONTROL Trello] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!UICONTROL Trello], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!DNL Trello] módulos, debe tener un [!UICONTROL Trello] cuenta.

## Connect [!UICONTROL Trello] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar su [!UICONTROL Trello] cuenta para [!DNL Workfront Fusion], consulte [Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL Trello] módulos y sus campos

Al configurar [!UICONTROL Trello] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!UICONTROL Trello] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Tableros](#boards)
* [Listas](#lists)
* [Tarjetas](#cards)
* [Miembros](#members)
* [Listas de comprobación](#checklists)
* [Etiquetas](#labels)
* [Comentarios](#comments)

### Tableros

+++ **[!UICONTROL Tableros]**

Este módulo de déclencheur inicia un escenario cuando se agrega un tablero nuevo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>El número máximo de tableros [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear un tablero]**

Este módulo de acción crea un tablero nuevo con la configuración seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Introduzca o asigne un nombre para el tablero nuevo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td> <p>Introduzca o asigne la descripción del tablero si es necesario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de organización]</p> </td> 
   <td> <p>Introduzca o asigne el ID de la organización. El ID de organización se puede recuperar mediante otro módulo, como el módulo Actividades de observación .</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nivel de permiso]</p> </td> 
   <td> <p>Los tableros tienen diferentes reglas de votación y comentarios para cada nivel de permiso. Por ejemplo: si el tablero es [!UICONTROL Private] y establece las reglas de votación y comentarios como [!UICONTROL All], recibirá un error. </p> <p>Votar y comentar está limitado a los siguientes grupos para cada nivel de permiso:</p> 
    <ul> 
     <li><strong>[!UICONTROL Privado]</strong>: —&gt;Miembros, miembros y observadores</li> 
     <li><strong>[!UICONTROL Para la organización]</strong>: —&gt;Miembros, miembros y observadores, Miembros de la Organización</li> 
     <li><strong>[!UICONTROL Public]</strong>: —&gt;Miembros, Miembros y Observadores, Miembros de la Organización, Todos</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Votación]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede votar en este tablero. Consulte el campo [!UICONTROL Nivel de permiso] para conocer las limitaciones de voto en los niveles de permiso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comentarios]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede comentar las tarjetas de este tablero. Consulte el campo [!UICONTROL Nivel de permiso] para comentar las limitaciones de los niveles de permiso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitaciones]</p> </td> 
   <td> <p>Seleccione quién puede invitar a otras personas a este tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Autounión]</p> </td> 
   <td> <p>Seleccione si los integrantes del equipo pueden unirse a la junta ellos mismos o si tienen que ser invitados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Etiquetas predeterminadas]</p> </td> 
   <td> <p>Seleccione si desea utilizar el conjunto predeterminado de etiquetas para el tablero nuevo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Listas predeterminadas]</p> </td> 
   <td> <p>Seleccione si desea añadir el conjunto predeterminado de listas al tablero ([!UICONTROL To Do], [!UICONTROL Doing], [!UICONTROL Done]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board source ID]</p> </td> 
   <td> <p>Seleccione o asigne el ID del tablero que desea copiar en el tablero nuevo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tapas de tarjetas]</p> </td> 
   <td> <p>Select <strong>[!UICONTROL Sí]</strong> si desea habilitar las tapas de tarjeta para el tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Fondo]</p> </td> 
   <td> <p>Seleccione el color del fondo o el fondo personalizado.</p> <p>Nota: Los fondos personalizados solo están disponibles para los suscriptores de [!UICONTROL Trello Gold y Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>Seleccione entre dos modos de envejecimiento de la tarjeta. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Las tarjetas se vuelven cada vez más transparentes a medida que envejecen. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Las tarjetas se romperán, amarillentas y se romperán como un viejo mapa pirata a medida que envejecen.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar un tablero]**

Este módulo de acción edita la configuración de un tablero existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID exclusivo de [!UICONTROL Trello] del tablero que desea que cree el módulo. Puede recuperar el ID del tablero mediante otro módulo, como el módulo de tableros de observación</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre]</td> 
   <td> <p> Introduzca o asigne un nuevo nombre para el tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nueva descripción]</td> 
   <td> <p> Introduzca o asigne una nueva descripción del tablero si es necesario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de organización]</p> </td> 
   <td> <p>Introduzca o asigne el ID exclusivo de [!UICONTROL Trello] del tablero que desea que edite el módulo. Puede recuperar el ID del tablero mediante otro módulo, como el [!DNL Watch Activities] módulo.</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suscribirse] </td> 
   <td> <p>Seleccione una opción para especificar si el usuario interino está suscrito al tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nivel de permiso]</p> </td> 
   <td> <p>Los tableros tienen diferentes reglas de votación y comentarios para cada nivel de permiso. Por ejemplo: si el tablero es [!UICONTROL Private] y establece las reglas de votación y comentarios como [!UICONTROL All], recibirá un error. </p> <p>Votar y comentar está limitado a los siguientes grupos para cada nivel de permiso:</p> 
    <ul> 
     <li><strong>[!UICONTROL Privado]</strong>: —&gt;Miembros, miembros y observadores</li> 
     <li><strong>[!UICONTROL Para la organización]</strong>: —&gt;Miembros, miembros y observadores, Miembros de la Organización</li> 
     <li><strong>[!UICONTROL Public]</strong>: —&gt;Miembros, Miembros y Observadores, Miembros de la Organización, Todos</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Votación]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede votar en este tablero. Consulte el campo [!UICONTROL Nivel de permiso] para conocer las limitaciones de voto en los niveles de permiso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comentarios]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede comentar las tarjetas de este tablero. Consulte el campo [!UICONTROL Nivel de permiso] para comentar las limitaciones de los niveles de permiso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitaciones] </td> 
   <td> <p>Seleccione quién puede invitar a personas a este tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autounión]</td> 
   <td> <p> Seleccione si los integrantes del equipo pueden unirse a la junta ellos mismos o si tienen que ser invitados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cubiertas de tarjetas]</td> 
   <td> <p> Seleccione si las tapas de la tarjeta deben mostrarse en este tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fondo] </td> 
   <td> <p>Seleccione el color del fondo o el fondo personalizado.</p> <p>Nota: Los fondos personalizados solo están disponibles para los suscriptores de [!UICONTROL Trello Gold y Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background ID]</td> 
   <td> <p> Si ha seleccionado utilizar un fondo personalizado en el campo [!UICONTROL Fondo], introduzca o asigne el ID del fondo que desea utilizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>Seleccione entre dos modos de envejecimiento de la tarjeta. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Las tarjetas se vuelven cada vez más transparentes a medida que envejecen. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Las tarjetas se romperán, amarillentas y se romperán como un viejo mapa pirata a medida que envejecen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fuente del calendario habilitada]</td> 
   <td> <p> Seleccione si la fuente del calendario está activada o no.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;color&gt; label name]</td> 
   <td> <p> Asigne un nombre a la etiqueta de color que desee.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo] </td> 
   <td> <p>Seleccione una opción para indicar si desea archivar (cerrar) el tablero. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtener un tablero]**

Este módulo de acción recupera los detalles de un tablero.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID del tablero del que desea recuperar información.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Este módulo de búsqueda recupera información sobre un tablero que especifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Introduzca o asigne el nombre (o una parte del nombre) del tablero del que desea obtener información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de tableros devueltos]</td> 
   <td> <p> Especifique el número máximo de tableros [!DNL Workfront Fusion] volverá durante un ciclo de ejecución. Este valor debe ser menor o igual que 1000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL parcial] </p> </td> 
   <td> <p>De forma predeterminada, este módulo busca contenido de miembro para encontrar coincidencias exactas de cada palabra de la consulta. Cuando [!UICONTROL Parcial] está habilitado, el módulo busca contenido que comience con cualquier palabra de la consulta.</p> <p> Por ejemplo, si está utilizando la palabra "desarrollo" para buscar un tablero titulado "Mi informe de estado de desarrollo", de forma predeterminada tendría que buscar toda la palabra. Si tiene [!UICONTROL Parcial] habilitado, podría buscar "dev" pero no "desarrollo".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Boards] </td> 
   <td> <p>Introduzca "mine" o asigne una lista de ID de tablero separados por comas.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archivar o desarchivar un tablero]**

Este módulo de acción cierra o vuelve a abrir un tablero que especifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Introduzca o asigne el ID del tablero que desea cerrar o volver a abrir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivar o desarchivar]</td> 
   <td> <p> Seleccione si desea cerrar (archivar) o volver a abrir (desarchivar) el tablero.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Asignar un miembro a un tablero]**

Este módulo de acción asigna un miembro a un tablero que especifique .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Seleccione el tablero en el que desea agregar un miembro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico]</td> 
   <td> <p> Introduzca o asigne la dirección de correo electrónico del miembro que desea agregar al tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de miembro]</p> </td> 
   <td> <p>Seleccione el tipo de miembro que desea agregar al tablero.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>: Un administrador del tablero puede realizar cualquier acción del tablero.</li> 
     <li><strong>[!UICONTROL Normal]</strong>: Un miembro normal es simplemente un miembro de la junta.</li> 
     <li><strong>[!UICONTROL Observador]</strong>: Un observador es un miembro con acceso de sólo lectura a la junta. <br>Los observadores solo están disponibles para equipos con [!UICONTROL Trello Business Class].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre completo]</td> 
   <td> <p> Escriba el nombre completo del usuario que desea agregar al tablero.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Anular la asignación de un miembro de un tablero]**

Este módulo de acción elimina un miembro de un tablero.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Introduzca (asigne o seleccione) el ID del tablero del que desea quitar al usuario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Miembro] </td> 
   <td> <p>Seleccione el miembro que desea quitar del tablero.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listas

+++ **[!UICONTROL Ver tarjetas movidas a una lista]**

Este módulo de déclencheur se activa cuando una tarjeta se mueve a una lista específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>Seleccione el tablero que contiene la lista que desea ver para las tarjetas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>Seleccione la lista que desea ver para las tarjetas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>El número máximo de tarjetas [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear una lista]**

Este módulo de acción crea una lista en un tablero que especifique .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Introduzca o asigne el ID del tablero en el que desea crear una lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Introduzca o asigne un nombre para la nueva lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleccione si desea añadir la lista a la parte superior o anexarla a la parte inferior de la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy list]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la lista que desea copiar.</p> 
    <ul> 
     <li> <p><strong>Introducir manualmente</strong> </p> <p>En el <strong>[!UICONTROL List ID]</strong> , introduzca o asigne el ID de la lista que desea copiar.<br></p> </li> 
     <li> <p><strong>Seleccionar</strong> </p> <p>Seleccione el tablero que contiene la lista que desea copiar y, a continuación, seleccione la lista.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar una lista]**

Este módulo de acción edita una lista existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> Introduzca o asigne el ID de la lista que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Introduzca o asigne un nuevo nombre para la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Asigne o seleccione el tablero en el que desea mover la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleccione si desea añadir la lista a la parte superior o anexarla a la parte inferior de la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suscrito]</td> 
   <td> <p>Active esta opción si desea suscribir al miembro activo a la lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtener una lista]**

Este módulo de acción recupera detalles sobre una lista específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID de la lista de la que desea recuperar información.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Tarjetas

+++ **[!UICONTROL Tarjetas de observación]**

Este módulo de déclencheur se activa cuando se añade una tarjeta nueva.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objeto vigilado]</td> 
   <td> <p>Seleccione la ubicación que desea ver para las tarjetas.</p> 
    <ul> 
     <li><strong>[!UICONTROL Todas las tarjetas]</strong> </li> 
     <li> <p><strong>Tarjetas en tableros específicos</strong> </p> <p>Seleccione el tablero que desea ver para las tarjetas</p> </li> 
     <li> <p><strong>[!UICONTROL Tarjetas de la lista específica]</strong> </p> <p>Seleccione el tablero que contiene la lista que desea ver para las tarjetas y, a continuación, seleccione la lista.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>El número máximo de tarjetas [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear una tarjeta]**

Este módulo de acción crea una tarjeta en una lista seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir un ID de lista]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la lista donde desea añadir una tarjeta.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL List ID]</strong> , introduzca o asigne el ID de la lista donde desea añadir una tarjeta.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la lista que desea copiar y, a continuación, seleccione la lista.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas] </td> 
   <td> <p>Para cada etiqueta que desee agregar a la tarjeta, introduzca el ID de la etiqueta. El ID se puede recuperar, por ejemplo, mediante el módulo [!UICONTROL Recuperar etiquetas].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Miembros]</td> 
   <td>Para cada miembro que desee agregar a la tarjeta, introduzca el ID del miembro. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Escriba un nombre para la tarjeta nueva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Descripción]</p> </td> 
   <td> <p>Introduzca la descripción de la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleccione si desea añadir la tarjeta a la parte superior o [!UICONTROL anexar] la tarjeta a la parte inferior de la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de vencimiento]</td> 
   <td> <p> Introduzca una fecha de vencimiento para la tarjeta. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vence de completar]</td> 
   <td> <p> Active esta opción para marcar que la tarjeta se complete en la fecha de vencimiento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL del archivo]</td> 
   <td> <p>Introduzca o asigne la dirección URL de un archivo que desea agregar como datos adjuntos a la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivo de origen]</p> </td> 
   <td> <p>Introduzca o asigne información de un archivo que desea agregar como datos adjuntos a la tarjeta.</p> 
    <ul> 
     <li>[!UICONTROL Nombre de archivo]: Introduzca o asigne el nombre de archivo, incluida la extensión de archivo.</li> 
     <li> 
     <p>Seleccione un archivo de un módulo anterior o asigne el nombre y los datos del archivo</p> 
     <p>Nota: Hay un límite de carga de archivos de 10 MB por archivo adjunto. Sin embargo, los miembros [!UICONTROL Business Class] y [!UICONTROL Trello Gold] tienen un límite de carga de archivos de 250 MB por archivo adjunto.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy card]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta que desea copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta que desea copiar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta que desea copiar, luego seleccione la lista que contiene la tarjeta y luego seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar una tarjeta]**

Este módulo de acción edita una tarjeta existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta que desea editar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta que desea editar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta que desea editar, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre]</td> 
   <td> <p>Escriba o asigne un nuevo nombre para la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nueva descripción]</p> </td> 
   <td> <p>Introduzca o asigne una nueva descripción para la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Mover una tarjeta]</p> </td> 
   <td> <p>Seleccione el tablero o el tablero y la lista donde desea mover la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas] </td> 
   <td> <p>Agregue los ID de cualquier etiqueta que desee agregar a la tarjeta. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleccione si desea añadir la tarjeta a la parte superior o [!UICONTROL anexar] la tarjeta a la parte inferior de la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de vencimiento]</td> 
   <td> <p> Introduzca una fecha de vencimiento para la tarjeta. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vence de completar]</td> 
   <td> <p> Si esta opción está habilitada, la tarjeta se marca como completada en la fecha de vencimiento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Miembros] </td> 
   <td> <p>Agregue o asigne el ID de los miembros que desee agregar a la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de la tapa de los archivos adjuntos]</p> </td> 
   <td> <p>Introduzca o asigne el ID del archivo adjunto de imagen que desea que utilice la tarjeta como portada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suscribirse] </td> 
   <td> <p>Seleccione si el miembro debe suscribirse a la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo] </td> 
   <td> <p>Seleccione una opción para indicar si desea archivar (cerrar) la tarjeta. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtener una tarjeta]**

Este módulo de acción recupera los detalles de una tarjeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p>Introduzca el ID del tablero que contiene la tarjeta de la que desea recuperar los detalles. Esto le permite ver los nombres de los campos personalizados del tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta de la que desea recuperar los detalles.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta de la que desea recuperar detalles.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta de la que desea recuperar detalles, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Buscar tarjetas]**

Este módulo de acción devuelve tarjetas que coinciden con la consulta de búsqueda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>Seleccione los tableros que desee buscar. Si no hay ningún tablero seleccionado, se buscarán todos los tableros.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Query]</p> </td> 
   <td> <p>Introduzca la consulta de búsqueda. Puede restringir la búsqueda utilizando los siguientes operadores de búsqueda:</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>Puede agregar "-" a cualquier operador para realizar una búsqueda negativa, como <code>[!UICONTROL -has:members]</code> para buscar tarjetas sin ningún miembro asignado.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Devuelve tarjetas asignadas a un miembro. También puede utilizar <code>member:</code>. Uso <code>@me</code> para incluir solo sus tarjetas.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Devuelve las tarjetas etiquetadas. También puede utilizar <code>label:</code>. Por ejemplo, <code>label:"FIX IT"</code> devolverá tarjetas con la etiqueta denominada "FIX IT".</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Devuelve tarjetas dentro de un tablero específico. Por ejemplo, <code>board:Trello</code> devolverá tarjetas en tableros con [!UICONTROL Trello] en el nombre del tablero.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Devuelve tarjetas de la lista denominada "name".</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Devuelve tarjetas con archivos adjuntos. La variable <code>has</code>: también se puede usar con otros atributos, como <code>has:description</code>, <code>has:cover</code>, <code>has:members</code>o <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Devuelve las tarjetas que vencen en un plazo de 24 horas. La variable <code>due:</code> también se puede usar con otros marcos de tiempo, como <code>due:week</code>, <code>due:month</code>o <code>due:overdue</code>. También puede buscar un intervalo de días específico. Por ejemplo, añadir <code>due:14</code> para buscar incluye tarjetas que vencen en los próximos 14 días.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Devuelve tarjetas creadas en las últimas 24 horas. La variable<code> created:</code> también se puede usar con otros marcos de tiempo como <code>created:week</code> o <code>created:month</code>. También puede buscar un intervalo de días específico. Por ejemplo, añadir <code>created:14</code> a la búsqueda incluye las tarjetas creadas en los últimos 14 días.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Devuelve tarjetas editadas en las últimas 24 horas. La variable <code>edited:</code> también se puede usar con otros marcos de tiempo, como <code>edited:week</code> o <code>edited:month</code>. También puede buscar un intervalo de días específico. Por ejemplo, añadir <code>edited:21</code> a la búsqueda incluye tarjetas editadas en los últimos 21 días.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Devuelve las tarjetas que coinciden con el texto de las descripciones de tarjetas, listas de comprobación, comentarios o nombres. Por ejemplo, comentario: "CORREGIR TI" devolverá tarjetas con "CORREGIR TI" en un comentario.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Devuelve tarjetas abiertas o archivadas. Si no se especifica ninguna de estas opciones, [!UICONTROL Trello] devuelve ambos tipos.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Sólo incluye tarjetas en tableros estelares.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de tarjetas devueltas]</td> 
   <td> <p> El número máximo de tarjetas [!DNL Workfront Fusion] volverá durante un ciclo de ejecución. Este valor debe ser menor o igual que 1000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL parcial] </td> 
   <td> <p>De forma predeterminada, este módulo busca contenido de miembro para encontrar coincidencias exactas de cada palabra de la consulta. Cuando [!UICONTROL Parcial] está habilitado, el módulo busca contenido que comience con cualquier palabra de la consulta.</p> <p> Por ejemplo, si está utilizando la palabra "desarrollo" para buscar un tablero titulado "Mi informe de estado de desarrollo", de forma predeterminada tendría que buscar toda la palabra. Si tiene [!UICONTROL Parcial] habilitado, podría buscar "dev" pero no "desarrollo".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cards] </td> 
   <td> <p>Añada las tarjetas que quiera buscar específicamente.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archivar o desarchivar una tarjeta]**

Este módulo de acción archiva o envía una tarjeta de vuelta al tablero.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card ID]</td> 
   <td> <p> Introduzca o asigne el ID de la tarjeta que desea archivar o devolver al tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivar o desarchivar]</td> 
   <td> <p> Seleccione si desea cerrar la tarjeta (archivar) o enviarla de nuevo al tablero (desarchivar).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Añadir un archivo adjunto]**

Este módulo de acción agrega un archivo adjunto a la tarjeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta de la que desea recuperar los detalles.</p> 
    <ul> 
     <li> <p><strong>Introducir manualmente</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta de la que desea recuperar detalles.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta de la que desea recuperar detalles, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de archivo adjunto]</p> </td> 
   <td> <p>Seleccione si desea cargar el archivo directamente o proporcionar una URL al archivo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Archivo]</strong> </p> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Introduzca la dirección URL del archivo y proporcione un nombre para el archivo adjunto.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Miembros

+++ **[!UICONTROL Asignar un miembro a un tablero]**

Consulte &quot;[!UICONTROL Asignar un miembro a un tablero]&quot; [Tableros](#boards).

+++

+++ **[!UICONTROL Anular la asignación de un miembro de un tablero]**

Consulte &quot;[!UICONTROL Anular la asignación de un miembro de un tablero]&quot; [Tableros](#boards).

+++

+++ **[!UICONTROL Agregar un miembro a una tarjeta]**

Este módulo de acción agrega el miembro especificado a la tarjeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Introducir ID de tarjeta e ID de miembro]</p> </td> 
   <td> <p>Elija cómo desea introducir el ID de tarjeta y el ID de miembro.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne la variable <strong>[!UICONTROL Card ID]</strong> y <strong>[!UICONTROL Member ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta a la que desea agregar un miembro y, a continuación, seleccione la lista que contiene la tarjeta, la tarjeta en sí y el miembro que desea agregar a la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Buscar miembros]**

Este módulo de acción recupera información sobre [!UICONTROL Trello] miembros.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Introduzca el nombre completo o el nombre de usuario del usuario que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL parcial] </td> 
   <td> <p>De forma predeterminada, este módulo busca contenido de miembro para encontrar coincidencias exactas de cada palabra de la consulta. Cuando [!UICONTROL Parcial] está habilitado, el módulo busca contenido que comience con cualquier palabra de la consulta.</p> <p> Por ejemplo, si está utilizando la palabra "desarrollo" para buscar un tablero titulado "Mi informe de estado de desarrollo", de forma predeterminada tendría que buscar toda la palabra. Si tiene [!UICONTROL Parcial] habilitado, podría buscar "dev" pero no "desarrollo".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de miembros devueltos]</td> 
   <td> <p> El número máximo de miembros [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listas de comprobación

+++ **[!UICONTROL Crear una lista de comprobación]**

Este módulo de acción crea una lista de comprobación en la tarjeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Especifique un ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea agregar una lista de comprobación.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta donde desea agregar una lista de comprobación.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Introduzca o asigne un nombre para la lista de comprobación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Seleccione si desea agregar la lista de comprobación a la parte superior o la lista de comprobación [!UICONTROL anexe la] al final de la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Introducir ID de lista de comprobación]</p> </td> 
   <td> <p>Introduzca o asigne el ID de una lista de comprobación de origen que desea copiar en la nueva.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear un elemento de lista de comprobación]**

Este módulo de acción agrega un elemento a una lista de comprobación específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de lista de comprobación]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la lista de comprobación en la que desea añadir un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Checklist ID]</strong> , introduzca o asigne el ID de la tarjeta donde desea agregar una lista de comprobación.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta, luego seleccione la tarjeta y, a continuación, seleccione la lista de comprobación.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nombre del elemento]</p> </td> 
   <td> <p>Escriba o asigne un nombre para el nuevo artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Seleccione si desea agregar el elemento a la parte superior o [!UICONTROL anexar] a la parte inferior de la lista de comprobación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL activado]</p> </td> 
   <td> <p>Active esta opción si desea agregar el elemento como está marcado.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar un elemento de lista de comprobación]**

Este módulo de acción edita una lista de comprobación existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introduzca un ID de tarjeta y un ID de elemento de lista de comprobación]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta y la lista de comprobación en la que desea editar un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Checklist ID]</strong> , introduzca o asigne el ID de la tarjeta donde desea agregar una lista de comprobación.</p> <p>En el <strong>[!UICONTROL Lista de comprobación ID de elemento]</strong> , introduzca o asigne el ID de la lista de comprobación.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta, luego seleccione la tarjeta y, a continuación, seleccione la lista de comprobación.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Checklist ID]</td> 
   <td>Seleccione o asigne la lista de comprobación a la que desea mover el elemento de la lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nombre del elemento]</p> </td> 
   <td> <p>Escriba o asigne un nombre para el nuevo artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Seleccione si desea agregar el elemento a la parte superior o anexar a la parte inferior de la lista de comprobación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>Seleccione si el elemento de la lista de comprobación está completo o incompleto.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Etiquetas

+++ **[!UICONTROL Agregar una etiqueta a una tarjeta]**

Este módulo de acción agrega una etiqueta a una tarjeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea agregar una lista de comprobación.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta donde desea agregar una lista de comprobación. En el<strong>[!UICONTROL Label ID]</strong> , introduzca o asigne el ID de la etiqueta que desea añadir.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta. </p> <p>Seleccione la etiqueta que desea agregar a la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Comentarios

+++ **[!UICONTROL Observar comentarios]**

Recupera detalles de comentarios cuando hay un comentario nuevo en una ubicación especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objeto vigilado]</td> 
   <td> <p>Seleccione la ubicación que desee ver para los comentarios.</p> 
    <ul> 
     <li><strong>[!UICONTROL Todas las tarjetas] en todas partes</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>Seleccione el tablero que desea ver para los comentarios</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>Seleccione el tablero que contiene la lista que desea ver para los comentarios y, a continuación, seleccione la lista.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>Seleccione el tablero que contiene la tarjeta que desea ver para comentarios, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>El número máximo de comentarios [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear un comentario en una tarjeta]**

Este módulo de acción agrega un comentario a una tarjeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Especifique un ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea agregar un comentario.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta en la que desea agregar un comentario.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta en la que desea agregar un comentario, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentario] </td> 
   <td> <p>Escriba el comentario que desea agregar a la tarjeta seleccionada.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Enumerar comentarios en una tarjeta]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Especifique un ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea agregar un comentario.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el <strong>[!UICONTROL Card ID]</strong> , introduzca o asigne el ID de la tarjeta en la que desea agregar un comentario.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta en la que desea agregar un comentario, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de comentarios devueltos]</td> 
   <td> <p> Escriba el número máximo de comentarios [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since] </td> 
   <td> <p>Establezca la fecha de inicio del periodo en el que se creó el comentario. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antes] </td> 
   <td> <p>Defina la fecha de finalización del periodo en el que se creó el comentario. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Trello] ID de objeto

* [Cómo encontrar el ID o el vínculo corto de una tarjeta en [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Búsqueda de ID de otros objetos en [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### Cómo encontrar el ID o el vínculo corto de una tarjeta en [!DNL Trello]

Si desea editar una tarjeta o crear un comentario nuevo, debe saber el ID de la tarjeta o su vínculo corto. Puede obtener esta información de la salida de la variable [!UICONTROL Nueva tarjeta] déclencheur. El enlace corto para una tarjeta también se puede obtener abriendo la tarjeta y haciendo clic en el botón [!UICONTROL Compartir] botón. El enlace corto se puede encontrar en la [!UICONTROL Vínculo a esta tarjeta] , al final de la dirección URL después de `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Búsqueda de ID de otros objetos en [!DNL Trello]

Los ID de tablero, lista y comentario solo se pueden obtener mediante déclencheur. La variable [!DNL trello.com] El sitio web no muestra estos ID.
