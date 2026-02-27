---
product-area: reporting
navigation-topic: report-usage
title: Uso de carpetas de informes compartibles
description: Utilice carpetas de informes que se pueden compartir para organizar los informes que crea y compartir esas carpetas con otros usuarios en Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 65831f2e-9092-4e99-a86b-40df42c713bf
source-git-commit: 650d24c36c3ccee810b8918ccdf456f607b055e9
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 8%

---

# Uso de carpetas de informes compartibles

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

<!-- This article is linked in the UI -->

Puede utilizar carpetas de informes que se pueden compartir para organizar informes y compartir esas carpetas con otros usuarios. Esta función está diseñada para equipos que administran grandes volúmenes de informes y necesitan un control de acceso escalable y coherente.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles de control y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprender los permisos de carpeta

Las carpetas de informes que se pueden compartir utilizan dos niveles de permisos:

* **Ver**: los usuarios pueden abrir informes en la carpeta, pero no pueden editar detalles de la carpeta, agregar o quitar elementos, ni eliminar la carpeta. Puede permitir que los usuarios con acceso de visualización compartan la carpeta habilitando la opción **Compartir** al conceder acceso.
* **Administrar**: los usuarios pueden editar los detalles de la carpeta y agregar o mover elementos del informe. También se les concede acceso de Administración a los informes dentro de la carpeta. Puede permitir que los usuarios con acceso de Administrar compartan la carpeta o eliminen carpetas habilitando la configuración de **Compartir** y **Eliminar** cuando conceda el acceso.

Comportamiento adicional:

* Los administradores del sistema pueden ver todas las carpetas.
* Otros usuarios solo ven las carpetas a las que tienen acceso.
* Los permisos concedidos a una carpeta principal se aplican a todas las subcarpetas e informes de ese árbol de carpetas.
* Los usuarios con acceso a una subcarpeta pueden ver sus carpetas principales para la navegación, pero no las carpetas del mismo nivel a menos que se conceda acceso.

## Crear una carpeta de informes que se pueda compartir

Solo los administradores del sistema pueden crear carpetas en el nivel superior. Una vez creada una carpeta que se puede compartir, los usuarios con acceso de Administración pueden crear subcarpetas dentro de ella.

{{step1-to-reports}}

1. Active la opción **Compartir carpetas de informes**.
1. Haga clic en **Crear carpeta**.
1. Introduzca un nombre para la carpeta.
1. Haga clic en **Crear**.

![crear una carpeta compartible](assets/add-sharable-folder.png)

## Crear una subcarpeta en una carpeta de informes que se pueda compartir

Puede crear hasta 3 niveles de subcarpetas dentro de una carpeta de informes que se puede compartir. Las subcarpetas heredan los permisos de la carpeta principal, pero también puede establecer permisos únicos para cada subcarpeta.

{{step1-to-reports}}

1. Busque la carpeta en la que desea crear una subcarpeta.
1. Haga clic en **Más** > **Agregar subcarpeta**.
1. Escriba un nombre para la subcarpeta.
1. Haga clic en **Crear**.

## Compartir una carpeta de informes con otros usuarios

Cuando comparte una carpeta con los usuarios, estos heredan el acceso a todas las subcarpetas de ese árbol de carpetas. Los usuarios también deben tener acceso a cada informe, ya sea mediante permisos de carpeta o compartiendo informes directamente.

{{step1-to-reports}}

1. Busque la carpeta que desee compartir.
1. Haga clic en **Más** > **Compartir**.
1. Agregar usuarios, equipos, funciones, grupos o empresas.
1. Elija el acceso de **Ver** o **Administrar**:
   * El acceso de visualización permite a los usuarios abrir informes en la carpeta. También puede permitir que los usuarios con acceso de Ver vuelvan a compartir la carpeta seleccionando **Compartir** en la configuración adicional.
   * El acceso de Administrar permite a los usuarios editar los detalles de la carpeta y agregar o quitar elementos. También puede permitir que los usuarios con acceso de Administrar eliminen carpetas o compartan la carpeta seleccionando **Eliminar** y **Compartir** en la configuración adicional.
1. Haga clic en **Guardar**.

   ![compartir una carpeta y ajustar el acceso](assets/share-settings-sharable-folders.png)

## Mover un informe a una carpeta compartible

Para mover un informe a una carpeta, debes tener derechos de **Administrar** tanto para el informe como para la carpeta que se puede compartir.

{{step1-to-reports}}

1. Seleccione la casilla de verificación situada junto al informe que desee mover.
1. Haga clic en **Mover a la carpeta** en la barra de acciones de la parte inferior de la pantalla.
1. Busque la carpeta a la que desea mover el informe y haga clic en **Mover**. El árbol de informes está contraído de forma predeterminada, por lo que es posible que tenga que expandir las carpetas para encontrar la carpeta de destino.

   ![mover un informe a una carpeta compartible](assets/move-to-folder.png)

## Eliminar una carpeta de informes que se puede compartir

Al eliminar una carpeta, también se eliminan las subcarpetas de dicha carpeta. Debe tener acceso de **Administrar** a la carpeta para eliminarla. Los informes de la carpeta no se eliminan y aún se pueden encontrar en la lista de informes principal.

Los permisos de informe concedidos a través de los permisos de carpeta se eliminan cuando se elimina la carpeta. Los permisos de informe concedidos directamente desde el informe o heredados de un tablero permanecen.


{{step1-to-reports}}

1. Haga clic en **Más** > **Eliminar**.
1. Haga clic en **Sí, eliminarlo** para confirmar.


## Nueva experiencia de lista para carpetas compartibles

Cuando acceda a carpetas compartibles en el área de Informes, verá una nueva experiencia de lista que le permitirá ver y administrar fácilmente sus carpetas e informes. Para obtener más información sobre la nueva experiencia de lista, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).