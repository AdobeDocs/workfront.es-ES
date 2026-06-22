---
navigation-topic: get-started-with-workfront
title: Personalización de las columnas de lista de trabajo Prioridades
description: Puede personalizar las columnas de la lista de trabajos en Prioridades para admitir su forma de trabajar.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: e4232fbe-1b5c-4614-8613-3b0e25ffee46
TQID: https://experienceleague.adobe.com/YIqeZbiTZH00yXJ6LnQrpEZuHvW4Y5QZVkYU3OquWqE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 14%

---

# Personalización de las columnas de lista de trabajo Prioridades

{{preview-fast-release-general}}

<!--I think this article can point to the Enhanced lists article for managing the view-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


Puede personalizar las columnas de la lista de trabajos en Prioridades para admitir su forma de trabajar.

Prioridades muestra los elementos de trabajo que tiene asignados. No puede ver los elementos de trabajo asignados a su equipo.

<!--
>[!NOTE]
>
>You cannot add custom data to columns at this time.
-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Paquete de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront</strong></td> 
   <td> 
   <p>Revisor o superior</p>
   <p>Ligero o superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Acceso de visualización o edición para el objeto en el que se encuentra la actualización</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de visualización al objeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalización de las columnas de lista de trabajo Prioridades

### Habilitar o deshabilitar columnas

{{step1-to-priorities}}

1. Haga clic en **Columnas** en la parte izquierda de la pantalla.

   <span class="preview">Imagen de muestra en el entorno de vista previa:</span>
   ![Columnas](assets/columns-new-060226.png)

   Imagen de muestra en el entorno de producción:
   ![Columnas](assets/columns-new.png)

1. Utilice las teclas de alternancia para mostrar u ocultar columnas en la lista de trabajos.

### Reordenar las columnas

{{step1-to-priorities}}

1. Haga clic en **Columnas** en la parte izquierda de la pantalla.
1. Haz clic en el icono **Arrastrar** y mueve la columna a la ubicación que desees. Al mover columnas, se actualiza automáticamente la lista de trabajo.
   ![Reordenar columnas](assets/reorder-columns-new.png)

>[!NOTE]
>
>La columna Nombre es fija y no se puede mover.

<div class="preview">

### Agregar y quitar columnas con el Administrador de columnas

{{step1-to-priorities}}

1. Haga clic en el icono + en la esquina superior derecha de la lista para abrir el cuadro **Administrador de columnas**.
1. Agregue o quite columnas y después haga clic en **Guardar**.

   >[!NOTE]
   >
   >Solo se pueden agregar campos existentes a la vista de lista. Tanto los campos nativos como los personalizados para tareas y problemas están disponibles para agregarlos como columnas.

Para obtener más información sobre el administrador de columnas, vea la sección [Agregar y quitar columnas con el administrador de columnas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) en el artículo [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

</div>

### Cambiar el alto de fila en la lista de prioridades

{{step1-to-priorities}}

1. Haga clic en el icono **Alto de fila**.

   Esto actualiza la longitud vertical de una fila. Elija entre las siguientes opciones:

   * Baja
   * Estándar. Esta es la opción predeterminada.
   * Media
   * Alta

   La lista se actualiza inmediatamente.

<div class="preview">

## Administrar vistas para la lista de prioridades

Una vista define las columnas, los filtros y las agrupaciones de la lista con ajustes preestablecidos.

Se asigna una vista predeterminada a la lista de prioridades. También puede crear y compartir sus propias vistas.

{{step1-to-priorities}}

1. Expanda el menú de vistas desplegables en la esquina superior izquierda de la lista para seleccionar otra vista, o haga clic en **Nueva vista** para crear otra.
1. Actualice las columnas, filtros y agrupaciones que desee incluir en la vista.

   Los cambios en las vistas se guardan automáticamente. La próxima vez que aplique esta vista, la configuración de columna y filtro seguirá siendo la misma que la establecida.

Para obtener más información sobre las vistas, consulte la sección [Actualizar elementos de lista mejorados](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#update-enhanced-list-elements) en el artículo [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

</div>
