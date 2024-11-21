---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: módulos de Power BI
description: Adobe Workfront Fusion requiere una licencia Adobe Workfront Fusion además de una licencia Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2493'
ht-degree: 0%

---

# [!DNL Power BI] módulos

[!DNL Power BI] es una aplicación que le permite visualizar y presentar datos a las partes interesadas. Puede tomar datos de una variedad de fuentes.

>[!NOTE]
>
>[!DNL Workfront Fusion] no es un origen de datos. Aunque [!DNL Workfront Fusion] puede crear y usar orígenes de datos, no almacena sus datos.


## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
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
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Información de API de Microsoft Power BI

El conector de Power BI de Microsoft utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://api.powerbi.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.0.2</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Power BI] módulos y sus campos

Al configurar [!DNL Power BI], [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Junto con estos, pueden mostrarse campos adicionales en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Paneles](#dashboards)
* [Informes](#reports)
* [Conjunto de datos](#dataset)
* [Aplicaciones](#apps)
* [Otro](#other)

### Paneles

* [Crear un tablero](#create-a-dashboard)
* [Obtener un panel](#get-a-dashboard)
* [Obtener un mosaico del panel](#get-a-dashboard-tile)
* [Mostrar mosaicos del panel](#list-dashboard-tiles)
* [Paneles de lista](#list-dashboards)

#### [!UICONTROL Crear un panel]

Este módulo de acción crea un nuevo tablero.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>Introduzca o asigne un nombre para el panel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del nuevo panel.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener un panel]

Este módulo de acción recupera los metadatos de un tablero especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un Id. de panel]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el panel para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Identificador de panel]</td>
      <td>
        <p>Introduzca o asigne el ID del panel para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario de los paneles para el que desea recuperar metadatos.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener un mosaico del panel]

Este módulo de acción recupera los metadatos de un mosaico de panel especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un Id. de panel]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir los detalles del panel que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Identificador de panel]</td>
      <td>
        <p>Introduzca o asigne el ID del tablero cuyos detalles desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de mosaico]</td>
      <td>Escriba o asigne el identificador del mosaico [!DNL Power BI] cuyos detalles desea recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del mosaico que desea recuperar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar Mosaicos Del Panel]

Este módulo de búsqueda recupera una lista de mosaicos de panel.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Escriba un Id. de panel]</td>
    <td>
      <p>Seleccione o asigne la opción para elegir el tablero cuyos mosaicos desee enumerar.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Identificador de panel]</td>
    <td>
      <p>Introduzca o asigne el ID del tablero que contiene los mosaicos que desea enumerar.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
    <td>Seleccione o asigne el ID del grupo propietario de los paneles que contienen los mosaicos que desea enumerar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Límite]  </td>
    <td>
      <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Paneles de lista]

Este módulo de búsqueda recupera una lista de paneles.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>
        <p>Seleccione o asigne el ID del grupo propietario de los paneles que desee enumerar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

### Informes

* [Copia de un informe](#copy-a-report)
* [Eliminar un informe](#delete-a-report)
* [Obtener un informe](#get-a-report)
* [Enumerar informes](#list-reports)

#### [!UICONTROL Copiar un informe]

Este módulo de acción copia un informe existente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un Id. de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe que desea copiar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de informe]</td>
      <td>
        <p>Introduzca o asigne el ID del informe que desea copiar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del informe que desea copiar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nuevo nombre de informe copiado]</td>
      <td>Introduzca o asigne un nombre para el nuevo informe.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminar un informe]

Este módulo de acción elimina un informe.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un Id. de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de informe]</td>
      <td>
        <p>Introduzca o asigne el ID del informe que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del informe que desea eliminar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener un informe]

Este módulo de acción recupera los metadatos de un informe especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un Id. de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe cuyos metadatos desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de informe]</td>
      <td>
        <p>Introduzca o asigne el ID del informe cuyos metadatos desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del informe cuyos metadatos desea recuperar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Informes de lista]

Este módulo de búsqueda recupera una lista de informes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>
        <p>Seleccione o asigne el ID del grupo propietario de los informes que desea enumerar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p>
      </td>
    </tr>
  </tbody>
</table>


### Conjunto de datos

