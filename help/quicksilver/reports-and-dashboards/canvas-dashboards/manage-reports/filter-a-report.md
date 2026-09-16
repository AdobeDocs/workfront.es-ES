---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrado de un informe en un panel de lienzo
description: Añada o edite un filtro en un informe para controlar qué datos se muestran en un panel de lienzo.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 19%
---
# Filtrado de un informe en un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Contacto con el servicio de asistencia al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Puede filtrar un informe para controlar qué datos se muestran, tanto mientras crea el informe como en cualquier momento posterior. Las opciones de filtrado y el comportamiento son los mismos en cualquier caso.

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
  </td> 
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

Debe tener un informe en un tablero o estar generando uno para poder filtrarlo. Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Adición o edición de un filtro de informe

Para agregar o editar un filtro en un informe:

1. Abra el panel de filtro del informe:

   * Si estás creando un informe, haz clic en el icono **Filtro** en el panel izquierdo del cuadro de diálogo **Configurar**.
   * Si está editando un informe existente, haga clic en el icono **Más** en la esquina superior derecha, seleccione **Editar** y, a continuación, haga clic en el panel **Filtros** del cuadro de diálogo **Configurar**.

1. Haga clic en **Editar filtro**.

1. Haga clic en **Agregar condición** y defina la condición:

   * Haga clic en **Seleccionar campo** y, a continuación, seleccione el campo por el que desee filtrar.
   * Seleccione el modificador que define qué tipo de condición debe cumplir el campo.
   * Escriba o seleccione el valor con el que se va a evaluar, si el modificador lo requiere.

   ![Agregar condición](assets/add-condition.png)

1. (Opcional) Repita el paso anterior para agregar más condiciones.

1. (Opcional) Haga clic en **Añadir grupo de filtros** para añadir otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

>[!NOTE]
>
>Para obtener la lista completa de campos, operadores, comodines y reglas de filtrado especiales, consulte [Referencia de filtro de informe para paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

1. Haga clic en **Guardar**.
