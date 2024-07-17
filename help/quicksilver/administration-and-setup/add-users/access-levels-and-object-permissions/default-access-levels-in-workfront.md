---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,modelo,canal,diagrama,niveles,permisos
navigation-topic: access-levels
title: Niveles de acceso integrados
description: Cada uno de los seis niveles de acceso integrados actuales está diseñado para un tipo particular de usuario, incluidos el administrador del sistema, el planificador, el trabajador, el revisor, el solicitante y el usuario externo. Estos niveles de acceso le permiten controlar lo que los usuarios pueden editar y ver en el sistema. Si necesita un nivel de acceso personalizado, puede copiar un nivel de acceso integrado y modificarlo según la cantidad de acceso que desee que permita para los distintos tipos de objetos de Workfront.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '1685'
ht-degree: 5%

---

# Niveles de acceso integrados

<!--Audited: 01/2024-->

>[!NOTE]
>
>En este artículo se describen los niveles de acceso integrados actuales en Adobe Workfront. Para obtener información acerca de los nuevos niveles de acceso integrados, vea [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Cada uno de los seis niveles de acceso integrados actuales está diseñado para un tipo particular de usuario. Estos niveles de acceso le permiten controlar lo que los usuarios pueden editar y ver en el sistema.

Cada uno de los seis niveles de acceso integrados está diseñado para los siguientes tipos de usuarios:

* Administrador del sistema
* Planificador
* Trabajador
* Revisor
* Solicitante
* Usuario externo

Según el nivel de acceso, hay disponibles hasta 3 configuraciones para la mayoría de los tipos de objetos de Workfront:

<table style="table-layout:auto">
    <tr>
        <td>Editar</td>
        <td>Los usuarios pueden crear, editar, eliminar y compartir el objeto de Workfront</td>
    </tr>
    <tr>
        <td>Ver</td>
        <td>Los usuarios pueden revisar y compartir el objeto de Workfront</td>
    </tr>
    <tr>
        <td>Sin acceso</td>
        <td>Los usuarios no pueden acceder al objeto Workfront</td>
    </tr>
</table>

Si necesita un nivel de acceso personalizado de Planificador, Trabajador, Solicitante o Revisor, puede copiar el nivel de acceso integrado y determinar la cantidad de acceso que desea que permita para los distintos tipos de objetos de Workfront.

>[!TIP]
>
>No puede modificar los niveles de acceso de Administrador del sistema o Usuario externo.

Para obtener información sobre cómo crear un nivel de acceso personalizado o modificar uno de los niveles de acceso integrados, vea [Crear y modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que deje los niveles de acceso integrados sin cambios para que pueda hacer referencia a ellos después de configurar los usuarios.

Para obtener información general sobre estos niveles de acceso, consulte [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Nivel de acceso del administrador del sistema

Adjuntado a la licencia de planificación, el nivel de acceso integrado Administrador del sistema está diseñado para un usuario a cargo de la administración del sistema de Adobe Workfront. No puede modificar este nivel de acceso integrado.

Los usuarios con nivel de acceso de administrador del sistema pueden hacer de todo en Workfront. Pueden ver y editar todos los objetos de Workfront y la información introducida en Workfront por todos los demás usuarios.

También tienen acceso completo al área de Configuración, donde pueden cambiar cualquier configuración en el sistema. Y pueden acceder a todas las áreas del menú principal ![](assets/main-menu-icon.png) o del menú principal ![](assets/lines-main-menu.png), si están disponibles.

Para obtener más información, consulte [Conceder acceso administrativo completo a un usuario](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Nivel de acceso del planificador

También se adjunta a la licencia de planificación, el nivel de acceso de Planificador está diseñado para:

* Administradores de grupos, equipos, proyectos y recursos
* Cualquier persona responsable de planificar, crear y administrar tareas, proyectos, portafolios y programas
* Cualquiera que sea responsable de asignar trabajo (tareas y problemas) a otros usuarios
* Usuarios que crean informes y aprueban hojas de horas, elementos de trabajo y documentos
* Usuarios que necesitan acceso a todas las áreas del menú principal ![](assets/main-menu-icon.png) o del menú principal ![](assets/lines-main-menu.png), si están disponibles

Puede crear una versión personalizada del nivel de acceso integrado del Planificador y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, vea [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

A continuación, se muestran las opciones de acceso más altas disponibles para los objetos en el nivel de acceso de Planificador:

| Tipo de objeto de Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyectos |   |   | ✓ |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   |   | ✓ |
| Programas |   |   | ✓ |
| Informes, paneles y calendarios |   |   | ✓ |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Equipos |   |   | ✓ |
| Plantillas |   |   | ✓ |
| Datos financieros |   |   | ✓ |
| Administración de recursos |   |   | ✓ |
| Planificador de escenarios |   |   | ✓ (La configuración predeterminada es Sin acceso.) |
| Workfront Goals |   |   | ✓ (La configuración predeterminada es Sin acceso.) |

{style="table-layout:auto"}

## Nivel de acceso del trabajador

Adjuntado a la licencia de trabajo, el nivel de acceso de Trabajador está diseñado para los usuarios que realizan el trabajo en Workfront. No planean el trabajo, lo completan.

Usuarios con este nivel de acceso:

* Están asignados a elementos de trabajo en los que pueden contribuir y registrar tiempo
* Pueden aprobar trabajos y documentos, pero no plantillas de horas
* Puede acceder a informes y compartirlos
* Puede comunicarse con otros usuarios del sistema
* No se puede obtener acceso a todas las áreas del menú principal ![](assets/main-menu-icon.png) o del menú principal ![](assets/lines-main-menu.png), si están disponibles, y el área &quot;Usuarios&quot; se denomina Equipos. En el área Equipos, los usuarios con este nivel de acceso solo pueden ver los equipos a los que pertenecen, junto con el trabajo asignado a esos equipos.
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas o informes.

Puede crear una versión personalizada del nivel de acceso integrado Trabajador y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, vea [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

A continuación se muestran las opciones de acceso más altas disponibles para los objetos en el nivel de acceso Trabajador:

| Tipo de objeto de Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyectos |   |   | ✓ (Limitado: los usuarios solo pueden compartir el proyecto, crear tareas y problemas en él y editar datos en formularios personalizados que ya estén adjuntos a él.) |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   | ✓ (La configuración predeterminada es Sin acceso.) |   |
| Programas |   | ✓ (La configuración predeterminada es Sin acceso.) |   |
| Informes, paneles y calendarios |   | ✓ |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Equipos |   |   | ✓ (acceso limitado) |
| Plantillas | ✓ |   |   |
| Datos financieros |   | ✓ (La configuración predeterminada es Sin acceso. La configuración Ver permite al usuario ver solo el área de Finanzas   en Detalles del proyecto). |   |
| Administración de recursos |   | ✓ |   |
| Planificador de escenarios |   |   | ✓ (La configuración predeterminada es Sin acceso.) |
| Workfront Goals |   |   | ✓ (La configuración predeterminada es Sin acceso.) |

{style="table-layout:auto"}

## Nivel de acceso del revisor

Adjuntado a la licencia de revisión, el nivel de acceso de revisor está diseñado para los ejecutivos que solicitan trabajo a otros usuarios y que revisan y aprueban el trabajo. No son propietarios de proyecto ni miembros del equipo, pero necesitan acceso a Workfront para ver los elementos de trabajo que supervisan.

Por ejemplo, una parte interesada con este nivel de acceso podría iniciar sesión en Workfront para participar en una revisión continua de los materiales de marketing, ver las actualizaciones de trabajo sobre el trabajo y revisar documentos, aprobaciones, informes y calendarios.

Usuarios con nivel de acceso de Revisor:

* No se pueden asignar elementos de trabajo ni aprobar plantillas de horas
* Puede acceder a las áreas Solicitudes y Documentos en el menú principal ![](assets/main-menu-icon.png) o en el menú principal ![](assets/lines-main-menu.png), si están disponibles
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas o informes.

Puede crear una versión personalizada del nivel de acceso integrado del Revisor y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, vea [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Más limitada para los proyectos y tareas que el nivel de acceso de Trabajador, la configuración de acceso más alta disponible para los objetos en el nivel de acceso de Revisor es la siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto de Workfront</th> 
   <th>Sin acceso</th> 
   <th>Ver acceso</th> 
   <th>Editar acceso</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Proyectos</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tareas</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portafolios</td> 
   <td> </td> 
   <td>✓ (La configuración predeterminada es Sin acceso.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td> </td> 
   <td>✓ (La configuración predeterminada es Sin acceso.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Informes, paneles y calendarios</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtros, vistas y agrupaciones</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuarios</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
<tr> 
   <td>Equipos</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr>

<tr> 
   <td>Plantillas</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Datos financieros</td> 
   <td> </td> 
   <td> <p>✓ (La configuración predeterminada es Sin acceso. La configuración Ver permite al usuario ver solo el área de Finanzas   en Detalles del proyecto).</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Administración de recursos</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planificador de escenarios </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (La configuración predeterminada es Sin acceso.)</td> 
  </tr> 
  <tr> 
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (La configuración predeterminada es Sin acceso.)</td> 
  </tr> 
 </tbody> 
</table>

## Nivel de acceso del solicitante

Adjuntado a la licencia de solicitud, el nivel de acceso de solicitante está diseñado para los usuarios que realizan y reciben solicitudes de trabajo sencillas en Workfront. De forma predeterminada, se limitan al área de Solicitudes.

Por ejemplo, un usuario puede registrar problemas en la cola de solicitudes del servicio de asistencia de su organización.

Usuarios con este nivel de acceso:

* Puede realizar solicitudes y actualizarlas
* Puede cargar y aprobar documentos
* Puede revisar el estado de los problemas que han enviado
* No se puede asignar a elementos de trabajo
* Solo puede acceder a las solicitudes desde el área Solicitudes del menú principal ![](assets/main-menu-icon.png) o el menú principal ![](assets/lines-main-menu.png), si están disponibles. Para obtener más información acerca de las colas de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Puede crear una versión personalizada del nivel de acceso integrado del solicitante y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, vea [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso Solicitante:

| Tipo de objeto de Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto |   | ✓ (Solo la página Detalles del proyecto) |   |
| Tarea |   | ✓ (Solo la página Detalles de la tarea) |   |
| Problema |   |   | ✓ |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes, paneles y calendarios |   | ✓ |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuario |   | ✓ |   |
| Equipos |   | ✓ |   |
| Plantillas | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Workfront Goals |   |   | ✓ (La configuración predeterminada es Sin acceso.) |

{style="table-layout:auto"}

## Nivel de acceso de usuario externo

El nivel de acceso de usuario externo no está adjunto a una licencia de Workfront de pago. Es el nivel de acceso más restrictivo, diseñado principalmente para colaboradores como consultores externos que no inician sesión en Workfront, pero que necesitan revisar, descargar o ver documentos ocasionalmente.

Los usuarios de Workfront pueden asignar tareas a usuarios externos aunque estos no puedan iniciar sesión en el sistema. Sin embargo, no se recomienda asignar tareas y problemas a usuarios externos, ya que ese trabajo seguiría sin resolverse en el sistema.

Usuarios con nivel de acceso de usuario externo:

* Solo puede ver documentos e informes de calendario que se han compartido con ellos
* Puede ver los usuarios que comparten documentos e informes de calendario con ellos
* Puede aprobar los documentos que se comparten con ellos

No puede modificar este nivel de acceso.

>[!IMPORTANT]
>
>Usuario externo solo está disponible si la opción &quot;Colaborar con personas sin cuentas de Workfront mediante el uso de su dirección de correo electrónico&quot; está activada en el área Preferencias del sistema en Configuración. Para obtener más información, consulte [Configurar las preferencias de seguridad del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Aunque esta configuración no está visible en el área Niveles de acceso del nivel de acceso Usuario externo, un usuario con este acceso tiene el siguiente acceso más alto a los tipos de objetos de Workfront:

| Tipo de objeto de Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto | ✓ |   |   |
| Tarea | ✓ | |   |
| Problema | ✓ |   |   |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes, paneles y calendarios |   | ✓ (Solo para informes de calendario; no se permite compartir informes) |   |
| Filtros, vistas y agrupaciones | ✓ |   |   |
| Documentos |   | ✓ (sin la capacidad de compartir documentos) |   |
| Usuarios |   | ✓ |   |
| Equipos |   | ✓ |   |
| Plantillas | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Workfront Goals | ✓ |   |   |
