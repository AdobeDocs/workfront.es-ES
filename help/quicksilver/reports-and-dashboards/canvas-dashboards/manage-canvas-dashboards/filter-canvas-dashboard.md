---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrado de un panel de lienzo
description: Puede aplicar un filtro a un panel de lienzo una vez que se haya creado.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 156e9d3f-49f6-4372-9749-c7124ff5baee
source-git-commit: 39a8d670baa19aa37e29b0312e6c9a296569f44c
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 9%

---

# Filtrado de un panel de lienzo

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes.</span>

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform


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

1. Seleccione **Editar filtros**. Se abre el cuadro de diálogo **Filtros del panel**.

1. (Opcional) Para agregar una regla, siga los pasos a continuación:

   1. Seleccione el icono **Editar** a la derecha del cuadro de reglas.

      ![Editar icono](assets/edit-icon.png)

   1. Haga clic en **Agregar condición** y, a continuación, agregue la siguiente información:
      * Seleccione un campo por el que desee filtrar.
      * Seleccione una opción (o modificador de filtro) para definir qué tipo de condición debe cumplir el campo.

   1. (Opcional) Haga clic en **Agregar grupo de filtros** para agregar otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Continúe con [Parte 2: Crear una solicitud de panel](#part-2-define-a-dashboard-prompt).


### Parte 2: Definir una solicitud de panel

Una solicitud de panel ofrece a los usuarios la opción de aplicar filtros personalizados adicionales a los informes disponibles en el panel.

>[!NOTE]
>
>Las opciones de solicitud de panel solo las puede configurar un usuario con acceso de Administración al panel.

1. Para agregar una solicitud, siga los pasos a continuación:

   1. Seleccione **Agregar solicitud**. Los nuevos campos aparecen en la parte derecha de la pantalla.

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


   1. (Opcional) Haga clic en **Agregar grupo de filtros** para agregar otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Haga clic en **Guardar** para aplicar el filtro al tablero.

1. Continúe con [Parte 3: Aplicar una solicitud de panel](#step-3-apply-a-dashboard-prompt).

### Paso 3: Aplicar una solicitud de panel

Todos los usuarios con acceso a un tablero pueden aplicar una solicitud de tablero a un tablero de lienzo una vez que se hayan creado el filtro y las solicitudes.

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, seleccione el panel al que desee aplicar la solicitud.

1. En la esquina superior izquierda de la página de detalles del panel, haga clic en **Filtros**. Se abrirá el panel lateral de filtros.

1. En la sección **Mostrar registros donde...**, elija una condición para uno o todos los mensajes mostrados. Se aplica la solicitud y aparece la etiqueta **Filtros del panel aplicados** en la esquina del widget de informe.
   ![Seleccionar condición](assets/prompts-list.png)

1. Haga clic en el icono **Cerrar** ![Cerrar icono](assets/close-icon.png) en la esquina superior derecha para ocultar el panel.

<span class="preview">

## Filtrado de un tablero por tipo de moneda

Puede alternar entre diferentes tipos de moneda en el nivel de panel. Los informes que contienen campos de moneda se actualizarán para reflejar el tipo de moneda seleccionado.

>[!NOTE]
>
>Los campos de moneda se pueden bloquear en el nivel de informe. Si un campo de moneda está bloqueado, el tipo de moneda de ese informe no cambiará al cambiar el tipo de moneda del panel.

Para cambiar el tipo de moneda del tablero,

1. Haga clic en el menú desplegable de moneda en la esquina superior derecha de la página de detalles del panel.
1. Seleccione el tipo de moneda deseado en la lista.

   ![cambiar lista desplegable de moneda](assets/filter-by-currency.png)

</span>