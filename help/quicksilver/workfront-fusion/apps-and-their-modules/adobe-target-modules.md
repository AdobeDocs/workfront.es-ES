---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Target
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] los módulos le permiten crear, leer, actualizar o eliminar registros, enumerar todos los registros de un tipo determinado, buscar registros según los criterios especificados o realizar una llamada API personalizada a la variable [!DNL Adobe Target] API.
author: Becky
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 0%

---

# [!DNL Adobe Target] Módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Target], así como conectarlo a varias aplicaciones y servicios de terceros. [!DNL Adobe Target] los módulos le permiten crear, leer, actualizar o eliminar registros, enumerar todos los registros de un tipo determinado, buscar registros según los criterios especificados o realizar una llamada API personalizada a la variable [!DNL Adobe Target] API.


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
    </tr>
  </tbody>
</table>


Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Antes de usar la variable [!DNL Adobe Target] , debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener un [!DNL Adobe Target] cuenta.

## Crear una conexión con [!DNL Adobe Target]

Para crear una conexión para su [!DNL Adobe Target] módulos:

1. Haga clic en **[!UICONTROL Agregar]** junto al cuadro Conexión.

1. Complete los campos siguientes:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Introduzca un nombre para esta conexión.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Escriba la [!DNL Adobe] ID de cliente. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Escriba la [!DNL Adobe] Secreto del cliente. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de organización]</td>
        <td>Escriba la [!DNL Adobe] ID de organización. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
        <td>Escriba la [!DNL Adobe] ID de cuenta técnica. Esto se puede encontrar en la sección [!UICONTROL Credentials details] de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Inquilino]</td>
        <td>
          <p> Para localizar su inquilino, inicie sesión en la [!DNL Adobe Experience Cloud], abra [!DNL Target]y haga clic en el botón [!DNL Target] tarjeta. Utilice el valor de ID de inquilino como se indica en el subdominio de URL.</p>
          <p>Por ejemplo, si la dirección URL al iniciar sesión en [!DNL Adobe Target] es <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> su ID de inquilino es "mycompany".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta-Scopes]</td>
        <td>Entrar <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Clave privada]</td>
        <td>
          <p>Introduzca la clave privada que se generó cuando se crearon sus credenciales en el [!DNL Adobe Developer Console]. </p>
          <p>Para extraer la clave privada o el certificado:</p>
          <ol>
            <li value="1">
              <p>Haga clic en <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Seleccione el tipo de archivo que está extrayendo.</p>
            </li>
            <li value="3">
              <p>Seleccione el archivo que contiene la clave privada o el certificado.</p>
            </li>
            <li value="4">
              <p>Introduzca la contraseña del archivo.</p>
            </li>
            <li value="5">
              <p>Haga clic en <b>[!UICONTROL Guardar]</b> para extraer el archivo y volver a la configuración de conexión.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Target] módulos y sus campos

Al configurar [!DNL Adobe Target] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Adobe Target] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)

