---
title: Ver información de inicio de sesión del usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puede ver la frecuencia con la que los usuarios inician sesión en Workfront, así como la última vez que inician sesión, indicando que desea incluir esta información en la vista de una lista de usuarios o en un informe para los usuarios.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Ver información de inicio de sesión del usuario

Puede ver la frecuencia con la que los usuarios inician sesión en Adobe Workfront, así como la última vez que inician sesión, indicando que desea incluir esta información en la vista de una lista de usuarios o en un informe para los usuarios.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener una de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p><b>Usuarios</b> en el nivel de acceso configurado para <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si es Usuario <b>Administración (usuarios del grupo)</b> está activada, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> <p>Para obtener más información sobre la variable <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Cómo registra Workfront la información de inicio de sesión

Workfront registra la siguiente información sobre los usuarios que inician sesión en el sistema:

* **Recuento de inicio de sesión**: Workfront cuenta un usuario que inicia sesión en la aplicación una vez cada 24 horas. Si un usuario inicia sesión varias veces con distintos navegadores, equipos o dispositivos móviles, Workfront cuenta todos los inicios de sesión que se produjeron en un día como un inicio de sesión. El recuento de inicios de sesión incluye información que comienza con el momento en que se creó el usuario.
* **Fecha del último inicio de sesión**: La última fecha en la que un usuario inició sesión. La fecha de cada inicio de sesión desde cualquier explorador, dispositivo móvil u otras aplicaciones se registra en este campo.

El inicio de sesión en Workfront de cualquiera de estas formas cuenta como un inicio de sesión en Workfront:

* La aplicación web de Workfront
* Aplicaciones móviles de Workfront (dispositivos iOS o Android)
* Cualquier integración compatible con Workfront con otra aplicación de terceros (Slack, Jira)
* Cualquier integración personalizada entre Workfront y otra aplicación de terceros.
* La API de Workfront

   >[!NOTE]
   >
   >El inicio de sesión en Workfront a través de la API de Workfront solo está disponible para las organizaciones que aún no están integradas en Adobe Business Platform.

## Mostrar la información de uso en una lista de usuarios o en un informe

Puede mostrar los campos Recuento de inicio de sesión y Fecha de último inicio de sesión en la vista de una lista de usuarios o en un informe para los usuarios.\
Para obtener más información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para mostrar la información de uso en la vista de una lista de usuarios:

1. Vaya a una lista de usuarios de Workfront.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. Haga clic en **Agregar columna** cerca de la esquina inferior derecha de la pantalla.
1. En el **Mostrar en esta columna** campo, empezar a escribir **Recuento de inicio de sesión** y selecciónela cuando aparezca en la lista de **Usuario**.

1. Haga clic en **Agregar columna** de nuevo.
1. En el **Mostrar en la columna** campo, empezar a escribir **Fecha del último inicio de sesión** y selecciónela cuando aparezca en la lista de **Usuario**.

1. (Opcional) Haga clic en **Opciones avanzadas** y, a continuación, seleccione un **Formato de campo** en el menú desplegable para incluir la hora o el día de la semana del último inicio de sesión en su columna.

1. Haga clic en **Guardar vista**.\
   La vista incluye información sobre cuántas veces los usuarios han iniciado sesión y cuándo lo hicieron por última vez.
