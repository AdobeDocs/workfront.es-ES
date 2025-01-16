---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos GitHub
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 83%

---

# Módulos de [!DNL GitHub]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos GitHub](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/github.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!UICONTROL GitHub], así como conectarlo a varias aplicaciones y servicios de terceros.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
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

Para usar los módulos [!DNL GitHub], debe tener una cuenta de [!DNL GitHub].

## Conectar [!DNL GitHub] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL GitHub] a [!UICONTROL Workfront Fusion], consulte [Crear una conexión a [!UICONTROL Adobe Workfront Fusion]: Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Módulos [!DNL GitHub] y sus campos.

Al configurar módulos [!DNL GitHub], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL GitHub] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activadores](#triggers)
* [Acciones](#actions)

### Activadores

* [[!UICONTROL Ver problemas]](#watch-issues)
* [[!UICONTROL Ver repositorios]](#watch-repositories)
* [[!UICONTROL Ver horquillas]](#watch-forks)
* [[!UICONTROL Ver comentarios]](#watch-comments)
* [[!UICONTROL Ver solicitudes de cambio]](#watch-pull-requests)

#### [!UICONTROL Ver problemas]

Este módulo se activa cuando se añade un problema nuevo o se modifica un problema existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL I want to watch]</td> 
   <td>Seleccione si desea ver todos los repositorios o solo uno.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Si ha elegido ver los problemas de un solo repositorio, seleccione el repositorio que desee ver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned issues]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar solo problemas nuevos o problemas nuevos y todos los cambios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Puede filtrar los problemas que desea tener en cuenta según la forma en que esté asociados a ellos.</p> 
    <ul> 
     <li>[!UICONTROL All issues]</li> 
     <li>[!UICONTROL Only issues assigned to me]</li> 
     <li>[!UICONTROL Only issues created by me]</li> 
     <li>[!UICONTROL Only issues mentioning me]</li> 
     <li>[!UICONTROL Only issues I'm subscribed to updates for]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleccione si solo desea inspeccionar los problemas abiertos o solo los problemas cerrados. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Añada una etiqueta. El módulo inspecciona los problemas con esta etiqueta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Repositorios de observación]

Este módulo se activa cuando se crea o modifica un repositorio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned repositories]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar nuevos repositorios y todos los cambios o solo nuevos repositorios.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Horquillas de observación]

Este módulo se activa cuando se crea una nueva horquilla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que desea inspeccionar en busca de ramificaciones.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned forks]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Comentarios sobre la observación]

Este módulo se activa cuando se añade un comentario nuevo o se modifica uno existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que desea inspeccionar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue number]</td> 
   <td>Si desea restringir la búsqueda buscando únicamente nuevos comentarios realizados sobre un problema específico, introduzca el número de problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned issues]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar solo comentarios nuevos o los comentarios y todos los cambios.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Solicitudes de extracción de observación]

