---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos Figma
description: Con la variable [!DNL Adobe Workfront Fusion] Los módulos Figma permiten recuperar listas de comentarios, archivos, versiones de archivos o proyectos. También puede publicar un comentario o realizar una llamada a la API de Figma.
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 1%

---

# [!DNL Figma] Módulos

Con la variable [!DNL Adobe Workfront Fusion] [!DNL Figma] , puede recuperar listas de comentarios, archivos, versiones de archivos o proyectos. También puede publicar un comentario o realizar una llamada a la variable [!DNL Figma] API.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] o superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo]</p>
      </td>
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

Para usar [!DNL Figma] módulos, debe tener un [!DNL Figma] cuenta.

## [!DNL Figma] módulos y sus campos

Al configurar [!DNL Figma] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Figma] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Comentarios](#comments)

* [Proyectos y archivos](#projects-and-files)

* [Componentes y estilos](#components-and-styles)

* [Otro](#other)


### Comentarios

* [Eliminar un comentario](#delete-a-comment)

* [Enumerar comentarios](#list-comments)

* [Publicar un comentario](#post-a-comment)


#### [!UICONTROL Eliminar un comentario]

Este módulo de acción elimina un solo comentario de un archivo.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>Introduzca o asigne el ID de archivo del archivo desde el que desea agregar un comentario. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comentario]</td>
      <td>Introduzca el texto del comentario que desea eliminar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar comentarios]

Este módulo de búsqueda enumera todos los comentarios adjuntos a un solo archivo en [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Introduzca o asigne el ID de archivo del archivo para el que desea recuperar comentarios. </p>
        <ul>
          <li>
            <p>Si no conoce el ID, haga clic en <b>[!UICONTROL Buscar archivos]</b> e introduzca o asigne el ID del proyecto al que está asociado el archivo y, a continuación, seleccione el archivo .</p>
          </li>
          <li>
            <p>Si no conoce el ID del proyecto, haga clic en <b>[!UICONTROL Buscar proyectos]</b> e introduzca o asigne el ID del equipo propietario del proyecto al que está asociado el archivo, seleccione el proyecto y, a continuación, seleccione el archivo.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de comentarios que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Publicar un comentario]

Este módulo de acción publica un comentario en un archivo Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Introduzca o asigne el ID de archivo del archivo al que desea publicar un comentario. </p>
        <ul>
          <li>
            <p>Si no conoce el ID del archivo, haga clic en <b>[!UICONTROL Buscar archivos]</b> e introduzca o asigne el ID del proyecto al que está asociado el archivo y, a continuación, seleccione el archivo .</p>
          </li>
          <li>
            <p>Si está intentando encontrar el ID del archivo y no conoce el ID del proyecto, haga clic en <b>[!UICONTROL Buscar proyectos]</b> e introduzca o asigne el ID del equipo propietario del proyecto al que está asociado el archivo. Seleccione el proyecto y, a continuación, seleccione el archivo .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comentario]</td>
      <td>Introduzca el texto del comentario.</td>
    </tr>
  </tbody>
</table>


### Proyectos y archivos

* [Obtener un archivo o una imagen](#get-a-file-or-image)

* [Historial de versiones del archivo de lista](#list-file-version-history)

* [Enumerar archivos de proyecto](#list-project-files)

* [Enumerar proyectos](#list-projects)


#### [!UICONTROL Obtener un archivo o una imagen]

Este módulo de acción recupera un solo archivo o imagen de una biblioteca Figma

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de objeto]</td>
      <td>
        <p>Seleccione el tipo de objeto que desea recuperar.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Archivo]</b>
            </p>
            <p>El módulo devuelve el documento al que [!UICONTROL Key] hace referencia como un objeto JSON. La clave del archivo se puede analizar desde cualquier dirección URL del archivo Figma.</p>
            <p>Para los campos, consulte <a href="#Get2" class="MCXref xref" >[!UICONTROL Obtener un archivo o una imagen: Archivo]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nodos de archivo]</b>
            </p>
            <p>Devuelve los nodos a los que hacen referencia los ID como un objeto JSON. Los nodos se recuperan de la variable [!DNL Figma] archivo al que hace referencia [!UICONTROL Key].</p>
            <p>Para los campos, consulte <a href="#Get3" class="MCXref xref" >[!UICONTROL Obtener un archivo o una imagen: Nodos de archivo]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image]</b>
            </p>
            <p>El módulo procesa imágenes de un archivo.</p>
            <p>Para los campos, consulte <a href="#Get4" class="MCXref xref" >[!UICONTROL Obtener un archivo o una imagen: Imagen]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Rellenos de imagen]</b>
            </p>
            <p>El módulo devuelve vínculos de descarga para todas las imágenes presentes en los rellenos de imágenes de un documento. Los rellenos de imágenes muestran [!DNL Figma] representa las imágenes suministradas por el usuario. Al arrastrar una imagen a [!DNL Figma], [!DNL Figma] crea un rectángulo con un relleno único que representa la imagen y el usuario puede transformar el rectángulo (y las propiedades del relleno).</p>
            <p>Para los campos, consulte <a href="#Get5" class="MCXref xref" >[!UICONTROL Obtener un archivo o una imagen: Rellenos de imagen]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Obtener un archivo o imagen: Archivo]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleccione el archivo desde el que desea devolver JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de versión]</td>
      <td>Introduzca o asigne la versión del archivo que desea que devuelva el módulo. Para el módulo actual, deje este campo en blanco.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de nodo]</td>
      <td>
        <p>Para devolver sólo un subconjunto del documento, introduzca los nodos que desea que devuelva el módulo. El módulo devuelve los nodos enumerados, sus elementos secundarios y cualquier cosa entre el nodo raíz y los nodos enumerados.</p>
        <p>Para cada nodo que desee devolver, haga clic en <b>[!UICONTROL Agregar]</b> e introduzca el texto del nodo .</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Profundidad]</td>
      <td>
        <p>Introduzca o asigne un entero que represente la profundidad en el árbol de documentos para la que desea devolver los resultados. </p>
        <div class="example"><span class="autonumber"><span><b>Ejemplo: </b></span></span>
          <ul>
            <li>
              <p>Para devolver solo páginas, escriba <code>1</code>.</p>
            </li>
            <li>
              <p>Para devolver páginas y objetos de nivel superior, escriba <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Para devolver todos los nodos, deje este campo en blanco.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Para devolver datos vectoriales, introduzca <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Una lista separada por comas de los ID de complemento o la cadena "[!UICONTROL shared]". Cualquier dato presente en el documento escrito por esos complementos se incluirá en el resultado de la <code>pluginData</code> y <code>sharedPluginData</code> propiedades.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Branch data]</td>
      <td>Active esta opción para devolver metadatos de rama para el archivo solicitado. Si el archivo es una rama, la clave del archivo principal se incluye en la respuesta devuelta. Si el archivo tiene ramas, sus metadatos se incluyen en la respuesta devuelta. Predeterminado: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Obtener un archivo o imagen: Nodos de archivo]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleccione el archivo desde el que desea devolver JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de nodo]</td>
      <td>
        <p>Introduzca los nodos que desea que el módulo devuelva y convierta</p>
        <p>Para cada nodo que desee devolver, haga clic en <b>[!UICONTROL Agregar]</b> e introduzca el texto del nodo .</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de versión]</td>
      <td>Introduzca o asigne la versión del archivo que desea que devuelva el módulo. Para el módulo actual, deje este campo en blanco.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Profundidad]</td>
      <td>
        <p>Introduzca o asigne un entero que represente la profundidad en el árbol de documentos para la que desea devolver los resultados. </p>
        <div class="example"><span class="autonumber"><span><b>Ejemplo: </b></span></span>
          <ul>
            <li>
              <p>Para devolver solo páginas, escriba <code>1</code>.</p>
            </li>
            <li>
              <p>Para devolver páginas y objetos de nivel superior, escriba <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Para devolver todos los nodos, deje este campo en blanco.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Para devolver datos vectoriales, introduzca <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Una lista separada por comas de los ID de complemento o la cadena "compartida". Cualquier dato presente en el documento escrito por esos complementos se incluirá en el resultado en las propiedades pluginData y sharedPluginData .</td>
    </tr>
  </tbody>