* [Búsquedas](#searches)


### Acciones

* [[!UICONTROL Crear un registro]](#create-a-record)

* [[!UICONTROL Realizar una llamada API personalizada]](#make-a-custom-api-call)

* [[!UICONTROL Eliminar un registro]](#delete-a-record)

* [[!UICONTROL Leer un registro]](#read-a-record)

* [[!UICONTROL Actualizar un registro]](#update-a-record)


#### [!UICONTROL Crear un registro]

Este módulo de acción crea una actividad AB o XT, una oferta o una audiencia.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Crear una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Seleccione el tipo de registro que desea crear.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Continúe con <a href="#AB%C2%A0Activ" class="MCXref xref" >Campos de actividad AB</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p>Continúe con <a href="#XT" class="MCXref xref" >Campos de actividad XT</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Offer]</p>
          <p>Continúe con <a href="#Offer" class="MCXref xref" >Campos de oferta</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Continúe con <a href="#Audience" class="MCXref xref" >Campos de audiencia</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### Campos de actividad AB

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Introduzca o asigne un nombre para esta actividad. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opciones]</td>
      <td>
        <p>Para cada opción que desee agregar a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Opción ID local]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla en el seguimiento de la opción entre solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Introduzca o asigne un nombre para la opción. El nombre no debe tener más de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de oferta]</b>
            </p>
          </li>
          <li>
            <p>Seleccione o asigne la opción Offer associated with the .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ubicaciones]</td>
      <td>
        <p>Para cada mbox que desee agregar a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p>[!UICONTROL ID de audiencia]</p>
            <p>Para cada audiencia que desee agregar a Mbox, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el ID de audiencia.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla en el seguimiento de la ubicación entre solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Introduzca o asigne un nombre para la ubicación. El nombre no debe tener más de 250 caracteres.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiencias]</td>
      <td>
        <p>Una lista de ubicaciones en la página donde se sirve la oferta de contenido. Una ubicación contiene lo siguiente:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Especifique o asigne el ID de la experiencia</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Introduzca o asigne el nombre de la experiencia

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Para cada audiencia que desee que vea la experiencia, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el ID de audiencia.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Porcentaje de visitantes]</b>
            </p>
            <p>Introduzca o asigne el porcentaje de visitantes asignado a la experiencia</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Métricas]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de terceros]</td>
      <td>Introduzca o asigne un ID para identificar esta actividad. Puede elegir este ID. Este ID no debe ser el mismo que otra actividad y no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comienza en]</td>
      <td>Introduzca o asigne la fecha y la hora en las que desea iniciar la actividad con el formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL finaliza en]</td>
      <td>Introduzca o asigne la fecha y la hora para finalizar la actividad con el formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Introduzca o asigne el estado de la actividad.</p>
        <ul>
          <li>
            <p>[!UICONTROL Aprobado]</p>
          </li>
          <li>
            <p>[!UICONTROL desactivado]</p>
          </li>
          <li>
            <p>[!UICONTROL en pausa]</p>
          </li>
          <li>
            <p>[!UICONTROL Guardado] </p>
          </li>
          <li>
            <p>[!UICONTROL Eliminado]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Introduzca un número que defina la prioridad de la actividad. Los números más altos tienen mayor prioridad. Este valor debe estar entre 0 y 999. El valor predeterminado es 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asignación automática del tráfico]</td>
      <td>
        <p>Active esta opción para asignar automáticamente el tráfico. La asignación automática envía más tráfico a la experiencia más exitosa.</p>
        <p>Seleccione o asigne los criterios de evaluación mediante los cuales juzgar qué experiencia tiene más éxito.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Introduzca o asigne el espacio de trabajo al que está asociada la actividad</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de propiedades] </td>
      <td>Para cada propiedad que desee agregar a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione o asigne el ID de la propiedad.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Audiencias de informes]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada audiencia de informes que desee agregar a la actividad, haga clic en [!UICONTROL Agregar elemento] e introduzca la siguiente información:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID local de audiencia de informes]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla con el fin de rastrear la audiencia de informes en todas las solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Introduzca o asigne el segmento que se utilizará en los informes</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla en el seguimiento de la métrica entre solicitudes de API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de actividad XT

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Introduzca o asigne un nombre para esta actividad. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opciones]</td>
      <td>
        <p>Para cada opción que desee agregar a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Opción ID local]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla en el seguimiento de la opción entre solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Introduzca o asigne un nombre para la opción. El nombre no debe tener más de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de oferta]</b>
            </p>
          </li>
          <li>
            <p>Seleccione o asigne la opción Offer associated with the .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ubicaciones]</td>
      <td>
        <p>Para cada mbox que desee agregar a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p>[!UICONTROL ID de audiencia]</p>
            <p>Para cada audiencia que desee agregar a Mbox, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el ID de audiencia.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla en el seguimiento de la ubicación entre solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Introduzca o asigne un nombre para la ubicación. El nombre no debe tener más de 250 caracteres.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiencias]</td>
      <td>
        <p>Una lista de ubicaciones en la página donde se sirve la oferta de contenido. Una ubicación contiene lo siguiente:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Especifique o asigne el ID de la experiencia</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Introduzca o asigne el nombre de la experiencia

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Para cada audiencia que desee que vea la experiencia, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el ID de audiencia.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Porcentaje de visitantes]</b>
            </p>
            <p>Introduzca o asigne el porcentaje de visitantes asignado a la experiencia</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Métricas]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de terceros]</td>
      <td>Introduzca o asigne un ID para identificar esta actividad. Puede elegir este ID. Este ID no debe ser el mismo que otra actividad y no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comienza en]</td>
      <td>Introduzca o asigne la fecha y la hora en las que desea iniciar la actividad con el formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL finaliza en]</td>
      <td>Introduzca o asigne la fecha y la hora para finalizar la actividad con el formato . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Introduzca o asigne el estado de la actividad.</p>
        <ul>
          <li>
            <p>[!UICONTROL Aprobado]</p>
          </li>
          <li>
            <p>[!UICONTROL desactivado]</p>
          </li>
          <li>
            <p>[!UICONTROL en pausa]</p>
          </li>
          <li>
            <p>[!UICONTROL Guardado] </p>
          </li>
          <li>
            <p>[!UICONTROL Eliminado]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Introduzca un número que defina la prioridad de la actividad. Los números más altos tienen mayor prioridad. Este valor debe estar entre 0 y 999. El valor predeterminado es 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asignación automática del tráfico]</td>
      <td>
        <p>Active esta opción para asignar automáticamente el tráfico. La asignación automática envía más tráfico a la experiencia más exitosa.</p>
        <p>Seleccione o asigne los criterios de evaluación mediante los cuales juzgar qué experiencia tiene más éxito.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Introduzca o asigne el espacio de trabajo al que está asociada la actividad</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de propiedades] </td>
      <td>Para cada propiedad que desee agregar a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione o asigne el ID de la propiedad.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Audiencias de informes]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada audiencia de informes que desee agregar a la actividad, haga clic en [!UICONTROL Agregar elemento] e introduzca la siguiente información:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID local de audiencia de informes]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla con el fin de rastrear la audiencia de informes en todas las solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Introduzca o asigne el segmento que se utilizará en los informes</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla en el seguimiento de la métrica entre solicitudes de API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de oferta

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Introduzca o asigne un nombre para esta actividad. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Introduzca o asigne el contenido de la oferta que se mostrará al usuario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Introduzca o asigne el ID del espacio de trabajo asociado a la oferta. Si se deja en blanco, la oferta se asocia con el espacio de trabajo predeterminado de la cuenta. Esta funcionalidad solo se aplica a [!DNL Target] Cuentas Premium.</p>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de audiencia

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Introduzca o asigne un nombre para esta audiencia. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Introduzca o asigne una descripción de esta audiencia.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Regla de destino]</td>
      <td>
        <p>Active la opción para crear reglas AND, es decir, todas las reglas deben aplicarse.</p>
        <p>Para cada regla que desee aplicar a la audiencia, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el JSON de la regla que desee aplicar. </p>
        <div class="example"><span class="autonumber"><span><b>Ejemplo: </b></span></span>
          <p>Ejemplos:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Introduzca o asigne el ID del espacio de trabajo asociado a la audiencia. Si se deja en blanco, la oferta se asocia con el espacio de trabajo predeterminado de la cuenta. Esta funcionalidad solo se aplica a [!DNL Target Premium] cuentas.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Realizar una llamada API personalizada]

