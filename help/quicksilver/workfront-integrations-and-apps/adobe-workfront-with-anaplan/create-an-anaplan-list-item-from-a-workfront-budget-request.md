---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Crear un  [!DNL Anaplan] elemento de lista a partir de una [!DNL Adobe Workfront] solicitud de presupuesto
description: Este escenario de integración vincula un  [!DNL Adobe Workfront] proyecto (campaña) con un [!DNL Anaplan] elemento de lista de presupuesto. Esto se logra agregando una solicitud de presupuesto al  [!DNL Workfront] proyecto que necesita recibir fondos. Este escenario observa las solicitudes de presupuesto no procesadas y luego ejecuta un proceso para crear un elemento de lista de presupuesto vacío en  [!DNL Anaplan]  para iniciar los procesos de asignación de presupuesto en Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Crear un elemento de lista [!DNL Anaplan] a partir de una solicitud de presupuesto de [!DNL Adobe Workfront]

Este escenario de integración vincula un proyecto (campaña) [!DNL Adobe Workfront] con un elemento de lista presupuestaria [!DNL Anaplan]. Esto se logra agregando una solicitud de presupuesto al proyecto [!DNL Workfront] que necesita recibir fondos. Este escenario observa las solicitudes de presupuesto no procesadas y luego ejecuta un proceso para crear un elemento de lista de presupuesto vacío en [!DNL Anaplan] para iniciar los procesos de asignación de presupuesto en [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Licencia de Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL Workfront Fusion para automatización e integración de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para usar la funcionalidad descrita en este artículo.</td> 
  </tr>
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

&#42;&#42;Para obtener información sobre[!DNL  Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento desencadenante

Este escenario está programado para ejecutarse cada 15 minutos.

## Configuración [!DNL Workfront] esperada

Debe tener lo siguiente en [!DNL Workfront] para utilizar este escenario:

* Un perfil de usuario de [!DNL Workfront] denominado *[!UICONTROL *[!DNL Anaplan] Integration]**, que tiene derechos de administrador del sistema.

  Para obtener información sobre cómo crear un usuario en [!DNL Workfront], consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Formulario personalizado **[!UICONTROL Solicitud de presupuesto]** adjunto al objeto [!UICONTROL Solicitud].

  Los siguientes campos obligatorios deben incluirse en el formulario personalizado para ayudar en la asignación de datos a [!DNL Anaplan]:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Nombre de campo</th> 
     <th>Tipo de campo</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Tipo de solicitud de presupuesto]</td> 
     <td> <p>[!UICONTROL Desplegable]</p> <p>Opciones:</p> 
      <ul> 
       <li> <p>[!UICONTROL Ajuste de fondos]</p> </li> 
       <li> <p>[!UICONTROL Financiación inicial]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fondos de mano de obra solicitados]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fondos de gasto solicitados]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  Para obtener información sobre cómo crear formularios personalizados, consulte [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Plantillas de proyecto que representan campañas y otros proyectos que requieren financiación, configuradas con un tema de cola [!UICONTROL Solicitud de presupuesto]. El tema de la cola [!UICONTROL Solicitud de presupuesto] está asignado para usar el formulario personalizado [!UICONTROL Solicitud de presupuesto].
* Un formulario **[!UICONTROL Resumen de campaña]** para el objeto de proyecto.

  Este formulario debe contener los campos siguientes:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Campo de texto enriquecido]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Mensaje de clave]</td> 
     <td>[!UICONTROL Campo de texto enriquecido]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Audiencia de destino]</td> 
     <td> <p>[!UICONTROL Desplegable]</p> <p>Incluya opciones que se ajusten a sus procesos.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Para obtener información sobre cómo crear formularios personalizados, consulte [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuración [!DNL Anaplan] esperada

Debe tener lo siguiente en [!DNL Anaplan] para utilizar este escenario:

* Un perfil de usuario de [!DNL Anaplan] denominado **[!UICONTROL [!DNL Workfront]Integration]**, que tiene derechos de administrador del sistema.
* El modelo [!DNL Anaplan] que desea usar para este escenario.
* La lista dentro del modelo [!DNL Anaplan] que captura los presupuestos de campaña.

  El módulo de la lista debe admitir la recepción de los atributos siguientes:

   * [!UICONTROL GUID de proyecto de Workfront]
   * [!UICONTROL Nombre de campaña]
   * [!UICONTROL Fondos de mano de obra solicitados]
   * [!UICONTROL Fondos de gastos solicitados]
   * [!UICONTROL Tipo de solicitud de presupuesto]
   * [!UICONTROL Motivo del ajuste de fondos]

  Esta lista y este módulo deben almacenar los detalles adicionales necesarios para la funcionalidad normal de [!DNL Anaplan], incluida la capacidad de establecer un presupuesto y comunicar que el elemento de la lista presupuestaria está listo para sincronizarse de nuevo con [!DNL Workfront].

Para obtener instrucciones sobre cualquiera de estas acciones, consulte la documentación de [!DNL Anaplan].

## Implementando en [!DNL Workfront Fusion]

Complete los siguientes pasos para implementar este escenario de integración en su cuenta de [!DNL Fusion]. Esto solo debe hacerse después de completar la configuración requerida de [!DNL Workfront] y [!DNL Anaplan].

1. Vaya al menú [!UICONTROL Plantillas] en [!DNL Workfront Fusion] y haga clic en el elemento de lista **[!UICONTROL Crear un elemento de lista [!DNL Anaplan] a partir de una plantilla de escenario de solicitud de presupuesto de Workfront]**.
1. Reemplace los valores de las variables para las siguientes [!DNL Anaplan] variables:

   | Nombre de variable | Reemplazar valor por |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | El identificador de un área de trabajo de su cuenta de [!DNL Anaplan]. |
   | [!UICONTROL [!DNL Anaplan] ID de modelo] | El identificador de un modelo de su cuenta de [!DNL Anaplan] y el área de trabajo seleccionada. |
   | [!UICONTROL [!DNL Anaplan] nombre de módulo] | Nombre del módulo que describe los atributos de campaña en la lista [!DNL Anaplan] seleccionada. |
   | [!UICONTROL Nombre de lista de campaña] | El nombre de la lista de su cuenta de [!DNL Anaplan] y el espacio de trabajo y modelo seleccionados. |

   {style="table-layout:auto"}

   Los detalles sobre cómo configurar los archivos y procesos se proporcionan en la documentación de instalación de [!DNL Anaplan].

1. Seleccione o agregue un perfil de conexión [!DNL Anaplan].
1. Actualice los [!DNL Anaplan] módulos restantes con una conexión de [!DNL Anaplan] cuando se le solicite.
1. Seleccione o agregue un perfil de conexión [!DNL Workfront].

   Después de implementar la plantilla, este es el módulo que actualizará para agregar o quitar referencias de campo personalizadas del valor de la propiedad fields si desea modificar los campos asignados predeterminados a [!DNL Anaplan].

1. Actualice los [!DNL Workfront] módulos restantes con una conexión de [!DNL Workfront] cuando se le solicite.

## Otras plantillas de escenario recomendadas

Para completar el flujo de trabajo representado por esta plantilla, también debe implementar la siguiente plantilla adicional:

* [[!UICONTROL Aplicar una [!DNL Anaplan] asignación de presupuesto a un [!DNL Adobe Workfront] proyecto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Otros escenarios para la optimización del gasto son:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de proyecto a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] actualizaciones de horas reales a un [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] gastos a [!DNL Anaplan] elemento de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
