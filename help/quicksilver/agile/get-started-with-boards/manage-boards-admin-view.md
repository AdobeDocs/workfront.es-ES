---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Administrar la vista de administración de tableros
description: La vista Administrador de tableros contiene una lista de todos los tableros de su cuenta que los administradores del sistema pueden utilizar para obtener una instantánea rápida de los detalles generales de los tableros.
author: Jenny
feature: Agile
source-git-commit: 56263c3f868e7abdaf973c5c03411a2e63ba645d
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 7%

---

# Administrar la vista de administración de tableros

La vista Administrador de tableros contiene una lista de todos los tableros de su cuenta que los administradores del sistema pueden utilizar para obtener una instantánea rápida de los detalles generales de los tableros, incluyendo cuándo se actualizaron por última vez, cuántas tarjetas tiene cada uno y más.

Desde esta área, puede realizar las siguientes acciones:

* Filtrar la lista de tableros
* Configuración de las columnas de lista Tableros
* Agrupar la lista de tableros

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
        <p> Plan </p></td> 
  </tr> 
    <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Administrador del sistema </p>
        </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crear un tablero para poder verlo desde la vista de administrador.

Para obtener más información, consulte [Crear o editar un tablero](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrar la lista de tableros

{{step1-to-boards}}

1. En la página **Tableros**, seleccione la pestaña **Vista de administración**.

1. Seleccione **Filtro**. Se abre el panel **Filtros**.

1. Siga los pasos a continuación para configurar el filtro:

   1. (Opcional) Haga clic en el icono **Calendario** ![Icono de calendario](assets/calendar-icon.png) y, a continuación, seleccione un intervalo de fechas para filtrar por tableros que se modificaron por última vez dentro de ese intervalo de tiempo.

   1. (Opcional) En la sección **Plantilla**, seleccione el tipo de plantilla de placa por el que filtrará la lista. Puede seleccionar más de un tipo de plantilla.
Para obtener más información acerca de los tipos de plantillas de tablero, vea [Crear o editar un tablero](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

   1. (Opcional) En la sección **Está archivado**, seleccione si se mostrarán los tableros archivados o no archivados. Puede seleccionar más de una opción.

      ![Sección archivada](assets/is-archived-section.png)

1. Haga clic fuera del panel **Filtros** para cerrarlo. Las selecciones de filtro permanecerán aplicadas a la lista Tableros hasta que se vuelva a cambiar a la vista predeterminada.

   >[!NOTE]
   >
   >Para quitar un filtro, abra el panel **Filtros** y haga clic en **Volver al valor predeterminado** en la esquina superior derecha.

## Configuración de las columnas de lista Tableros

{{step1-to-boards}}

1. En la página **Tableros**, seleccione la pestaña **Vista de administración**.

1. Seleccionar **columnas**. Se abre el panel **Campos de visibilidad y orden**.

1. Configure las columnas que aparecerán en la lista Tableros seleccionando o anulando la selección de la opción en línea con cada columna:

   * **Propietario**
   * **Última actualización**
   * **Miembros**
   * **Archivado**
   * **Plantilla**
   * **Recuento de tarjetas**

1. (Opcional) Para ajustar el orden en el que aparecen los campos, mantenga presionado el icono **Arrastrar** a la izquierda de un campo y arrástrelo a una nueva posición.

   ![Haga clic y arrastre](assets/click-and-drag.png)

1. Haga clic fuera del panel **Campos de visibilidad y orden** para cerrarlo. Las configuraciones de columna permanecerán aplicadas a la lista de tableros hasta que se modifiquen.

   >[!NOTE]
   >
   > Cuando se modifican las columnas de la lista Tableros, aparece un punto azul sobre el icono **Columnas** para indicar que la vista actual se ha modificado respecto a la predeterminada.

## Agrupar la lista de tableros por un campo específico

{{step1-to-boards}}

1. En la página **Tableros**, seleccione la pestaña **Vista de administración**.

1. Seleccionar **grupo**. Se abre el panel **Agrupar por**.

1. Seleccione el campo por el que desea agrupar la lista Tableros:

   * **Archivado**
   * **Propietario**
   * **Plantilla**

1. (Opcional) Para expandir o contraer la agrupación desde el panel **Agrupar por**, haga clic en **Contraer todo** o **Expandir todo**.

   ![Contraer todo](assets/collapse-all.png)

1. (Opcional) Para cambiar el orden de visualización de la agrupación de A-Z a Z-A, seleccione el campo por el que está agrupada la lista y, a continuación, seleccione **Z-A** en la lista desplegable.

   ![Mostrar por pedido](assets/display-by-order.png)

1. Haga clic fuera del panel **Agrupar por** para cerrarlo. Desde aquí, puede contraer o expandir la agrupación aplicada en la lista seleccionando la flecha junto al título de la agrupación.

   ![Contraer o expandir](assets/collapse-or-expand.png)

   >[!NOTE]
   >   
   >Cuando se modifica la visualización de la agrupación de la lista Tableros, aparece un punto azul encima del icono **Grupo** para indicar que la vista actual es diferente de la predeterminada. <br>
   >Si desea quitar una agrupación, abra el panel **Agrupar por** y seleccione **Borrar todo** en la esquina superior derecha.
