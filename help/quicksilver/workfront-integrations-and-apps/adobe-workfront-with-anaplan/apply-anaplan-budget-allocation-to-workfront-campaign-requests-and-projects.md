---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Aplicar una asignación de presupuesto  [!DNL Anaplan] a una solicitud de campaña o a un proyecto de campaña [!DNL Adobe Workfront] s
description: Este escenario de integración sincroniza cualquier asignación de presupuesto que se haya realizado en [!DNL Anaplan] de nuevo en [!DNL Workfront]. El escenario extrae todos los elementos de presupuesto de campaña vinculados y, a continuación, pasa el valor presupuestado al proyecto de Workfront vinculado si se ha cambiado el valor presupuestario.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Aplicar una asignación de presupuesto de [!DNL Anaplan] a una solicitud de campaña o a un proyecto de campaña [!DNL Adobe Workfront]

Este escenario de integración sincroniza cualquier asignación de presupuesto que se haya realizado en [!DNL Anaplan] con [!DNL Workfront]. El escenario extrae todos los elementos de presupuesto vinculados de la campaña y, a continuación, pasa el valor de presupuesto al proyecto vinculado [!DNL Workfront] si se ha cambiado el valor de presupuesto.

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

* Un perfil de usuario de [!DNL Workfront] denominado **[!DNL Anaplan Integration]**, que tiene derechos de administrador del sistema.

  Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuración [!DNL Anaplan] esperada

Debe tener lo siguiente en [!DNL Anaplan] para utilizar este escenario:

* Un perfil de usuario de [!DNL Anaplan] denominado **[!UICONTROL [!DNL Workfront]Integration]**, que tiene derechos de administrador del sistema.
* El modelo [!DNL Anaplan] que desea usar para este escenario.
* La lista dentro del modelo [!DNL Anaplan] que captura los presupuestos de campaña.

  El módulo de la lista debe admitir la recepción de los atributos siguientes:

   * [!UICONTROL [!DNL Workfront] solicitud GUID]
   * [!UICONTROL [!DNL Workfront] GUID de proyecto]
   * [!UICONTROL Nombre de campaña]
   * [!UICONTROL Fondos de mano de obra solicitados]
   * [!UICONTROL Ingresos estimados]
   * [!UICONTROL Marca]

  Esta lista y este módulo deben almacenar los detalles adicionales necesarios para la funcionalidad normal de [!DNL Anaplan], incluida la capacidad de establecer un presupuesto y comunicar que el elemento de la lista presupuestaria está listo para sincronizarse de nuevo con [!DNL Workfront].

* Una vista en [!DNL Anaplan] llamó a **[!UICONTROL Campañas.Actualizar campañas en Adobe Workfront]**.

  Esta vista debe contener las columnas siguientes, en este orden:

   1. [!UICONTROL Nombre de elemento]

   2. [!UICONTROL [!DNL Workfront] solicitud GUID]

   3. [!UICONTROL [!DNL Workfront] GUID de proyecto]

   4. [!UICONTROL Nombre de campaña]

   5. [!UICONTROL Presupuesto]

   6. [!UICONTROL Ingresos estimados]

   7. [!UICONTROL Marca]

  La vista debe filtrarse para mostrar elementos que tengan un [!UICONTROL [!DNL Workfront] GUID de proyecto] y algún indicador de que las asignaciones presupuestarias deben transmitirse a Workfront.

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la documentación de [!DNL Anaplan].

## Implementación en Workfront Fusion

Complete los siguientes pasos para implementar este escenario de integración en su cuenta de Fusion. Esto solo debe hacerse después de completar la configuración requerida de [!DNL Workfront] y [!DNL Anaplan].

1. Vaya al menú [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en la plantilla de escenario **[!UICONTROL Aplicar asignaciones presupuestarias de [!DNL Anaplan] a solicitudes y proyectos de campaña de Workfront]**.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nombre de vista]</td> 
      <td> <p>Nombre de la vista que contiene los presupuestos de campaña listos para transmitir a [!DNL Workfront].</p> <p>(Ejemplo: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Los detalles sobre cómo configurar los archivos y procesos se proporcionan en la documentación de instalación de [!DNL Anaplan].

1. Seleccione o agregue un perfil de conexión [!DNL Anaplan].
1. Actualice los [!DNL Anaplan] módulos restantes con una conexión de [!DNL Anaplan] cuando se le solicite.
1. En el módulo **[!UICONTROL Convertir CSV a objeto JSON]**, agregue una nueva estructura de datos para asignar las columnas CSV a un objeto JSON utilizable.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Request GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Cuando se le solicite, seleccione esta estructura de datos para otros módulos en esta implementación de escenario.
1. En el módulo **[!UICONTROL Comprobar proyecto vinculado]**, seleccione o agregue un perfil de conexión [!DNL Workfront].
1. Actualice los [!DNL Workfront] módulos restantes con una conexión de [!DNL Workfront] cuando se le solicite.

## Otras plantillas de escenario recomendadas

Para completar el flujo de trabajo representado por esta plantilla, también debe implementar la siguiente plantilla adicional:

* [[!UICONTROL Crear un [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Otros escenarios para la optimización del gasto son:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de proyecto a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de horas reales a un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] gastos a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
