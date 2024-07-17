---
title: Información general sobre nuevos niveles de acceso
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso, nivel, sistema, administrador, estándar, ligero, colaborador
navigation-topic: access-levels
description: Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront. El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 2da3c687b33d808ec4bf19d380bc82759d19bf99
workflow-type: tm+mt
source-wordcount: '1702'
ht-degree: 5%

---

# Información general sobre nuevos niveles de acceso

Como administrador de Adobe Workfront, asigna un nivel de acceso a un usuario para dos fines:

* Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront.
* El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.

## Nuevos niveles de acceso integrados en Adobe Workfront {#built-in-access}

Workfront tiene 5 nuevos niveles de acceso integrados:

* Administrador del sistema
* Estándar
* Ligero
* Colaborador
* Externo

Según el nivel de acceso, hay disponibles hasta 3 permisos para la mayoría de los tipos de objetos de Workfront:

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

Si necesita un nivel de acceso personalizado, puede copiar el nivel de acceso integrado y ajustar la cantidad de acceso que desea que permita para los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que deje los niveles de acceso integrados sin cambios para que pueda hacer referencia a ellos después de configurar los usuarios.

### Nivel de acceso del administrador del sistema

Adjuntado a la licencia estándar, este nivel de acceso integrado está diseñado para un usuario que esté a cargo de la administración del sistema de Adobe Workfront. No puede modificar este nivel de acceso integrado.

Los usuarios con nivel de acceso de administrador del sistema pueden hacer de todo dentro de Workfront. Pueden ver y editar todos los objetos de Workfront y la información introducida en Workfront por todos los demás usuarios.

También tienen acceso al área de Configuración completa, donde pueden cambiar cualquier ajuste a nivel del sistema, y pueden acceder a todas las áreas en el menú principal.

