---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Uso de campos de moneda en paneles de lienzo
description: Puede utilizar los campos de moneda en un panel de lienzo.
author: Courtney
feature: Reports and Dashboards
source-git-commit: f8c41105607e972d3395cf8d89fb1fdf29f0da85
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 10%

---


# Uso de campos de moneda en paneles de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquiera </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td> 
<p>Estándar</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Editar el acceso a Informes, Paneles de control y Calendarios</p>
   <p>Ver acceso a datos financieros</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td><p>Administración de permisos para el tablero</p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

1. Debe tener varios tipos de moneda configurados en la instancia de Workfront para utilizar la funcionalidad descrita en este artículo. Para obtener más información, consulte [Configurar tasas de cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   >[!IMPORTANT]
   >
   >La funcionalidad descrita en este artículo se aplica solo a los campos de moneda nativa. Si tiene configurados tipos de cambio de moneda, próximamente se ofrecerá compatibilidad con los campos de moneda personalizados.


## Establecer una moneda predeterminada para un panel de lienzo

Al crear un panel de lienzo, puede establecer una moneda predeterminada para el panel. Esta moneda se utilizará para mostrar todos los campos de moneda nativa en los informes en el panel, a menos que el campo de moneda esté bloqueado en el nivel de informe.

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. Haga clic en **Nuevo panel** en la esquina superior derecha.

1. En el cuadro **Crear tablero**,

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nombre</strong></td>
      <td><p>Escriba un nombre para el tablero. Se recomienda utilizar solo caracteres UTF-8 para evitar problemas de compatibilidad.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descripción (opcional)</strong></td>
      <td>Escriba una descripción del tablero.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Divisa</strong></td>
      <td>Seleccione el tipo de moneda predeterminado para el panel. <br>
      <br>Los usuarios pueden alternar entre diferentes tipos de moneda al filtrar el panel.</td>
     </tr>
    </tbody>
   </table>


## Cambiar entre monedas en un panel de lienzo

Puede cambiar entre diferentes tipos de moneda en el nivel de panel. Los informes que contienen campos de moneda se actualizarán para reflejar el tipo de moneda seleccionado.

Los campos de moneda se pueden bloquear en el nivel de informe. Si un campo de moneda está bloqueado, el tipo de moneda de ese informe no cambiará al cambiar el tipo de moneda del panel.

Para cambiar el tipo de moneda del tablero,

1. Haga clic en el menú desplegable de moneda en la esquina superior derecha de la página de detalles del panel.
1. Seleccione el tipo de moneda deseado en la lista.

   ![cambiar lista desplegable de moneda](assets/filter-by-currency.png)


## Limitaciones

En la tabla siguiente se describen las limitaciones cuando se definen monedas en el área Tasas de cambio en Configuración.

<table> 
<tr>
<td></td>
<td>Los usuarios pueden</td>
<td>Los usuarios no pueden</td>
</tr>
<tr> 
<td>Se ha definido una sola moneda</td>
<td>
<ul>
<li>Usar campos de moneda nativa en informes de lienzo, gráfico, KPI y tabla</li>
<li>Usar campos de moneda personalizados en informes de lienzo, gráfico y KPI</li>
</ul>
</td>
<td>
<ul>
<li>Asigne una moneda predeterminada al tablero (al crearlo o al editarlo)</li>
<li>Consulte y utilice la opción de moneda de nivel de panel</li>
<li>Bloquear una moneda específica para verla en un gráfico de lienzo, KPI o informe de tabla</li>
<li>Usar campos monetarios de Planning en un gráfico de lienzo, KPI e informes de tabla</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>Se definen varias monedas</td>
<td>
<ul>
  <li>Usar campos de moneda nativa en informes de lienzo, gráfico, KPI y tabla</li>
  <li>Establezca una moneda predeterminada para el tablero (al crearlo o al editarlo)</li>
  <li>Consulte y utilice la opción de moneda de nivel de panel</li>
  <li>Bloquee una moneda específica para verla en un gráfico de lienzo, KPI o informe de tabla y, así, omita la preferencia de alternancia de moneda del panel</li>
</ul>
</td>
<td><ul>
  <li>Usar campos de moneda de datos personalizados en informes de lienzo, KPI y tabla</li>
  <li>Usar campos monetarios de Planning en un gráfico de lienzo, KPI e informes de tabla</li>
</ul>
</td>
</tr></table>





