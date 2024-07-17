---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Enviar  [!DNL Adobe Workfront] actualizaciones de horas reales a un elemento de lista [!DNL Anaplan] an
description: Este escenario de integración comparte los detalles de horas reales capturadas en un  [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista presupuestaria. Compartir esta información le permite aprovechar mejor la optimización de gastos y el análisis financiero que [!DNL Anaplan] proporciona.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Enviar [!DNL Adobe Workfront] actualizaciones de horas reales a un elemento de lista [!DNL Anaplan]

Este escenario de integración comparte los detalles de horas reales capturadas en un proyecto [!DNL Adobe Workfront] con un elemento de lista presupuestaria [!DNL Anaplan]. Compartir esta información le permite aprovechar mejor la optimización de gastos y el análisis financiero que [!DNL Anaplan] proporciona.

Esta plantilla de escenario ofrece una lista de horas resumidas por proyecto, día y función registradas en proyectos activos durante los últimos 3 meses.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p> </td> 
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

* Un perfil de usuario de [!DNL Workfront] denominado **[!UICONTROL Integración de Anaplan]**, que tiene derechos de administrador del sistema.

  Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuración [!DNL Anaplan] esperada

Debe tener lo siguiente en [!DNL Anaplan] para utilizar este escenario:

* Un perfil de usuario de [!DNL Anaplan] denominado **[!UICONTROL [!DNL Workfront]Integration]**, que tiene derechos de administrador del sistema.
* El modelo [!DNL Anaplan] que desea usar para este escenario.
* La lista dentro del modelo [!DNL Anaplan] que desea usar para este escenario.
* Un archivo de [!DNL Anaplan] denominado **[!UICONTROL Importación de horas reales de Anaplan]** que contiene las siguientes columnas, en este orden:

   1. [!UICONTROL GUID de proyecto de Workfront]

   2. [!UICONTROL Horas]

   3. [!UICONTROL Costo estimado de horas]

   4. [!UICONTROL Fecha de entrada]

   5. [!UICONTROL Nombre de rol]

   6. [!UICONTROL Nombre de campaña]

   7. [!UICONTROL [!DNL Anaplan] id. de elemento de lista]

  Para preparar el archivo del informe de gastos reales de [!DNL Anaplan]:

   1. Copie y pegue lo siguiente en un editor de texto o [!DNL Excel]
   1. Guarde el archivo en formato CSV
   1. Cargue el archivo en [!DNL Anaplan].

      Para obtener instrucciones, consulte la documentación de [!DNL Anaplan] acerca de cómo importar datos en módulos desde un archivo.

   1. Tome nota del nombre que dio al archivo; se usará durante la implementación de la plantilla de escenario [!UICONTROL Fusion].

  Ejemplo de contenido CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* Proceso de **[!UICONTROL importación de horas reales del proyecto]** preparado para ejecutar la importación de los datos entregados en una carga de archivo.

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la documentación de [!DNL Anaplan].

## Implementando en [!DNL Workfront Fusion]

Complete los siguientes pasos para implementar este escenario de integración en su cuenta de [!DNL Fusion]. Esto solo debe hacerse después de completar la configuración requerida de [!DNL Workfront] y [!DNL Anaplan].

1. Vaya al menú [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en la plantilla de escenario **[!UICONTROL Enviar actualizaciones de horas reales de Workfront a [!DNL Anaplan] elemento de lista]**.
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
      <td role="rowheader">[!UICONTROL Nombre de archivo: importación de horas reales]</td> 
      <td> <p>Nombre del archivo que recibirá los datos de horas reales del proyecto.</p> <p> (Ejemplo: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de proceso: importación de horas reales]</td> 
      <td> <p>Nombre del proceso que ejecutará la importación de datos de horas del proyecto.</p> <p>(Ejemplo: WF Int - Cargar horas del proyecto por rol)</p> </td> 
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
1. Actualice los [!DNL Workfront] módulos restantes con una conexión de [!DNL Workfront] cuando se le solicite.

## Otras plantillas de escenario recomendadas

Esta plantilla de escenario se complementa con las siguientes plantillas de escenario de optimización de gasto que también se pueden implementar:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de proyecto a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] gastos a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Escenarios adicionales para vincular solicitudes de presupuesto:

* [[!UICONTROL Crear un [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de presupuesto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar una [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] proyecto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Escenarios adicionales para vincular solicitudes de campaña:

* [[!UICONTROL Crear un [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar una [!DNL Anaplan] asignación de presupuesto a una [!DNL Adobe Workfront] solicitud o proyecto de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
