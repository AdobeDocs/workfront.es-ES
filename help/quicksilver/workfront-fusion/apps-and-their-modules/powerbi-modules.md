---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: módulos de Power BI
description: Adobe Workfront Fusion requiere una licencia de Adobe Workfront Fusion además de una licencia de Adobe Workfront.
author: Becky
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 6d6aaa4e85690307f93dfc5179a489a09e9a2381
workflow-type: tm+mt
source-wordcount: '2352'
ht-degree: 0%

---

# [!DNL Power BI] Módulos

[!DNL Power BI] es una aplicación que le permite visualizar y presentar datos a los interesados. Puede tomar datos de una variedad de fuentes.

>[!NOTE]
>
>[!DNL Workfront Fusion] no es una fuente de datos. While [!DNL Workfront Fusion] puede crear y utilizar fuentes de datos; no almacena los datos.


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
   <td> <p>[!UICONTROL Workfront Fusion para automatización e integración del trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] módulos y sus campos

Al configurar [!DNL Power BI], [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Junto con estos, podrían mostrarse campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita de un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Paneles

#### [!UICONTROL Tableros de lista]

Este módulo de búsqueda recupera una lista de tableros.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Seleccione o asigne el ID del grupo que posee los tableros que desea enumerar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Lista de mosaicos del panel]

Este módulo de búsqueda recupera una lista de mosaicos de tablero.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Introducir un ID de tablero]</td>
    <td>
      <p>Seleccione o asigne la opción para elegir el tablero cuyos mosaicos desea enumerar.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID del panel]</td>
    <td>
      <p>Introduzca o asigne el ID del tablero que contiene los mosaicos que desea enumerar.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>Seleccione o asigne el ID del grupo propietario de los tableros que contienen los mosaicos que desea enumerar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Límite]  </td>
    <td>
      <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Obtener un tablero]

Este módulo de acción recupera los metadatos de un tablero especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un ID de tablero]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el panel para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID del panel]</td>
      <td>
        <p>Introduzca o asigne el ID del panel para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo que posee los tableros para los que desea recuperar los metadatos.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener un mosaico del tablero]

Este módulo de acción recupera los metadatos de un mosaico de tablero especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un ID de tablero]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir los detalles del tablero que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID del panel]</td>
      <td>
        <p>Introduzca o asigne el ID del tablero para el que desea recuperar los detalles.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de mosaico]</td>
      <td>Introduzca o asigne el ID de la variable [!DNL Power BI] mosaico para el que desea recuperar detalles.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del mosaico que desea recuperar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Crear un tablero]

Este módulo de acción crea un nuevo tablero.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Escriba o asigne un nombre para el tablero.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del nuevo panel.</td>
    </tr>
  </tbody>
</table>

### Informes

#### [!UICONTROL Informes de lista]

Este módulo de búsqueda recupera una lista de informes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Seleccione o asigne el ID del grupo propietario de los informes que desea enumerar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p>
      </td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un ID de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Introduzca o asigne el ID del informe para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del informe para el que desea recuperar los metadatos.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Copiar un informe]

Este módulo de acción copia un informe existente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un ID de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe que desea copiar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Introduzca o asigne el ID del informe que desea copiar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un ID de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe que desee eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Introduzca o asigne el ID del informe que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del informe que desea eliminar.</td>
    </tr>
  </tbody>
</table>

### Conjunto de datos

#### [!UICONTROL Conjuntos de datos de lista]

Este módulo de búsqueda recupera una lista de conjuntos de datos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del informe para el que desea recuperar los metadatos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]</td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo [action] durante cada ciclo de ejecución del escenario.</p>
      </td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un ID de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el informe para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Introduzca o asigne el ID del conjunto de datos para el que desea recuperar los metadatos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo propietario del conjunto de datos para el que desea recuperar los metadatos.</td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Introduzca o asigne un nombre para el conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo que será el propietario del nuevo conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Modo predeterminado]</td>
      <td>
        <p>Seleccione o asigne el modo predeterminado para el conjunto de datos:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Como Azure]</b>: Un conjunto de datos con conexión activa a [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>: Un conjunto de datos con conexión activa a [!DNL On-premise Analysis] Servicio</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: Conjunto de datos que permite el acceso programático para introducir datos [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: Conjunto de datos que admite flujo de datos y permite el acceso programático para introducir datos [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: Un conjunto de datos compatible con la transmisión de datos</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tablas]</td>
      <td>Agregue tablas al conjunto de datos. Para los campos, consulte <a href="#Table" class="MCXref_0">Campos de tabla</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Agregue las fuentes de datos. Para los campos, consulte <a href="#Data" class="MCXref_0">Campos de fuentes de datos</a>.</td>
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
            <p>[!UICONTROL Basic FIFO]</p>
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
      <td role="rowheader">[!UICONTROL Name]</td>
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
            <p><b>[!UICONTROL Name]</b>
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
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
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
      <td>Introduzca o asigne detalles de fila.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Measures]</td>
      <td>Agregue la medida para las tablas.</td>
    </tr>
  </tbody>
</table>

##### Campos de fuentes de datos

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Database]  </td>
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
      <td role="rowheader">[!UICONTROL Data source ID]</td>
      <td>
        <p>  Introduzca o asigne el ID del origen de datos.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de fuente de datos]  </td>
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

