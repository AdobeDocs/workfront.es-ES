---
navigation-topic: use-lists
title: Modificar el modo en que se muestra la lista
description: En [!DNL Adobe Workfront], puede personalizar el modo en que se muestra una lista. Otros usuarios que ven la lista no ven los cambios.
feature: Get Started with Workfront
author: Lisa
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Modificar el modo en que se muestra la lista

En [!DNL Adobe Workfront], puede personalizar el modo en que se muestra una lista. Otros usuarios que ven la lista no ven los cambios.

Puede realizar las siguientes personalizaciones:

* El número de elementos que se muestran
* Anchura o orden de columna
* Si las agrupaciones se expanden o se contraen

>[!NOTE]
>
>Los cambios de visualización anteriores que realice se revertirán cuando cierre la sesión de [!DNL Workfront] o cierre el explorador. Estos cambios también se pueden revertir después de un período de 8 horas.

Además de las personalizaciones temporales anteriores, también puede ajustar qué columnas ordena la lista por qué, qué [!DNL Workfront] se conserva incluso después de cerrar la sesión o cerrar el explorador. Sin embargo, si alguien edita las opciones de ordenación en la vista de una lista, no se conserva la selección de ordenación anterior.

Para obtener información sobre cómo modificar la información que aparece en la lista, consulte [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de [!UICONTROL View] al área en la que se encuentra la lista</p> <p>Por ejemplo, para modificar la vista de un proyecto, es necesario que [!UICONTROL View] tenga acceso a Proyectos.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de [!UICONTROL View] o superior para la vista aplicada a la lista</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Modificar el modo en que se muestra la lista

1. Vaya a la lista en [!DNL Workfront] que desea modificar.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (Opcional y condicional) Si las agrupaciones de la lista están contraídas y desea ver más información, haga clic en la agrupación que desee para expandir la lista y mostrar la información que aparece en ella.

   O

   Para expandir todas las agrupaciones, haga clic en la flecha a la derecha de la casilla de verificación en el encabezado de la columna.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (Opcional y condicional) Si desea mostrar un número específico de elementos en la pantalla, haga clic en el botón **[!UICONTROL Mostrando]** menú desplegable en la esquina inferior derecha de la pantalla y, a continuación, seleccione para mostrar **100**, **250**, **500**, **[!UICONTROL Todo]** o **2000** elementos.

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >De forma predeterminada, se muestran 2000 elementos para listas actualizadas y 100 para listas heredadas. Si la lista contiene más de 2000 elementos, no puede mostrar todos los elementos en una página.
   >
   >
   >Para obtener el mejor rendimiento en listas grandes donde los objetos contienen campos de texto con formato, se recomienda limitar este número a 250.
   >
   >
   >Para obtener más información sobre los dos tipos de lista, consulte la sección [La diferencia entre las listas actualizadas y las listas heredadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) en el artículo [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   Los resultados de la lista se paginan para mostrar el número seleccionado de elementos por página. Para acceder a los resultados de otras páginas, haga clic en las flechas hacia atrás y hacia adelante o seleccione una página específica.

1. Para cambiar el tamaño del ancho de una columna, pase el ratón sobre la línea que separa 2 columnas y, a continuación, haga clic en para arrastrarla al ancho deseado.

   Se cambia el tamaño de la columna hasta que se borra la caché en el explorador o hasta que se cambia el tamaño manualmente de nuevo.

1. Para reordenar las columnas de una lista, pase el ratón sobre el encabezado de una columna para mostrar la herramienta mano y, a continuación, haga clic en para arrastrar la columna a la que desea que se muestre.

   La posición de la columna se guarda hasta que actualice la página.\
   Para obtener más información sobre la personalización del ancho y el orden de las columnas de una lista, consulte el artículo [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. Para ajustar el orden de clasificación de una lista, haga clic en el encabezado de una columna para seleccionarla y, a continuación, mantenga pulsada la tecla CMD (en [!DNL Mac]) o la tecla CTRL (activada [!DNL Windows]) en el teclado y seleccione hasta 2 encabezados de columna adicionales para ordenarlos por ellos.

   La lista se ordena por cada una de las columnas seleccionadas en el orden de selección.

   Todas las modificaciones que realice en la lista se guardan al instante.

   >[!NOTE]
   >
   >Si está ordenando grupos en la variable [!UICONTROL Grupos] área [!UICONTROL Configuración], la vista de jerarquía de los grupos y sus subgrupos no se rompe al cambiar la forma en que se ordena la lista: los subgrupos permanecen con sus grupos principales. La lista se ordena primero por grupos de nivel superior. A continuación, debajo de cada grupo principal, la lista de subgrupos que están en el mismo nivel se ordenan juntos.
