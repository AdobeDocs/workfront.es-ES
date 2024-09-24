---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Trello
description: En un escenario  [!DNL Adobe Workfront Fusion] puede automatizar los flujos de trabajo que utilizan Trello, así como conectarlo a múltiples aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 16cd5dee183153540bcccea8ce469a461d0e8562
workflow-type: tm+mt
source-wordcount: '5095'
ht-degree: 0%

---

# [!UICONTROL Trello] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que usan [!UICONTROL Trello], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar módulos de [!DNL Trello], debes tener una cuenta de [!UICONTROL Trello].

## Conectar [!UICONTROL Trello] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar tu cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], consulta [Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL Trello] módulos y sus campos

Al configurar los módulos [!UICONTROL Trello], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!UICONTROL campos Trello] adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Tableros](#boards)
* [Listas](#lists)
* [Tarjetas](#cards)
* [Miembros](#members)
* [Listas de comprobación](#checklists)
* [Etiquetas](#labels)
* [Comentarios](#comments)

### Tableros

+++ **[!UICONTROL Tableros de observación]**

Este módulo de déclencheur inicia un escenario cuando se añade un nuevo tablero.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>El número máximo de tableros [!DNL Workfront Fusion] se devolverá durante un ciclo de ejecución.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca o asigne un nombre para el nuevo tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td> <p>Introduzca o asigne la descripción del tablero si es necesario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de organización]</p> </td> 
   <td> <p>Introduzca o asigne el ID de la organización. El ID de organización se puede recuperar mediante otro módulo, como el módulo Actividades de observación.</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nivel de permiso]</p> </td> 
   <td> <p>Los tableros tienen diferentes reglas de votación y comentarios para cada nivel de permiso. Por ejemplo: si el tablero es [!UICONTROL Private] y establece las reglas de votación y comentarios como [!UICONTROL All], recibirá un error. </p> <p>Votar y comentar está limitado a los siguientes grupos para cada nivel de permiso:</p> 
    <ul> 
     <li><strong>[!UICONTROL Privado]</strong>: 
      —&gt;Miembros, miembros y observadores</li> 
     <li><strong>[!UICONTROL Para la organización]</strong>: 
      —&gt;Miembros, miembros y observadores, miembros de la organización</li> 
     <li><strong>[!UICONTROL Público]</strong>: 
      —&gt;Miembros, Miembros y observadores, Miembros de la organización, Todos</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede votar en este tablero. Consulte el campo [!UICONTROL Nivel de permiso] para ver las limitaciones de voto en los niveles de permisos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comentarios]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede realizar comentarios en las tarjetas de este tablero. Consulte el campo [!UICONTROL nivel de permisos] para comentar las limitaciones de los niveles de permisos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitaciones]</p> </td> 
   <td> <p>Seleccione quién puede invitar a otras personas a este tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Self-join]</p> </td> 
   <td> <p>Seleccione si los integrantes del equipo pueden unirse al tablero ellos mismos o si tienen que ser invitados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Etiquetas predeterminadas]</p> </td> 
   <td> <p>Seleccione si desea utilizar el conjunto predeterminado de etiquetas para el nuevo tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Listas predeterminadas]</p> </td> 
   <td> <p>Seleccione si desea agregar el conjunto predeterminado de listas al tablero ([!UICONTROL Tareas pendientes], [!UICONTROL Tareas pendientes], [!UICONTROL Listo]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Id. de origen de tablero]</p> </td> 
   <td> <p>Seleccione o asigne el ID del tablero que desea copiar en el nuevo tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cubiertas de tarjeta]</p> </td> 
   <td> <p>Seleccione <strong>[!UICONTROL Yes]</strong> si desea habilitar las cubiertas de tarjeta para el tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Fondo]</p> </td> 
   <td> <p>Seleccione el color del fondo o el fondo personalizado.</p> <p>Nota: los fondos personalizados solo están disponibles para suscriptores de [!UICONTROL Trello Gold y Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Antigüedad de tarjeta]</p> </td> 
   <td> <p>Seleccione entre dos modos de caducidad de la tarjeta. </p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong>: Las tarjetas se vuelven cada vez más transparentes a medida que envejecen. </li> 
     <li><strong>[!UICONTROL Pirata]</strong>: Las cartas se rasgarán, se pondrán amarillas y se agrietarán como un viejo mapa pirata a medida que envejezcan.</li> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Id. de tablero]</p> </td> 
   <td> <p>Introduzca o asigne el ID [!UICONTROL Trello] único del tablero que desea que cree el módulo. Puede recuperar el ID de tablero con otro módulo, como el módulo Tableros de inspección</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre]</td> 
   <td> <p> Introduzca o asigne un nombre nuevo para el tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción nueva]</td> 
   <td> <p> Introduzca o asigne una nueva descripción de tablero si es necesario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de organización]</p> </td> 
   <td> <p>Introduzca o asigne el ID [!UICONTROL Trello] único del tablero que desea que edite el módulo. Puede recuperar el ID de tablero mediante otro módulo, como el módulo [!DNL Watch Activities].</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suscribirse] </td> 
   <td> <p>Seleccione una opción para especificar si el usuario interino está suscrito al tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nivel de permiso]</p> </td> 
   <td> <p>Los tableros tienen diferentes reglas de votación y comentarios para cada nivel de permiso. Por ejemplo: si el tablero es [!UICONTROL Private] y establece las reglas de votación y comentarios como [!UICONTROL All], recibirá un error. </p> <p>Votar y comentar está limitado a los siguientes grupos para cada nivel de permiso:</p> 
    <ul> 
     <li><strong>[!UICONTROL Privado]</strong>: 
      —&gt;Miembros, miembros y observadores</li> 
     <li><strong>[!UICONTROL Para la organización]</strong>: 
      —&gt;Miembros, miembros y observadores, miembros de la organización</li> 
     <li><strong>[!UICONTROL Público]</strong>: 
      —&gt;Miembros, Miembros y observadores, Miembros de la organización, Todos</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede votar en este tablero. Consulte el campo [!UICONTROL Nivel de permiso] para ver las limitaciones de voto en los niveles de permisos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comentarios]</p> </td> 
   <td> <p>Seleccione una opción para especificar quién puede realizar comentarios en las tarjetas de este tablero. Consulte el campo [!UICONTROL nivel de permisos] para comentar las limitaciones de los niveles de permisos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitaciones] </td> 
   <td> <p>Seleccione quién puede invitar a personas a este tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-join]</td> 
   <td> <p> Seleccione si los integrantes del equipo pueden unirse al tablero ellos mismos o si tienen que ser invitados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cubiertas de tarjeta]</td> 
   <td> <p> Seleccione si las cubiertas de tarjeta deben mostrarse en este tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fondo] </td> 
   <td> <p>Seleccione el color del fondo o el fondo personalizado.</p> <p>Nota: los fondos personalizados solo están disponibles para suscriptores de [!UICONTROL Trello Gold y Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de fondo]</td> 
   <td> <p> Si ha seleccionado utilizar un fondo personalizado en el campo [!UICONTROL Fondo], introduzca o asigne el ID del fondo que desea utilizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Antigüedad de tarjeta]</p> </td> 
   <td> <p>Seleccione entre dos modos de caducidad de la tarjeta. </p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong>: Las tarjetas se vuelven cada vez más transparentes a medida que envejecen. </li> 
     <li><strong>[!UICONTROL Pirata]</strong>: Las cartas se rasgarán, se pondrán amarillas y se agrietarán como un viejo mapa pirata a medida que envejezcan.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fuente de calendario habilitada]</td> 
   <td> <p> Seleccione si la fuente del calendario está habilitada o no.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Color&gt; nombre de etiqueta]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Id. de tablero]</p> </td> 
   <td> <p>Introduzca o asigne el ID del tablero sobre el que desea recuperar información.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Este módulo de búsqueda recupera información sobre un tablero que usted especifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta] </td> 
   <td> <p>Introduzca o asigne el nombre (o una parte del nombre) del tablero sobre el que desea obtener información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de tableros devueltos]</td> 
   <td> <p> Introduzca el número máximo de tableros que devolverá [!DNL Workfront Fusion] durante un ciclo de ejecución. Este valor debe ser inferior o igual a 1000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parcial] </p> </td> 
   <td> <p>De forma predeterminada, este módulo busca coincidencias exactas de cada palabra de la consulta en el contenido de los miembros. Cuando [!UICONTROL Partial] está habilitado, el módulo busca contenido que comience con cualquier palabra de la consulta.</p> <p> Por ejemplo, si está utilizando la palabra "desarrollo" para buscar un tablero llamado "Mi informe de estado de desarrollo", de forma predeterminada deberá buscar la palabra completa. Si tiene [!UICONTROL Parcial] habilitado, podrá buscar "dev" pero no "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tableros] </td> 
   <td> <p>Escriba "mío" o asigne una lista de ID de tablero separados por comas.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archivar o desarchivar un tablero]**

