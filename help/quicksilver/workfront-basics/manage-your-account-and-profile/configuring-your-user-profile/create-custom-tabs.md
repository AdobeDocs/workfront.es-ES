---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Creación de secciones personalizadas
description: La información que ve en la aplicación web  [!DNL Workfront] se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente sobre un área u objeto  [!DNL Workfront] .
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Creación de secciones personalizadas

## [!DNL Adobe Workfront] secciones

La información que ve en la aplicación web [!DNL Workfront] se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente acerca de un área u objeto [!DNL Workfront].\
Para obtener más información sobre las áreas predeterminadas de [!DNL Workfront], consulte el artículo [Acerca del diseño predeterminado [!DNL Adobe Workfront] 3}.](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)

Además de las secciones que vienen con [!DNL Workfront] de manera predeterminada, puede agregar un tablero en el que puede mostrar información relacionada con el flujo de trabajo. No se puede agregar un tablero a todas las áreas y objetos.

La siguiente tabla enumera todas las [!DNL Workfront] áreas y objetos que contienen secciones en el panel izquierdo y cuáles de ellos se pueden personalizar:

| **[!DNL Workfront]área u objeto** | **Secciones predeterminadas del sistema** | **Secciones personalizadas** |
|---|---|---|
| Área de [!UICONTROL proyectos] | ✓ | ✓ |
| [!UICONTROL Equipo] | ✓ |   |
| Área de [!UICONTROL solicitudes] | ✓ |   |
| Área de [!UICONTROL hojas de horas] | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programa] | ✓ | ✓ |
| [!UICONTROL Proyecto] | ✓ | ✓ |
| [!UICONTROL Tarea] | ✓ |  ✓ |
| [!UICONTROL Problema] |  ✓ |  ✓ |
| [!UICONTROL Usuario] |  ✓ |  ✓ |
| [!UICONTROL Documento] |  ✓ |  ✓ |

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td>[!UICONTROL Reviewer] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td>Ver acceso al tipo de objeto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Agregar un panel en el panel izquierdo de un objeto o área [!DNL Workfront]

Para poder agregar un tablero, debe crearlo con toda la información que desee mostrar en él. También puede crear una página externa.\
Para obtener más información acerca de la creación de paneles, vea el artículo [Crear un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Para obtener más información acerca de la creación de páginas externas, vea el artículo [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Después de crear el tablero o la página externa, puede agregarlos al panel izquierdo.

1. Vaya a una de las [!DNL Workfront] áreas u objetos donde puede agregar una sección personalizada en el panel izquierdo.\
   O
1. Vaya a un objeto donde pueda agregar un [!UICONTROL panel] en el panel izquierdo.\
   Para obtener más información sobre las áreas y los objetos a los que puede agregar secciones personalizadas, vea [[!DNL Adobe Workfront] secciones](#adobe-workfront-sections).
1. Haga clic en **[!UICONTROL Agregar tablero]** en el panel izquierdo.
1. Escriba un nombre para el tablero en el campo **[!UICONTROL Nombre de vínculo rápido]**. Esto solo es visible para usted.
1. Empiece a escribir el nombre de un panel existente o de una página externa en el campo **[!UICONTROL Elegir un panel]** y, a continuación, seleccione el panel cuando se muestre en la lista.
1. Haga clic en **[!UICONTROL Agregar]**.
1. (Opcional) Arrastre y suelte las secciones en el orden en que desee mostrarlas.

   La sección superior es la sección predeterminada de la página.

   Las secciones creadas para objetos individuales se muestran al acceder a todos los objetos del mismo tipo y sólo están disponibles para usted.

## Mostrar paneles en el panel izquierdo de objetos

Para obtener más información sobre cómo agregar un panel debajo de un objeto, consulte la sección [[!UICONTROL Agregar un panel] en el panel izquierdo de un objeto o área de Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) en este artículo.

Cuando se agrega un tablero a una sección personalizada debajo de un objeto, el objeto actúa como filtro para el tablero. Por ejemplo, si agrega un informe de tareas a un panel y agrega el panel a un proyecto, la sección personalizada que contiene el panel del proyecto sólo muestra las tareas del proyecto que está viendo.

Los objetos siguientes se filtran para el objeto bajo el que se muestran, si ese objeto es superior en jerarquía que ellos:

* Proyecto
* Tarea
* Problema
* Proceso de aprobación
* Nota
* Documento

Para obtener más información acerca de la jerarquía y la interdependencia de objetos, vea la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalización del panel izquierdo en una plantilla de diseño

Al agregar paneles a la instancia [!DNL Workfront], solo son visibles para usted.

Puede personalizar las secciones de [!DNL Workfront] y compartir el nuevo diseño con varios usuarios en una plantilla de diseño. Solamente un administrador de sistema o de grupo puede compartirlos con otros usuarios en una plantilla de diseño. Para obtener más información sobre cómo personalizar el panel izquierdo con una plantilla de diseño, consulte [Personalizar el panel izquierdo con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
