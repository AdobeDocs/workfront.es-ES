---
product-area: reporting
keywords: cambiar,propietario,compartido,informe,compartir,ejecutar,usuario,acceso,derechos,introducido,último,visto,fecha,informes,actividades
navigation-topic: report-usage
title: Creación de un informe sobre las actividades de creación de informes
description: Al crear un informe sobre los informes, puede identificar información específica, que puede incluir si los informes se asignan a usuarios desactivados, si los informes se definen para que se ejecuten con los derechos de acceso de un usuario desactivado, si los usuarios acceden a un informe que planea eliminar, etc.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Creación de un informe sobre las actividades de creación de informes

Al crear un informe sobre los informes, puede identificar información específica, que puede incluir si los informes se asignan a usuarios desactivados, si los informes se definen para que se ejecuten con los derechos de acceso de un usuario desactivado, si los usuarios acceden a un informe que planea eliminar, etc.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Creación del informe sobre informes existentes {#create-the-report-about-existing-reports}

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Informes** y luego en **Nuevo informe**.
1. En el menú desplegable **Nuevo informe**, seleccione **Informe** para crear un informe con los informes existentes.

1. En la ficha **Columnas (Ver)**, agregue las columnas que desee en el informe.\
   Algunos de los siguientes campos pueden resultar útiles:

   | Campo | Descripción |
   |---|---|
   | **Ejecutar como usuario: Nombre** | Usuario especificado en **Ejecutar este informe con los derechos de acceso de:** en el informe. Si se desactiva este usuario, no se muestra ningún informe de nadie con quien se comparta el informe. |
   | **Compartido Con** | Estas son todas las entidades con las que se comparte el informe. |
   | **Ingresado Por** | Es el propietario del informe. |
   | **Fecha de última visualización** | Es la fecha y la hora en que un usuario vio el informe por última vez. |

   {style="table-layout:auto"}

1. (Opcional) Para limitar la lista de informes a usuarios desactivados específicos:

   1. Seleccione la ficha **Filtros** y, a continuación, haga clic en **Agregar una regla de filtro**.

   1. Agregue el filtro **Ejecutar como id. de usuario** > **Igual**.

   1. Escriba el nombre del usuario desactivado que desea agregar al filtro y, a continuación, haga clic en el nombre cuando se muestre en la lista.
   1. Repita el paso C hasta que haya seleccionado todos los usuarios desactivados que desee incluir en el informe.

1. (Opcional) Para limitar la lista de informes a informes programados:

   1. Seleccione la ficha **Filtros** y, a continuación, haga clic en **Agregar una regla de filtro**.

   1. Agregue el filtro **Id. de informe programado** > **No está en blanco**.

1. Haga clic en **Guardar + Cerrar**, escriba un nombre para el informe y haga clic en **Guardar informe**.

   Se muestra la información del informe.

1. (Opcional) Exporte este informe a Excel y guárdelo en el equipo.\
   Para obtener información sobre cómo exportar un informe, consulte [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Actualización de información sobre un informe

Después de crear el informe, puede actualizarlo según sea necesario.

1. Vaya al informe que desee actualizar.
1. Según la acción que desee realizar, realice una de las siguientes acciones:

   * Actualice el campo **Ejecutar este informe con los derechos de acceso de:** a un usuario activo: Para obtener más información, vea [Ejecutar y enviar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Crear una copia del informe: para obtener más información, vea [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Eliminar un informe: para obtener más información, consulte la sección [Crear una copia exacta de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) del artículo [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Compartir un informe: para obtener más información, vea [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Condicional) Si copia los informes originales, use la información del informe que creó en [Cree el informe sobre los informes existentes](#create-the-report-about-existing-reports) para compartir las copias nuevas con las mismas entidades que los informes originales.
