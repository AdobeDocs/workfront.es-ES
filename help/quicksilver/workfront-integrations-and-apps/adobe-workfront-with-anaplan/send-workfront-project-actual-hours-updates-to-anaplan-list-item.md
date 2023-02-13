---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Enviar [!DNL Adobe Workfront] actualizaciones de horas reales en un [!DNL Anaplan] elemento de lista
description: Este escenario de integración comparte detalles de horas reales capturados en un [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista de presupuesto. El uso compartido de esta información le permite aprovechar mejor la optimización del gasto y el análisis financiero que [!DNL Anaplan] proporciona.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Enviar [!DNL Adobe Workfront] actualizaciones de horas reales en un [!DNL Anaplan] elemento de lista

Este escenario de integración comparte detalles de horas reales capturados en un [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista de presupuesto. El uso compartido de esta información le permite aprovechar mejor la optimización del gasto y el análisis financiero que [!DNL Anaplan] proporciona.

Esta plantilla de escenario ofrece una lista de horas resumidas por proyecto, día y función registrados en proyectos activos durante los últimos 3 meses.

>[!IMPORTANT]
>
>&quot;Campaña&quot; en este artículo se refiere al caso de uso de la campaña de marketing que representa este escenario y que no está de ningún modo conectado al [!DNL Workfront Fusion] Conector de Adobe Campaign o al recientemente obsoleto [!UICONTROL Campaign] en [!DNL Workfront].

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento de activación

Este escenario está programado para ejecutarse cada 15 minutos.

## Esperado [!DNL Workfront] Configuración

Debe tener lo siguiente en [!DNL Workfront] para usar este escenario:

* Un perfil de usuario en [!DNL Workfront] named **[!UICONTROL Integración de Anaplan]**, que tiene derechos de administrador del sistema.

   Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Esperado [!DNL Anaplan] Configuración

Debe tener lo siguiente en [!DNL Anaplan] para usar este escenario:

* Un perfil de usuario en [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront ]Integración]**, que tiene derechos de administrador del sistema.
* La variable [!DNL Anaplan] Modelo que desea utilizar para este escenario.
* La lista dentro de la variable [!DNL Anaplan] Modelo que desea utilizar para este escenario.
* Un archivo en [!DNL Anaplan] named **[!UICONTROL Importación de horas reales de Anaplan]** que contiene las columnas siguientes, en este orden:

   1. [!UICONTROL GUID de proyecto de Workfront]

   2. [!UICONTROL Horas]

   3. [!UICONTROL Coste estimado de horas]

   4. [!UICONTROL Fecha de entrada]

   5. [!UICONTROL Nombre del rol]

   6. [!UICONTROL Nombre de la campaña]

   7. [!UICONTROL [!DNL Anaplan] ID de elemento de lista]
   Para preparar la [!DNL Anaplan] Archivo de informe de gastos reales:

   1. Copie y pegue lo siguiente en un editor de texto o [!DNL Excel]
   1. Guarde el archivo en formato CSV
   1. Cargue el archivo en [!DNL Anaplan].

      Para obtener instrucciones, consulte la [!DNL Anaplan] documentación sobre la importación de datos en módulos desde un archivo.

   1. Anote el nombre que dio al expediente; se utilizará durante la implementación del [!UICONTROL Fusión] plantilla de escenario.

   Ejemplo de contenido de CSV

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL Importación de horas reales del proyecto]** proceso preparado para ejecutar la importación de datos entregados en una carga de archivo.

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la [!DNL Anaplan] documentación.

## Implementación para [!DNL Workfront Fusion]

Complete los siguientes pasos para implementar este escenario de integración en su [!DNL Fusion] cuenta. Esto solo debe hacerse después de completar el [!DNL Workfront] y [!DNL Anaplan] configuración.

1. Vaya a la [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en el botón **[!UICONTROL Enviar actualizaciones de horas reales de Workfront a [!DNL Anaplan] elemento de lista]** plantilla de escenario.
1. Reemplace los valores de las variables para lo siguiente [!DNL Anaplan] variables:

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de espacio de trabajo]</td> 
      <td>El ID de un espacio de trabajo de su [!DNL Anaplan] cuenta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Id. de modelo] </td> 
      <td>El ID de un modelo de su [!DNL Anaplan] y el espacio de trabajo seleccionado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>El nombre de la lista de su [!DNL Anaplan] y el espacio de trabajo y modelo seleccionados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre del archivo: Importación de horas reales]</td> 
      <td> <p>Nombre del archivo que recibirá los datos de horas reales del proyecto.</p> <p> (Ejemplo: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre del proceso: Importación de horas reales]</td> 
      <td> <p>Nombre del proceso que ejecutará la importación de datos de horas del proyecto.</p> <p>(Ejemplo: Int de WF: cargar horas del proyecto por función)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdominio]</td> 
      <td>El subdominio de su [!DNL Workfront] cuenta. Se utiliza para crear un vínculo de vuelta a su [!DNL Workfront] proyecto en una nota que se puede generar.</td> 
     </tr> 
    </tbody> 
   </table>

   En la sección [!DNL Anaplan] documentación de configuración.

1. Seleccione o agregue un [!DNL Anaplan] perfil de conexión.
1. Actualizar el resto [!DNL Anaplan] módulos con un [!DNL Anaplan] cuando se le pida.
1. Seleccione o agregue un [!DNL Workfront] perfil de conexión.
1. Actualizar el resto [!DNL Workfront] módulos con un [!DNL Workfront] cuando se le pida.

## Otras plantillas de escenario recomendadas

Esta plantilla de escenario se complementa con las siguientes plantillas de escenario de optimización de gastos que también se pueden implementar:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones del proyecto a un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] los gastos de [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Situaciones adicionales para vincular solicitudes de presupuesto:

* [[!UICONTROL Cree un [!DNL Anaplan] elemento de lista de un [!DNL Adobe Workfront] solicitud de presupuesto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar un [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] proyecto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Situaciones adicionales para vincular solicitudes de campaña:

* [[!UICONTROL Cree un [!DNL Anaplan] elemento de lista de un [!DNL Adobe Workfront] solicitud de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar un [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] solicitud de campaña o proyecto de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
