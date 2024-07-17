---
title: Eliminar una condición personalizada
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Puede eliminar una condición personalizada.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Eliminar una condición personalizada

## Requisitos de acceso

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminar una condición personalizada

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

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
