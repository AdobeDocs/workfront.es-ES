---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Copiar un panel de lienzo
description: Puede Copiar un panel de lienzo para crear una variación del mismo, como una copia específica de la audiencia, sin volver a crearlo desde cero.
author: Courtney
feature: Reports and Dashboards
source-git-commit: b66f6931ee2fe83688fb8910861af6e958d1f74f
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 16%

---

# Copiar un panel de lienzo

{{highlighted-preview-article-level}}

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Contacto con el servicio de asistencia al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Puede copiar un panel de lienzo para crear una variación de él para una audiencia diferente, como una copia a nivel de director de un panel ejecutivo, sin reconstruirlo desde cero.

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
<p>Estándar </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Editar o crear acceso a paneles</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td><p>Ver acceso al panel</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Debe crear un tablero para poder duplicarlo.

Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Copiar un tablero

>[!NOTE]
>
>Las preferencias de uso compartido no se copian en el nuevo tablero. Si un widget tiene una configuración de **Ejecutar como usuario**, esa configuración solo se conservará en la copia si usted es el usuario designado o un administrador del sistema.

Para copiar un tablero:

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, abra el panel que desee copiar.

1. En la esquina superior derecha, seleccione el icono **Más** ![Más](assets/more-icon.png) y, a continuación, seleccione **Copiar**.
   ![Opción de menú Copiar panel](assets/duplicate-dashboard.png)

1. En el cuadro de diálogo **Copiar panel**, escriba un **Nombre** para el nuevo panel, que toma como valor predeterminado el nombre del panel de origen seguido de &quot;(Copiar)&quot;.

1. (Opcional) En la ficha **Detalles del panel**, actualice la **Descripción** o la **Moneda** para el nuevo panel.
   ![Copiar tablero: ficha Detalles del tablero](assets/duplicate-details.png)

1. (Opcional) Haga clic en la ficha **Widgets** y, a continuación, anule la selección de los widgets que no desee incluir en el tablero duplicado.
   ![Copiar tablero: ficha Widgets](assets/copy-widgets.png)

1. (Opcional) Haga clic en la ficha **Filtros e indicadores** y, a continuación, desactive **Copiar filtros de tablero** o **Copiar indicadores de tablero** para excluirlos del tablero duplicado.
   ![Copiar tablero: ficha Filtros e indicadores](assets/copy-filters.png)

1. Haga clic en **Copiar tablero**.

Aparece un mensaje de confirmación con un vínculo al nuevo panel.