Este módulo realiza una llamada API personalizada a la variable [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Crear una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Dirección URL base]</td>
      <td>Introduzca o asigne su [!DNL Target] URL base.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Introduzca una ruta relativa a {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina una sola actividad AB, actividad XT, oferta o audiencia.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Crear una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Seleccione el tipo de registro que desea eliminar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Introduzca o asigne el ID del registro que desea eliminar.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción recupera datos para una sola actividad, oferta, audiencia, propiedad o informe.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Crear una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Seleccione el tipo de registro que desea leer.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Introduzca o asigne el ID del registro que desea leer.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza una Actividad, Oferta o Audiencia.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Crear una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>
        <p>Seleccione el tipo de registro que desea actualizar.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#AB%C2%A0Activ" class="MCXref xref" >Campos de actividad AB</a> under <a href="#Create2" class="MCXref xref" >Crear un registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#XT" class="MCXref xref" >Campos de actividad XT</a> under <a href="#Create2" class="MCXref xref" >Crear un registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Otra actividad]</b>
            </p>
            <p>Seleccione el campo para el que desea actualizar un valor e introduzca el nuevo valor para el campo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#Offer" class="MCXref xref" >Campos de oferta</a> under <a href="#Create2" class="MCXref xref" >Crear un registro</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#Audience" class="MCXref xref" >Campos de audiencia</a> under <a href="#Create2" class="MCXref xref" >Crear un registro</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Introduzca o asigne el ID del registro que desea actualizar.</td>
    </tr>
  </tbody>
</table>

### Búsquedas

* [[!UICONTROL Obtención de registros]](#get-records)

* [[!UICONTROL Buscar]](#search)


#### [!UICONTROL Obtención de registros]

Este módulo de búsqueda recupera una lista de registros del tipo seleccionado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Crear una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>Seleccione el tipo de registro que desea actualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordenar por]</td>
      <td>Para cada campo por el que desee ordenar, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el campo y si los resultados devueltos deben ser ascendentes o descendentes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comienza en]</td>
      <td>
        <p>Introduzca la fecha más temprana para la que desea recuperar registros. </p>
        <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Termina En]</td>
      <td>
        <p>Introduzca la última fecha para la que desea recuperar registros. </p>
        <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Buscar]

Este módulo de búsqueda busca Actividades, Ofertas o Audiencias según los criterios especificados.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obtener instrucciones sobre la creación de una conexión con [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Crear una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Seleccione el tipo de registro que desea actualizar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Ordenar por]</td>
    <td>Para cada campo por el que desee ordenar, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el campo y si los resultados devueltos deben ser ascendentes o descendentes.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Criterios de búsqueda]</td>
    <td>Para cada regla que desee configurar, seleccione el campo , el operador y el valor. Haga clic en <b>[!UICONTROL Agregar Y regla]</b> para crear reglas adicionales.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Desplazamiento]</td>
    <td>
      <p>Introduzca el número de la primera respuesta que desea que devuelva el módulo. La primera respuesta devuelta tiene un desplazamiento de <code>0</code>. Utilice este campo en combinación con el campo [!UICONTROL Número máximo de resultados devueltos] para paginar las respuestas.</p>
      <p>Por ejemplo, para ver la tercera página de respuestas, cuando cada página tiene diez respuestas, establezca [!UICONTROL Offset] en 20 y [!UICONTROL Maximum number of return] en 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Número máximo de resultados devueltos]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario. Utilice este campo en combinación con el campo [!UICONTROL Offset] para paginar las respuestas.</p>
      <p>Por ejemplo, para ver la tercera página de respuestas, cuando cada página tiene diez respuestas, establezca [!UICONTROL Offset] en 20 y [!UICONTROL Maximum number of return] en 10.</p>
    </td>
  </tr>
</tbody>
</table>