Este módulo de acción cierra o vuelve a abrir un tablero especificado por el usuario

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de tablero]</td> 
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

Este módulo de acción asigna un miembro al tablero que especifique

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de tablero]</td> 
   <td> <p> Seleccione el tablero en el que desea agregar un miembro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico]</td> 
   <td> <p> Escriba o asigne la dirección de correo electrónico del miembro que desea agregar al tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de miembro]</p> </td> 
   <td> <p>Seleccione el tipo de miembro que desea añadir al tablero.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>: un administrador del tablero puede realizar cualquier acción en el tablero.</li> 
     <li><strong>[!UICONTROL Normal]</strong>: un miembro normal es simplemente un miembro del tablero.</li> 
     <li><strong>[!UICONTROL Observer]</strong>: Observer es un miembro con acceso de solo lectura al tablero. <br>Los observadores sólo están disponibles para los equipos con [!UICONTROL Trello Business Class].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre completo]</td> 
   <td> <p> Introduzca el nombre completo del usuario que desea agregar al tablero.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Anular la asignación de un miembro del tablero]**

Este módulo de acción elimina un miembro de un tablero.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de tablero]</td> 
   <td> <p> Introduzca (asigne o seleccione) el ID del tablero desde el que desea eliminar al usuario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Miembro] </td> 
   <td> <p>Seleccione el miembro que desea eliminar del tablero.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listas