</table>


##### Obtener un archivo o imagen: Imagen

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleccione el archivo desde el que desea devolver JSON.</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>ID de nodo]</td>
      <td>
        <p>Introduzca los nodos que desea que el módulo procese.</p>
        <p>Para cada nodo que desee procesar, haga clic en <b>[!UICONTROL Agregar]</b> e introduzca el texto del nodo .</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>Para escalar la imagen, introduzca o asigne el factor de escala. Este número debe estar entre 0,01 y 4.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Formato]</td>
      <td>
        <p>Seleccione el formato para la salida de imagen.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Incluir ID]</td>
      <td>Active esta opción para incluir atributos de ID para todos los elementos del SVG. Predeterminado: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplificar trazo]</td>
      <td>Active esta opción para simplificar los trazos interiores/exteriores y utilizar el atributo de trazo si es posible en lugar de &lt;mask&gt;. Predeterminado: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Usar límites absolutos]</td>
      <td>Active esta opción para utilizar todas las dimensiones del nodo independientemente de si se recorta o no o de si el espacio que lo rodea está vacío. Utilice esto para exportar nodos de texto sin recortar. Predeterminado: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de versión]</td>
      <td>Introduzca o asigne la versión del archivo que desea que devuelva el módulo. Para el módulo actual, deje este campo en blanco.</td>
    </tr>
  </tbody>