Este módulo se activa cuando se añade una nueva solicitud de extracción o se modifica una existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que desea inspeccionar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned pull requests]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleccione si desea ver solicitudes [!UICONTROL only open pull], solicitudes [!UICONTROL only closed ones] o todas las solicitudes de extracción. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar solo nuevas solicitudes de extracción, o nuevas solicitudes de extracción y todos los cambios.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Buscar un problema]](#search-for-an-issue)
* [[!UICONTROL Crear un problema]](#create-an-issue)
* [[!UICONTROL Actualizar un problema]](#update-an-issue)
* [[!UICONTROL Obtener un problema]](#get-an-issue)
* [[!UICONTROL Añadir usuarios asignados]](#add-assignees)
* [[!UICONTROL Quitar usuarios asignados]](#remove-assignees)
* [[!UICONTROL Añadir etiquetas a un problema]](#add-labels-to-an-issue)
* [[!UICONTROL Quitar una etiqueta de un problema]](#remove-a-label-from-an-issue)
* [[!UICONTROL Crear un comentario]](#create-a-comment)
* [[!UICONTROL Enumerar comentarios]](#list-comments)

#### [!UICONTROL Buscar un problema]

Este módulo busca los problemas que coinciden con los criterios de búsqueda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned issues]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo (el número de repeticiones por ejecución de escenario). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>Seleccione cómo desea ordenar los resultados de la búsqueda.</p> 
    <ul> 
     <li> <p>[!UICONTROL Best match] </p> </li> 
     <li>[!UICONTROL Date created]</li> 
     <li>[!UICONTROL Date updated]</li> 
     <li>[!UICONTROL Number of comments]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort direction]</td> 
   <td> <p>Seleccione de subida o de bajada. </p> <p>Para las fechas, al seleccionar <strong>[!UICONTROL descending]</strong> se obtendrá primero la fecha más reciente. </p> <p>Para [!UICONTROL number of comments], al seleccionar <strong>[!UICONTROL descending]</strong> se obtendrá el problema con el número más alto de comentarios primero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Escriba o asigne la consulta de búsqueda. Para obtener una descripción detallada de las opciones de búsqueda, consulte <a href="https://docs.github.com/es/github/searching-for-information-on-github/searching-issues-and-pull-requests">Búsqueda de problemas y solicitudes de extracción</a> en el sitio de ayuda de [!DNL GitHub].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un problema]

Este módulo crea un nuevo problema en el repositorio seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio en el que desea crear un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione las personas que desea asignar al problema. Entre los usuarios asignados disponibles se encuentran los que tienen permisos de escritura en el repositorio y los miembros de la organización con permisos de lectura en el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Seleccione el hito que desea asociar con el nuevo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Seleccione las etiquetas que desee aplicar al nuevo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Escriba o asigne un título para el nuevo problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Introduzca o asigne el cuerpo del problema como descripción o información adicional</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un problema]

Este módulo actualiza un problema de [!DNL GitHub] existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio en el que desea actualizar un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione las personas que desea asignar al problema. Entre los asignados disponibles se encuentran todos los que tienen permisos de escritura en el repositorio y los miembros de la organización con permisos de lectura en el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Seleccione el hito que desea asociar con el problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Seleccione las etiquetas que desee aplicar al problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número del problema que desee actualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleccione el estado con el que desea actualizar el problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Introduzca o asigne un título para el problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Introduzca o asigne el cuerpo del problema como descripción o información adicional</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un problema]

Este módulo recupera detalles sobre el problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que contiene el problema cuyos detalles desea recuperar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema cuyos detalles desee recuperar. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir asignados]

Este módulo añade asignados al problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que contiene el problema al que desea añadir asignados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione las personas que desea asignar al problema. Entre los asignados disponibles se encuentran todos los que tienen permisos de escritura en el repositorio y los miembros de la organización con permisos de lectura en el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema al que desea añadir asignados. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar asignados]

Este módulo quita los asignados del problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea quitar asignados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione las personas que desee quitar del problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del que desea eliminar las personas asignadas. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir etiquetas a un problema]

Este módulo añade etiquetas a un problema. Las etiquetas se definen en el nivel de repositorio y solo las puede crear alguien con acceso de escritura al repositorio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que contiene el problema al que desea añadir etiquetas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Seleccione las etiquetas que desea añadir al problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número del problema al que desea añadir etiquetas.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar una etiqueta de un problema]

Este módulo quita una sola etiqueta de un problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea quitar una etiqueta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Seleccione la etiqueta que desea quitar del problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problemas del que desea quitar una etiqueta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un comentario]

Este módulo crea un comentario sobre el problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que contiene el problema en el que desea crear un comentario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problemas sobre el que desea crear un comentario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Introduzca o asigne el contenido del comentario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar comentarios]

Este módulo enumera todos los comentarios sobre el problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea enumerar comentarios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problemas del que desea enumerar comentarios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>El módulo devolverá los comentarios creados después de esta fecha. Para obtener una lista de formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned comments]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