+++ **[!UICONTROL Ver tarjetas trasladadas a una lista]**

Este módulo de déclencheur se activa cuando se mueve una tarjeta a una lista específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tablero]</td> 
   <td>Seleccione el tablero que contiene la lista que desea ver para las tarjetas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lista]</td> 
   <td>Seleccione la lista que desea ver para las tarjetas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>El número máximo de tarjetas [!DNL Workfront Fusion] se devolverá durante un ciclo de ejecución.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear una lista]**

Este módulo de acción crea una lista en un tablero que especifique

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de tablero]</td> 
   <td> <p> Introduzca o asigne el ID del tablero en el que desea crear una lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca o asigne un nombre para la nueva lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posición] </td> 
   <td> <p>Seleccione si desea agregar la lista al principio o anexarla al final de la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lista de copias]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la lista que desea copiar.</p> 
    <ul> 
     <li> <p><strong>Introducir manualmente</strong> </p> <p>En el campo <strong>[!UICONTROL List ID]</strong>, escriba o asigne el identificador de la lista que desea copiar.<br></p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> Introduzca o asigne el ID de la lista que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca o asigne un nuevo nombre para la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de tablero]</td> 
   <td> <p> Asigne o seleccione el tablero al que desea mover la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posición] </td> 
   <td> <p>Seleccione si desea agregar la lista al principio o anexarla al final de la tarjeta.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID de la lista de la que desea recuperar información.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Tarjetas

+++ **[!UICONTROL Ver tarjetas]**

