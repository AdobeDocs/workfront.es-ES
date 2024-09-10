---
title: Eliminar una condición personalizada
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Puede eliminar una condición personalizada.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Eliminar una condición personalizada

Puede eliminar una condición personalizada si ya no la necesita.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar una condición personalizada

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Condiciones**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Seleccione la ficha del tipo de objeto (**Proyecto**, **Tarea** o **Problema**) donde se encuentra la condición que desea eliminar.

1. Pase el ratón sobre la condición que quiera eliminar y luego haga clic en el icono **Eliminar** ![](assets/delete.png) que aparece en el extremo derecho.
1. En el mensaje de confirmación que aparece, haga clic en **Eliminar condición**.

1. En el cuadro **Eliminar condición** que aparece, seleccione una nueva condición en la lista desplegable para todos los proyectos que estaban utilizando la condición que está eliminando.

   Las condiciones personalizadas solo están disponibles en la lista desplegable si se equiparan con la misma condición integrada que la que está eliminando. Por ejemplo, si elimina una condición que es igual a En riesgo, solo se podrán seleccionar las condiciones personalizadas que también sean iguales a En riesgo.

1. Haga clic en **Eliminar condición**.

>[!NOTE]
>
>No puede eliminar las condiciones integradas, que son En el destino, En riesgo y Con problemas. Sin embargo, puede cambiar sus nombres y colores.

Para obtener información acerca de las condiciones personalizadas, vea [Condiciones personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