* [Agregar o eliminar filas en una tabla de conjunto de datos](#add-or-delete-rows-in-a-dataset-table)
* [Crear un conjunto de datos](#create-a-dataset)
* [Eliminar un conjunto de datos](#delete-a-dataset)
* [Obtener un conjunto de datos](#get-a-dataset)
* [Enumerar conjuntos de datos](#list-datasets)
* [Actualizar un conjunto de datos](#refresh-a-dataset)

#### [!UICONTROL Agregar o eliminar filas en una tabla de conjunto de datos]

Este módulo de acción agrega o elimina filas de una tabla de conjunto de datos push especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba una tabla]</td>
      <td>Seleccione o asigne la opción para seleccionar el conjunto de datos que contiene la tabla que desea ajustar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de conjunto de datos]</td>
      <td>Introduzca o asigne el ID del conjunto de datos que contiene las filas que desea agregar o eliminar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre de tabla]  </td>
      <td>
        <p>Escriba o asigne el nombre de la tabla que contiene las filas que desea agregar o eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Introduzca o asigne el ID del grupo propietario del conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seleccione la acción]</td>
      <td>
        <p>Seleccione o asigne la acción que desea realizar.</p>
        <ul>
          <li>
            <p>[!UICONTROL Agregar filas]</p>
          </li>
          <li>
            <p>[!UICONTROL Eliminar todas las filas]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Filas]</td>
      <td>
        <p>Agregue los campos de fila.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Introduzca o asigne el nombre de clave.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Tipo de campo]</b>
            </p>
            <p>Seleccione o asigne el tipo de campo:</p>
            <ul>
              <li>
                <p>Booleano</p>
              </li>
              <li>
                <p>Fecha</p>
              </li>
              <li>
                <p>Texto</p>
              </li>
              <li>
                <p>Número</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL Valor]</p>
            <p>Introduzca o asigne el valor clave.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Crear un conjunto de datos]

Este módulo de acción crea un nuevo conjunto de datos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>Introduzca o asigne un nombre para el conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo que será propietario del nuevo conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Modo predeterminado]</td>
      <td>
        <p>Seleccione o asigne el modo predeterminado para el conjunto de datos:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: Un conjunto de datos con una conexión activa a [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>: Un conjunto de datos con una conexión activa al servicio [!DNL On-premise Analysis]</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: conjunto de datos que permite el acceso mediante programación para insertar datos en [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: conjunto de datos que admite la transmisión de datos y permite el acceso mediante programación para la inserción de datos en [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: conjunto de datos que admite la transmisión de datos</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tablas]</td>
      <td>Agregue tablas al conjunto de datos. Para ver los campos, consulte <a href="#Table" class="MCXref_0">Campos de tabla</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Añada las fuentes de datos. Para ver los campos, consulte <a href="#Data" class="MCXref_0">Campos de orígenes de datos</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Seleccione o asigne la directiva intencional para el conjunto de datos:</p>
        <ul>
          <li>
            <p>[!UICONTROL Ninguno]</p>
          </li>
          <li>
            <p>[!UICONTROL FIFO básico]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de tabla

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>
        <p>  Introduzca o asigne un nombre para la tabla.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Columnas]</td>
      <td>
        <p>Añada las columnas:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Nombre]</b>
            </p>
            <p>Introduzca (asigne) un nombre de columna.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Tipo de datos]</b>
            </p>
            <p>Seleccione o asigne el tipo de datos:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Entero]</p>
              </li>
              <li>
                <p>[!UICONTROL Booleano]</p>
              </li>
              <li>
                <p>[!UICONTROL Fecha y hora]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Cadena de formato]</b>
            </p>
            <p>Introduzca (asigne) la cadena de formato.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Filas]</td>
      <td>Especifique o asigne detalles de fila.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Medidas]</td>
      <td>Añada la medida para las tablas.</td>
    </tr>
  </tbody>
</table>

##### Campos de fuentes de datos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Base de datos]  </td>
      <td>
        <p>Introduzca o asigne la base de datos que desea utilizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Introduzca o asigne el nombre del servidor que desea utilizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Introduzca o asigne la dirección URL que desea utilizar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de origen de datos]</td>
      <td>
        <p>  Introduzca o asigne el ID de la fuente de datos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de origen de datos]  </td>
      <td>
        <p>Seleccione o asigne el tipo de fuente de datos. Ejemplo: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>Introduzca o asigne el ID de la puerta de enlace que desea utilizar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminar un conjunto de datos]