Este módulo de déclencheur se activa cuando se añade una tarjeta nueva.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objeto inspeccionado]</td> 
   <td> <p>Seleccione la ubicación en la que desea ver las tarjetas.</p> 
    <ul> 
     <li><strong>[!UICONTROL Todas las tarjetas]</strong> </li> 
     <li> <p><strong>Tarjetas en tablero específico</strong> </p> <p>Seleccione el tablero que desea ver para las tarjetas</p> </li> 
     <li> <p><strong>[!UICONTROL Tarjetas en la lista específica]</strong> </p> <p>Seleccione el tablero que contiene la lista que desea inspeccionar para buscar tarjetas y, a continuación, seleccione la lista.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>El número máximo de tarjetas [!DNL Workfront Fusion] se devolverá durante un ciclo de ejecución.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de lista]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la lista donde desea agregar una tarjeta.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL List ID]</strong>, escriba o asigne el ID de la lista a la que desea agregar una tarjeta.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la lista que desea copiar y, a continuación, seleccione la lista.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas] </td> 
   <td> <p>Para cada etiqueta que desee agregar a la tarjeta, introduzca el ID de la etiqueta. El ID se puede recuperar, por ejemplo, mediante el módulo [!UICONTROL Retrieve Labels].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Miembros]</td> 
   <td>Para cada miembro que desee agregar a la tarjeta, escriba el ID del miembro. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Escriba un nombre para la tarjeta nueva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Descripción]</p> </td> 
   <td> <p>Escriba la descripción de la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posición] </td> 
   <td> <p>Seleccione si desea agregar la tarjeta al principio o [!UICONTROL anexar] la tarjeta al final de la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de vencimiento]</td> 
   <td> <p> Escriba una fecha límite para la tarjeta. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vencimiento completado]</td> 
   <td> <p> Active esta opción para marcar que la tarjeta está completa en la fecha de vencimiento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL de archivo]</td> 
   <td> <p>Introduzca o asigne la dirección URL del archivo que desee agregar como datos adjuntos a la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL archivo Source]</p> </td> 
   <td> <p>Escriba o asigne información para un archivo que desee agregar como datos adjuntos a la tarjeta.</p> 
    <ul> 
     <li>[!UICONTROL Nombre de archivo]: escriba o asigne el nombre de archivo, incluida la extensión.</li> 
     <li> 
     <p>Seleccione un archivo de un módulo anterior o asigne el nombre y los datos del archivo</p> 
     <p>Nota: Hay un límite de carga de archivos de 10 MB por archivo adjunto. Sin embargo, los miembros de [!UICONTROL Business Class] y [!UICONTROL Trello Gold] tienen un límite de carga de archivos de 250 MB por archivo adjunto.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta que desea copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL ID de tarjeta]</strong>, escriba o asigne el ID de la tarjeta que desea copiar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta que desea copiar y, a continuación, seleccione la lista que contiene la tarjeta. A continuación, seleccione la tarjeta.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta que desea editar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL ID de tarjeta]</strong>, escriba o asigne el ID de la tarjeta que desea editar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta que desea editar, seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre]</td> 
   <td> <p>Escriba o asigne un nombre nuevo para la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Descripción nueva]</p> </td> 
   <td> <p>Escriba o asigne una nueva descripción para la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Mover una tarjeta]</p> </td> 
   <td> <p>Seleccione el tablero o el tablero y enumere dónde desea mover la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas] </td> 
   <td> <p>Agregue los ID de las etiquetas que desee agregar a la tarjeta. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posición] </td> 
   <td> <p>Seleccione si desea agregar la tarjeta al principio o [!UICONTROL anexar] la tarjeta al final de la lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de vencimiento]</td> 
   <td> <p> Escriba una fecha límite para la tarjeta. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vencimiento completado]</td> 
   <td> <p> Si esta opción está habilitada, la tarjeta se marca como completada en la fecha de vencimiento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Miembros] </td> 
   <td> <p>Agregue o asigne el ID de cualquier miembro que desee agregar a la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Id. de portada de datos adjuntos]</p> </td> 
   <td> <p>Introduzca o asigne el ID del archivo adjunto de imagen que desea que la tarjeta use como portada.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de tablero]</td> 
   <td> <p>Introduzca el ID del tablero que contiene la tarjeta sobre la que desea recuperar los detalles. Esto le permite ver los nombres de los campos personalizados del tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta cuyos detalles desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL ID de tarjeta]</strong>, escriba o asigne el ID de la tarjeta cuyos detalles desee recuperar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta sobre la que desea recuperar los detalles, seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tablero] </td> 
   <td> <p>Seleccione los tableros en los que quiera buscar. Si no se ha seleccionado ningún tablero, se buscarán todos los tableros.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Consulta]</p> </td> 
   <td> <p>Introduzca la consulta de búsqueda. Puede restringir la búsqueda mediante los siguientes operadores de búsqueda:</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>Puede agregar "-" a cualquier operador para realizar una búsqueda negativa, como <code>[!UICONTROL -has:members]</code> para buscar tarjetas sin ningún miembro asignado.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Devuelve las tarjetas asignadas a un miembro. También puede usar <code>member:</code>. Use <code>@me</code> para incluir solamente sus tarjetas.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Devuelve tarjetas etiquetadas. También puede usar <code>label:</code>. Por ejemplo, <code>label:"FIX IT"</code> devolverá tarjetas con la etiqueta "FIX IT".</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Devuelve tarjetas dentro de un tablero específico. Por ejemplo, <code>board:Trello</code> devolverá tarjetas en tableros con [!UICONTROL Trello] en el nombre del tablero.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Devuelve tarjetas dentro de la lista llamada "nombre".</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Devuelve tarjetas con datos adjuntos. El operador <code>has</code>: también se puede usar con otros atributos, como <code>has:description</code>, <code>has:cover</code>, <code>has:members</code> o <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Devuelve las tarjetas con vencimiento en 24 horas. El operador <code>due:</code> también se puede usar con otros marcos de tiempo, como <code>due:week</code>, <code>due:month</code> o <code>due:overdue</code>. También puede buscar un intervalo de días específico. Por ejemplo, si se agrega <code>due:14</code> a la búsqueda, se incluirán las tarjetas que vencen en los próximos 14 días.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Devuelve las tarjetas creadas en las últimas 24 horas. El operador <code> created:</code> también se puede usar con otros marcos de tiempo como <code>created:week</code> o <code>created:month</code>. También puede buscar un intervalo de días específico. Por ejemplo, al agregar <code>created:14</code> a la búsqueda se incluyen las tarjetas creadas en los últimos 14 días.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Devuelve las tarjetas editadas en las últimas 24 horas. El operador <code>edited:</code> también se puede usar con otros marcos de tiempo, como <code>edited:week</code> o <code>edited:month</code>. También puede buscar un intervalo de días específico. Por ejemplo, agregar <code>edited:21</code> a la búsqueda incluye tarjetas editadas en los últimos 21 días.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Devuelve tarjetas que coinciden con el texto de las descripciones, listas de comprobación, comentarios o nombres de las tarjetas. Por ejemplo, el comentario: "CORREGIRLO" devolverá tarjetas con "CORREGIRLO" en un comentario.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Devuelve las tarjetas abiertas o archivadas. Si no se especifica ninguno, [!UICONTROL Trello] devuelve ambos tipos.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Solo incluye tarjetas en tableros con estrellas.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de tarjetas devueltas]</td> 
   <td> <p> El número máximo de tarjetas [!DNL Workfront Fusion] se devolverá durante un ciclo de ejecución. Este valor debe ser inferior o igual a 1000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parcial] </td> 
   <td> <p>De forma predeterminada, este módulo busca coincidencias exactas de cada palabra de la consulta en el contenido de los miembros. Cuando [!UICONTROL Partial] está habilitado, el módulo busca contenido que comience con cualquier palabra de la consulta.</p> <p> Por ejemplo, si está utilizando la palabra "desarrollo" para buscar un tablero llamado "Mi informe de estado de desarrollo", de forma predeterminada deberá buscar la palabra completa. Si tiene [!UICONTROL Parcial] habilitado, podrá buscar "dev" pero no "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tarjetas] </td> 
   <td> <p>Añada las tarjetas que desee buscar específicamente.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archivar o desarchivar una tarjeta]**

