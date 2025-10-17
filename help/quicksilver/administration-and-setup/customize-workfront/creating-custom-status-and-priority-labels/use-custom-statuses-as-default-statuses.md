---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Usar estados personalizados como estados predeterminados
description: Cuando un estado personalizado se establece como estado predeterminado, el nuevo estado predeterminado se utiliza en todo el sistema de varias formas. La forma en que se usa depende de si se establece como estado predeterminado de nivel del sistema o como estado predeterminado de nivel de grupo.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 97%

---

# Usar estados personalizados como estados predeterminados

Cuando un estado personalizado se establece como estado predeterminado, el nuevo estado predeterminado se utiliza en todo el sistema de varias formas. La forma en que se usa depende de si se establece como estado predeterminado de nivel del sistema o como estado predeterminado de nivel de grupo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Estados personalizados predeterminados de nivel del sistema

Cuando establece un estado personalizado como estado predeterminado del sistema, los nuevos grupos creados en el sistema lo heredan.

Los grupos que ya existían al establecer el nuevo estado predeterminado del sistema no lo heredan automáticamente.

Por ejemplo, supongamos que ya hay dos grupos creados en su entorno de Adobe Workfront (Marketing y Ventas). Se crea un nuevo estado personalizado que equivale a Actual y se llama al estado En proceso. Ahora creará un nuevo grupo llamado Ingeniería. En esta situación, el grupo Ingeniería hereda el nuevo estado predeterminado; los grupos Marketing y Ventas no.

## Estados personalizados predeterminados de nivel de grupo

Se utiliza un estado personalizado que se establece como estado de grupo predeterminado en las siguientes circunstancias:

* **Cuando el sistema de Workfront elige un estado automáticamente, se usa el estado de grupo predeterminado:** el estado personalizado que ha establecido como estado de grupo predeterminado se usa cuando el sistema de Workfront asigna automáticamente un estado a un objeto.

  Por ejemplo, se puede configurar una tarea para que cambie automáticamente al estado Completar cuando el porcentaje completado alcance el 100 %. Si crea un estado personalizado que equivale a Completo y establece ese estado personalizado como estado predeterminado, Workfront cambia el estado de la tarea al nuevo estado predeterminado.

  Los estados personalizados se utilizan de esta manera solo con estados de grupo asociados a una tarea o problema. Los estados personalizados no se pueden utilizar de esta manera para los estados asociados a un proyecto.

* El **estado de un proyecto está determinado por el grupo asociado con el proyecto**: si el grupo asociado con un proyecto determinado cambia, el estado del proyecto cambia según los estados predeterminados definidos para el grupo. (Un grupo se puede asociar con un proyecto mediante el campo Grupos al editar el proyecto).

  Si ese grupo cambia, el estado del proyecto cambia si el nuevo grupo tiene un estado predeterminado diferente definido que coincide con el estado actual del proyecto.

  Por ejemplo, un proyecto se puede asociar con el grupo Marketing y el estado del proyecto se establece en Planificar. El proyecto se edita para que ahora esté asociado con el grupo Ventas. El grupo Ventas tiene un estado de grupo predeterminado personalizado denominado Pensar (y este estado equivale a Planificar). Dado que el grupo del proyecto ha cambiado, el estado del proyecto cambia ahora a Pensando.

Si es administrador de un grupo, consulte [Definir un estado personalizado como estado predeterminado para un grupo](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Estados de los problemas

Si el estado personalizado es un estado de problema, deben habilitarse los cuatro tipos de problemas (informe de errores, solicitud de cambio, problema y solicitud). Por ejemplo, en el estado de problema que se muestra a continuación, el estado Reabierto no se puede utilizar como estado por defecto porque el tipo de problema Solicitud de cambio no está seleccionado:

![Todos los tipos de problemas habilitados](assets/all-4-issue-types-enabled.png)

## Definir un estado personalizado como estado predeterminado

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Estados**.
1. (Condicional) Si está configurando un estado predeterminado para un grupo, empiece a escribir el nombre del grupo en el menú de la esquina superior derecha y, a continuación, selecciónelo cuando aparezca.
1. Abra la pestaña **Proyecto**, **Tareas** o **Problemas**, según el tipo de estado que desee establecer como estado predeterminado.
1. Haga clic en el menú desplegable **Establecer estados predeterminados**.
1. En el área desplegable que se muestra, junto al estado en el que desea establecer el estado predeterminado, seleccione el estado predeterminado que desee.
1. Haga clic en **Guardar**.
1. Asocie el proyecto con el grupo en el que reside el estado.

   >[!NOTE]
   >
   >Si se establece el estado personalizado para un grupo y posteriormente se asigna el proyecto a un grupo diferente, el estado del proyecto se volverá a cargar y podría cambiar.

   1. Vaya al proyecto en el que desea utilizar el estado personalizado.
   1. Haga clic en el icono Más del menú ![Más](assets/more-icon.png) y, a continuación, haga clic en **Editar**.
   1. En el cuadro **Editar proyecto** que se muestra, en el campo **Grupo**, en **Asociación del proyecto**, seleccione el grupo donde resida el estado.
   1. Haga clic en **Guardar cambios**.
