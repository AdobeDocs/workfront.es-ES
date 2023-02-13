---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de GitHub
description: En un [!DNL Adobe Workfront Fusion] en este caso, puede automatizar los flujos de trabajo que utilizan GitHub, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!UICONTROL GitHub], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar [!DNL GitHub] módulos, debe tener una [!DNL GitHub] cuenta.

## Connect [!DNL GitHub] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!UICONTROL Workfront Fusion], consulte [Crear una conexión con [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] y sus campos.

Al configurar [!DNL GitHub] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL GitHub] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)

### Déclencheur

* [[!UICONTROL Problemas de Watch]](#watch-issues)
* [[!UICONTROL Repositorios de Watch]](#watch-repositories)
* [[!UICONTROL Horquillas de observación]](#watch-forks)
* [[!UICONTROL Observar comentarios]](#watch-comments)
* [[!UICONTROL Ver solicitudes de extracción]](#watch-pull-requests)

#### [!UICONTROL Problemas de Watch]

Este módulo déclencheur cuando se agrega un problema nuevo o se modifica un problema existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quiero ver]</td> 
   <td>Seleccione si desea ver todos los repositorios o solo un repositorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Si ha elegido ver los problemas en un solo repositorio, seleccione el repositorio que desee ver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas devueltos]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea ver solo los problemas nuevos, o los problemas nuevos y todos los cambios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Puede filtrar los problemas que desea ver según su asociación con ellos.</p> 
    <ul> 
     <li>[!UICONTROL Todos los problemas]</li> 
     <li>[!UICONTROL Solo problemas asignados a mí]</li> 
     <li>[!UICONTROL Solo problemas creados por mí]</li> 
     <li>[!UICONTROL Solo problemas que me mencionan]</li> 
     <li>[!UICONTROL Solo problemas para los que estoy suscrito a actualizaciones]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleccione si desea ver solo los problemas abiertos o solo los problemas cerrados. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Agregue una etiqueta . El módulo observa los problemas con esta etiqueta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Repositorios de Watch]

Este módulo déclencheur cuando se crea o modifica un repositorio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de repositorios devueltos]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea ver los repositorios nuevos y todos los cambios, o solo los nuevos.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Horquillas de observación]

Este módulo déclencheur cuando se crea una nueva ramificación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que desea ver para las ramificaciones.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de ramificaciones devueltas]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar comentarios]

Este módulo déclencheur cuando se agrega un comentario nuevo o se modifica un comentario existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que desea ver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de problema]</td> 
   <td>Si desea restringir la búsqueda buscando solo los comentarios nuevos realizados sobre un problema específico, introduzca el número de problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas devueltos]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea ver solo los comentarios nuevos o los comentarios y todos los cambios.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver solicitudes de extracción]

Este módulo déclencheur cuando se agrega una nueva solicitud de extracción o se modifica una solicitud de extracción existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que desea ver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de solicitudes de extracción devueltas]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleccione si desea ver las solicitudes de [!UICONTROL solo apertura de extracción], [!UICONTROL solo cerradas] o todas las solicitudes de extracción. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Seleccione si desea ver solo las nuevas solicitudes de extracción o las nuevas solicitudes de extracción y todos los cambios.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Buscar un problema]](#search-for-an-issue)
* [[!UICONTROL Crear un problema]](#create-an-issue)
* [[!UICONTROL Actualizar un problema]](#update-an-issue)
* [[!UICONTROL Obtener un problema]](#get-an-issue)
* [[!UICONTROL Agregar usuarios asignados]](#add-assignees)
* [[!UICONTROL Eliminar usuarios asignados]](#remove-assignees)
* [[!UICONTROL Añadir etiquetas a un problema]](#add-labels-to-an-issue)
* [[!UICONTROL Eliminación de una etiqueta de un problema]](#remove-a-label-from-an-issue)
* [[!UICONTROL Crear un comentario]](#create-a-comment)
* [[!UICONTROL Enumerar comentarios]](#list-comments)

#### [!UICONTROL Buscar un problema]

Este módulo busca problemas que coincidan con sus criterios de búsqueda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas devueltos]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo (el número de repeticiones por ejecución de escenario). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Seleccione cómo desea ordenar los resultados de la búsqueda.</p> 
    <ul> 
     <li> <p>[!UICONTROL Mejor coincidencia] </p> </li> 
     <li>[!UICONTROL Fecha de creación]</li> 
     <li>[!UICONTROL Fecha actualizada]</li> 
     <li>[!UICONTROL Número de comentarios]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Orden dirección]</td> 
   <td> <p>Seleccione ascendente o descendente. </p> <p>Para fechas, seleccione <strong>[!UICONTROL descendente]</strong> devolverá primero la fecha más reciente. </p> <p>Para [!UICONTROL número de comentarios], seleccione <strong>[!UICONTROL descendente]</strong> devolverá primero el problema con el mayor número de comentarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Introduzca o asigne la consulta de búsqueda. Para obtener una descripción detallada de las opciones de búsqueda, consulte <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Búsqueda de problemas y solicitudes de extracción</a> en el [!DNL GitHub] sitio de ayuda.</td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio en el que desea crear un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione las personas que desea asignar al problema. Los usuarios asignados disponibles incluyen a cualquier persona con permisos de escritura en el repositorio y miembros de la organización con permisos de lectura en el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Seleccione el hito que desea asociar al nuevo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Seleccione las etiquetas que desee aplicar al nuevo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Introduzca o asigne un título para el nuevo problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Introduzca o asigne el cuerpo del problema, como una descripción o información adicional</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un problema]

Este módulo actualiza una [!DNL GitHub] problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio en el que desea actualizar un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione las personas que desea asignar al problema. Los destinatarios asignados disponibles incluyen a cualquier persona con permisos de escritura para el repositorio y los miembros de la organización con permisos de lectura para el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Seleccione el hito que desea asociar al problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Seleccione las etiquetas que desee aplicar al problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema que desea actualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Seleccione el estado al que desea actualizar el problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Introduzca o asigne un título para el problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea recuperar detalles.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema del que desea recuperar detalles. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar usuarios asignados]

Este módulo agrega asignadores al problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema al que desea agregar asignadores.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione las personas que desea asignar al problema. Los destinatarios asignados disponibles incluyen a cualquier persona con permisos de escritura para el repositorio y los miembros de la organización con permisos de lectura para el repositorio. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema al que desea agregar asignadores. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar usuarios asignados]

Este módulo elimina los usuarios asignados del problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema del que desea quitar los usuarios asignados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>Seleccione a las personas que desee eliminar del problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del que desea quitar los asignadores. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir etiquetas a un problema]

Este módulo agrega etiquetas a un problema. Las etiquetas se definen en el nivel de repositorio y solo las puede crear alguien con acceso de escritura al repositorio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
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
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema al que desea añadir etiquetas.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminación de una etiqueta de un problema]

Este módulo elimina una sola etiqueta de un problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
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
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del que desea quitar una etiqueta.</td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema en el que desea crear un comentario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema en el que desea crear un comentario.</td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL GitHub] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositorio]</td> 
   <td>Seleccione el repositorio que contiene el problema desde el que desea enumerar los comentarios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Introduzca o asigne el número de problema del problema desde el que desea enumerar los comentarios.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>El módulo devolverá comentarios creados después de esta fecha. Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de comentarios devueltos]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo. </td> 
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
