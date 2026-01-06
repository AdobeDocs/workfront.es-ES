---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Agregar un panel en el panel izquierdo de un objeto o área de Workfront
description: La información que ve en la aplicación web de  [!DNL Workfront]  se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente sobre un área u objeto de  [!DNL Workfront] .
author: Becky and Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 72%

---

# Agregar un tablero en el panel izquierdo de un objeto o área de Workfront

## Secciones de [!DNL Adobe Workfront] 

La información que ve en la aplicación web [!DNL Workfront] se muestra a menudo en las secciones del panel izquierdo de forma predeterminada. Cada sección contiene información diferente acerca de un área u objeto de [!DNL Workfront].

Para obtener más información sobre las áreas predeterminadas de [!DNL Workfront], consulte el artículo [Acerca del diseño predeterminado [!DNL Adobe Workfront] .](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)

Además de las secciones que se incluyen con [!DNL Workfront] de manera predeterminada, es posible añadir un panel de control en el que se puede mostrar información relacionada con el flujo de trabajo. No se puede añadir un panel de control a todas las áreas y objetos.

La siguiente tabla enumera todas las [!DNL Workfront] áreas y objetos que contienen secciones en el panel izquierdo y cuáles de ellos se pueden personalizar con un panel:

| Área u objeto de **[!DNL Workfront]** | **Secciones predeterminadas del sistema** | **Paneles de control** |
|---|---|---|
| Área de proyectos de  | ✓ | ✓ |
| [!UICONTROL Equipo] | ✓ |    |
| Área de [!UICONTROL solicitudes] | ✓ |    |
| Área de [!UICONTROL plantillas de horas] | ✓ |    |
| [!UICONTROL Portafolio] | ✓ | ✓ |
| [!UICONTROL Programa] | ✓ | ✓ |
| [!UICONTROL Proyecto] | ✓ | ✓ |
| [!UICONTROL Tarea] | ✓ | ✓ |
| [!UICONTROL Problema] | ✓ | ✓ |
| [!UICONTROL Usuario] | ✓ | ✓ |
| [!UICONTROL Documento] | ✓ | ✓ |
| Área de [!UICONTROL recursos] | ✓ | ✓ |

{style="table-layout:auto"}

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Ligero o superior</p>
   <p>Revisión o superior</p></td>
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td><p>Ver acceso al tipo de objeto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir un panel de control en el panel izquierdo de un objeto o área de [!DNL Workfront]

Para poder añadir un panel de control, debe crearlo con toda la información que desee mostrar en él. También puede crear una página externa.

Para obtener más información acerca de la creación de paneles de control, consulte el artículo [Crear un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Para obtener más información acerca de la creación de páginas externas, consulte el artículo [Incrustar una página web externa en un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Después de crear el panel de control o la página externa, puede añadirlos al panel izquierdo.

1. Vaya a una de las [!DNL Workfront] áreas u objetos donde puede agregar un tablero en el panel izquierdo.

   Para obtener más información sobre las áreas y los objetos a los que puede agregar paneles, consulte [[!DNL Adobe Workfront] secciones](#adobe-workfront-sections).

1. Haga clic en **[!UICONTROL Agregar tablero]** en el panel izquierdo.
1. Escriba un nombre para el panel de control en el campo **[!UICONTROL Nombre del vínculo rápido]**. Esto solo es visible para el propio usuario.
1. Empiece a escribir el nombre de un panel de control existente o de una página externa en el campo **[!UICONTROL Elegir un panel de control]** y, a continuación, seleccione el panel de control cuando se muestre en la lista.
1. Haga clic en **[!UICONTROL Añadir]**.
1. (Opcional) Arrastre y suelte las secciones en el orden en que desee mostrarlas.

   La sección superior es la sección predeterminada de la página.

   Los paneles que ha agregado solo están disponibles para usted.

## Mostrar paneles de control en el panel izquierdo de objetos

Para obtener más información sobre cómo añadir un panel de control debajo de un objeto, consulte la sección [[!UICONTROL Añadir un panel de control] en el panel izquierdo de un objeto o área de Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) de este artículo.

Cuando se agrega un tablero de mandos al panel izquierdo de un objeto, el objeto actúa como filtro para el tablero de mandos. Por ejemplo, si agrega un informe de tareas a un panel y agrega el panel a un proyecto, el panel solo muestra las tareas del proyecto que está viendo.

Los objetos siguientes se filtran para el objeto bajo el que se muestran, si dicho objeto es superior en jerarquía a ellos:

* Proyecto
* Tarea
* Problema
* Proceso de aprobación
* Nota
* Documento

Para obtener más información acerca de la jerarquía y la interdependencia de objetos, consulte la sección [Interdependencia y jerarquía de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalización del panel izquierdo en una plantilla de diseño

Al añadir paneles de control a la instancia de [!DNL Workfront], estos solo son visibles para usted.

Solamente un administrador de sistema o de grupo puede compartir tableros con otros usuarios en una plantilla de diseño. Para obtener más información sobre cómo personalizar el panel izquierdo con una plantilla de diseño, consulte [Personalizar el panel izquierdo con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
