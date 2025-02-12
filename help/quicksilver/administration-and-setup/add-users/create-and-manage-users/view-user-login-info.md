---
title: Ver información de inicio de sesión de usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puede ver la frecuencia con la que los usuarios inician sesión en Workfront, así como la última vez que lo hicieron, indicando que desea incluir esta información en la vista de una lista de usuarios o en un informe para usuarios.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 94%

---

# Ver información de inicio de sesión de usuario

Puede ver la frecuencia con la que los usuarios inician sesión en Adobe Workfront, así como la última vez que lo hicieron, indicando que desea incluir esta información en la vista de una lista de usuarios o en un informe para usuarios.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p><p>O</p><p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Edición</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si <b>Administrador de usuarios (usuarios de grupo)</b> está habilitado, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cómo registra Workfront la información de inicio de sesión

Workfront registra la siguiente información sobre los usuarios que inician sesión en el sistema:

* **Recuento de inicio de sesión**: Workfront cuenta el inicio de sesión en la aplicación por parte de un usuario una vez cada 24 horas. Si un usuario inicia sesión varias veces con diferentes exploradores, equipos o dispositivos móviles, Workfront cuenta todos los inicios de sesión de un mismo día como un único inicio de sesión. El recuento de inicio de sesión incluye información a partir del momento en que se creó el usuario.
* **Fecha del último inicio de sesión**: la última fecha en la que un usuario inició sesión. En este campo se registra la fecha de cada inicio de sesión desde cualquier navegador, dispositivo móvil u otras aplicaciones.

El inicio de sesión en Workfront de cualquiera de las siguientes maneras cuenta como un inicio de sesión en Workfront:

* La aplicación web de Workfront
* Las aplicaciones móviles de Workfront (dispositivos iOS o Android)
* Cualquier integración de Workfront compatible con una aplicación de terceros (Slack, Jira)
* Cualquier integración personalizada entre Workfront y una aplicación de terceros.
* La API de Workfront

  >[!NOTE]
  >
  >El inicio de sesión en Workfront a través de la API de Workfront solo está disponible para organizaciones que aún no se han incorporado a Adobe Business Platform.

## Mostrar información de uso en una lista de usuarios o un informe

Puede mostrar los campos Recuento de inicio de sesión y Fecha de último inicio de sesión en la vista de una lista de usuarios o en un informe para usuarios.\
Para obtener más información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para mostrar la información de uso en la vista de una lista de usuarios:

1. Vaya a una lista de usuarios en Workfront.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. Haga clic en **Agregar columna** cerca de la esquina inferior derecha de la pantalla.
1. En el campo **Mostrar en esta columna**, empiece a escribir **Recuento de inicio de sesión** y, a continuación, selecciónelo cuando aparezca en la lista bajo **Usuario**.

1. Haga clic en **Añadir columna** de nuevo.
1. En el campo **Mostrar en la columna**, empiece a escribir **Fecha de último inicio de sesión** y, a continuación, selecciónela cuando aparezca en la lista bajo **Usuario**.

1. (Opcional) Haga clic en **Opciones avanzadas** y, a continuación, seleccione un **Formato de campo** en el menú desplegable para incluir la hora o el día de la semana del último inicio de sesión en su columna.

1. Pulse **Guardar vista**.\
   La vista incluye información sobre cuántas veces han iniciado sesión los usuarios y cuándo iniciaron sesión por última vez.
