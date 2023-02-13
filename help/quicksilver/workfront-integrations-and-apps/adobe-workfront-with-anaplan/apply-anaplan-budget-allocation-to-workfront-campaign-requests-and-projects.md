---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Aplicar un [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] solicitud de campaña o proyecto de campaña
description: Este escenario de integración sincroniza cualquier asignación de presupuesto que se haya realizado en [!DNL Anaplan] volver a [!DNL Workfront]. El escenario extrae todos los elementos de presupuesto de campaña vinculados y, a continuación, pasa el valor presupuestado al proyecto de Workfront vinculado si se ha cambiado el valor del presupuesto.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Aplicar un [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] solicitud de campaña o proyecto de campaña

Este escenario de integración sincroniza cualquier asignación de presupuesto que se haya realizado en [!DNL Anaplan] volver a [!DNL Workfront]. El escenario extrae todos los elementos de presupuesto de campaña vinculados y luego pasa el valor de presupuesto al [!DNL Workfront] proyecto si se ha cambiado el valor del presupuesto.

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

* Un perfil de usuario en [!DNL Workfront] named **[!DNL Anaplan Integration]**, que tiene derechos de administrador del sistema.

   Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Esperado [!DNL Anaplan] Configuración

Debe tener lo siguiente en [!DNL Anaplan] para usar este escenario:

* Un perfil de usuario en [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront]Integración]**, que tiene derechos de administrador del sistema.
* La variable [!DNL Anaplan] Modelo que desea utilizar para este escenario.
* La lista dentro de la variable [!DNL Anaplan] Modelo que captura los presupuestos de campaña.

   El módulo de la lista debe admitir la recepción de los siguientes atributos:

   * [!UICONTROL [!DNL Workfront] GUID de solicitud]
   * [!UICONTROL [!DNL Workfront] GUID del proyecto]
   * [!UICONTROL Nombre de la campaña]
   * [!UICONTROL Fondos laborales solicitados]
   * [!UICONTROL Ingresos estimados]
   * [!UICONTROL Marca]

   Esta lista y módulo deben almacenar los detalles adicionales que son necesarios para la funcionalidad normal de [!DNL Anaplan], incluida la capacidad de establecer un presupuesto y comunicar que el elemento de la lista de presupuestos está listo para ser sincronizado de nuevo en [!DNL Workfront].

* Una vista en [!DNL Anaplan] llamado **[!UICONTROL Campañas.Actualizar campañas en Adobe Workfront]**.

   Esta vista debe contener las columnas siguientes, en este orden:

   1. [!UICONTROL Nombre del elemento]

   2. [!UICONTROL [!DNL Workfront] GUID de solicitud]

   3. [!UICONTROL [!DNL Workfront] GUID del proyecto]

   4. [!UICONTROL Nombre de la campaña]

   5. [!UICONTROL Presupuesto]

   6. [!UICONTROL Ingresos estimados]

   7. [!UICONTROL Marca]
   La vista debe filtrarse para que muestre los elementos que tienen un [!UICONTROL [!DNL Workfront] GUID del proyecto] y algunos indicadores de que las asignaciones presupuestarias deben transmitirse al Workfront.

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la [!DNL Anaplan] documentación.

## Implementación en Workfront Fusion

Complete los siguientes pasos para implementar este escenario de integración en su cuenta de Fusion. Esto solo debe hacerse después de completar el [!DNL Workfront] y [!DNL Anaplan] configuración.

1. Vaya a la [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en el botón **[!UICONTROL Aplicar [!DNL Anaplan] asignaciones presupuestarias a solicitudes y proyectos de campaña de Workfront]** plantilla de escenario.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Ver nombre]</td> 
      <td> <p>Nombre de la vista que contiene presupuestos de campaña listos para transmitir a [!DNL Workfront].</p> <p>(Ejemplo: [!UICONTROL Campañas.Cargar campañas a [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   En la sección [!DNL Anaplan] documentación de configuración.

1. Seleccione o agregue un [!DNL Anaplan] perfil de conexión.
1. Actualizar el resto [!DNL Anaplan] módulos con un [!DNL Anaplan] cuando se le pida.
1. En el **[!UICONTROL Convertir CSV a objeto JSON]** , agregue una nueva estructura de datos para asignar las columnas CSV a un objeto JSON utilizable.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Cuando se le pida, seleccione esta estructura de datos para otros módulos en esta implementación de escenario.
1. En el **[!UICONTROL Comprobar proyecto vinculado]** módulo, seleccione o agregue un [!DNL Workfront] perfil de conexión.
1. Actualizar el resto [!DNL Workfront] módulos con un [!DNL Workfront] cuando se le pida.

## Otras plantillas de escenario recomendadas

Para completar el flujo de trabajo representado por esta plantilla, también debe implementar la siguiente plantilla adicional:

* [[!UICONTROL Cree un [!DNL Anaplan] elemento de lista de un [!DNL Adobe Workfront] solicitud de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Entre los escenarios adicionales para la optimización de los gastos se incluyen:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones del proyecto a un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de horas reales en un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] los gastos de [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