Este módulo de acción archiva o devuelve una tarjeta al tablero.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de tarjeta]</td> 
   <td> <p> Introduzca o asigne el ID de la tarjeta que desea archivar o devolver al tablero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivar o desarchivar]</td> 
   <td> <p> Seleccione si desea cerrar la tarjeta (archivo) o enviarla de vuelta al tablero (desarchivo).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Agregar datos adjuntos]**

Este módulo de acción agrega un archivo adjunto a la tarjeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta cuyos detalles desea recuperar.</p> 
    <ul> 
     <li> <p><strong>Introducir manualmente</strong> </p> <p>En el campo <strong>[!UICONTROL ID de tarjeta]</strong>, escriba o asigne el ID de la tarjeta cuyos detalles desee recuperar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta sobre la que desea recuperar los detalles, seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de datos adjuntos]</p> </td> 
   <td> <p>Seleccione si desea cargar el archivo directamente o proporcionar una dirección URL para el archivo.</p> 
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

Consulte &quot;[!UICONTROL Asignar un miembro a un tablero]&quot; en [Tableros](#boards).

+++

+++ **[!UICONTROL Anular la asignación de un miembro del tablero]**

Consulte &quot;[!UICONTROL Anular la asignación de un miembro de un tablero]&quot; en [Tableros](#boards).

+++

+++ **[!UICONTROL Agregar un miembro a una tarjeta]**

Este módulo de acción agrega el miembro especificado a la tarjeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Introducir ID de tarjeta e ID de miembro]</p> </td> 
   <td> <p>Elija cómo desea introducir el ID de tarjeta y el ID de miembro.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Escriba o asigne el <strong>[!UICONTROL ID de tarjeta]</strong> y el <strong>[!UICONTROL ID de miembro]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta a la que desea agregar un miembro y, a continuación, seleccione la lista que contiene la tarjeta, la propia tarjeta y el miembro que desea agregar a la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Buscar miembros]**

