---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,modelo,canal,diagrama,niveles,permisos
navigation-topic: access-levels
title: Niveles de acceso integrados en Adobe Workfront
description: Cada uno de los seis niveles de acceso integrados está diseñado para un tipo particular de usuario, que incluye Administrador del sistema, Planificador, Trabajador, Revisor, Solicitante y Usuario externo. Estos niveles de acceso le permiten controlar lo que los usuarios pueden editar y ver en el sistema. Si necesita un nivel de acceso personalizado, puede copiar el nivel de acceso integrado y determinar la cantidad de acceso que desea permitir para los distintos tipos de objetos de Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 6%

---

# Niveles de acceso integrados en Adobe Workfront

Cada uno de los seis niveles de acceso integrados está diseñado para un tipo particular de usuario:

* Administrador del sistema
* Planificador
* Trabajador
* Revisor
* Solicitante
* Usuario externo

Según el nivel de acceso, hay hasta 3 configuraciones disponibles para la mayoría de los tipos de objetos de Workfront:

<table style="table-layout:auto">
    <tr>
        <td>Editar</td>
        <td>Los usuarios pueden crear, editar, eliminar y compartir el objeto de Workfront</td>
    </tr>
    <tr>
        <td>Vista</td>
        <td>Los usuarios pueden revisar y compartir el objeto de Workfront</td>
    </tr>
    <tr>
        <td>Sin acceso</td>
        <td>Los usuarios no pueden acceder al objeto Workfront</td>
    </tr>
</table>

Si necesita un nivel de acceso personalizado de Planificador, Trabajador, Solicitante o Revisor, puede copiar el nivel de acceso integrado y determinar la cantidad de acceso que desea permitir para los distintos tipos de objetos de Workfront. Para obtener información sobre la creación de un nivel de acceso personalizado o la modificación de uno de los niveles de acceso integrados, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Se recomienda dejar los niveles de acceso integrados sin cambios para poder consultarlos después de configurar los usuarios.

