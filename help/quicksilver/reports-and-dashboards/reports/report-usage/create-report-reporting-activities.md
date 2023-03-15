---
product-area: reporting
keywords: cambiar,propietario,compartido,informe,compartir,ejecutar,usuario,acceso,derechos,introducido,último,visualizado,fecha,informes,actividades
navigation-topic: report-usage
title: Crear un informe sobre las actividades de informes
description: Cuando crea un informe sobre los informes, puede identificar información específica del informe, que puede incluir si los informes están asignados a usuarios desactivados, si los informes están configurados para ejecutarse con los derechos de acceso de un usuario desactivado, si los usuarios están accediendo a un informe que planea eliminar, etc.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 1%

---

# Crear un informe sobre las actividades de informes

Cuando crea un informe sobre los informes, puede identificar información específica del informe, que puede incluir si los informes están asignados a usuarios desactivados, si los informes están configurados para ejecutarse con los derechos de acceso de un usuario desactivado, si los usuarios están accediendo a un informe que planea eliminar, etc.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un informe sobre informes existentes {#create-the-report-about-existing-reports}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Informes**, luego **Nuevo informe**.
1. En el **Nuevo informe** menú desplegable, seleccione **Informe** para crear un informe sobre los informes existentes.

1. En el **Columnas (Vista)** , añada las columnas que desee en el informe.\
   Algunos de los campos siguientes pueden ser útiles:

   | Campo | Descripción |
   |---|---|
   | **Ejecutar como usuario: Nombre** | Este es el usuario especificado en la variable **Ejecute este informe con los derechos de acceso de:** en el informe. Si este usuario está desactivado, no se muestra ningún informe para nadie con el que se comparta el informe. |
   | **Compartido con** | Estas son todas las entidades con las que se comparte el informe. |
   | **Ingresado por** | Este es el propietario del informe. |
   | **Fecha de última visualización** | Esta es la fecha y la hora en que un usuario vio por última vez el informe. |

   {style="table-layout:auto"}

1. (Opcional) Para limitar la lista de informes a usuarios desactivados específicos:

   1. Seleccione el **Filtros** a continuación, haga clic en **Agregar una regla de filtro**.

   1. Añadir el filtro **Ejecutar como ID de usuario** > **Igual**.

   1. Escriba el nombre del usuario desactivado que desea agregar al filtro y, a continuación, haga clic en el nombre cuando se muestre en la lista.
   1. Repita el paso C hasta que haya seleccionado todos los usuarios desactivados que desee incluir en el informe.

1. (Opcional) Para limitar la lista de informes a informes programados:

   1. Seleccione el **Filtros** a continuación, haga clic en **Agregar una regla de filtro**.

   1. Añadir el filtro **ID de informe programado** > **No está en blanco**.

1. Haga clic en **Guardar + Cerrar**, luego escriba un nombre para el informe y haga clic en **Guardar informe**.

   Se muestra la información del informe.

1. (Opcional) Exporte este informe a Excel y guárdelo en el equipo.\
   Para obtener información sobre cómo exportar un informe, consulte [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Actualizar información sobre un informe

Después de crear el informe, puede actualizar los informes según sea necesario.

1. Vaya al informe que desee actualizar.
1. En función de la acción que desee realizar, realice una de las siguientes acciones:

   * Actualice el **Ejecute este informe con los derechos de acceso de:** para un usuario activo: Para obtener más información, consulte [Ejecutar y enviar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Cree una copia del informe: Para obtener más información, consulte [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Eliminar un informe: para obtener más información, consulte la [Crear una copia exacta de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) sección del artículo [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Compartir un informe: para obtener más información, consulte [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Condicional) Si copia los informes originales, utilice la información del informe que creó en [Crear un informe sobre informes existentes](#create-the-report-about-existing-reports) para compartir las nuevas copias con las mismas entidades que los informes originales.
