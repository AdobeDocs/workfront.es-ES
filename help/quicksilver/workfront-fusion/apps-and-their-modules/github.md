---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de GitHub
description: En un escenario de  [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan GitHub, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 16cd5dee183153540bcccea8ce469a461d0e8562
workflow-type: tm+mt
source-wordcount: '1839'
ht-degree: 0%

---

# [!DNL GitHub] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!UICONTROL GitHub], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar módulos de [!DNL GitHub], debe tener una cuenta de [!DNL GitHub].

## Conectar [!DNL GitHub] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL GitHub] a [!UICONTROL Workfront Fusion], consulta [Crear una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] módulos y sus campos.

Al configurar [!DNL GitHub] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL GitHub] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)

### Déclencheur

* [[!UICONTROL Problemas de observación]](#watch-issues)
* [[!UICONTROL Repositorios de observación]](#watch-repositories)
* [[!UICONTROL Horquillas de observación]](#watch-forks)
* [[!UICONTROL Observar comentarios]](#watch-comments)
* [[!UICONTROL Solicitudes de extracción de observación]](#watch-pull-requests)

#### [!UICONTROL Problemas de observación]

Este módulo crea un déclencheur cuando se agrega un problema nuevo o se modifica uno existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quiero ver]</td> 
   <td>Seleccione si desea ver todos los repositorios o sólo uno.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Si ha elegido inspeccionar los problemas solo en un repositorio, seleccione el repositorio que desee inspeccionar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas devueltos]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar solo los problemas nuevos o los problemas nuevos y todos los cambios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Puede filtrar los problemas que desea tener en cuenta según la forma en que estén asociados a ellos.</p> 
    <ul> 
     <li>[!UICONTROL Todos los problemas]</li> 
     <li>[!UICONTROL Solo problemas asignados a mí]</li> 
     <li>[!UICONTROL Solo problemas creados por mí]</li> 
     <li>[!UICONTROL Solo problemas que me mencionan]</li> 
     <li>[!UICONTROL Solo problemas para los que estoy suscrito a actualizaciones]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Seleccione si desea ver sólo los problemas abiertos o sólo los problemas cerrados. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Añada una etiqueta. El módulo observa los problemas con esta etiqueta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Repositorios de observación]

Este módulo crea un déclencheur cuando se crea o modifica un repositorio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de repositorios devueltos]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar nuevos repositorios y todos los cambios, o sólo nuevos repositorios.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Horquillas de observación]

Este módulo crea un déclencheur cuando se crea una nueva ramificación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que desea inspeccionar en busca de ramificaciones.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de bifurcaciones devueltas]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar comentarios]

Este módulo crea un déclencheur cuando se agrega un comentario nuevo o se modifica uno existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que desea ver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de problema]</td> 
   <td>Si desea restringir la búsqueda buscando únicamente nuevos comentarios realizados sobre un problema específico, introduzca el número de problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas devueltos]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar sólo los comentarios nuevos o los comentarios y todos los cambios.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Solicitudes de extracción de observación]