Para obtener información general sobre estos niveles de acceso, consulte [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Nivel de acceso del administrador del sistema

Adjunto a la licencia de Plan, este nivel de acceso integrado está diseñado para un usuario que está a cargo de la administración del sistema Adobe Workfront. No puede modificar este nivel de acceso integrado.

Los usuarios con nivel de acceso de administrador del sistema pueden hacer todo lo posible dentro de Workfront. Pueden ver y editar todos los objetos e información de Workfront introducidos en Workfront por todos los demás usuarios.

También tienen acceso al área de configuración completa, donde pueden cambiar cualquier configuración a nivel del sistema. Y pueden acceder a todas las áreas del menú principal ![](assets/main-menu-icon.png).

Para obtener más información, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Nivel de acceso del planificador

Este nivel de acceso, también adjunto a la licencia del Plan, está diseñado para:

* Administradores de grupos, equipos, proyectos y recursos
* Cualquiera que sea responsable de planificar, crear y administrar tareas, proyectos, portafolios y programas
* Cualquier persona responsable de asignar trabajo (tareas y problemas) a otros usuarios
* Usuarios que crean informes y aprueban hojas de horas, elementos de trabajo y documentos
* Usuarios que necesitan acceder a todas las áreas del menú principal ![](assets/main-menu-icon.png)

Puede crear una versión personalizada del nivel de acceso integrado de Planificador y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Niveles de acceso integrados en Adobe Workfront](#Customiz) en este artículo.

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso del Planificador:

| Tipo de objeto Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyectos |   |   | ✓ |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   |   | ✓ |
| Programas |   |   | ✓ |
| Informes (incluidos tableros e informes de calendario) |   |   | ✓ |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Plantillas |   |   | ✓ |
| Datos financieros |   |   | ✓ |
| Administración de recursos |   |   | ✓ |
| Planificador de escenarios |   |   | ✓ (el valor predeterminado es Sin acceso). |
| Workfront Goals |   |   | ✓ (el valor predeterminado es Sin acceso). |

{style=&quot;table-layout:auto&quot;}

## Nivel de acceso del trabajador

Adjunto a la licencia de trabajo, este nivel de acceso integrado está diseñado para los usuarios que realizan el trabajo en Workfront. No planifican el trabajo; lo completan.

Usuarios con este nivel de acceso:

* Se asignan a elementos de trabajo donde pueden contribuir y registrar la hora
* Pueden aprobar trabajos y documentos, pero no hojas de horas
* Pueden acceder y compartir informes
* Pueden comunicarse con otros usuarios del sistema
* Puede acceder a todas las áreas del menú principal ![](assets/main-menu-icon.png), pero su área &quot;Usuarios&quot; se denomina Equipos. En el área Equipos, los usuarios con este nivel de acceso solo pueden ver los equipos a los que pertenecen, junto con el trabajo asignado a esos equipos.
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas ni informes.

Puede crear una versión personalizada del nivel de acceso integrado de Worker y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Niveles de acceso integrados en Adobe Workfront](#Customiz) en este artículo.

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso de trabajo:

| Tipo de objeto Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyectos |   |   | ✓ (Limitado: los usuarios solo pueden compartir el proyecto, crear tareas y problemas y editar los datos en formularios personalizados que ya estén adjuntos.) |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   | ✓ (el valor predeterminado es Sin acceso). |   |
| Programas |   | ✓ (el valor predeterminado es Sin acceso). |   |
| Informes (incluidos tableros e informes de calendario) |   | ✓ |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Plantillas | ✓ |   |   |
| Datos financieros |   | ✓ (el valor predeterminado es Sin acceso. La configuración Ver permite al usuario ver solo el área Finanzas de Detalles del proyecto). |   |
| Administración de recursos |   | ✓ |   |
| Planificador de escenarios |   |   | ✓ (el valor predeterminado es Sin acceso). |
| Workfront Goals |   |   | ✓ (el valor predeterminado es Sin acceso). |

{style=&quot;table-layout:auto&quot;}

## Nivel de acceso del revisor

Adjunto a la licencia de revisión, este nivel de acceso está diseñado para ejecutivos que soliciten trabajo a otros usuarios y que revisen y aprueben el trabajo. No son propietarios de proyectos ni miembros del equipo, pero necesitan acceder a Workfront para ver los elementos de trabajo que supervisan.

Por ejemplo, un interesado con este nivel de acceso podría iniciar sesión en Workfront para participar en una revisión en curso del material de marketing, ver actualizaciones del trabajo y revisar documentos, aprobaciones, informes y calendarios.

Usuarios con nivel de acceso de Revisor:

* No se pueden asignar elementos de trabajo ni aprobar hojas de tiempo
* Puede acceder a solicitudes y documentos en el menú principal ![](assets/main-menu-icon.png).
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas ni informes.

Puede crear una versión personalizada del nivel de acceso integrado de Revisor y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Niveles de acceso integrados en Adobe Workfront](#Customiz) en este artículo.

Más limitado para proyectos y tareas que el nivel de acceso del trabajador, los siguientes son los ajustes de acceso más altos disponibles para los objetos en el nivel de acceso del revisor:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto Workfront</th> 
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
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td> </td> 
   <td>✓ (el valor predeterminado es Sin acceso).</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Informes (incluidos tableros e informes de calendario)</td> 
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
   <td>Plantillas</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Datos financieros</td> 
   <td> </td> 
   <td> <p>✓ (el valor predeterminado es Sin acceso. La configuración Ver permite al usuario ver solo el área Finanzas de Detalles del proyecto).</p> </td> 
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
   <td>✓ (el valor predeterminado es Sin acceso).</td> 
  </tr> 
  <tr> 
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (el valor predeterminado es Sin acceso).</td> 
  </tr> 
 </tbody> 
</table>

## Nivel de acceso del solicitante

Este nivel de acceso integrado, adjunto a la licencia de Solicitud, está diseñado para usuarios que realizan y reciben solicitudes de trabajo sencillas en Workfront. De forma predeterminada, se limitan al área Solicitudes .

Por ejemplo, un usuario puede registrar problemas en la cola de solicitudes del servicio de asistencia al cliente de su organización.

Usuarios con este nivel de acceso integrado:

* Puede realizar solicitudes y actualizarlas
* Puede cargar y aprobar documentos
* Puede revisar el estado de los problemas que han presentado
* No se puede asignar a elementos de trabajo
* Solo se puede acceder a las solicitudes desde el menú principal ![](assets/main-menu-icon.png). Para obtener más información sobre las colas de solicitud, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Puede crear una versión personalizada del nivel de acceso integrado del solicitante y determinar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener más información, consulte [Niveles de acceso integrados en Adobe Workfront](#Customiz) en este artículo.

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso del solicitante:

| Tipo de objeto Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto |   | ✓ (solo la página Detalles del proyecto) |   |
| Tarea |   | ✓ (solo la página Detalles) |   |
| Problema |   |   | ✓ |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes (incluidos tableros e informes de calendario) |   | ✓ (solo la página Detalles) |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documento |   |   | ✓ |
| Usuario |   | ✓ |   |
| Plantilla | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Workfront Goals |   |   | ✓ (el valor predeterminado es Sin acceso). |

{style=&quot;table-layout:auto&quot;}

## Nivel de acceso de usuario externo

Este nivel de acceso no está adjunto a una licencia de Workfront de pago. Es el nivel de acceso más restrictivo, diseñado principalmente para colaboradores como consultores externos que no inician sesión en Workfront, pero que necesitan revisar, descargar o ver documentos ocasionalmente.

Los usuarios de Workfront pueden asignar tareas a usuarios externos aunque los usuarios externos no puedan iniciar sesión en el sistema. Sin embargo, aconsejamos que no se haga esto porque esa labor seguiría sin resolverse en el sistema.

Usuarios con nivel de acceso de usuario externo:

* Solo pueden ver documentos e informes de calendario que se han compartido con ellos
* Ver los usuarios que comparten documentos e informes de calendario con ellos
* Aprobar los documentos que se comparten con ellos

No puede modificar este nivel de acceso.

>[!IMPORTANT]
>
>El usuario externo solo está disponible si la opción &quot;Colaborar con personas sin cuentas de Workfront mediante su dirección de correo electrónico&quot; está habilitada en el área Preferencias del sistema de Configuración. Para obtener más información, consulte [Configuración de las preferencias de seguridad del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Las siguientes son las opciones de acceso más altas disponibles para objetos en el nivel de acceso de Usuario externo .

| Tipo de objeto Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto | ✓ |   |   |
| Tarea | ✓ | ✓ |   |
| Problema | ✓ |   |   |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes (incluidos tableros e informes de calendario) |   | ✓ (solo para informes de calendario) no se puede compartir informes) |   |
| Filtros, vistas y agrupaciones | ✓ |   |   |
| Documento |   | ✓ (sin la capacidad de compartir documentos) |   |
| Usuario |   | ✓ |   |
| Plantilla | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Workfront Goals | ✓ |   |   |
