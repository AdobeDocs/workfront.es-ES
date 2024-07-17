---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Enviar  [!DNL Adobe Workfront] gastos a un [!DNL Anaplan] elemento de lista
description: Este escenario de integración comparte detalles relacionados con los gastos de un  [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista de presupuesto. Compartir esta información le permite aprovechar mejor la optimización de gastos y el análisis financiero que [!DNL Anaplan] proporciona.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Enviar [!DNL Adobe Workfront] gastos a un elemento de lista [!DNL Anaplan]

Este escenario de integración comparte detalles relacionados con los gastos de un proyecto [!DNL Adobe Workfront] con un elemento de la lista presupuestaria [!DNL Anaplan]. Compartir esta información le permite aprovechar mejor la optimización de gastos y el análisis financiero que [!DNL Anaplan] proporciona.

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
   <td role="rowheader">Product</td> 
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

* Un perfil de usuario de [!DNL Workfront] denominado *[!UICONTROL *[!DNL Anaplan] Integration]**, que tiene derechos de administrador del sistema.

  Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Se ha adjuntado un formulario personalizado **[!UICONTROL Resumen de campaña]** al objeto de proyecto para almacenar los valores de datos personalizados que el usuario decida enviar a [!DNL Anaplan].

  El formulario debe contener los campos siguientes:

  | Nombre de campo | Tipo de campo |
  |---|---|
  | [!UICONTROL Fecha de última transmisión] | Fecha |
  | [!UICONTROL Notas de integración] | Campo de texto de párrafo |

  Para obtener información sobre cómo crear formularios personalizados, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Configuración [!DNL Anaplan] esperada

Debe tener lo siguiente en [!DNL Anaplan] para utilizar este escenario:

* Un perfil de usuario de [!DNL Anaplan] denominado **[!UICONTROL [!DNL Workfront]Integration]**, que tiene derechos de administrador del sistema.
* El modelo [!DNL Anaplan] que desea usar para este escenario.
* La lista dentro del modelo [!DNL Anaplan] que desea que capture los presupuestos de campaña.
* Un archivo de **[!UICONTROL importación real de gastos de Anaplan]** que contiene las siguientes columnas, en este orden:

   1. [!UICONTROL [!DNL Workfront] GUID de gasto]

   2. [!UICONTROL [!DNL Workfront] GUID de proyecto]

   3. [!UICONTROL Importe real]

   4. [!UICONTROL Descripción]

   5. [!UICONTROL Tipo de gasto]

   6. [!UICONTROL Fecha de vigencia]

   7. [!UICONTROL Nombre de campaña]

   8. [!UICONTROL [!DNL Anaplan] id. de elemento de lista]

  Para preparar el archivo [!UICONTROL [!DNL Anaplan] de importación de gastos reales ]:

   1. Copie y pegue lo siguiente en un editor de texto o [!DNL Excel].
   1. Guarde el archivo en formato CSV.
   1. Cargue el archivo en [!DNL Anaplan].

      Para obtener instrucciones, consulte la documentación de [!DNL Anaplan] acerca de cómo importar datos en módulos desde un archivo.

   1. Tome nota del nombre que dio al archivo; se usará durante la implementación de la plantilla de escenario [!UICONTROL Fusion].

  Ejemplo de contenido CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Archivo **[!UICONTROL [!DNL Anaplan]de importación de gastos planificada]** que contiene las siguientes columnas, en este orden:

   1. [!UICONTROL [!DNL Workfront] GUID de gasto]

   2. [!UICONTROL [!DNL Workfront] GUID de proyecto]

   3. [!UICONTROL Importe real]

   4. [!UICONTROL Descripción]

   5. [!UICONTROL Tipo de gasto]

   6. [!UICONTROL Fecha de vigencia]

   7. [!UICONTROL Nombre de campaña]

   8. [!UICONTROL [!DNL Anaplan] id. de elemento de lista]

  Para preparar el archivo [!UICONTROL [!DNL Anaplan] de importación de gastos planificada ]:

   1. Copie y pegue lo siguiente en un editor de texto o [!DNL Excel]
   1. Guarde el archivo en formato CSV
   1. Cargue el archivo en Anaplan.

      Para obtener instrucciones, consulte la documentación de [!DNL Anaplan] acerca de cómo importar datos en módulos desde un archivo.

   1. Tome nota del nombre que dio al archivo; se usará durante la implementación de la plantilla de escenario [!UICONTROL Fusion].

  Ejemplo de contenido CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Un proceso de **[!UICONTROL importación de actualización de proyecto]** preparado para ejecutar la importación de los datos entregados en una carga de archivo.

>[!NOTE]
>
>Existen archivos de importación independientes para los gastos planificados y reales, de modo que se puedan registrar de forma independiente en las fechas planificadas y en vigor, respectivamente.

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la documentación de [!DNL Anaplan].

## Implementando en [!DNL Fusion]

Complete los siguientes pasos para implementar este escenario de integración en su cuenta de [!DNL Fusion]. Esto solo debe hacerse después de completar la configuración requerida de [!DNL Workfront] y [!DNL Anaplan].

1. Vaya al menú [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en la plantilla de escenario **[!UICONTROL Enviar actualizaciones de gastos de Workfront a [!DNL Anaplan] elemento de lista]**.
1. Reemplace los valores de las variables para las siguientes [!DNL Anaplan] variables:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nombre de variable</th> 
      <th>Reemplazar valor por</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>Identificador del área de trabajo de su cuenta de [!DNL Anaplan] que desea usar para este escenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de modelo] </td> 
      <td>El identificador del modelo de su cuenta de [!DNL Anaplan] y el área de trabajo seleccionada que desea usar para este escenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de lista de campañas]</td> 
      <td>El nombre de la lista de su cuenta de [!DNL Anaplan] y el área de trabajo y modelo seleccionados que desea usar para este escenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de archivo: importación de gastos real]</td> 
      <td> <p>Nombre del archivo que recibirá los datos de gastos reales del proyecto.</p> <p> (Ejemplo: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de archivo: importación de gastos planificada]</td> 
      <td> <p>Nombre del archivo que recibirá los datos de gastos planeados del proyecto.</p> <p> (Ejemplo: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de proceso: importación de actualización de proyecto]</td> 
      <td> <p>Nombre del proceso que ejecutará la importación de datos de gastos del proyecto.</p> <p>(Ejemplo: WF Int - Cargar gastos del proyecto)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Los detalles sobre cómo configurar los archivos y procesos se proporcionan en la documentación de instalación de [!DNL Anaplan].