Este módulo de acción recupera información sobre los miembros de [!UICONTROL Trello].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta] </td> 
   <td> <p>Introduzca el nombre completo o el nombre de usuario del usuario que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parcial] </td> 
   <td> <p>De forma predeterminada, este módulo busca coincidencias exactas de cada palabra de la consulta en el contenido de los miembros. Cuando [!UICONTROL Partial] está habilitado, el módulo busca contenido que comience con cualquier palabra de la consulta.</p> <p> Por ejemplo, si está utilizando la palabra "desarrollo" para buscar un tablero llamado "Mi informe de estado de desarrollo", de forma predeterminada deberá buscar la palabra completa. Si tiene [!UICONTROL Parcial] habilitado, podrá buscar "dev" pero no "development".</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea añadir una lista de comprobación.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL Card ID]</strong>, escriba o asigne el ID de la tarjeta donde desea agregar una lista de comprobación.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca o asigne un nombre para la lista de comprobación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posición] </td> 
   <td> <p>Seleccione si desea agregar la lista de comprobación a la parte superior o [!UICONTROL anexar la lista de comprobación] a la parte inferior de la tarjeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Introducir ID de lista de comprobación]</p> </td> 
   <td> <p>Introduzca o asigne el ID de una lista de comprobación de origen que desee copiar en la nueva.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear un elemento de lista de comprobación]**

Este módulo de acción añade un elemento a una lista de comprobación específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de lista de comprobación]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la lista de comprobación en la que desea añadir un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL Checklist ID]</strong>, escriba o asigne el ID de la tarjeta donde desea agregar una lista de comprobación.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta, luego seleccione la tarjeta y luego seleccione la lista de comprobación.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nombre de elemento]</p> </td> 
   <td> <p>Escriba o asigne un nombre para el nuevo elemento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Posición]</p> </td> 
   <td> <p>Seleccione si desea agregar el elemento al principio o [!UICONTROL anexar] al final de la lista de comprobación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comprobado]</p> </td> 
   <td> <p>Active esta opción si desea agregar el elemento como ya seleccionado.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de tarjeta y un Id. de elemento de lista de comprobación]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta y la lista de comprobación donde desea editar un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL Checklist ID]</strong>, escriba o asigne el ID de la tarjeta donde desea agregar una lista de comprobación.</p> <p>En el campo <strong>[!UICONTROL Checklist Item ID]</strong>, introduzca o asigne el ID de la lista de comprobación.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta, luego seleccione la tarjeta y luego seleccione la lista de comprobación.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de lista de comprobación]</td> 
   <td>Seleccione o asigne la lista de comprobación a la que desea mover el elemento de la lista de comprobación.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nombre de elemento]</p> </td> 
   <td> <p>Escriba o asigne un nombre para el nuevo elemento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Posición]</p> </td> 
   <td> <p>Seleccione si desea agregar el elemento al principio o anexar al final de la lista de comprobación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estado]</p> </td> 
   <td> <p>Seleccione si el elemento de la lista de comprobación está completo o incompleto.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Etiquetas

