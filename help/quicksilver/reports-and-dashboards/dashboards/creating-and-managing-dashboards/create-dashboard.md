---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Crear un tablero
description: Puede crear tableros para acceder rápidamente a la información de los informes, calendarios y páginas externas.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Crear un tablero

Puede crear tableros para acceder rápidamente a la información de los informes, calendarios y páginas externas.

Para obtener más información sobre los paneles, consulte [Introducción a los paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>plan de Adobe Workfront*</strong></p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Licencia de Adobe Workfront*</strong></p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Obtendrá permisos de administración para el nuevo panel</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.<br>Para obtener más información sobre los permisos de los tableros, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Compartir informes, tableros y calendarios </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crear cualquiera de los siguientes objetos antes de agregarlos a un tablero:

* **Informes**: Para obtener información sobre la creación de informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendarios**: Para obtener información sobre la creación de calendarios, consulte [Información general sobre los informes del calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* **Páginas externas**: Para obtener información sobre la creación de páginas externas, consulte [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Crear un tablero

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon.png)y haga clic en **Tableros.**
1. Haga clic en **Nuevo tablero**.\
   Aparece el cuadro de diálogo Nuevo tablero .

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nombre</strong></td>
      <td><p>Este es el nombre de su tablero.</p><p>Si no especifica ningún nombre, el nombre del primer informe del tablero se convierte de forma predeterminada en el nombre del tablero.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descripción (opcional)</strong></td>
      <td>Esta es una descripción del tablero.</td>
     </tr>
    </tbody>
   </table>

1. Para seleccionar un diseño, haga clic en el botón de opción correspondiente.

   El diseño de una sola columna es el predeterminado.

   Para obtener información sobre el diseño del informe en los tableros, consulte [Comprender cómo se muestran los informes en un tablero](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Consider adding the information from this article here, at some point, instead of linking to it.)
   </MadCap:conditionalText>
   -->

1. Agregue informes, calendarios o páginas externas existentes; para ello, búsquelos en la **Buscar por nombre o tipo ...** , arrastrándolos al panel de diseño, cuando aparezcan en la lista.

   >[!NOTE]
   >
   >Al buscar un elemento, la búsqueda devuelve cualquiera de los 2000 informes creados más recientemente. Los nombres de informes que incluyen caracteres Unicode no se devuelven en los resultados de búsqueda. Como práctica recomendada, evite incluir caracteres Unicode al asignar nombres a los objetos en Workfront escribiendo nombres en lugar de copiar y pegar nombres de otro origen.

   ![Buscar informes](assets/qs-new-dashboard-ui-0722.png)

1. (Opcional) Haga clic en **Agregar página externa** para agregar una página externa al tablero.\
   Para obtener más información sobre la creación de páginas externas y su incrustación en tableros, consulte [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Haga clic en **Guardar + Cerrar**.\
   Se muestra una marca de tiempo en la esquina superior derecha del tablero. La marca de tiempo incluye la fecha, la hora y el huso horario en que se actualizó el tablero por última vez.
