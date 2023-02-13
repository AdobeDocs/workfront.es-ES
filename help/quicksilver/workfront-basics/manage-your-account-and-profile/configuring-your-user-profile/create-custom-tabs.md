---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Crear secciones personalizadas
description: La información que ve en la sección [!DNL Workfront] la aplicación web se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente sobre [!DNL Workfront] área u objeto.
author: Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 2%

---

# Crear secciones personalizadas

## [!DNL Adobe Workfront] secciones

La información que ve en la sección [!DNL Workfront] la aplicación web se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente sobre [!DNL Workfront] área u objeto.\
Para obtener más información sobre las áreas predeterminadas de [!DNL Workfront], consulte el artículo [Acerca de los valores predeterminados [!DNL Adobe Workfront] layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Además de las secciones que incluyen [!DNL Workfront] de forma predeterminada, puede agregar un tablero en el que puede mostrar información relevante para el flujo de trabajo. No se puede agregar un tablero a todas las áreas y objetos.

La tabla siguiente enumera todas las [!DNL Workfront] áreas y objetos que contienen secciones en el panel izquierdo y que se pueden personalizar:

| **[!DNL Workfront]área u objeto** | **Secciones predeterminadas del sistema** | **Secciones personalizadas** |
|---|---|---|
| [!UICONTROL Proyectos] area | ✓ | ✓ |
| [!UICONTROL Equipo] | ✓ |   |
| [!UICONTROL Solicitudes] area | ✓ |   |
| [!UICONTROL Hojas de tiempo] area | ✓ |   |
| [!UICONTROL Portafolio] | ✓ | ✓ |
| [!UICONTROL Programar] | ✓ | ✓ |
| [!UICONTROL Proyecto] | ✓ | ✓ |
| [!UICONTROL Tarea] | ✓ |  ✓ |
| [!UICONTROL Problema] |  ✓ |  ✓ |
| [!UICONTROL Usuario] |  ✓ |  ✓ |
| [!UICONTROL Documento] |  ✓ |  ✓ |

{style=&quot;table-layout:auto&quot;}

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

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Agregar un tablero al panel izquierdo de un [!DNL Workfront] objeto o área

Antes de agregar un tablero, debe crearlo con toda la información que desee mostrar. También puede crear una página externa.\
Para obtener más información sobre la creación de tableros, consulte el artículo [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Para obtener más información sobre la creación de páginas externas, consulte el artículo [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Después de crear el tablero o la página externa, puede agregarlos al panel izquierdo.

1. Vaya a una de las [!DNL Workfront] áreas u objetos en los que puede agregar una sección personalizada en el panel izquierdo.\
   O
1. Vaya a un objeto en el que puede agregar un [!UICONTROL tablero] en el panel izquierdo.\
   Para obtener más información sobre las áreas y los objetos a los que puede agregar secciones personalizadas, consulte [[!DNL Adobe Workfront] secciones](#adobe-workfront-sections).
1. Haga clic en **[!UICONTROL Agregar tablero]** en el panel izquierdo.
1. Escriba un nombre para el tablero en el **[!UICONTROL Nombre del vínculo rápido]** campo . Esto solo es visible para usted.
1. Empiece a escribir el nombre de un tablero existente o una página externa en la **[!UICONTROL Elegir un tablero]** y, a continuación, seleccione el panel cuando se muestre en la lista.
1. Haga clic en **[!UICONTROL Agregar]**.
1. (Opcional) Arrastre y suelte las secciones en el orden en que desee mostrarlas.

   La sección superior es la sección predeterminada de la página.

   Las secciones que ha creado para objetos individuales se muestran cuando accede a todos los objetos del mismo tipo y solo están disponibles para usted.

## Mostrar tableros en el panel izquierdo de objetos

Para obtener más información sobre cómo agregar un tablero debajo de un objeto, consulte la sección [[!UICONTROL Agregar un tablero] en el panel izquierdo de un objeto o área de Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) en este artículo.

Cuando agrega un tablero a una sección personalizada debajo de un objeto, el objeto actúa como filtro para el tablero. Por ejemplo, si agrega un informe de tareas en un tablero y agrega el tablero a un proyecto, la sección personalizada que contiene el tablero del proyecto solo mostrará las tareas del proyecto que esté viendo.

Los siguientes objetos se filtran para el objeto bajo el que se muestran, si ese objeto tiene una jerarquía superior a ellos:

* Proyecto
* Tarea
* Problema
* Proceso de aprobación
* Nota
* Documento

Para obtener más información sobre la jerarquía y la interdependencia de los objetos, consulte la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalización del panel izquierdo en una plantilla de diseño

Al agregar tableros al [!DNL Workfront] por ejemplo, solo son visibles para usted.

Puede personalizar las secciones de [!DNL Workfront] y compartir el nuevo diseño con varios usuarios en una plantilla de diseño. Solo un administrador de sistemas o grupos puede compartirlos con otros usuarios en una plantilla de diseño. Para obtener más información sobre la personalización del panel izquierdo con una plantilla de diseño, consulte [Personalización del panel izquierdo mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
