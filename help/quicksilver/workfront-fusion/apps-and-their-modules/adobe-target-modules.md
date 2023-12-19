---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Target
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] Los módulos de le permiten crear, leer, actualizar o eliminar registros, enumerar todos los registros de un tipo determinado, buscar registros basados en los criterios especificados o realizar una llamada de API personalizada a [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: c0be0a1f21d5db3a480485a39e019a129d248574
workflow-type: tm+mt
source-wordcount: '2665'
ht-degree: 0%

---

# [!DNL Adobe Target] Módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Adobe Target], así como conectarlo a múltiples aplicaciones y servicios de terceros. [!DNL Adobe Target] Los módulos de le permiten crear, leer, actualizar o eliminar registros, enumerar todos los registros de un tipo determinado, buscar registros basados en los criterios especificados o realizar una llamada de API personalizada a [!DNL Adobe Target] API.


Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario](../../workfront-fusion/scenarios/create-a-scenario.md).

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
        <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>
      <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td>
    </tr>
    </tr>
  </tbody>
</table>


Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Antes de usar el [!DNL Adobe Target] Conector de, debe asegurarse de que se cumplen los siguientes requisitos previos:

* Debe tener un activo [!DNL Adobe Target] cuenta.

## Cree una conexión con [!DNL Adobe Target]

Para crear una conexión para su [!DNL Adobe Target] módulos:

1. Clic **[!UICONTROL Añadir]** situado junto al cuadro Conexión.

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
        <td role="rowheader">[!UICONTROL ID de cliente]</td>
        <td>Introduzca su [!DNL Adobe] ID de cliente. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
        <td>Introduzca su [!DNL Adobe] Secreto del cliente. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de organización]</td>
        <td>Introduzca su [!DNL Adobe] ID de organización. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
        <td>Introduzca su [!DNL Adobe] ID de cuenta técnica. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Inquilino]</td>
        <td>
          <p> Para localizar a su inquilino, inicie sesión en [!DNL Adobe Experience Cloud], abrir [!DNL Target]y haga clic en [!DNL Target] Tarjeta de. Utilice el valor ID de inquilino como se indica en el subdominio URL.</p>
          <p>Por ejemplo, si su dirección URL al iniciar sesión en [!DNL Adobe Target] es <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> a continuación, su ID de inquilino es "mycompany".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL MetaÁmbitos]</td>
        <td>Entrar <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Clave privada]</td>
        <td>
          <p>Introduzca la clave privada que se generó cuando se crearon las credenciales en la [!DNL Adobe Developer Console]. </p>
          <p>Para extraer la clave privada o el certificado:</p>
          <ol>
            <li value="1">
              <p>Clic <b>[!UICONTROL Extraer]</b>.</p>
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
              <p>Clic <b>[!UICONTROL Guardar]</b> para extraer el archivo y volver a la configuración de conexión.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## [!DNL Adobe Target] módulos y sus campos

Al configurar [!DNL Adobe Target] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Adobe Target] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)