Este módulo de acción elimina un conjunto de datos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un Id. de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el conjunto de datos que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de informe]</td>
      <td>
        <p>Introduzca o asigne el ID del conjunto de datos que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del conjunto de datos que desea eliminar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener un conjunto de datos]

Este módulo de acción recupera los metadatos de un conjunto de datos especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un Id. de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe cuyos metadatos desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de informe]</td>
      <td>
        <p>Introduzca o asigne el ID del conjunto de datos para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del conjunto de datos para el que desea recuperar metadatos.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Conjuntos de datos de lista]

Este módulo de búsqueda recupera una lista de conjuntos de datos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del informe cuyos metadatos desea recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo [action] ejecute durante cada ciclo de ejecución de escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Actualizar un conjunto de datos]

Este módulo de acción actualiza un conjunto de datos especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escriba un conjunto de datos]</td>
      <td>Seleccione o asigne la opción para seleccionar el conjunto de datos que desea actualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de conjunto de datos]</td>
      <td>Introduzca o asigne el ID del conjunto de datos que desea actualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nombre de tabla]  </td>
      <td>
        <p>Escriba o asigne el nombre de la tabla que contiene las filas que desea agregar o eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de grupo]  </td>
      <td>Introduzca o asigne el ID del grupo propietario del conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Notificar opción]  </td>
      <td>
        <p>Seleccione o asigne la opción para notificar a:</p>
        <ul>
          <li>
            <p>[!UICONTROL Correo tras la finalización]</p>
          </li>
          <li>
            <p>[!UICONTROL Correo en caso de error]</p>
          </li>
          <li>
            <p>[!UICONTROL Sin notificación]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aplicaciones

* [Obtener una aplicación](#get-an-app)
* [Obtener el tablero de una aplicación](#get-an-apps-dashboard)
* [Obtener el informe de una aplicación](#get-an-apps-report)
* [Enumerar los paneles de la aplicación](#list-apps-dashboards)
* [Enumerar los informes de la aplicación](#list-apps-reports)
* [Enumerar aplicaciones](#list-apps)
* [Ver aplicaciones](#watch-apps)

#### [!UICONTROL Obtener una aplicación]

Este módulo de acción recupera los metadatos de una aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de aplicación]  </td>
      <td>
        <p>Seleccione o asigne el ID de la aplicación que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener el tablero de una aplicación]

Este módulo de acción recupera los metadatos del tablero de una aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de aplicación]  </td>
      <td>
        <p>Seleccione o asigne el ID de la aplicación que contiene el tablero que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de informe]</td>
      <td>
        <p>  Seleccione o asigne el ID del tablero que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener el informe de una aplicación]

Este módulo de acción recupera los metadatos del informe de una aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de aplicación]  </td>
      <td>
        <p>Seleccione o asigne el ID de la aplicación que contiene el informe que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de informe]</td>
      <td>
        <p>  Seleccione o asigne el ID del informe que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar aplicaciones]

Este módulo de búsqueda recupera una lista de todas las aplicaciones instaladas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar los paneles de la aplicación]

Este módulo de búsqueda recupera una lista de paneles de una aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de aplicación]</td>
      <td>Seleccione o asigne el ID de la aplicación desde la que desea enumerar los paneles.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Enumerar informes de aplicaciones]

Este módulo de búsqueda recupera una lista de todos los informes de la aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de aplicación]</td>
      <td>Seleccione o asigne el ID de la aplicación desde la que desea enumerar los informes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ver aplicaciones]

Este módulo de déclencheur inicia un escenario cuando se actualiza una aplicación.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

### Otro

#### [!UICONTROL Realizar una llamada API]

Este módulo de acción realiza una llamada API a la API [!DNL Power BI].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Power BI] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Ruta]</p>
      </td>
      <td>
        <p>Escriba una ruta relativa a <code>https://api.powerbi.com</code>. Ejemplo: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
      <td>
        <p>Seleccione el método de solicitud [!UICONTROL HTTP] que necesita para configurar la llamada de API. Para obtener más información, vea Métodos de solicitud [!UICONTROL HTTP].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] agrega automáticamente encabezados de autorización y encabezados x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Introduzca la cadena de consulta de solicitud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cuerpo]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
