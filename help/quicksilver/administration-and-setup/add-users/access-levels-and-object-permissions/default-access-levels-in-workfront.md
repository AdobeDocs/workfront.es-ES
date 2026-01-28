---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,modelo,canal,diagrama,niveles,permisos
navigation-topic: access-levels
title: Niveles de acceso integrados (heredados)
description: Cada uno de los seis niveles de acceso integrados actuales está diseñado para un tipo particular de usuario, incluidos administrador del sistema, planificador, trabajador, revisor, solicitante y usuario externo. Estos niveles de acceso le permiten controlar lo que los usuarios pueden editar y ver en el sistema. Si necesita un nivel de acceso personalizado, puede copiar un nivel de acceso integrado y modificarlo según la cantidad de acceso que desee que permita para los distintos tipos de objetos de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1656'
ht-degree: 84%

---

# Niveles de acceso integrados (heredados)

<!--Audited: 01/2024-->

>[!NOTE]
>
>La información de este artículo hace referencia a los niveles de acceso heredados. Para obtener información acerca de los niveles de acceso actuales, vea [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Cada uno de los seis niveles de acceso integrados actuales está diseñado para un tipo particular de usuario. Estos niveles de acceso le permiten controlar lo que los usuarios pueden editar y ver en el sistema.

Cada uno de los seis niveles de acceso integrados está diseñado para los siguientes tipos de usuarios:

* Administrador del sistema
* Planificador
* Trabajador
* Revisor
* Solicitante
* Usuario externo

Según el nivel de acceso, hay disponibles hasta tres configuraciones para la mayoría de los tipos de objetos de Workfront:

<table style="table-layout:auto">
    <tr>
        <td>Editar</td>
        <td>Los usuarios pueden crear, editar, eliminar y compartir el objeto de Workfront. </td>
    </tr>
    <tr>
        <td>Ver</td>
        <td>Los usuarios pueden revisar y compartir el objeto de Workfront</td>
    </tr>
    <tr>
        <td>Sin acceso</td>
        <td>Los usuarios no pueden acceder al objeto de Workfront</td>
    </tr>
</table>

Si necesita un nivel de acceso personalizado de planificador, trabajador, solicitante o revisor, puede copiar el nivel de acceso integrado y determinar la cantidad de acceso que desea que permita para los distintos tipos de objetos de Workfront.

>[!TIP]
>
>No puede modificar los niveles de acceso de administrador del sistema o usuario externo.

Para obtener información sobre cómo crear un nivel de acceso personalizado o modificar uno de los niveles de acceso integrados, consulte [Crear y modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que no modifique los niveles de acceso integrado para poder consultarlos después de configurar los usuarios.

Para obtener información general sobre estos niveles de acceso, consulte [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Nivel de acceso de administrador del sistema

Adjunto a la licencia de planificación, el nivel de acceso integrado de administrador del sistema está diseñado para un usuario a cargo de la administración del sistema de Adobe Workfront. Este nivel de acceso integrado no puede modificarse.

Los usuarios con nivel de acceso de administrador del sistema pueden hacer de todo en Workfront. Pueden ver y editar todos los objetos de Workfront y la información introducida en Workfront por todos los demás usuarios.

También tienen acceso completo al área de Configuración, donde pueden cambiar cualquier configuración a nivel de sistema. Y pueden acceder a todas las áreas del menú principal ![icono del menú principal](assets/main-menu-icon.png) o del menú principal ![icono del menú principal](assets/main-menu-icon.png), si están disponibles.

Para obtener más información, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Nivel de acceso de planificador

También adjuntado a la licencia de planificación, el nivel de acceso de planificador está diseñado para lo siguiente:

* Administradores de grupos, equipos, proyectos y recursos
* Cualquier usuario responsable de planificar, crear y administrar tareas, proyectos, portafolios y programas
* Cualquier persona responsable de asignar trabajo (tareas y problemas) a otros usuarios
* Usuarios que crean informes y aprueban hojas de horas, elementos de trabajo y documentos
* Usuarios que necesitan acceso a todas las áreas del menú principal ![icono del menú principal](assets/main-menu-icon.png) o del menú principal ![icono del menú principal](assets/main-menu-icon.png), si están disponibles

Puede crear una versión personalizada del nivel de acceso integrado de planificador y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

A continuación, se muestran las opciones de acceso más altas disponibles para los objetos en el nivel de acceso de planificador:

| Tipo de objeto de Workfront | Sin acceso | Acceso de visualización | Acceso de edición |
|---|---|---|---|
| Proyectos |   |   | ✓ |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   |   | ✓ |
| Programas |   |   | ✓ |
| Informes, paneles de control y calendarios |   |   | ✓ |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Equipos |   |   | ✓ |
| Plantillas |   |   | ✓ |
| Datos financieros |   |   | ✓ |
| Administración de recursos |   |   | ✓ |
| Planificador de escenarios |   |   | ✓ (La configuración predeterminada es Sin acceso). |
| Workfront Goals |   |   | ✓ (La configuración predeterminada es Sin acceso). |

{style="table-layout:auto"}

## Nivel de acceso de trabajador

Adjunto a la licencia de trabajo, el nivel de acceso de trabajador está diseñado para los usuarios que realizan el trabajo en Workfront. No planean el trabajo; lo completan.

Usuarios con este nivel de acceso:

* Están asignados a elementos de trabajo en los que pueden colaborar y registrar tiempo
* Pueden aprobar trabajos y documentos, pero no plantillas de horas
* Pueden acceder a informes y compartirlos
* Pueden comunicarse con otros usuarios del sistema
* No se puede acceder a todas las áreas del menú principal ![Icono del menú principal](assets/main-menu-icon.png) o del menú principal ![Icono del menú principal](assets/main-menu-icon.png), si están disponibles, y su área &quot;Usuarios&quot; se denomina Equipos. En el área Equipos, los usuarios con este nivel de acceso solo pueden ver los equipos a los que pertenecen, junto con el trabajo asignado a dichos equipos.
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas o informes.

Pueden crear una versión personalizada del nivel de acceso integrado de trabajador y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Creación y modificación de niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

A continuación se muestran las opciones de acceso más altas disponibles para los objetos en el nivel de acceso de trabajador:

| Tipo de objeto de Workfront | Sin acceso | Acceso de visualización | Acceso de edición |
|---|---|---|---|
| Proyectos |   |   | ✓ (Limitado: los usuarios solo pueden compartir el proyecto, crear tareas y problemas en él y editar datos en formularios personalizados que ya estén adjuntos a él). |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   | ✓ (La configuración predeterminada es Sin acceso). |   |
| Programas |   | ✓ (La configuración predeterminada es Sin acceso). |   |
| Informes, paneles de control y calendarios |   | ✓ |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Equipos |   |   | ✓ (acceso limitado) |
| Plantillas | ✓ |   |   |
| Datos financieros |   | ✓ (La configuración predeterminada es Sin acceso. La configuración Ver permite al usuario ver solo el área de Finanzas en Detalles del proyecto). |   |
| Administración de recursos |   | ✓ |   |
| Planificador de escenarios |   |   | ✓ (La configuración predeterminada es Sin acceso). |
| Workfront Goals |   |   | ✓ (La configuración predeterminada es Sin acceso). |

{style="table-layout:auto"}

## Nivel de acceso del revisor

Adjunto a la licencia de revisión, el nivel de acceso de revisor está diseñado para los ejecutivos que solicitan trabajo a otros usuarios y que revisan y aprueban el trabajo. No son propietarios del proyecto ni miembros del equipo, pero necesitan acceso a Workfront para ver los elementos de trabajo que supervisan.

Por ejemplo, una parte interesada con este nivel de acceso podría iniciar sesión en Workfront para participar en una revisión continua de los materiales de marketing, ver las actualizaciones de trabajo sobre el trabajo y revisar documentos, aprobaciones, informes y calendarios.

Usuarios con nivel de acceso de revisor:

* No se pueden asignar elementos de trabajo ni aprobar hojas de horas
* Puede acceder a las áreas Solicitudes y Documentos en el menú principal ![icono del menú principal](assets/main-menu-icon.png) o en el menú principal ![icono del menú principal](assets/main-menu-icon.png), si está disponible
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas o informes.

Puede crear una versión personalizada del nivel de acceso integrado de revisor y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Más limitada para los proyectos y tareas que el nivel de acceso de trabajador, la configuración de acceso más alta disponible para los objetos en el nivel de acceso de revisor es la siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto de Workfront</th> 
   <th>Sin acceso</th> 
   <th>Acceso de visualización</th> 
   <th>Acceso de edición</th> 
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
   <td>✓ (La configuración predeterminada es Sin acceso).</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td> </td> 
   <td>✓ (La configuración predeterminada es Sin acceso).</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Informes, paneles de control y calendarios</td> 
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
   <td> <p>✓ (La configuración predeterminada es Sin acceso. La configuración Ver permite al usuario ver solo el área de Finanzas en Detalles del proyecto.</p> </td> 
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
   <td>✓ (La configuración predeterminada es Sin acceso).</td> 
  </tr> 
  <tr> 
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (La configuración predeterminada es Sin acceso).</td> 
  </tr> 
 </tbody> 
</table>

## Nivel de acceso de solicitante

Adjuntado a la licencia de solicitud, el nivel de acceso de solicitante está diseñado para los usuarios que realizan y reciben solicitudes de trabajo sencillas en Workfront.  De forma predeterminada, se limitan al área de Solicitudes.

Por ejemplo, un usuario puede registrar problemas en la cola de solicitudes del servicio de asistencia de su organización.

Usuarios con este nivel de acceso:

* Puede realizar solicitudes y actualizarlas
* Puede cargar y aprobar documentos
* Puede revisar el estado de los problemas que han enviado
* No se puede asignar a elementos de trabajo
* Solo puede acceder a las solicitudes desde el área Solicitudes del menú principal ![icono del menú principal](assets/main-menu-icon.png) o el ![icono del menú principal](assets/main-menu-icon.png), si está disponible. Para obtener más información acerca de las colas de solicitudes, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Puede crear una versión personalizada del nivel de acceso integrado de solicitante y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso de solicitante:

| Tipo de objeto de Workfront | Sin acceso | Acceso de visualización | Acceso de edición |
|---|---|---|---|
| Proyecto |   | ✓ (solo la página de detalles del proyecto) |   |
| Tarea |   | ✓(solo la página Detalles de la tarea) |   |
| Problema |   |   | ✓ |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes, paneles de control y calendarios |   | ✓ |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuario |   | ✓ |   |
| Equipos |   | ✓ |   |
| Plantillas | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Workfront Goals |   |   | ✓ (La configuración predeterminada es Sin acceso). |

{style="table-layout:auto"}

## Nivel de acceso de usuario externo

El nivel de acceso del usuario externo no está asociado a una licencia de Workfront de pago. Es el nivel de acceso más restrictivo, diseñado principalmente para colaboradores como consultores externos que no inician sesión en Workfront, pero que necesitan revisar, descargar o ver documentos ocasionalmente.

Los usuarios de Workfront pueden asignar tareas a usuarios externos, aunque estos no puedan iniciar sesión en el sistema. Sin embargo, no se recomienda asignar tareas y problemas a usuarios externos, ya que ese trabajo seguiría sin resolverse en el sistema.

Usuarios con nivel de acceso de usuario externo:

* Solo pueden ver documentos e informes de calendario que se han compartido con ellos
* Pueden ver los usuarios que comparten documentos e informes de calendario con ellos
* Pueden aprobar los documentos que se comparten con ellos

No es posible modificar este nivel de acceso.

>[!IMPORTANT]
>
>El usuario externo solo está disponible si la opción “Colaborar con personas sin cuentas de Workfront mediante el uso de su dirección de correo electrónico” está habilitada en el área Preferencias del sistema en Configuración. Para obtener más información, consulte [Configurar las preferencias de seguridad del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Aunque esta configuración no está visible en el área de Niveles de acceso para el nivel de acceso del usuario externo, un usuario con este acceso tiene el siguiente acceso más alto a los tipos de objetos de Workfront:

| Tipo de objeto de Workfront | Sin acceso | Acceso de visualización | Acceso de edición |
|---|---|---|---|
| Proyecto | ✓ |   |   |
| Tarea | ✓ | |   |
| Problema | ✓ |   |   |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes, paneles de control y calendarios |   | ✓ (solo para informes de calendario; no se pueden compartir informes) |   |
| Filtros, vistas y agrupaciones | ✓ |   |   |
| Documentos |   | ✓ (sin la capacidad de compartir documentos) |   |
| Usuarios |   | ✓ |   |
| Equipos |   | ✓ |   |
| Plantillas | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Workfront Goals | ✓ |   |   |
