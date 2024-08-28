---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Instalación de un paquete de promoción de entorno
description: La capacidad de promoción de entornos está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. Obtenga información sobre cómo instalar un paquete de promoción de entorno en un entorno de destino.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Instalación de un paquete de promoción de entorno

Después de crear un paquete, puede instalarlo en un entorno diferente.

Debe instalar un paquete en el entorno en el que desea copiar los objetos **a**. Por ejemplo, si está configurando un proyecto en el entorno de espacio aislado de actualización personalizado y lo está promocionando al entorno de producción, debe instalar el paquete en el entorno de producción.

>[!IMPORTANT]
>
>Si la zona protegida de actualización personalizada se actualiza mientras configura un objeto para la promoción del entorno, esa configuración se perderá durante la actualización. Le recomendamos que no actualice la zona protegida de actualización personalizada a menos que todos los objetos y paquetes de promoción de entorno pendientes se hayan promocionado correctamente.

## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime o Ultimate (solo planes nuevos)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licencias</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Se debe crear un paquete de promoción de entorno para poder instalarlo.

Para obtener instrucciones, consulte [Crear o editar un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Estado del paquete para la instalación

Un paquete debe estar en estado ACTIVO para poder instalarse en el entorno de producción.

Se recomienda mover el paquete al estado TESTING e instalarlo en otra zona protegida para probar el paquete.  Si esta prueba se realiza correctamente y no hay errores, mueva el paquete a ACTIVO para instalarlo en el entorno de producción.

Para editar el estado de un paquete:

1. Seleccione el paquete como se describe en [Editar o ensamblar un paquete existente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) en el artículo Crear y editar paquetes de promoción de entorno.
1. Haga clic en **Editar paquete**.
1. Haga clic en **Estado**.
1. Seleccione el estado que desee en el menú desplegable.

Para obtener más información sobre los estados, consulte [Estados de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) en el artículo Información general sobre cómo mover objetos entre entornos de Workfront.

## Instalación de un paquete

>[!NOTE]
>
>* Para instalar un paquete, debe haber iniciado sesión en el entorno en el que desea instalarlo. Este es el entorno en el que está copiando los objetos **a**.

1. Vaya al entorno en el que desea instalar el paquete.
1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **Sistema** en el panel de navegación izquierdo, luego seleccione **Promoción de entorno**.
1. Seleccione el paquete en la lista mostrada.
1. Para cada objeto que tenga un conflicto, seleccione cómo resolver el conflicto.

   Para resolver un conflicto, haga clic en la flecha desplegable situada junto al tipo de objeto y seleccione la acción que desee realizar.

   Para obtener más información, vea [Conflictos](#collisions) en este artículo
1. Para implementar el paquete en el nuevo entorno, haga clic en **Implementar** en la parte superior derecha de la pantalla.

## Conflictos

Un conflicto es un objeto que se encuentra en el entorno de destino de una instalación que coincide con uno de los objetos que se están instalando desde el entorno de origen. Los conflictos se detectan comparando los nombres e ID de los objetos de origen con los objetos del entorno de destino. Los conflictos también se detectan comparando objetos de origen con registros de objetos instalados anteriormente.

Cuando se produce una colisión, puede seleccionar cómo resolverla. Los conflictos se resuelven en el nivel de objeto.

Para ver los conflictos, haga clic en la lista desplegable situada junto a cada tipo de objeto. Los conflictos se muestran en la columna Conflicto.

>[!NOTE]
>
>Es posible que los conflictos detectados no sean los objetos que desea anular o utilizar en la instalación. Se recomienda validar los conflictos detectados para garantizar que los destinos de instalación son correctos.

Para resolver un conflicto, seleccione una acción en la columna Acción de implementación o utilice la acción predeterminada que ya se muestra.

* **Crear con nuevo nombre**: cree un nuevo objeto en el entorno de destino. Si el objeto existe en el entorno de destino, puede crear un nuevo objeto con un nombre nuevo. Si no existe en el entorno de destino, puede crear el objeto con un nombre nuevo o con el nombre que tiene el objeto en el paquete.
* **Usar existente**: el objeto del paquete no está instalado y el objeto que ya existía en el entorno de destino no se ha modificado.
* **Sobrescribir**: el objeto del paquete reemplaza el objeto existente en el entorno de destino.

  También puede elegir objetos para sobrescribirlos incluso si no se detecta ninguna colisión.

  Para obtener detalles sobre cómo la sobrescritura afecta a los objetos principales y secundarios, consulte [Sobrescritura de objetos principales y secundarios](#overwriting-parent-and-child-objects) en este artículo.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Los valores predeterminados son `Create new` si el objeto no existe en el entorno de destino y `Use existing` si el objeto no existe en el entorno de destino. Para volver a la asignación predeterminada, haga clic en **Restablecer asignación predeterminada**.

## Sobrescribir objetos principales y secundarios

Algunos objetos del paquete de promoción pueden tener objetos secundarios. Por ejemplo, un proyecto (principal) tiene tareas (secundarias). Al sobrescribir un objeto principal, los objetos secundarios se gestionan de la siguiente manera:

* Los objetos secundarios que existen tanto en el paquete como en el destino se actualizarán en el destino para que coincidan con el paquete.
* Se crearán los objetos secundarios que existan en el paquete pero no el destino.
* Los objetos secundarios que existen en el destino pero no en el paquete permanecerán sin cambios.

Esta funcionalidad afecta a los siguientes objetos principales y secundarios:

| Objeto principal | Objetos secundarios |
|---|---|
| Proyecto | Tarea<br>QueueDef (definición de cola)<br>RoutingRule |
| Plantilla | TemplateTask<br>QueueDef (definición de cola)<br>RoutingRule |
| Parámetro (campo de formulario personalizado) | ParameterOption (opción de campo de formulario personalizado) |
| CalendarInfo | SecciónCalendario |
| QueueDef (definición de cola) | QueueTopicGroup<br>QueueTopic |

