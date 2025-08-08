---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Crear secciones personalizadas
description: La información que ve en la aplicación web de  [!DNL Workfront]  se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente sobre un área u objeto de  [!DNL Workfront] .
author: Courtney
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: ac34076ddc0b5815c262a61326534a1241c17a4c
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 99%

---

# Crear secciones personalizadas

## Secciones de [!DNL Adobe Workfront] 

La información que ve en la aplicación web [!DNL Workfront] se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente acerca de un área u objeto de [!DNL Workfront].\
Para obtener más información sobre las áreas predeterminadas de [!DNL Workfront], consulte el artículo [Acerca del diseño predeterminado [!DNL Adobe Workfront] .](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)

Además de las secciones que se incluyen con [!DNL Workfront] de manera predeterminada, es posible añadir un panel en el que se puede mostrar información relacionada con el flujo de trabajo. No se puede añadir un panel de control a todas las áreas y objetos.

La siguiente tabla enumera todas las áreas y objetos de [!DNL Workfront] que contienen secciones en el panel izquierdo y cuáles se pueden personalizar:

| Área u objeto de **[!DNL Workfront]** | **Secciones predeterminadas del sistema** | **Secciones personalizadas** |
|---|---|---|
| Área de proyectos de  | ✓ | ✓ |
| [!UICONTROL Equipo] | ✓ |   |
| Área de [!UICONTROL solicitudes] | ✓ |   |
| Área de [!UICONTROL plantillas de horas] | ✓ |   |
| [!UICONTROL Portafolio] | ✓ | ✓ |
| [!UICONTROL Programa] | ✓ | ✓ |
| [!UICONTROL Proyecto] | ✓ | ✓ |
| [!UICONTROL Tarea] | ✓ |  ✓ |
| [!UICONTROL Problema] |  ✓ |  ✓ |
| [!UICONTROL Usuario] |  ✓ |  ✓ |
| [!UICONTROL Documento] |  ✓ |  ✓ |
| Área de [!UICONTROL recursos] | ✓ | ✓ |

{style="table-layout:auto"}

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td>[!UICONTROL Reviewer] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Ver acceso al tipo de objeto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Añadir un panel en el panel izquierdo de un objeto o área de [!DNL Workfront]

Para poder añadir un panel, debe crearlo con toda la información que desee mostrar en él. También puede crear una página externa.\
Para obtener más información acerca de la creación de paneles, consulte el artículo [Crear un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Para obtener más información acerca de la creación de páginas externas, consulte el artículo [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Después de crear el panel o la página externa, puede añadirlos al panel izquierdo.

1. Vaya a una de las áreas u objetos de [!DNL Workfront] donde puede añadir una sección personalizada en el panel izquierdo.\
   O
1. Vaya a un objeto donde pueda añadir un [!UICONTROL panel] en el panel izquierdo.\
   Para obtener más información sobre las áreas y los objetos a los que puede añadir secciones personalizadas, consulte el apartado [[!DNL Adobe Workfront] secciones](#adobe-workfront-sections).
1. Haga clic en **[!UICONTROL Añadir al panel]** en el panel izquierdo.
1. Escriba un nombre para el panel en el campo **[!UICONTROL Nombre del vínculo rápido]**. Esto solo es visible para el propio usuario.
1. Empiece a escribir el nombre de un panel existente o de una página externa en el campo **[!UICONTROL Elegir un panel]** y, a continuación, seleccione el panel cuando se muestre en la lista.
1. Haga clic en **[!UICONTROL Añadir]**.
1. (Opcional) Arrastre y suelte las secciones en el orden en que desee mostrarlas.

   La sección superior es la sección predeterminada de la página.

   Las secciones creadas para objetos individuales se muestran al acceder a todos los objetos del mismo tipo y solo están disponibles para el usuario.

## Mostrar paneles en el panel izquierdo de objetos

Para obtener más información sobre cómo añadir un panel debajo de un objeto, consulte la sección [[!UICONTROL Añadir un panel] en el panel izquierdo de un objeto o área de Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) de este artículo.

Cuando se añade un panel a una sección personalizada debajo de un objeto, el objeto actúa como filtro para el panel. Por ejemplo, si añade un informe de tareas a un panel y añade el panel a un proyecto, la sección personalizada que contiene el panel del proyecto solo muestra las tareas del proyecto que está consultando.

Los objetos siguientes se filtran para el objeto bajo el que se muestran, si dicho objeto es superior en jerarquía a ellos:

* Proyecto
* Tarea
* Problema
* Proceso de aprobación
* Nota
* Documento

Para obtener más información acerca de la jerarquía y la interdependencia de objetos, consulte la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalización del panel izquierdo en una plantilla de diseño

Al añadir paneles a la instancia de [!DNL Workfront], estos solo son visibles para usted.

Puede personalizar las secciones de [!DNL Workfront] y compartir el nuevo diseño con varios usuarios en una plantilla de diseño. Solamente un administrador de sistema o de grupo puede compartirlos con otros usuarios en una plantilla de diseño. Para obtener más información sobre cómo personalizar el panel izquierdo con una plantilla de diseño, consulte [Personalizar el panel izquierdo con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