+++ **[!UICONTROL Agregar una etiqueta a una tarjeta]**

Este módulo de acción agrega una etiqueta a la tarjeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir ID de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea añadir una lista de comprobación.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL Card ID]</strong>, escriba o asigne el ID de la tarjeta donde desea agregar una lista de comprobación. En el campo <strong>[!UICONTROL Label ID]</strong>, escriba o asigne el ID de la etiqueta que desea agregar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta donde desea agregar una lista de comprobación, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta. </p> <p>Seleccione la etiqueta que desee agregar a la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Comentarios

+++ **[!UICONTROL Observar comentarios]**

Recupera detalles del comentario cuando hay un nuevo comentario en una ubicación especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objeto inspeccionado]</td> 
   <td> <p>Seleccione la ubicación en la que desea ver los comentarios.</p> 
    <ul> 
     <li><strong>[!UICONTROL Todas las tarjetas] en todas partes</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>Seleccione el tablero que desea ver para ver los comentarios</p> </li> 
     <li> <p><strong>[!UICONTROL Lista]</strong> </p> <p>Seleccione el tablero que contiene la lista que desea inspeccionar para ver si hay comentarios y, a continuación, seleccione la lista.</p> </li> 
     <li><strong>[!UICONTROL Tarjeta]</strong> </li> 
     <li>Seleccione el tablero que contiene la tarjeta que desea inspeccionar en busca de comentarios, a continuación, seleccione la lista que contiene la tarjeta y, por último, seleccione la tarjeta.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Se devolverá el número máximo de comentarios [!DNL Workfront Fusion] durante un ciclo de ejecución.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea agregar un comentario.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL ID de tarjeta]</strong>, escriba o asigne el ID de la tarjeta donde desea agregar un comentario.<br></p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Trello] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de tarjeta]</td> 
   <td> <p> Seleccione cómo desea introducir el ID de la tarjeta en la que desea agregar un comentario.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo <strong>[!UICONTROL ID de tarjeta]</strong>, escriba o asigne el ID de la tarjeta donde desea agregar un comentario.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar]</strong> </p> <p>Seleccione el tablero que contiene la tarjeta en la que desea agregar un comentario, luego seleccione la lista que contiene la tarjeta y, a continuación, seleccione la tarjeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de comentarios devueltos]</td> 
   <td> <p> Introduzca el número máximo de comentarios que devolverá [!DNL Workfront Fusion] durante un ciclo de ejecución.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde] </td> 
   <td> <p>Establezca la fecha de inicio del periodo en el que se creó el comentario. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antes] </td> 
   <td> <p>Establezca la fecha de finalización del periodo en el que se creó el comentario. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Id. de objeto Trello]

* [Cómo encontrar el ID o el vínculo abreviado de una tarjeta en  [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Cómo buscar los identificadores de otros objetos en  [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### Cómo encontrar el ID o el vínculo abreviado de una tarjeta en [!DNL Trello]

Si desea editar una tarjeta o crear un nuevo comentario, debe conocer el ID de la tarjeta o su vínculo abreviado. Puede obtener esta información en el resultado del déclencheur [!UICONTROL Nueva tarjeta]. El vínculo corto de una tarjeta también se puede obtener abriéndola y haciendo clic en el botón [!UICONTROL Compartir]. El vínculo abreviado se encuentra en el cuadro [!UICONTROL Vínculo a esta tarjeta], al final de la dirección URL después de `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Cómo buscar los identificadores de otros objetos en [!DNL Trello]

Los ID de tablero, lista y comentario solo se pueden obtener mediante déclencheur. El sitio web [!DNL trello.com] no muestra estos identificadores.
