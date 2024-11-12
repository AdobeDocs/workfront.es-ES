---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Workfront Planning
description: Con los módulos  [!DNL Adobe Workfront Planning] puede iniciar un escenario [!DNL Adobe Workfront Fusion] basado en los eventos de su cuenta de Workfront Planning, crear, leer o actualizar acuerdos y otros registros, buscar registros con los criterios establecidos y cargar documentos. [!DNL Adobe]
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: 8cb79a06f46c9a379f7394a6bef14f97d4ff7f98
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning] módulos

Con los módulos [!DNL Adobe Workfront Planning], puede almacenar en déclencheur un escenario cuando se produzcan eventos en Workfront Planning. También puede crear, leer, actualizar y eliminar registros, o realizar una llamada de API personalizada a su cuenta de [!DNL Adobe Workfront Planning].

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

## Crear una conexión con [!DNL Adobe Workfront Planning]

Puede crear una conexión con su cuenta de [!DNL Workfront Planning] directamente desde un módulo de [!DNL Workfront Fusion].

1. En cualquier módulo de [!DNL Adobe Workfront Planning], haga clic en **[!UICONTROL Agregar]** junto al cuadro Conexión.

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
          <td>Escriba su [!UICONTROL Client ID] [!DNL Adobe]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Secreto de cliente]<p>(Opcional)</p></td>
          <td>Escriba su [!UICONTROL Secreto de cliente] [!DNL Adobe]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
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
1. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Workfront Planning] módulos y sus campos

### Déclencheur

#### Ver eventos

Este módulo de déclencheur inicia un escenario cuando se crea, actualiza o elimina un registro, tipo de registro o espacio de trabajo en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Seleccione el webhook que desee utilizar o haga clic en Agregar para crear uno nuevo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de objeto]</td>
      <td>Seleccione si desea ver registros, tipos de registros o espacios de trabajo.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Filtros de eventos]</p> </td> 
      <td> <p>Puede establecer filtros para inspeccionar sólo los registros que cumplan los criterios seleccionados.</p> <p>Para cada filtro, introduzca el campo que desea que evalúe el filtro, el operador y el valor que desea que permita el filtro. Puede utilizar más de un filtro añadiendo reglas AND.</p> <p>Nota: No puede editar filtros en los [!DNL Workfront] webhooks existentes. Para configurar diferentes filtros para [!DNL Workfront] suscripciones de evento, elimine el webhook actual y cree uno nuevo.</p> <p>Para obtener más información sobre los filtros de eventos, consulte <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Filtros de suscripción de eventos en los módulos [!DNL Workfront] &gt; [!UICONTROL Watch Events]</a> en el artículo Módulos de Workfront.</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">[!UICONTROL Objetos que ver]</td>
      <td>Seleccione si desea ver las nuevas. registros actualizados, nuevos y actualizados o eliminados.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Excluir actualizaciones realizadas por esta conexión]</p>
      </td>
      <td>Habilite esta opción para evitar que el escenario se active cuando la conexión utilizada por este módulo realice un cambio. Esto evita que se active otra instancia del escenario si este realiza una acción de activación.</td> 
      </tr>
  </tbody>
</table>

### Acciones

* [Eliminación de un tipo de registro](#delete-a-record-type)
* [Realizar una llamada de IA personalizada](#make-a-custom-api-call)

#### Eliminación de un tipo de registro

Este módulo de acción elimina un solo tipo de registro en Workfront Planning por su ID.

>[!WARNING]
>
>Al eliminar un tipo de registro en Workfront Planning también se eliminan todos los registros de la tabla de tipo de registro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Introduzca o asigne el ID del campo que desea eliminar.</td> 
      </tr>
  </tbody>
</table>

#### Realizar una llamada de API personalizada

Este módulo realiza una llamada de API personalizada a la API [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Introduzca una ruta relativa a <code>https://(YOUR_WORKFRONT_DOMAIN)/maestro/api/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Para cada par clave/valor que desee agregar a la cadena de consulta, haga clic en <b>Agregar elemento</b> e introduzca la clave y el valor.</p>
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

<!--
### Searches

#### Search records

This action module retrieves a list of records based on criteria you specify.

-->

### Sin categoría


#### Creación de un registro

Esta acción crea un único registro en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de tipo de registro]</p>
      </td>
      <td>Introduzca o asigne el tipo de registro que desea crear. Los tipos de registro disponibles se basan en su cuenta de Workfront Planning.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Otros campos</p>
      </td>
      <td>Estos campos se basan en el tipo de registro seleccionado.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Eliminación de un registro

Este módulo de acción elimina el registro especificado en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de registro]</p>
      </td>
      <td>Introduzca o asigne el ID del registro que desea eliminar.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Obtener un registro

Este módulo de acción recupera un único registro de [!DNL Adobe Workfront Planning], especificado por su identificador.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de registro]</td>
      <td>Introduzca o asigne el ID del registro que desea recuperar.</td>
    </tr>
  </tbody>
</table>

### Obtener registros por tipo de registro

Este módulo de acción recupera todos los registros del tipo especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Seleccione o asigne el espacio de trabajo que contiene los registros que desea recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>Seleccione el tipo de registro que desea recuperar.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Número máximo de registros devueltos]</p>
      </td>
      <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tbody>
</table>

### Obtener tipos de registros

Este módulo de acción recupera una lista de tipos de registro en una cuenta de [!DNL Adobe Workfront Planning].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
  </tbody>
</table>

### Actualizar registro

Esta acción actualiza un único registro en Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Workfront Planning], vea <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Crear una conexión con [!DNL Adobe Workfront Planning]</a> en este artículo.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL ID de registro]</p>
      </td>
      <td>Introduzca o asigne el tipo de registro que desea actualizar Los tipos de registro disponibles se basan en su cuenta de Workfront Planning.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Otros campos</p>
      </td>
      <td>Estos campos se basan en el tipo de registro seleccionado.</td> 
      </tr>
     <tr>
  </tbody>
</table>
