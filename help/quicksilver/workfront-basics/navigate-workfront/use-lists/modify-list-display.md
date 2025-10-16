---
navigation-topic: use-lists
title: Modificación del modo en que se muestra una lista
description: En  [!DNL Adobe Workfront], puede personalizar el modo en que se muestra una lista. Otros usuarios que ven la lista no ven los cambios.
feature: Get Started with Workfront
author: Nolan
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: f0b3b8aa64fa0b03a196bbcc2bdd037eeeb0f89e
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 6%

---

# Modificación del modo en que se muestra una lista

<!--Audited: 11/2024-->

En [!DNL Adobe Workfront], puede personalizar el modo en que se muestra una lista. Otros usuarios que ven la lista no ven los cambios.

Puede realizar las siguientes personalizaciones:

* El número de elementos que se muestran
* Anchura o orden de columna
* Si las agrupaciones están expandidas o contraídas

>[!NOTE]
>
>Los cambios de visualización anteriores que realice se revertirán cuando cierre la sesión de [!DNL Workfront] o el explorador. Estos cambios también pueden revertirse después de un período de 8 horas.

Además de las personalizaciones temporales anteriores, también puede ajustar por qué columnas ordena la lista y qué [!DNL Workfront] conserva incluso después de cerrar la sesión o el explorador. Sin embargo, si alguien edita las opciones de ordenación en la vista de una lista, no se conserva la selección de ordenación anterior.

Para obtener información sobre cómo modificar la información que aparece en la lista, vea [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior </p>
   <p>Solicitud o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL View] al área donde se encuentra la lista</p> <p>Por ejemplo, para modificar la vista de un proyecto, necesita el acceso de [!UICONTROL View] a Proyectos.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] o permisos superiores a la vista aplicada a la lista</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificación de una lista

1. Vaya a la lista de [!DNL Workfront] que desea modificar.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (Opcional y condicional) Si las agrupaciones de la lista están contraídas y desea ver más información, haga clic en la agrupación deseada para expandir la lista y mostrar la información que contiene.

   O

   Para expandir todas las agrupaciones, haga clic en la flecha situada a la derecha de la casilla de verificación del encabezado de columna.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (Opcional y condicional) Si desea mostrar un número específico de elementos en la pantalla, haga clic en el menú desplegable **[!UICONTROL Mostrando]** en la esquina inferior derecha de la pantalla y, a continuación, seleccione para mostrar **100**, **250**, **500**, **[!UICONTROL Todos]** o **2000** elementos.

   ![Número de lista en la página](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >De forma predeterminada, se muestran 2000 elementos para listas actualizadas y 100 elementos para listas heredadas. Si la lista contiene más de 2000 elementos, no podrá mostrar todos en una página.
   >
   >
   >Para obtener el mejor rendimiento en listas grandes en las que los objetos contienen campos de texto con formato, se recomienda limitar este número a 250.
   >
   >
   >Para obtener más información sobre los dos tipos de lista, vea la sección [Diferencia entre las listas actualizadas y las heredadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) en el artículo [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   Los resultados de la lista se paginan para mostrar el número seleccionado de elementos por página. Puede acceder a los resultados de otras páginas haciendo clic en las flechas hacia atrás y hacia adelante o seleccionando una página específica.

1. Para cambiar el tamaño de la anchura de una columna, pase el ratón sobre la línea que separa 2 columnas y, a continuación, haga clic en para arrastrarla hasta la anchura deseada.

   Se cambia el tamaño de la columna hasta que se borra la caché del explorador o hasta que se vuelve a cambiar manualmente su tamaño.

1. Para reordenar las columnas de una lista, pase el ratón sobre el encabezado de una columna para mostrar la herramienta de mano y, a continuación, haga clic en para arrastrar la columna hasta el lugar en el que desee que se muestre.

   La posición de la columna se guardará hasta que actualice la página.

   Para obtener más información acerca de cómo personalizar el ancho y el orden de las columnas de una lista, vea el artículo [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. Para ajustar el orden de clasificación de una lista, haga clic en un encabezado de columna para seleccionarlo, luego presione y mantenga presionada la tecla CMD (en [!DNL Mac]) o la tecla CTRL (en [!DNL Windows]) en el teclado y seleccione hasta 2 encabezados de columna adicionales para ordenarlos.

   La lista se ordena por cada una de las columnas seleccionadas en el orden de selección.

   Todas las modificaciones que realice en la lista se guardarán al instante.

   >[!NOTE]
   >
   >Si está ordenando grupos en el área [!UICONTROL Grupos] en [!UICONTROL Configuración], la vista de jerarquía de los grupos y sus subgrupos no se rompe al cambiar la forma en que se ordena la lista: los subgrupos permanecen con sus grupos principales. La lista se ordena primero por grupos de nivel superior. A continuación, en cada grupo principal, la lista de subgrupos que se encuentran en el mismo nivel se ordenan juntos.