Para obtener más información, consulte [Conceder acceso administrativo completo a un usuario](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Nivel de acceso estándar

Este nivel de acceso, que también se adjunta a la licencia estándar, está diseñado para los usuarios que:

* Planifique, cree y rastree todos los proyectos en un solo lugar
* Automatización de procesos rutinarios
* Administración de recursos
* Seguimiento y colaboración en solicitudes
* Seguimiento e informes sobre las finanzas del proyecto
* Solicitudes de trabajo entrantes de inicio
* Colaborar en proyectos, tareas y problemas

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado Estándar y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para los objetos del nivel de acceso Estándar:

| Tipo de objeto de Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyectos |   |   | ✓ |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   |   | ✓ |
| Programas |   |   | ✓ |
| Informes (incluidos informes de tableros y calendarios) |   |   | ✓ |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Plantillas |   |   | ✓ |
| Datos financieros |   |   | ✓ |
| Administración de recursos |   |   | ✓ |
| Planificador de escenarios |   |   | ✓ (La configuración predeterminada es Sin acceso.) |
| Tableros |   |   | ✓ |
| Inicio |   |   | ✓ |
| Metas |   |   | ✓ |

{style="table-layout:auto"}

### Nivel de acceso ligero

Adjuntado a la licencia básica, este nivel de acceso está diseñado para los usuarios que:

* Ver todos los elementos y actualizaciones vinculados al trabajo
* Aprobar proyectos, tareas y problemas
* Ver paneles e informes
* Rastrear horas y aprobar hojas de horas
* Crear y administrar problemas
* Actualizar el trabajo

Usuarios con el nivel de acceso Ligero:

* Se pueden asignar elementos de trabajo pero no se pueden completar.
* Puede acceder a solicitudes y documentos en el menú principal.
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas o informes.

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado Ligero y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

Los siguientes son los ajustes de acceso más altos disponibles para los objetos del nivel de acceso Claro:

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
   <td>Informes (incluidos informes de tableros y calendarios)</td> 
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
   <td></td> 
   <td> <p>✓</p> </td> 
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
   <td>Tableros </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
     <tr> 
   <td>Inicio </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr>   
   <td>Metas </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
 </tbody> 
</table>

### Nivel de acceso de colaborador

Adjuntado a la licencia de colaborador, este nivel de acceso está diseñado para los usuarios que:

* Envío de solicitudes
* Seguimiento de solicitudes
* Actualizar y revisar solicitudes
* Aprobar solicitudes

Usuarios con este nivel de acceso integrado:

* Puede realizar solicitudes y actualizarlas
* Puede cargar y aprobar documentos
* Puede aprobar proyectos, tareas y problemas
* Puede revisar el estado de los problemas que han enviado
* Se puede asignar a elementos de trabajo pero no se pueden completar
* Solo puede acceder a las solicitudes desde el menú principal. Para obtener más información acerca de las colas de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado Colaborador y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

A continuación se muestran las opciones de acceso más altas disponibles para los objetos del nivel de acceso Colaborador:

| Tipo de objeto de Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto |   | ✓ |   |
| Tarea |   | ✓ |   |
| Problema |   |   | ✓ |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes (incluidos informes de tableros y calendarios) |   | ✓ (Solo la pestaña Detalles) |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documento |   |   | ✓ |
| Usuario |   | ✓ |   |
| Equipos |   | ✓ |   |
| Plantilla | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Tableros |   |   | ✓ (Tarjetas simples) |
| Inicio |   | ✓ (Mis actualizaciones) |   |
| Metas |   |   | ✓ |

{style="table-layout:auto"}

### Nivel de acceso de usuario externo

Este nivel de acceso no está adjunto a una licencia de Workfront de pago. Es el nivel de acceso más restrictivo, diseñado principalmente para colaboradores como consultores externos que no inician sesión en Workfront, pero que necesitan revisar, descargar o ver documentos ocasionalmente.

Los usuarios de Workfront pueden asignar tareas a usuarios externos aunque estos no puedan iniciar sesión en el sistema. Pero aconsejamos que no se haga porque ese trabajo seguiría sin resolverse en el sistema.

Usuarios con nivel de acceso de usuario externo:

* Solo puede ver documentos e informes de calendario que se han compartido con ellos
* Vea los usuarios que comparten documentos e informes de calendario con ellos
* Aprobar los documentos que se comparten con ellos

No puede modificar este nivel de acceso.

>[!IMPORTANT]
>
>Usuario externo solo está disponible si la opción &quot;Colaborar con personas sin cuentas de Workfront mediante el uso de su dirección de correo electrónico&quot; está activada en el área Preferencias del sistema en Configuración. Para obtener más información, consulte [Configurar las preferencias de seguridad del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso Usuario externo.

| Tipo de objeto de Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto | ✓ |   |   |
| Tarea | ✓ |   |   |
| Problema | ✓ |   |   |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes (incluidos informes de tableros y calendarios) |   | ✓ (Solo para informes de calendario; no se permite compartir informes) |   |
| Filtros, vistas y agrupaciones | ✓ |   |   |
| Documento |   | ✓ (No es posible compartir documentos) |   |
| Usuario |   | ✓ |   |
| Equipos | ✓ |   |   |
| Plantilla | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Tableros | ✓ |   |   |
| Inicio | ✓ |   |   |
| Metas | ✓ |   |   |


## Cómo funcionan juntos los niveles de acceso y los permisos

Los niveles de acceso definen lo que los usuarios pueden ver y hacer con los tipos de objetos y áreas generales del sistema, como proyectos, tareas y problemas. Los permisos definen a qué tiene acceso sobre objetos específicos creados por otras personas en el sistema, como un proyecto creado para ejecutar una campaña de marketing.

En la tabla siguiente se compara el acceso general de un usuario a los objetos (definido por su nivel de acceso) con los permisos de un objeto compartido específico:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Nivel de acceso </th> 
   <th>Permisos </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Concedido por un administrador de Workfront en el nivel de acceso de un usuario</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Concedido por un usuario que comparte un objeto en el nivel de objeto</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Heredado de un objeto compartido de mayor clasificación 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Las actividades que un usuario puede realizar con un objeto se definen mediante una combinación de su nivel de acceso y los permisos que se les otorgan.

![](assets/security-model-hierachy-copy.png)

### Conceder permisos mediante el uso compartido de objetos

Los usuarios obtienen acceso a objetos individuales cuando otros usuarios comparten y conceden determinados permisos sobre dichos objetos.

>[!NOTE]
>
>* Si un usuario comparte un objeto con ciertos permisos y ese objeto tiene objetos secundarios debajo, el destinatario hereda los mismos permisos para esos objetos secundarios.
>* Si un nivel de acceso restringe a los usuarios de eliminar ciertos objetos, esto no impide que eliminen objetos secundarios contenidos en esos objetos.

Un usuario puede conceder al destinatario cualquiera de los siguientes permisos al objeto individual:

* **Vista**: este nivel de permiso permite al destinatario compartir el objeto de una de las siguientes maneras:

   * En todo el sistema para que todos los usuarios puedan verlo (no disponible para todos los objetos)
   * Con usuarios externos sin licencia de Workfront (no disponible para todos los objetos)
   * Con una dirección de correo electrónico (disponible solo para documentos y calendarios)

* **Contribute**: (no disponible para todos los objetos)
* **Administrar**: cuando alguien comparte un objeto, los derechos del destinatario sobre el objeto están determinados por una combinación del nivel de acceso del destinatario y los permisos para el objeto que concedió el que comparte. El grado más bajo de acceso disponible en esa combinación es lo que determina lo que el destinatario puede hacer con el objeto.

### Casos de ejemplo

#### **Escenario 1**

Si el nivel de acceso del destinatario no permite la edición del proyecto, esa persona no puede editar ni eliminar un proyecto aunque el usuario que comparte haya concedido permisos para administrarlo.

O bien, si el nivel de acceso del destinatario permite la edición del proyecto, pero el usuario que comparte ha concedido permisos de solo vista a un proyecto, el usuario no puede editar ni eliminar el proyecto.

#### **Escenario 2**

Cuando Olivia comparte un proyecto de Workfront con Tony, el acceso de Tony a él está determinado por una combinación de dos cosas:

* Nivel de acceso de Tony, asignado por el administrador de Workfront
* Los permisos de Tony para el proyecto, especificados por Olivia

Las acciones de Tony en el proyecto pueden restringirse aún más en el proyecto, pero no pueden ser ilimitadas más allá de lo permitido en su nivel de acceso:

* Si el nivel de acceso de Tony no le permite crear tareas, no puede agregar tareas al proyecto , incluso si Olivia le dio permisos para agregarle tareas.
* Si el nivel de acceso de Tony le permite crear tareas, pero Olivia no concedió permisos para agregar tareas al proyecto, no puede agregar tareas a ese proyecto, pero puede agregar tareas a otros proyectos en los que se le han concedido permisos para hacerlo.
