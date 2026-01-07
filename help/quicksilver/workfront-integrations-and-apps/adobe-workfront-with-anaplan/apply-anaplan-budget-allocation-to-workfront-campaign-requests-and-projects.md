---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Aplicar una asignación de presupuesto de [!DNL Anaplan] a una solicitud de campaña o a un proyecto de campaña [!DNL Adobe Workfront] '
description: Este escenario de integración sincroniza cualquier asignación de presupuesto que se haya realizado en [!DNL Anaplan] de nuevo en [!DNL Workfront]. El escenario extrae todas las partidas presupuestarias de campaña vinculadas y, a continuación, pasa el valor presupuestado al proyecto de Workfront vinculado si se ha modificado el valor del presupuesto.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 99%

---

# Aplicar una asignación de presupuesto de [!DNL Anaplan] a una solicitud de campaña o a un proyecto de campaña de [!DNL Adobe Workfront]

Este escenario de integración sincroniza cualquier asignación de presupuesto que se haya realizado en [!DNL Anaplan] de nuevo en [!DNL Workfront]. El escenario extrae todas las partidas presupuestarias de campaña vinculadas y, a continuación, pasa el valor presupuestado al proyecto de [!DNL Workfront] vinculado si se ha modificado el valor del presupuesto.

>[!IMPORTANT]
>
>“Campaña” en este artículo se refiere al caso de uso de campaña de marketing que representa este escenario, y no está relacionado en modo alguno con el conector [!DNL Workfront Fusion] Adobe Campaign ni con el objeto [!UICONTROL Campaña] de [!DNL Workfront], recientemente obsoleto.


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete del flujo de trabajo de Adobe Workfront y cualquier paquete de integración y automatización de Adobe Workfront</p><p>Workfront Ultimate</p><p>Paquetes Workfront Prime y Select, con una compra adicional de Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> <p>Estándar</p><p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront Fusion</td> 
   <td>
   <p>Basado en operaciones: no se requiere licencia de Workfront Fusion</p>
   <p>Basado en conector (heredado): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Si su organización tiene un paquete de Workfront Select o Prime que no incluye la automatización y la integración de Workfront, su organización debe adquirir Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de Adobe Workfront Fusion, consulte [licencias de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Evento desencadenante

Este escenario está programado para ejecutarse cada 15 minutos.

## Configuración de [!DNL Workfront] prevista

Debe tener lo siguiente en [!DNL Workfront] para utilizar este escenario:

* Un perfil de usuario de [!DNL Workfront] denominado **[!DNL Anaplan Integration]**, que tiene derechos de administrador del sistema.

  Para obtener información sobre la creación de un usuario en [!DNL Workfront], consulte [Añadir usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuración de [!DNL Anaplan] prevista

Debe tener lo siguiente en [!DNL Anaplan] para utilizar este escenario:

* Un perfil de usuario de [!DNL Anaplan] denominado Integración de **[!UICONTROL [!DNL Workfront]]**, que tiene derechos de administrador del sistema.
* El modelo de [!DNL Anaplan] que desea usar para este escenario.
* La lista dentro del modelo de [!DNL Anaplan] que captura los presupuestos de campaña.

  El módulo de la lista debe admitir la recepción de los atributos siguientes:

   * Solicitud GUID de [!UICONTROL [!DNL Workfront]]
   * GUID de proyecto de [!UICONTROL [!DNL Workfront]]
   * [!UICONTROL Nombre de campaña]
   * [!UICONTROL Fondos de mano de obra solicitados]
   * [!UICONTROL Ingresos estimados]
   * [!UICONTROL Marca]

  Esta lista y el módulo deben almacenar detalles adicionales necesarios para la funcionalidad normal de [!DNL Anaplan], incluida la capacidad de establecer un presupuesto y comunicar que el elemento de la lista presupuestaria está listo para sincronizarse de nuevo con [!DNL Workfront].

* Una vista en [!DNL Anaplan] llamó a **[!UICONTROL Campañas.Actualizar campañas en Adobe Workfront]**.

  Esta vista debe contener las columnas siguientes, en este orden:

   1. [!UICONTROL Nombre de elemento]

   2. Solicitud GUID de [!UICONTROL [!DNL Workfront]]

   3. GUID de proyecto de [!UICONTROL [!DNL Workfront]]

   4. [!UICONTROL Nombre de campaña]

   5. [!UICONTROL Presupuesto]

   6. [!UICONTROL Ingresos estimados]

   7. [!UICONTROL Marca]

  La vista debe filtrarse para mostrar elementos que tengan un GUID de proyecto de [!UICONTROL [!DNL Workfront]] y algún indicador de que las asignaciones presupuestarias deben transmitirse a Workfront.

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la documentación de [!DNL Anaplan].

## Implementación en Workfront Fusion

Complete los siguientes pasos para implementar este escenario de integración en su cuenta de Fusion. Esto solo debe hacerse después de completar la configuración requerida de [!DNL Workfront] y [!DNL Anaplan].

1. Vaya al menú [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en la plantilla de escenario **[!UICONTROL Aplicar asignaciones presupuestarias de [!DNL Anaplan] a solicitudes y proyectos de campaña de Workfront]**.
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
      <td>El ID de un espacio de trabajo de su cuenta de [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>El ID de un modelo de su cuenta de [!DNL Anaplan] y el espacio de trabajo seleccionado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>El nombre de la lista de su cuenta de [!DNL Anaplan] y el espacio de trabajo y modelo seleccionados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] View Name]</td> 
      <td> <p>Nombre de la vista que contiene los presupuestos de campaña listos para transmitir a [!DNL Workfront].</p> <p>(Ejemplo: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Los detalles sobre cómo configurar los archivos y procesos se proporcionan en la documentación de instalación de [!DNL Anaplan].

1. Seleccione o añada un perfil de conexión de [!DNL Anaplan].
1. Actualice todos los módulos restantes de [!DNL Anaplan] con una conexión de [!DNL Anaplan] cuando se le pida.
1. En el módulo **[!UICONTROL Convertir CSV a objeto JSON]**, añada una nueva estructura de datos para asignar las columnas CSV a un objeto JSON utilizable.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Request GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Cuando se le solicite, seleccione esta estructura de datos para otros módulos en esta implementación de escenario.
1. En el módulo **[!UICONTROL Comprobar proyecto vinculado]**, seleccione o añada un perfil de conexión de [!DNL Workfront].
1. Actualice los módulos de [!DNL Workfront] restantes con una conexión de [!DNL Workfront] cuando se le solicite.

## Otras plantillas de escenario recomendadas

Para completar el flujo de trabajo representado por esta plantilla, también debe implementar la siguiente plantilla adicional:

* [[!UICONTROL Crear un elemento de lista de  [!DNL Anaplan]  a partir de una solicitud de campaña de  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Otros escenarios para la optimización del gasto son:

* [[!UICONTROL Enviar actualizaciones de proyecto de  [!DNL Adobe Workfront]  a un elemento de lista de  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar actualizaciones de horas reales de  [!DNL Adobe Workfront]  a un elemento de lista de  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar gastos de  [!DNL Adobe Workfront]  a un elemento de lista de  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
