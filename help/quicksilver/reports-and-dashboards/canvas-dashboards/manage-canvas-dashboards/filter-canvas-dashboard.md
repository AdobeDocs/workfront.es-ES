---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrar un panel de lienzo
description: Puede aplicar un filtro a un panel de lienzo una vez que se haya creado.
author: Courtney
feature: Reports and Dashboards
exl-id: 156e9d3f-49f6-4372-9749-c7124ff5baee
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/SRUCt-lfcaIOPghpl2PfbbSMO4oMy4E1hfS7NensXL8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f465ac03e0ff91216d1ef934a1696127796645ba
workflow-type: tm+mt
source-wordcount: 1057
ht-degree: 12%

---

# Filtrar un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

<!--
Take Preview and production mentions out at release
-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Puede aplicar un filtro a un panel de lienzo que contenga mensajes. Una solicitud funciona como un modificador de filtro que aplica criterios de filtrado adicionales para que pueda reducir aún más los resultados. Estos indicadores se pueden modificar cada vez que se aplica el filtro, lo que permite ajustar los resultados mostrados sin necesidad de editar los criterios de filtro principales del panel o de cada informe individual.

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

Debe crear un tablero para poder filtrarlo.

Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Filtrado de un tablero

Siga estos pasos en el orden indicado para filtrar un tablero:

* [Parte 1: Crear un filtro de panel](#part-1-create-a-dashboard-filter)
* [Parte 2: Crear una solicitud de panel](#part-2-define-a-dashboard-prompt)
* [Parte 3: Aplicar un indicador de panel](#step-3-apply-a-dashboard-prompt)

>[!NOTE]
>
>El filtro de tablero se aplicará a todos los informes en los que los filtros de nivel de tablero no estén desactivados.  Puede excluir informes individuales de la aplicación de filtros a nivel de panel. Para ello, expanda el menú de acciones de cada informe y seleccione la opción **Deshabilitar filtros**.


### Parte 1: Crear un filtro de panel

Con un filtro de panel, puede aplicar un filtro común a todos los informes disponibles en un panel sin tener que modificar los filtros para cada informe individual.

>[!NOTE]
>
>Estos filtros solo los puede configurar un usuario con acceso de Administración al panel.


{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, seleccione el panel al que desee aplicar un filtro.

1. En la esquina superior izquierda de la página de detalles del panel, haga clic en **Filtros**. Se abrirá el panel lateral de filtros.

1. (Conditionalt) En el entorno Producción, haga clic en **Editar filtros** o en <span class="preview">en el entorno Vista previa, haga clic en el menú **Más** ![Menú Más](assets/more-icon.png) y, a continuación, haga clic en</span> **Editar filtros**. Se abre el cuadro de diálogo **Filtros del panel**.

1. (Opcional) Para agregar una regla, siga los pasos a continuación:

   1. Seleccione el icono **Editar** a la derecha del cuadro de reglas.

      ![Editar icono](assets/edit-icon.png)

   1. Haga clic en **Agregar condición** y, a continuación, agregue la siguiente información:
      * Haga clic en **Seleccionar campo** para seleccionar un campo por el que desee filtrar.
      * Seleccione una opción (o modificador de filtro) para definir qué tipo de condición debe cumplir el campo.

   1. (Opcional) Haga clic en **Añadir grupo de filtros** para añadir otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Continúe con [Parte 2: Crear una solicitud de panel](#part-2-define-a-dashboard-prompt).


### Parte 2: Definir una solicitud de panel

Una solicitud de panel ofrece a los usuarios la opción de aplicar filtros personalizados adicionales a los informes disponibles en el panel.

>[!NOTE]
>
>Las opciones de solicitud de panel solo las puede configurar un usuario con acceso de Administración al panel.

1. Para agregar una solicitud, siga los pasos a continuación:

   1. Haga clic en **Agregar solicitud**. Los nuevos campos aparecen en la parte derecha de la pantalla.

   1. Escriba una etiqueta en el campo **Personalizar etiqueta**.

   1. Seleccione el campo en el que desea basar la solicitud escribiendo el nombre del campo y seleccionándolo cuando aparezca en la lista. 

1. Para agregar una solicitud personalizada, siga los pasos a continuación:

   1. Seleccione **Agregar solicitud personalizada**. Los nuevos campos aparecen en la parte derecha de la pantalla.

   1. (Opcional) Escriba una etiqueta nueva en el campo **Personalizar etiqueta**. De manera predeterminada, se asigna la etiqueta *Nueva solicitud personalizada*.

   1. Haga clic en **Agregar nueva opción**.

   1. Escriba el nombre del mensaje en el campo **Valor de opción**.

   1. Haga clic en **Agregar condición** y, a continuación, especifique el campo por el que desea filtrar y el modificador que define qué tipo de condición debe cumplir el campo.

      >[!NOTE]
      >
      >La condición de un mensaje personalizado solo se puede editar mediante el modo de texto. Esto permite aplicar varias condiciones en un único campo.


   1. (Opcional) Haga clic en **Añadir grupo de filtros** para añadir otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Haga clic en **Guardar** para aplicar el filtro al tablero.


1. <span class="preview">Para guardar las peticiones de datos como predeterminadas, haga lo siguiente después de guardar la petición de datos: </span>

   <div class="preview">

   1. (Opcional) Haga clic en el menú **Más** ![Menú más](assets/more-icon.png) y, a continuación, haga clic en **Guardar como mensajes predeterminados**.

      El filtro del mensaje se aplica cada vez que se carga el panel para cualquier persona con permisos de Vista o superiores.
   1. (Condicional) Si accede a un panel con una solicitud predeterminada aplicada, puede modificar el filtro y las modificaciones se guardan como preferencia personal. Se dan los siguientes escenarios:

      * Si tiene permisos de administración en el tablero, haga clic en **Guardar como mensajes predeterminados** para guardar las modificaciones como filtro predeterminado. Esto reemplaza los valores predeterminados originales.
      * Si tiene permisos de visualización en el panel, las modificaciones solo se mostrarán por usted. Al actualizar la página, se conserva la configuración.

   1. (Condicional) Si ha modificado la configuración de la petición de datos predeterminada, haga clic en el menú **Más** ![Menú más](assets/more-icon.png) y, a continuación, haga clic en **Aplicar valores predeterminados del tablero** para volver a los resultados de filtro predeterminados.
   1. (Opcional) Haga clic en **Restablecer valores predeterminados** para reemplazar la configuración predeterminada original con las modificaciones. Esta opción solo está disponible para los administradores de tableros.

   </div>


1. Continúe con [Parte 3: Aplicar una solicitud de panel](#step-3-apply-a-dashboard-prompt).

### Paso 3: Aplicar una solicitud de panel

Todos los usuarios con acceso a un tablero pueden aplicar una solicitud de tablero a un tablero de lienzo una vez que se hayan creado el filtro y las solicitudes.

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, seleccione el panel al que desee aplicar la solicitud.

1. En la esquina superior izquierda de la página de detalles del panel, haga clic en **Filtros**. Se abrirá el panel lateral de filtros.

1. En la sección **Mostrar registros donde...**, elija una condición para uno o todos los mensajes mostrados. Se aplica la solicitud y aparece la etiqueta **Solicitudes del panel aplicadas** en la esquina del widget de informe.
   ![Seleccionar condición](assets/prompts-list.png)

1. Haga clic en el icono **Cerrar** ![Cerrar icono](assets/close-icon.png) en la esquina superior derecha para ocultar el panel.



