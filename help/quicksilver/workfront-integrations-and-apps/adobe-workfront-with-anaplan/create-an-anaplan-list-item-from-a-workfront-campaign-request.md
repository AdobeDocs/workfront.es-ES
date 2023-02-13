---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Cree un [!DNL Anaplan] elemento de lista de un [!DNL Adobe Workfront] solicitud de campaña
description: Este escenario de integración vincula un [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista de presupuesto.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 2%

---

# Cree un [!DNL Anaplan] elemento de lista de un [!DNL Adobe Workfront] solicitud de campaña

Este escenario de integración vincula un [!DNL Adobe Workfront] proyecto con un [!DNL Anaplan] elemento de lista de presupuesto.

Este escenario observa las nuevas solicitudes de campaña agregadas a una cola de solicitudes. Tan pronto como se registra una solicitud de campaña, se agrega un elemento de línea de presupuesto en [!DNL Anaplan] para iniciar el proceso de financiación.

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
   <td role="rowheader">Plan de [!UICONTROL Adobe Workfront]*</td> 
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

* Un perfil de usuario en [!DNL Workfront] named **[!UICONTROL [!DNL Anaplan]Integración]**, que tiene derechos de administrador del sistema.

   Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Informe de campaña]** formulario personalizado adjunto al [!UICONTROL Solicitud] objeto.

   Los siguientes campos obligatorios deben incluirse en el formulario personalizado para ayudar en la asignación de datos a Anaplan:

   | Nombre de campo | Tipo de campo |
   |---|---|
   | [!UICONTROL Total de fondos solicitados] |  |
   | [!UICONTROL Fondos laborales solicitados] |  |
   | [!UICONTROL Fondos de gastos solicitados] |  |
   | [!UICONTROL Se envió a [!DNL Anaplan]] | Casilla de verificación |

   Los siguientes campos opcionales pueden estar presentes en el formulario. Este escenario asigna solo los campos anteriores, pero cualquier campo adicional del informe de campaña puede asignarse.

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
     <td role="rowheader">[!UICONTROL En Fecha De Inicio Del Mercado]</td> 
     <td>Fecha </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL En Fecha De Finalización Del Mercado]</td> 
     <td>Fecha</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>Campo de texto de párrafo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Mensaje clave]</td> 
     <td>Campo de texto de párrafo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Audiencia de destino]</td> 
     <td> <p>Lista desplegable</p> <p>Incluya opciones que se ajusten a sus procesos.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Para obtener información sobre la creación de formularios personalizados, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Proyecto configurado como cola de solicitudes para capturar nuevas solicitudes de campaña. La variable [!UICONTROL Informe de campaña] debe adjuntarse a estas solicitudes.

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
   * [!UICONTROL Fondos de gastos solicitados]
   * [!UICONTROL Tipo de solicitud de presupuesto]

   Esta lista y módulo deben almacenar los detalles adicionales que son necesarios para la funcionalidad normal de [!DNL Anaplan], incluida la capacidad de establecer un presupuesto y comunicar que el elemento de la lista de presupuestos está listo para ser sincronizado de nuevo en [!DNL Workfront].

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la [!DNL Anaplan] documentación.

## Implementación para [!DNL Workfront Fusion]

Complete los siguientes pasos para implementar este escenario de integración en su [!DNL Fusion] cuenta. Esto solo debe hacerse después de completar el [!DNL Workfront] y [!DNL Anaplan] configuración.

1. Vaya a la [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en el botón **[!UICONTROL Cree un [!DNL Anaplan] elemento de lista de una solicitud de campaña de Workfront]** plantilla de escenario.
1. Reemplace los valores de las variables para lo siguiente [!DNL Anaplan] variables:

   | Nombre de variable | Reemplazar valor por |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] ID de espacio de trabajo] | El ID de un espacio de trabajo de su [!DNL Anaplan] cuenta. |
   | [!UICONTROL [!DNL Anaplan] ID de modelo] | El ID de un modelo de su [!DNL Anaplan] y el espacio de trabajo seleccionado. |
   | [!UICONTROL [!DNL Anaplan] Nombre del módulo] | El nombre del módulo que describe los atributos de campaña en el [!DNL Anaplan] Lista. |
   | [!UICONTROL Nombre de la lista de campañas] | El nombre de la lista de su [!DNL Anaplan] y el espacio de trabajo y modelo seleccionados. |

   {style=&quot;table-layout:auto&quot;}

   En la sección [!DNL Anaplan] documentación de configuración.

1. Seleccione o agregue un [!DNL Anaplan] perfil de conexión.
1. Actualizar el resto [!DNL Anaplan] módulos con un [!DNL Anaplan] cuando se le pida.
1. Seleccione o agregue un [!DNL Workfront] perfil de conexión.

   Después de implementar la plantilla, este es el módulo que desea actualizar para agregar o quitar referencias de campo personalizadas del valor de la propiedad fields si desea modificar los campos asignados predeterminados a [!DNL Anaplan].

1. Actualizar el resto [!DNL Workfront] módulos con un [!DNL Workfront] cuando se le pida.

## Otras plantillas de escenario recomendadas

Para completar el flujo de trabajo representado por esta plantilla, también debe implementar la siguiente plantilla adicional:

* [[!UICONTROL Aplicar un [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] solicitud de campaña o proyecto de campaña]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Entre los escenarios adicionales para la optimización de los gastos se incluyen:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones del proyecto a un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de horas reales en un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] los gastos de [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