Este módulo crea un déclencheur cuando se añade una nueva solicitud de extracción o se modifica una solicitud de extracción existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que desea ver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de solicitudes de extracción devueltas]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Seleccione si desea ver solicitudes de [!UICONTROL sólo abrir extracción], solicitudes de [!UICONTROL sólo cerradas] o todas las solicitudes de extracción. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar sólo las nuevas solicitudes de extracción, o las nuevas solicitudes de extracción y todos los cambios.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Buscar un problema]](#search-for-an-issue)
* [[!UICONTROL Crear un problema]](#create-an-issue)
* [[!UICONTROL Actualizar un problema]](#update-an-issue)
* [[!UICONTROL Obtener un problema]](#get-an-issue)
* [[!UICONTROL Agregar usuarios asignados]](#add-assignees)
* [[!UICONTROL Quitar personas asignadas]](#remove-assignees)
* [[!UICONTROL Agregar etiquetas a un problema]](#add-labels-to-an-issue)
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas devueltos]</td> 
   <td>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo (el número de repeticiones por ejecución de escenario). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Seleccione cómo desea ordenar los resultados de la búsqueda.</p> 
    <ul> 
     <li> <p>[!UICONTROL Mejor coincidencia] </p> </li> 
     <li>[!UICONTROL Fecha de creación]</li> 
     <li>[!UICONTROL Fecha de actualización]</li> 
     <li>[!UICONTROL Número de comentarios]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de orden]</td> 
   <td> <p>Seleccione ascendente o descendente. </p> <p>Para las fechas, seleccionar <strong>[!UICONTROL descendente]</strong> devolverá primero la fecha más reciente. </p> <p>Para [!UICONTROL número de comentarios], seleccionar <strong>[!UICONTROL descendente]</strong> devolverá el problema con el número más alto de comentarios primero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td>Escriba o asigne la consulta de búsqueda. Para obtener una descripción detallada de las opciones de búsqueda, consulte <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Búsqueda de problemas y solicitudes de extracción</a> en el sitio de ayuda de [!DNL GitHub].</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio en el que desea crear un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asignado]</td> 
   <td>Seleccione las personas que desea asignar al problema. Entre los usuarios asignados disponibles se encuentran todos los que tienen permisos de escritura en el repositorio y los miembros de la organización con permisos de lectura en el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hito]</td> 
   <td>Seleccione el hito que desea asociar con el nuevo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Seleccione las etiquetas que desee aplicar al nuevo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título]</td> 
   <td>Escriba o asigne un título para el nuevo problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td>Introduzca o asigne el cuerpo del problema, como una descripción o información adicional</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio en el que desea actualizar un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asignado]</td> 
   <td>Seleccione las personas que desea asignar al problema. Entre los usuarios asignados disponibles se encuentran todos los que tienen permisos de escritura en el repositorio y los miembros de la organización con permisos de lectura en el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hito]</td> 
   <td>Seleccione el hito que desea asociar con el problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Seleccione las etiquetas que desee aplicar al problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del problema que desea actualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Seleccione el estado en el que desea actualizar el problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título]</td> 
   <td>Escriba o asigne un título para el problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td>Introduzca o asigne el cuerpo del problema, como una descripción o información adicional</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea obtener detalles.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del que desea recuperar los detalles. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar usuarios asignados]

Este módulo agrega usuarios asignados al problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema al que desea agregar usuarios asignados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asignado]</td> 
   <td>Seleccione las personas que desea asignar al problema. Entre los usuarios asignados disponibles se encuentran todos los que tienen permisos de escritura en el repositorio y los miembros de la organización con permisos de lectura en el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del problema al que desea agregar usuarios asignados. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar personas asignadas]

Este módulo quita las personas asignadas del problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea eliminar las personas asignadas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asignado]</td> 
   <td>Seleccione las personas que desea eliminar del problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del que desea eliminar las personas asignadas. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar etiquetas a un problema]

Este módulo agrega etiquetas a un problema. Las etiquetas se definen en el nivel de repositorio y solo las puede crear alguien con acceso de escritura al repositorio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema al que desea agregar etiquetas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Seleccione las etiquetas que desee agregar al problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del problema al que desea agregar etiquetas.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar una etiqueta de un problema]

Este módulo elimina una sola etiqueta de un problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea quitar una etiqueta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Seleccione la etiqueta que desee eliminar del problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del que desea eliminar una etiqueta.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema en el que desea crear un comentario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del problema en el que desea crear un comentario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL GitHub] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea enumerar los comentarios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Introduzca o asigne el número de problema del problema desde el que desea enumerar los comentarios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde]</td> 
   <td>El módulo devolverá los comentarios creados después de esta fecha. Para obtener una lista de formatos de fecha admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de comentarios devueltos]</td> 
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