* [Búsquedas](#searches)


### Acciones

* [[!UICONTROL Creación de un registro]](#create-a-record)

* [[!UICONTROL Realizar una llamada de API personalizada]](#make-a-custom-api-call)

* [[!UICONTROL Eliminación de un registro]](#delete-a-record)

* [[!UICONTROL Leer un registro]](#read-a-record)

* [[!UICONTROL Actualización de un registro]](#update-a-record)


#### [!UICONTROL Creación de un registro]

Este módulo de acción crea una actividad AB o XT, una oferta o una audiencia.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexión]</td>
    <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Cree una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Seleccione el tipo de registro que desea crear.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Continuar a <a href="#ab-activity-fields" class="MCXref xref" >Campos de actividad AB</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p>Continuar a <a href="#xt-activity-fields" class="MCXref xref" >Campos de actividad XT</a>.</p>
        </li>
        <li>
          <p>Oferta de [!UICONTROL]</p>
          <p>Continuar a <a href="#offer-fields" class="MCXref xref" >Campos de oferta</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Continuar a <a href="#audience-fields" class="MCXref xref" >Campos de audiencia</a>.</p>
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>Introduzca o asigne un nombre para esta actividad. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opciones]</td>
      <td>
        <p>Para cada opción que desee añadir a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Id. local de opción]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizar en el seguimiento de la opción entre solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nombre]</b>
            </p>
            <p>Introduzca o asigne un nombre para la opción. El nombre no debe tener más de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de oferta]</b>
            </p>
          </li>
          <li>
            <p>Seleccione o asigne la opción Oferta asociada a.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ubicaciones]</td>
      <td>
        <p>Para cada Mbox que desee añadir a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p>[!UICONTROL ID de audiencia]</p>
            <p>Para cada audiencia que desee agregar al mbox, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el ID de audiencia.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Id. local de ubicación]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla para rastrear la ubicación en varias solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nombre]</b>
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
            <p><b>[!UICONTROL ID local de experiencia]</b>
            </p>
            <p>Introduzca o asigne el ID de la experiencia</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nombre]</b>
            </p>
            <p>Introduzca o asigne el nombre de la experiencia

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Para cada audiencia en la que desee ver la experiencia, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el ID de audiencia.

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
      <td role="rowheader">[!UICONTROL Empieza en]</td>
      <td>Introduzca o asigne la fecha y la hora de inicio de la actividad con el formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Finaliza en]</td>
      <td>Introduzca o asigne la fecha y la hora de finalización de la actividad con el formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Estado]</td>
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
            <p>[!UICONTROL En pausa]</p>
          </li>
          <li>
            <p>[!UICONTROL Guardado] </p>
          </li>
          <li>
            <p>[!UICONTROL eliminado]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Prioridad]</td>
      <td>Introduzca un número que defina la prioridad de la actividad. Los números más altos tienen mayor prioridad. Este valor debe estar entre 0 y 999. El valor predeterminado es 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tráfico de asignación automática]</td>
      <td>
        <p>Active esta opción para asignar automáticamente el tráfico. La asignación automática envía más tráfico a una experiencia más exitosa.</p>
        <p>Seleccione o asigne los criterios de evaluación según los cuales se juzgará qué experiencia tiene más éxito.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Introduzca o asigne el espacio de trabajo al que está asociada la actividad</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de propiedad] </td>
      <td>Para cada propiedad que desee añadir a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione o asigne el ID de la propiedad.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada audiencia de informes que desee agregar a la actividad, haga clic en [!UICONTROL Agregar elemento] e introduzca la siguiente información:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizar en el seguimiento de la audiencia de informes en las solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de audiencia]</b>
            </p>
            <p>Introduzca o asigne el segmento que se utilizará en el sistema de informes</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local de métrica]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla para rastrear la métrica en varias solicitudes de API.</p>
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>Introduzca o asigne un nombre para esta actividad. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opciones]</td>
      <td>
        <p>Para cada opción que desee añadir a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Id. local de opción]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizar en el seguimiento de la opción entre solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nombre]</b>
            </p>
            <p>Introduzca o asigne un nombre para la opción. El nombre no debe tener más de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de oferta]</b>
            </p>
          </li>
          <li>
            <p>Seleccione o asigne la opción Oferta asociada a.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ubicaciones]</td>
      <td>
        <p>Para cada Mbox que desee añadir a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y rellene los campos siguientes:</p>
        <ul>
          <li>
            <p>[!UICONTROL ID de audiencia]</p>
            <p>Para cada audiencia que desee agregar al mbox, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione el ID de audiencia.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Id. local de ubicación]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla para rastrear la ubicación en varias solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nombre]</b>
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
            <p><b>[!UICONTROL ID local de experiencia]</b>
            </p>
            <p>Introduzca o asigne el ID de la experiencia</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nombre]</b>
            </p>
            <p>Introduzca o asigne el nombre de la experiencia

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Para cada audiencia en la que desee ver la experiencia, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el ID de audiencia.

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
      <td role="rowheader">[!UICONTROL Empieza en]</td>
      <td>Introduzca o asigne la fecha y la hora de inicio de la actividad con el formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Finaliza en]</td>
      <td>Introduzca o asigne la fecha y la hora de finalización de la actividad con el formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Estado]</td>
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
            <p>[!UICONTROL En pausa]</p>
          </li>
          <li>
            <p>[!UICONTROL Guardado] </p>
          </li>
          <li>
            <p>[!UICONTROL eliminado]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Prioridad]</td>
      <td>Introduzca un número que defina la prioridad de la actividad. Los números más altos tienen mayor prioridad. Este valor debe estar entre 0 y 999. El valor predeterminado es 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tráfico de asignación automática]</td>
      <td>
        <p>Active esta opción para asignar automáticamente el tráfico. La asignación automática envía más tráfico a una experiencia más exitosa.</p>
        <p>Seleccione o asigne los criterios de evaluación según los cuales se juzgará qué experiencia tiene más éxito.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Introduzca o asigne el espacio de trabajo al que está asociada la actividad</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Id. de propiedad] </td>
      <td>Para cada propiedad que desee añadir a la actividad, haga clic en <b>[!UICONTROL Agregar elemento]</b> y seleccione o asigne el ID de la propiedad.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada audiencia de informes que desee agregar a la actividad, haga clic en [!UICONTROL Agregar elemento] e introduzca la siguiente información:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizar en el seguimiento de la audiencia de informes en las solicitudes de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de audiencia]</b>
            </p>
            <p>Introduzca o asigne el segmento que se utilizará en el sistema de informes</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local de métrica]</b>
            </p>
            <p>Introduzca o asigne una cadena para utilizarla para rastrear la métrica en varias solicitudes de API.</p>
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>Introduzca o asigne un nombre para esta actividad. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Contenido]</td>
      <td>
        <p>Introduzca o asigne el contenido de la oferta que se mostrará al usuario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Introduzca o asigne el ID del espacio de trabajo asociado a la oferta. Si se deja en blanco, la oferta se asocia al espacio de trabajo predeterminado de la cuenta. Esta funcionalidad solo se aplica a [!DNL Target] Cuentas Premium.</p>
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
      <td role="rowheader">[!UICONTROL Nombre]</td>
      <td>Introduzca o asigne un nombre para esta audiencia. El nombre no puede tener más de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Contenido]</td>
      <td>
        <p>Introduzca o asigne una descripción de esta audiencia.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Regla de destino]</td>
      <td>
        <p>Active el botón de alternancia para crear reglas AND, es decir, todas las reglas deben aplicarse.</p>
        <p>Para cada regla que desee aplicar a la audiencia, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el JSON de la regla que desea aplicar. </p>
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
        <p>Introduzca o asigne el ID del espacio de trabajo asociado a la audiencia. Si se deja en blanco, la oferta se asocia al espacio de trabajo predeterminado de la cuenta. Esta funcionalidad solo se aplica a [!DNL Target Premium] cuentas.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Realizar una llamada de API personalizada]