</table>

##### Obtener un archivo o imagen: Rellenos de imagen

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Seleccione el archivo desde el que desea devolver JSON.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL Historial de versiones del archivo de lista]

Este módulo de búsqueda devuelve el historial de versiones de un solo archivo en [!UICONTROL Figma].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Introduzca o asigne el ID de archivo del archivo para el que desea recuperar el historial de versiones. </p>
        <ul>
          <li>
            <p>Si no conoce el ID del archivo, haga clic en <b>[!UICONTROL Buscar archivos]</b> e introduzca o asigne el ID del proyecto al que está asociado el archivo y, a continuación, seleccione el archivo .</p>
          </li>
          <li>
            <p>Si está intentando encontrar el ID del archivo y no conoce el ID del proyecto, haga clic en <b>[!UICONTROL Buscar proyectos]</b> e introduzca o asigne el ID del equipo propietario del proyecto al que está asociado el archivo. Seleccione el proyecto y, a continuación, seleccione el archivo .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar archivos de proyecto]

Este módulo de búsqueda devuelve una lista de todos los archivos del proyecto especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Introduzca o asigne el ID del proyecto para el que desea recuperar archivos. </p>
        <ul>
          <li>
            <p>Si no conoce el ID de los proyectos, haga clic en <b>[!UICONTROL Buscar proyectos]</b> e introduzca o asigne el ID del equipo al que está asociado el proyecto y, a continuación, seleccione el proyecto.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar proyectos]

Este módulo de búsqueda devuelve una lista de todos los proyectos del equipo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Introduzca o asigne el ID de proyecto del proyecto para el que desea recuperar archivos. El ID del equipo se puede encontrar en la dirección URL de la página del equipo en Figma</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</td>
    </tr>
  </tbody>
</table>


### Componentes y estilos

#### [!UICONTROL Obtener un estilo o componente]

Este módulo de acción recupera un único estilo o componente, o un conjunto de estilos o componentes.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object&gt; key]</td>
      <td>Introduzca la clave (identificador único) del objeto que desea recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Introduzca o asigne el ID del equipo al que están asociados el registro o los registros.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tamaño de página]</td>
      <td>Introduzca o asigne el número o los resultados que se devolverán por página. Predeterminado: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>Introduzca o asigne el número del resultado después del cual desea empezar a recuperar los resultados. Esto se puede combinar con el campo [!UICONTROL Tamaño de página] para paginar los resultados.</p>
        <p>Este valor no se corresponde con los ID de objeto.</p>
        <p>Este campo no se puede utilizar en combinación con el campo [!UICONTROL Antes].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Antes]</td>
      <td>
        <p>Introduzca o asigne el número del resultado antes del cual desea empezar a recuperar los resultados. Esto se puede combinar con el campo [!UICONTROL Tamaño de página] para paginar los resultados.</p>
        <p>Este valor no se corresponde con los ID de objeto.</p>
        <p>Este campo no se puede utilizar en combinación con el campo [!UICONTROL After].</p>
      </td>
    </tr>
  </tbody>
</table>


### Otro

* [Realizar una llamada de API](#make-an-api-call)

* [Ver eventos](#watch-events)


#### [!UICONTROL Realizar una llamada de API]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API de Figma sin tener que pensar en la autenticación. De esta manera, puede crear una automatización del flujo de datos que no se pueda lograr con los otros módulos de Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Especifique una ruta relativa a <code>https://api.figma.com/v1/</code>.</p>
        <p>Por ejemplo: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Método]</td>
      <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]</td>
      <td>
        <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p>
        <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Ver eventos]

Este módulo de déclencheur inicia un escenario cuando se produce uno de los siguientes eventos para un equipo específico de su [!DNL Figma] espacio de equipo

* Actualización de archivos

* Actualización de la versión del archivo

* Eliminar archivo

* Publicación de biblioteca

* Comentario del archivo

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Weblock]</td>
      <td>
        <p>Seleccione el enlace web que el módulo ve.</p>
        <p>Para agregar un nuevo vínculo web:</p>
        <ol>
          <li value="1">
            <p>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL Weblock].</p>
          </li>
          <li value="2">
            <p>Seleccione la conexión que desee utilizar para este vínculo web. Para obtener instrucciones sobre cómo conectar su [!DNL Figma] cuenta para [!UICONTROL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas.</a></p>
          </li>
          <li value="3">
            <p>Seleccione el tipo de evento que desea que vea el módulo.</p>
          </li>
          <li value="4">
            <p>Introduzca el ID del equipo cuyos eventos desea que vea el vínculo web.</p>
          </li>
          <li value="5">
            <p>Introduzca el [!UICONTROL Status] o [!UICONTROL Description] de eventos que desea que el enlace web vea.</p>
          </li>
          <li value="6">
            <p>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
