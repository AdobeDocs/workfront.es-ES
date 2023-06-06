---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Creación de secciones personalizadas
description: La información que se ve en la [!DNL Workfront] la aplicación web suele mostrarse en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente sobre un [!DNL Workfront] área u objeto.
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 2%

---

# Creación de secciones personalizadas

## [!DNL Adobe Workfront] secciones

La información que se ve en la [!DNL Workfront] la aplicación web suele mostrarse en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente sobre un [!DNL Workfront] área u objeto.\
Para obtener más información sobre las áreas predeterminadas de [!DNL Workfront], consulte el artículo [Acerca del valor predeterminado [!DNL Adobe Workfront] layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Además de las secciones que vienen con [!DNL Workfront] de forma predeterminada, se puede agregar un panel en el que se puede mostrar información relevante para el flujo de trabajo. No se puede agregar un tablero a todas las áreas y objetos.

La siguiente tabla enumera todas las [!DNL Workfront] áreas y objetos que contienen secciones en el panel izquierdo y cuáles de ellos se pueden personalizar:

| **[!DNL Workfront]área u objeto** | **Secciones predeterminadas del sistema** | **Secciones personalizadas** |
|---|---|---|
| [!UICONTROL Proyectos] área | ✓ | ✓ |
| [!UICONTROL Equipo] | ✓ |   |
| [!UICONTROL Solicitudes] área | ✓ |   |
| [!UICONTROL Plantillas de horas] área | ✓ |   |
| [!UICONTROL Portafolio] | ✓ | ✓ |
| [!UICONTROL Programar] | ✓ | ✓ |
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

&#42;Para averiguar qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Añadir un tablero en el panel izquierdo de una [!DNL Workfront] objeto o área

Para poder agregar un tablero, debe crearlo con toda la información que desee mostrar en él. También puede crear una página externa.\
Para obtener más información sobre la creación de paneles, consulte el artículo [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Para obtener más información sobre la creación de páginas externas, consulte el artículo [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Después de crear el tablero o la página externa, puede agregarlos al panel izquierdo.

1. Vaya a uno de los [!DNL Workfront] áreas u objetos en los que puede agregar una sección personalizada en el panel izquierdo.\
   O
1. Vaya a un objeto donde pueda agregar un [!UICONTROL tablero] en el panel izquierdo.\
   Para obtener más información sobre las áreas y los objetos a los que puede agregar secciones personalizadas, consulte [[!DNL Adobe Workfront] secciones](#adobe-workfront-sections).
1. Clic **[!UICONTROL Agregar panel]** en el panel izquierdo.
1. Escriba un nombre para el tablero en **[!UICONTROL Nombre de vínculo rápido]** field. Esto solo es visible para usted.
1. Empiece a escribir el nombre de un tablero existente o de una página externa en la **[!UICONTROL Elija un tablero]** y, a continuación, seleccione el tablero cuando se muestre en la lista.
1. Clic **[!UICONTROL Añadir]**.
1. (Opcional) Arrastre y suelte las secciones en el orden en que desee mostrarlas.

   La sección superior es la sección predeterminada de la página.

   Las secciones creadas para objetos individuales se muestran al acceder a todos los objetos del mismo tipo y sólo están disponibles para usted.

## Mostrar paneles en el panel izquierdo de objetos

Para obtener más información sobre cómo agregar un tablero debajo de un objeto, consulte la sección [[!UICONTROL Agregar un tablero] en el panel izquierdo de un objeto o área de Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) en este artículo.

Cuando se agrega un tablero a una sección personalizada debajo de un objeto, el objeto actúa como filtro para el tablero. Por ejemplo, si agrega un informe de tareas a un panel y agrega el panel a un proyecto, la sección personalizada que contiene el panel del proyecto sólo muestra las tareas del proyecto que está viendo.

Los objetos siguientes se filtran para el objeto bajo el que se muestran, si ese objeto es superior en jerarquía que ellos:

* Proyecto
* Tarea
* Problema
* Proceso de aprobación
* Nota
* Documento

Para obtener más información sobre la jerarquía y la interdependencia de objetos, vea la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalización del panel izquierdo en una plantilla de diseño

Al agregar paneles a su [!DNL Workfront] Por ejemplo, solo son visibles para usted.

Puede personalizar las secciones en [!DNL Workfront] y compartir el nuevo diseño con varios usuarios en una plantilla de diseño. Solamente un administrador de sistema o de grupo puede compartirlos con otros usuarios en una plantilla de diseño. Para obtener más información sobre cómo personalizar el panel izquierdo con una plantilla de diseño, consulte [Personalización del panel izquierdo con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
