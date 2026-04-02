---
content-type: overview
product-area: projects
navigation-topic: financials
title: Anular tasas de costo de usuario en el nivel de proyecto
description: Este artículo describe cómo puede anular las tasas de costo de usuario del sistema para un proyecto.
author: Lisa
feature: Work Management
source-git-commit: cb21414992587c62c37580f156100f2b5b755e9b
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 13%

---

# Anular las tasas de costo de usuario en el nivel de proyecto

{{highlighted-preview-article-level}}

Puede especificar la tasa de costo de un usuario en un proyecto específico. Esta tasa de coste a nivel de proyecto anula la tasa de coste a nivel de sistema para este usuario. Workfront utiliza la tasa de coste a nivel de proyecto de la función de trabajo para calcular el coste, en lugar de utilizar la tasa de coste a nivel de sistema.

Este artículo describe cómo puede anular las tasas de costo de usuario del sistema para un proyecto.

Para obtener más información sobre el cálculo de costos en el proyecto, vea [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) y [Seguimiento de costos](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>Estándar</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos y datos financieros</p>
       <p><p>También debe tener uno de los siguientes:</p> 
        <ul> 
          <li> <p>El nivel de acceso del administrador del sistema. </li> 
          <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Edición</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si <b>Administrador de usuarios (usuarios de grupo)</b> está habilitado, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administrar permisos para el proyecto que incluye Editar datos financieros </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

El usuario debe tener habilitado el campo **Anulación de tasa de costo permitida** en su perfil de usuario. Cuando un usuario no tiene habilitado el campo de anulación de costes, no se permiten anulaciones de costes para ese usuario en ningún proyecto y el sistema utiliza la tasa en el perfil de usuario para calcular el coste.

Para obtener más información, consulte [Editar el perfil de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Anular las tasas de costo de usuario en el nivel de proyecto

1. Vaya al proyecto para el que desea anular las tasas de coste.
1. Haga clic en **Tasas** en el panel izquierdo. Es posible que primero tenga que hacer clic en **Mostrar más**.
1. Haga clic en la ficha **Costo** si aún no está seleccionada.
1. Haga clic en **Agregar tarifa de costo** > **Nueva tarifa de costo de usuario**.

   Se abre el cuadro Nueva tasa de costo de usuario.

1. En el campo **Usuario**, seleccione el usuario para el que desea cambiar la tasa de costo.
1. Seleccione la **Moneda** para la anulación de tasa de costo.
1. En el campo **Tasa de costo**, escriba la primera anulación de la tasa de costo.
1. (Opcional) Haga clic en **Agregar tarifa vigente por fecha** para agregar más anulaciones de tarifa de costo.

   >[!NOTE]
   >
   >Si introduce una sola anulación de tasa, se aplica durante toda la vida del proyecto.
   >Si desea tener tasas diferentes con el tiempo, puede agregar varias invalidaciones con fecha en vigor.

1. (Condicional) Si agrega varias anulaciones de tasa de coste, especifique la siguiente información para cada fila:

   * **Tasa de costo**: el valor de la tasa de costo durante el período de tiempo especificado.
   * **Fecha de inicio**: la fecha en la que comienza la invalidación de la tasa de costo.
   * **Fecha de finalización**: la fecha en la que finaliza la invalidación de la tasa de costo.

   ![Nueva casilla de tasa de costo de usuario que muestra fechas efectivas](assets/new-user-cost-rate-box.png)

   Workfront aplica la tasa de rol de reemplazo a las horas que ocurren durante estos lapsos de tiempo al calcular el costo en el proyecto.

   No debe haber espacios entre los marcos de tiempo de dos tasas de anulación. La **fecha de inicio** de una tasa de invalidación debe ser el día inmediatamente posterior a la **fecha de finalización** de la fecha de invalidación anterior.

   No es necesario especificar una fecha de inicio para la primera tasa de sustitución, ni una fecha de finalización para la última tasa de sustitución.

   Le recomendamos que utilice la Tasa predeterminada para la primera tasa de anulación.

   Workfront supone que la primera tasa de anulación se aplica a todas las horas con una fecha anterior a la fecha de finalización de la primera anulación y que la última tasa de anulación se aplica a todas las horas con una fecha posterior a la fecha de inicio de la última anulación.

   Si se registra una hora antes de la fecha planificada de inicio del proyecto, se utiliza la primera tasa de coste.

   Si se registra una hora después de la fecha planificada de finalización del proyecto, se utiliza la última tasa de coste.

1. Haga clic en **Guardar**.