Este módulo realiza una llamada de API personalizada a [!DNL Adobe Target] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Cree una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] URL base]</td>
      <td>Introduzca o asigne su [!DNL Target] URL base.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Ruta]</p>
      </td>
      <td>
        <p>Introduzca una ruta relativa a {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminación de un registro]

Este módulo de acción elimina una sola actividad AB, actividad XT, oferta o audiencia.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexión]</td>
    <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Cree una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Seleccione el tipo de registro que desea eliminar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID de registro]</td>
    <td>Introduzca o asigne el ID del registro que desea eliminar.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción recupera datos de una sola actividad, oferta, audiencia, propiedad o informe.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexión]</td>
    <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Cree una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Seleccione el tipo de registro que desea leer.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID de registro]</td>
    <td>Introduzca o asigne el ID del registro que desea leer.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Actualización de un registro]

Este módulo de acción actualiza una actividad, oferta o audiencia.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Cree una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>
        <p>Seleccione el tipo de registro que desea actualizar.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#ab-activity-fields" class="MCXref xref" >Campos de actividad AB</a> bajo <a href="#create-a-record" class="MCXref xref" >Creación de un registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#xt-activity-fields" class="MCXref xref" >Campos de actividad XT</a> bajo <a href="#create-a-record" class="MCXref xref" >Creación de un registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Otra actividad]</b>
            </p>
            <p>Seleccione el campo para el que desea actualizar un valor e introduzca el nuevo valor para el campo.</p>
          </li>
          <li>
            <p><b>Oferta de [!UICONTROL]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#offer-fields" class="MCXref xref" >Campos de oferta</a> bajo <a href="#create-a-record" class="MCXref xref" >Creación de un registro</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Consulte las descripciones de los campos en <a href="#audience-fields" class="MCXref xref" >Campos de audiencia</a> bajo <a href="#create-a-record" class="MCXref xref" >Creación de un registro</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de registro]</td>
      <td>Introduzca o asigne el ID del registro que desea actualizar.</td>
    </tr>
  </tbody>
</table>

### Búsquedas

* [[!UICONTROL Obtener registros]](#get-records)

* [[!UICONTROL Búsqueda]](#search)


#### [!UICONTROL Obtener registros]

Este módulo de búsqueda recupera una lista de registros del tipo seleccionado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexión]</td>
      <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Cree una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
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
      <td role="rowheader">[!UICONTROL Comienza En]</td>
      <td>
        <p>Introduzca la fecha más temprana para la que desea recuperar registros. </p>
        <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Finaliza En]</td>
      <td>
        <p>Introduzca la última fecha para la que desea recuperar registros. </p>
        <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Búsqueda]

Este módulo de búsqueda busca Actividades, Ofertas o Audiencias en función de los criterios especificados.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexión]</td>
    <td>Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Cree una conexión con [!DNL Adobe Target]</a> en este artículo.</td>
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
    <td>Para cada regla que desee configurar, seleccione el campo, el operador y el valor. Clic <b>[!UICONTROL Agregar regla AND]</b> para crear reglas adicionales.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Desplazamiento]</td>
    <td>
      <p>Introduzca el número de la primera respuesta que desea que devuelva el módulo. La primera respuesta devuelta tiene un desplazamiento de <code>0</code>. Utilice este campo en combinación con el campo [!UICONTROL Número máximo de resultados devueltos] para paginar las respuestas.</p>
      <p>Por ejemplo, para ver la tercera página de respuestas, cuando cada página tenga diez respuestas, establezca [!UICONTROL Desplazamiento] en 20 y [!UICONTROL Número máximo de resultados devueltos] en 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Número máximo de resultados devueltos]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario. Utilice este campo en combinación con el campo [!UICONTROL Offset] para paginar las respuestas.</p>
      <p>Por ejemplo, para ver la tercera página de respuestas, cuando cada página tenga diez respuestas, establezca [!UICONTROL Desplazamiento] en 20 y [!UICONTROL Número máximo de resultados devueltos] en 10.</p>
    </td>
  </tr>
</tbody>
</table>