#### [!UICONTROL Agregar o eliminar filas de una tabla de conjunto de datos]

Este módulo de acción agrega o elimina filas de una tabla de conjuntos de datos push especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir una tabla]</td>
      <td>Seleccione o asigne la opción para seleccionar el conjunto de datos que contiene la tabla que desea ajustar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID del conjunto de datos]</td>
      <td>Introduzca o asigne el ID del conjunto de datos que contiene las filas que desea agregar o eliminar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Introduzca o asigne el nombre de la tabla que contiene las filas que desea agregar o eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Introduzca o asigne el ID del grupo propietario del conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seleccionar la acción]</td>
      <td>
        <p>Seleccione o asigne la acción que desee realizar.</p>
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
        <p>Añada los campos de fila.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Introduzca o asigne el nombre de la clave.</p>
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

#### [!UICONTROL Actualizar un conjunto de datos]

Este módulo de acción actualiza un conjunto de datos especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un conjunto de datos]</td>
      <td>Seleccione o asigne la opción para seleccionar el conjunto de datos que desea actualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID del conjunto de datos]</td>
      <td>Introduzca o asigne el ID del conjunto de datos que desea actualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Introduzca o asigne el nombre de la tabla que contiene las filas que desea agregar o eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Introduzca o asigne el ID del grupo propietario del conjunto de datos.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opción Notificar]  </td>
      <td>
        <p>Seleccione o asigne la opción para notificar:</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail on Completion]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL Sin notificación]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminación de un conjunto de datos]

Este módulo de acción elimina un conjunto de datos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Introducir un ID de informe]</td>
      <td>
        <p>Seleccione o asigne la opción para elegir el conjunto de datos que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Introduzca o asigne el ID del conjunto de datos que desea eliminar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Seleccione o asigne el ID del grupo que posee el conjunto de datos que desea eliminar.</td>
    </tr>
  </tbody>
</table>

### Aplicaciones

#### [!UICONTROL Aplicaciones de Watch]

Este módulo de déclencheur inicia un escenario cuando se actualiza una aplicación.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Aplicaciones de lista]

Este módulo de búsqueda recupera una lista de todas las aplicaciones instaladas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Lista de informes de aplicaciones]

Este módulo de búsqueda recupera una lista de todos los informes de la aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Seleccione o asigne el ID de la aplicación desde la que desea enumerar los informes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Lista de paneles de la aplicación]

Este módulo de búsqueda recupera una lista de tableros de una aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Seleccione o asigne el ID de la aplicación desde la que desea enumerar los tableros.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener una aplicación]

Este módulo de acción recupera los metadatos de una aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Seleccione o asigne el ID de la aplicación que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener un informe de aplicación]

Este módulo de acción recupera los metadatos de un informe de aplicación especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Seleccione o asigne el ID de la aplicación que contiene el informe que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Seleccione o asigne el ID del informe que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtener el panel de una aplicación]

Este módulo de acción recupera los metadatos del panel de una aplicación especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Seleccione o asigne el ID de la aplicación que contiene el panel que desea recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Seleccione o asigne el ID del tablero que desea recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo de acción realiza una llamada API a la función [!DNL Power BI] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Power BI] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Especifique una ruta relativa a <code>https://api.powerbi.com</code>. Ejemplo: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
      <td>
        <p>Seleccione el método de solicitud [!UICONTROL HTTP] que necesita para configurar la llamada de API. Para obtener más información, consulte métodos de solicitud [!UICONTROL HTTP].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] añade automáticamente encabezados de autorización y encabezados x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Introduzca la cadena de consulta de solicitud.</p>
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
