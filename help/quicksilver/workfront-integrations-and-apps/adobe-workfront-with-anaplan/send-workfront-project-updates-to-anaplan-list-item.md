---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Enviar  [!DNL Adobe Workfront] actualizaciones de proyecto a un [!DNL Anaplan] elemento de lista
description: Este escenario de integración comparte el progreso, el estado y los detalles de programación clave de un  [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista de presupuesto. Compartir esta información le permite aprovechar mejor la optimización de gastos y el análisis financiero que [!DNL Anaplan] proporciona.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# Enviar [!DNL Adobe Workfront] actualizaciones de proyecto a un elemento de lista [!DNL Anaplan]

Este escenario de integración comparte el progreso, el estado y los detalles de programación clave de un proyecto [!DNL Adobe Workfront] con un elemento de lista presupuestaria [!DNL Anaplan]. Compartir esta información le permite aprovechar mejor la optimización de gastos y el análisis financiero que [!DNL Anaplan] proporciona.

>[!IMPORTANT]
>
>&quot;Campaña&quot; en este artículo hace referencia al caso de uso de la campaña de marketing que representa este escenario y no está conectado de ninguna manera al conector Adobe Campaign [!DNL Workfront Fusion] ni al objeto [!UICONTROL Campaign] recientemente obsoleto en [!DNL Workfront].

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
   <td> <p>Workfront Fusion para la automatización e integración del trabajo </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para usar la funcionalidad descrita en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento desencadenante

Este escenario está programado para ejecutarse cada 15 minutos.

## Configuración [!DNL Workfront] esperada

Debe tener lo siguiente en [!DNL Workfront] para utilizar este escenario:

* Un perfil de usuario de [!DNL Workfront] denominado **[!UICONTROL [!DNL Anaplan]Integration]**, que tiene derechos de administrador del sistema.

  Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Se ha adjuntado un formulario personalizado **[!UICONTROL Resumen de campaña]** al objeto de proyecto para almacenar los valores de datos personalizados que decida enviar a Anaplan.

  Los siguientes campos representan ejemplos de campos que se pueden incluir en el formulario personalizado para ayudar en la asignación de datos a Anaplan, pero no son necesarios para este escenario de integración:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Nombre de campo</th> 
     <th>Tipo de campo</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL En Fecha de inicio del mercado]</td> 
     <td>[!UICONTROL Fecha] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL En Fecha de finalización de mercado]</td> 
     <td>[!UICONTROL Fecha]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Información general de [!UICONTROL Campaign]</td> 
     <td>[!UICONTROL Campo de texto de párrafo]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Mensaje de clave]</td> 
     <td>[!UICONTROL Campo de texto de párrafo]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Audiencia de destino]</td> 
     <td> <p>[!UICONTROL Desplegable]</p> <p>Incluya opciones que se ajusten a sus procesos.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Configuración [!DNL Anaplan] esperada

Debe tener lo siguiente en [!DNL Anaplan] para utilizar este escenario:

* Un perfil de usuario de [!DNL Anaplan] denominado **[!UICONTROL [!DNL Workfront]Integration]**, que tiene derechos de administrador del sistema.
* El modelo [!DNL Anaplan] que desea usar para este escenario.
* La lista dentro del modelo [!DNL Anaplan] que desea usar para este escenario.
* Archivo de **[!UICONTROL importación de actualización de proyecto]** que contiene las siguientes columnas, en este orden:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] GUID de proyecto]

3. [!UICONTROL Nombre de campaña]

4. [!UICONTROL Porcentaje completado]

5. [!UICONTROL Fecha planificada de inicio]

6. [!UICONTROL Fecha planificada de finalización]

7. [!UICONTROL Horas planificadas]

8. [!UICONTROL Coste planificado]

9. [!UICONTROL Costo de gasto planificado]

10. [!UICONTROL Costo real de mano de obra]

11. [!UICONTROL Costo de mano de obra planificado]

12. [!UICONTROL Estado]

Para preparar el archivo [!UICONTROL [!DNL Anaplan] de importación de gastos planificada ]:

1. Copie y pegue lo siguiente en un editor de texto o [!DNL Excel]
1. Guarde el archivo en formato CSV
1. Cargue el archivo en Anaplan.

   Para obtener instrucciones, consulte la documentación de [!DNL Anaplan] acerca de cómo importar datos en módulos desde un archivo.

1. Tome nota del nombre que dio al archivo; se usará durante la implementación de la plantilla de escenario [!UICONTROL Fusion].

Ejemplo de contenido CSV

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Las columnas opcionales pueden incluir:

1. [!UICONTROL Información general de campaña]

2. [!UICONTROL Mensaje de clave]

3. [!UICONTROL Fecha de inicio del mercado]

4. [!UICONTROL Fecha de finalización del mercado]

5. [!UICONTROL Audiencia de destino]

Incluya también cualquier otro campo que desee establecer en la asignación.

* Un proceso de **[!UICONTROL importación de actualización de proyecto]** preparado para ejecutar la importación de los datos entregados en una carga de archivo.

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la documentación de [!DNL Anaplan].

## Implementando en [!DNL Workfront Fusion]

Complete los siguientes pasos para implementar este escenario de integración en su cuenta de Fusion. Esto solo debe hacerse después de completar la configuración requerida de [!DNL Workfront] y [!DNL Anaplan].

1. Vaya al menú [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en la plantilla de escenario **[!UICONTROL Enviar actualizaciones de proyecto de Workfront a [!DNL Anaplan] elemento de lista]**.
1. Reemplace los valores de las variables para las siguientes [!DNL Anaplan] variables:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Nombre de variable</th> 
      <th>Reemplazar valor por</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>El identificador de un área de trabajo de su cuenta de [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de modelo] </td> 
      <td>El identificador de un modelo de su cuenta de [!DNL Anaplan] y el área de trabajo seleccionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de lista de campañas]</td> 
      <td>El nombre de la lista de su cuenta de [!DNL Anaplan] y el espacio de trabajo y modelo seleccionados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de archivo: importación de actualización de proyecto]</td> 
      <td>Nombre del archivo que recibirá los datos de actualización del proyecto.<p>(Ejemplo: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de proceso: importación de actualización de proyecto]</td> 
      <td> <p>Nombre del proceso que ejecutará la importación de datos del proyecto.</p> <p>(Ejemplo: WF Int - Actualizar detalles de la campaña)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdominio]</td> 
      <td>El subdominio de su cuenta de [!DNL Workfront]. Se usa para crear un vínculo de regreso al proyecto [!DNL Workfront] en una nota que se puede generar.</td> 
     </tr> 
    </tbody> 
   </table>

   Los detalles sobre cómo configurar los archivos y procesos se proporcionan en la documentación de instalación de [!DNL Anaplan].

1. Seleccione o agregue un perfil de conexión [!DNL Anaplan].
1. Actualice los [!DNL Anaplan] módulos restantes con una conexión de [!DNL Anaplan] cuando se le solicite.
1. Seleccione o agregue un perfil de conexión [!DNL Workfront].

   El filtro está configurado para extraer todos los proyectos vinculados incompletos y aquellos proyectos completados en los últimos 29 minutos. Si cambia la frecuencia del escenario [!DNL Fusion], querrá actualizar este valor una vez que se haya implementado la plantilla de escenario.

1. En el módulo **[!UICONTROL Generar proyectos y actualizar CSV]**, agregue una nueva estructura de datos para asignar los atributos del proyecto a columnas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Actualice los [!DNL Workfront] módulos restantes con una conexión de [!DNL Workfront] cuando se le solicite.

## Otras plantillas de escenario recomendadas

Esta plantilla de escenario se complementa con las siguientes plantillas de escenario de optimización de gasto que también se pueden implementar:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de horas reales a un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] gastos a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Escenarios adicionales para vincular solicitudes de presupuesto:

* [[!UICONTROL Crear un [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de presupuesto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar una [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] proyecto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Escenarios adicionales para vincular solicitudes de campaña:

* [[!UICONTROL Crear un [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar una [!DNL Anaplan] asignación de presupuesto a una [!DNL Adobe Workfront] solicitud o proyecto de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