1. Seleccione o agregue un perfil de conexión [!DNL Anaplan].
1. Actualice los [!DNL Anaplan] módulos restantes con una conexión de [!DNL Anaplan] cuando se le solicite.
1. Seleccione o agregue un perfil de conexión [!DNL Workfront].
1. Actualice los [!DNL Workfront] módulos restantes con una conexión de [!DNL Workfront] cuando se le solicite.
1. En el módulo **[!UICONTROL Generar CSV de gastos reales]**, agregue una nueva estructura de datos para asignar los atributos del proyecto a columnas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. En el módulo **[!UICONTROL Generar CSV de gastos planificados]**, agregue una nueva estructura de datos para asignar los atributos del proyecto a columnas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Otras plantillas de escenario recomendadas

Esta plantilla de escenario se complementa con las siguientes plantillas de escenario de optimización de gasto que también se pueden implementar:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de proyecto a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de horas reales a un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Escenarios adicionales para vincular solicitudes de presupuesto:

* [[!UICONTROL Crear un [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de presupuesto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar una [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] proyecto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Escenarios adicionales para vincular solicitudes de campaña:

* [[!UICONTROL Crear un [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar una [!DNL Anaplan] asignación de presupuesto a una [!DNL Adobe Workfront] solicitud o proyecto de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
