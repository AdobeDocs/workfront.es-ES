---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Enviar gastos de  [!DNL Adobe Workfront]  a un elemento de lista de  [!DNL Anaplan] '
description: Este escenario de integración comparte detalles relacionados con los gastos de un  [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista de presupuesto. Compartir esta información le permite aprovechar mejor la optimización de gastos y el análisis financiero que  [!DNL Anaplan]  proporciona.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 53%

---

# Enviar [!DNL Adobe Workfront] gastos a un elemento de lista [!DNL Anaplan]

Este escenario de integración comparte detalles relacionados con los gastos de un proyecto [!DNL Adobe Workfront] con un elemento de la lista presupuestaria [!DNL Anaplan]. Compartir esta información le permite aprovechar mejor la optimización de los gastos y el análisis financiero que proporciona [!DNL Anaplan].

>[!IMPORTANT]
>
>“Campaign” en este artículo hace referencia al caso de uso de la campaña de marketing que representa este escenario y no está conectado de ninguna manera al conector de Adobe Campaign [!DNL Workfront Fusion] ni al objeto [!UICONTROL Campaign] recientemente en desuso en [!DNL Workfront].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de flujo de trabajo de Adobe Workfront y cualquier paquete de integración y automatización de Adobe Workfront</p><p>Workfront Ultimate</p><p>Paquetes Workfront Prime y Select, con una compra adicional de Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> <p>Estándar</p><p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront Fusion</td> 
   <td>
   <p>Basado en operaciones: no se requiere licencia de Workfront Fusion</p>
   <p>Basado en conectores (heredado): Workfront Fusion para la automatización e integración del trabajo </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Si su organización tiene un paquete Select o Prime Workfront que no incluye la automatización y la integración de Workfront, su organización debe adquirir Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de Adobe Workfront Fusion, consulte [licencias de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Evento desencadenante

Este escenario está programado para ejecutarse cada 15 minutos.

## Configuración de [!DNL Workfront] prevista

Debe tener lo siguiente en [!DNL Workfront] para utilizar este escenario:

* Un perfil de usuario de [!DNL Workfront] denominado *[!UICONTROL *[!DNL Anaplan] Integration]**, que tiene derechos de administrador del sistema.

  Para obtener información sobre la creación de un usuario en [!DNL Workfront], consulte [Añadir usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Se ha adjuntado un formulario personalizado **[!UICONTROL Resumen de campaña]** al objeto de proyecto para almacenar los valores de datos personalizados que el usuario decida enviar a [!DNL Anaplan].

  El formulario debe contener los campos siguientes:

  | Nombre de campo | Tipo de campo |
  |---|---|
  | [!UICONTROL Fecha de última transmisión] | Fecha |
  | [!UICONTROL Notas de integración] | Campo de texto de párrafo |

  Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuración de [!DNL Anaplan] prevista

Debe tener lo siguiente en [!DNL Anaplan] para utilizar este escenario:

* Un perfil de usuario de [!DNL Anaplan] denominado Integración de **[!UICONTROL [!DNL Workfront]]**, que tiene derechos de administrador del sistema.
* El modelo de [!DNL Anaplan] que desea usar para este escenario.
* La lista dentro del modelo [!DNL Anaplan] que desea que capture los presupuestos de campaña.
* Un archivo de **[!UICONTROL importación real de gastos de Anaplan]** que contiene las siguientes columnas, en este orden:

   1. [!UICONTROL [!DNL Workfront] GUID de gasto]

   2. GUID de proyecto de [!UICONTROL [!DNL Workfront]]

   3. [!UICONTROL Importe real]

   4. [!UICONTROL Descripción]

   5. [!UICONTROL Tipo de gasto]

   6. [!UICONTROL Fecha de vigencia]

   7. [!UICONTROL Nombre de la campaña]

   8. [!UICONTROL [!DNL Anaplan] ID de elemento de lista]

  Para preparar el archivo [!UICONTROL [!DNL Anaplan] de importación de gastos reales &#x200B;]:

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

   2. GUID de proyecto de [!UICONTROL [!DNL Workfront]]

   3. [!UICONTROL Importe real]

   4. [!UICONTROL Descripción]

   5. [!UICONTROL Tipo de gasto]

   6. [!UICONTROL Fecha de vigencia]

   7. [!UICONTROL Nombre de la campaña]

   8. [!UICONTROL [!DNL Anaplan] ID de elemento de lista]

  Para preparar el archivo [!UICONTROL [!DNL Anaplan]Coste planificado de gastos]:

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
1. Reemplace los valores de las variables para las siguientes variables de [!DNL Anaplan]:

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>Identificador del área de trabajo de su cuenta de [!DNL Anaplan] que desea usar para este escenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>El identificador del modelo de su cuenta de [!DNL Anaplan] y el área de trabajo seleccionada que desea usar para este escenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
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
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Nombre del proceso que ejecutará la importación de datos de gastos del proyecto.</p> <p>(Ejemplo: WF Int - Cargar gastos del proyecto)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Los detalles sobre cómo configurar los archivos y procesos se proporcionan en la documentación de instalación de [!DNL Anaplan].

1. Seleccione o añada un perfil de conexión de [!DNL Anaplan].
1. Actualice todos los módulos de [!DNL Anaplan] restantes con una conexión de [!DNL Anaplan] cuando se le solicite.
1. Seleccione o añada un perfil de conexión de [!DNL Workfront].
1. Actualice todos los módulos de [!DNL Workfront] restantes con una conexión de [!DNL Workfront] cuando se le solicite.
1. En el módulo **[!UICONTROL Generar CSV de gastos reales]**, agregue una nueva estructura de datos para asignar los atributos del proyecto a columnas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. En el módulo **[!UICONTROL Generar CSV de gastos planificados]**, agregue una nueva estructura de datos para asignar los atributos del proyecto a columnas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Otras plantillas de escenario recomendadas

Esta plantilla de escenario se complementa con las siguientes plantillas de escenario de optimización de gastos que también se pueden implementar:

* [[!UICONTROL Enviar actualizaciones de proyecto de  [!DNL Adobe Workfront]  a un elemento de lista de  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar actualizaciones de horas reales de  [!DNL Adobe Workfront]  a un elemento de lista de  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Escenarios adicionales para vincular solicitudes de presupuesto:

* [[!UICONTROL Crear un elemento de lista de [!DNL Anaplan] a partir de una solicitud de presupuesto de [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar una asignación de presupuesto de [!DNL Anaplan] a un proyecto de [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Escenarios adicionales para vincular solicitudes de campaña:

* [[!UICONTROL Crear un elemento de lista de [!DNL Anaplan] a partir de una solicitud de campaña de [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar una asignación de presupuesto de [!DNL Anaplan] a una solicitud o proyecto de campaña de [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
