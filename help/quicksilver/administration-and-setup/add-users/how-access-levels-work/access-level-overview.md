---
title: Información general sobre los nuevos niveles de acceso
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,nivel,sistema,administrador,estándar,luz,colaborador
navigation-topic: access-levels
description: Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront. El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 4af7a72a3633f1b669cbc681f230727cc4f54d1e
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 4%

---

# Información general sobre los nuevos niveles de acceso

Como administrador de Adobe Workfront, se asigna un nivel de acceso a un usuario por 2 motivos:

* Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront.
* El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.

## Nuevos niveles de acceso integrados en Adobe Workfront {#built-in-access}

Workfront tiene 6 nuevos niveles de acceso integrados:

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
        <td>Vista</td>
        <td>Los usuarios pueden revisar y compartir el objeto de Workfront</td>
    </tr>
    <tr>
        <td>Sin acceso</td>
        <td>Los usuarios no pueden acceder al objeto Workfront</td>
    </tr>
</table>

Si necesita un nivel de acceso personalizado, puede copiar el nivel de acceso integrado y ajustar la cantidad de acceso que desee para permitir los distintos tipos de objetos de Workfront. Para obtener información sobre la creación de un nivel de acceso personalizado, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Se recomienda dejar los niveles de acceso integrados sin cambios para poder consultarlos después de configurar los usuarios.

### Nivel de acceso del administrador del sistema

Adjunto a la licencia Standard, este nivel de acceso integrado está diseñado para un usuario que esté a cargo de la administración del sistema Adobe Workfront. No puede modificar este nivel de acceso integrado.

Los usuarios con nivel de acceso de administrador del sistema pueden hacer todo lo posible dentro de Workfront. Pueden ver y editar todos los objetos e información de Workfront introducidos en Workfront por todos los demás usuarios.

También tienen acceso al área de configuración completa, donde pueden cambiar cualquier configuración a nivel de sistema, y pueden acceder a todas las áreas del menú principal.

Para obtener más información, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Nivel de acceso estándar

Este nivel de acceso, también adjunto a la licencia Standard, está diseñado para usuarios que:

* Planificar, crear y rastrear todos los proyectos en un solo lugar
* Automatizar procesos rutinarios
* Administrar recursos
* Seguimiento y colaboración en solicitudes
* Seguimiento e informe sobre las finanzas de los proyectos
* Activación de solicitudes de trabajo entrantes
* Colaborar en proyectos, tareas y problemas

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado estándar y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre la creación de un nivel de acceso personalizado, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso estándar:

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
| Tableros |   |   | ✓ |
| Página de inicio |   |   | ✓ |
| Metas |   |   | ✓ |

{style="table-layout:auto"}

### Nivel de acceso claro

Este nivel de acceso, adjunto a la licencia Light, está diseñado para los usuarios que:

* Ver todos los elementos y actualizaciones vinculados al trabajo
* Aprobar proyectos, tareas y problemas
* Ver tableros e informes
* Seguimiento del tiempo
* Crear y administrar problemas
* Hacer actualizaciones en el trabajo

Usuarios con nivel de acceso ligero:

* No se pueden asignar elementos de trabajo o aprobar hojas de horas
* Puede acceder a solicitudes y documentos en el menú principal.
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas ni informes.

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado Light y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre la creación de un nivel de acceso personalizado, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso ligero:

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
   <td>✓ (el valor predeterminado es Sin acceso).</td> 
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
   <td>✓</td> 
   <td> <p> </p> </td> 
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
   <td>Tableros </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
     <tr> 
   <td>Página de inicio </td> 
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

### Nivel de acceso del colaborador

Adjunto a la licencia de colaborador, este nivel de acceso está diseñado para los usuarios que:

* Enviar solicitudes
* Seguimiento de solicitudes
* Actualizar y revisar solicitudes.

Usuarios con este nivel de acceso integrado:

* Puede realizar solicitudes y actualizarlas
* Puede cargar y aprobar documentos
* Puede revisar el estado de los problemas que han presentado
* No se puede asignar a elementos de trabajo
* Solo puede acceder a las solicitudes desde el menú principal. Para obtener más información sobre las colas de solicitud, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado del colaborador y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre la creación de un nivel de acceso personalizado, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso del colaborador :

| Tipo de objeto Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto |   | ✓ (solo la página Detalles del proyecto) |   |
| Tarea |   | ✓ (solo la página Detalles) |   |
| Problema |   |   | ✓ |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes (incluidos tableros e informes de calendario) |   | ✓ (solo la ficha Detalles) |   |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documento |   |   | ✓ |
| Usuario |   | ✓ |   |
| Equipos |   | ✓ |   |
| Plantilla | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Tableros |   |   | ✓ (tarjetas simples) |
| Página de inicio |   | ✓ (Mis actualizaciones) |   |
| Metas |   |   | ✓ |

{style="table-layout:auto"}

### Nivel de acceso de usuario externo

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

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para objetos en el nivel de acceso de Usuario externo .

| Tipo de objeto Workfront | Sin acceso | Ver acceso | Editar acceso |
|---|---|---|---|
| Proyecto | ✓ |   |   |
| Tarea | ✓ |   |   |
| Problema | ✓ |   |   |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes (incluidos tableros e informes de calendario) |   | ✓ (solo para informes de calendario) no se puede compartir informes) |   |
| Filtros, vistas y agrupaciones | ✓ |   |   |
| Documento |   | ✓ (no es posible compartir documentos) |   |
| Usuario |   | ✓ |   |
| Equipos | ✓ |   |   |
| Plantilla | ✓ |   |   |
| Datos financieros | ✓ |   |   |
| Administración de recursos | ✓ |   |   |
| Planificador de escenarios | ✓ |   |   |
| Tableros | ✓ |   |   |
| Página de inicio | ✓ |   |   |
| Metas | ✓ |   |   |


## Cómo funcionan juntos los niveles de acceso y los permisos

Los niveles de acceso definen lo que los usuarios pueden ver y hacer con los tipos de objetos generales y las áreas del sistema, como proyectos, tareas y problemas. Los permisos definen a lo que tiene acceso en objetos específicos creados por otras personas del sistema, como un proyecto creado para ejecutar una campaña de marketing.

La siguiente tabla compara el acceso general de un usuario a objetos (definido por el nivel de acceso del usuario) con los permisos para un objeto compartido específico:

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
   <td> <p>Heredado de un objeto compartido de clasificación superior 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Las actividades que un usuario puede realizar con un objeto se definen mediante una combinación de su nivel de acceso y los permisos que se les otorgan.

![](assets/security-model-hierachy-copy.png)

### Conceder permisos mediante objetos de uso compartido

Los usuarios obtienen acceso a objetos individuales cuando otros usuarios comparten y conceden determinados permisos sobre esos objetos.

>[!NOTE]
>
>* Si un usuario comparte un objeto con ciertos permisos y ese objeto tiene cualquier objeto secundario debajo de él, el destinatario hereda los mismos permisos para esos objetos secundarios.
>* Si un nivel de acceso impide que los usuarios eliminen determinados objetos, no impide que eliminen objetos secundarios contenidos en ellos.


Un usuario puede conceder al destinatario cualquiera de los siguientes permisos para el objeto individual:

* **Ver**: Este nivel de permiso permite que el destinatario comparta el objeto de una de las siguientes maneras:

   * Todo el sistema para que todos los usuarios puedan verlo (no disponible para todos los objetos)
   * Con usuarios externos que no tienen una licencia de Workfront (no disponible para todos los objetos)
   * Con una dirección de correo electrónico (disponible solo para documentos y calendarios)

* **Contribute**: (no disponible para todos los objetos)
* **Administrar**: Cuando alguien comparte un objeto, los derechos del destinatario al objeto están determinados por una combinación del nivel de acceso del destinatario y los permisos al objeto que concedió el usuario que comparte. El menor grado de acceso disponible en esa combinación es el que determina lo que el destinatario puede hacer con el objeto.

### Situaciones de ejemplo

#### **Escenario 1**

Si el nivel de acceso del destinatario no permite la edición de proyectos, esa persona no puede editar ni eliminar un proyecto aunque la persona que comparte haya concedido permisos para administrarlo.

O bien, si el nivel de acceso del destinatario permite la edición del proyecto, pero el usuario que comparte solo concede permisos de visualización a un proyecto, el usuario no puede editar ni eliminar el proyecto.

#### **Escenario 2**

Cuando Olivia comparte un proyecto de Workfront con Tony, el acceso de Tony a él está determinado por una combinación de dos cosas:

* Nivel de acceso de Tony, asignado por el administrador de Workfront
* Permisos de Tony para el proyecto, especificados por Olivia

Las acciones de Tony en el proyecto pueden ser restringidas aún más en el proyecto, pero no pueden ser ilimitadas más allá de lo que está permitido en su nivel de acceso:

* Si el nivel de acceso de Tony no le permite crear tareas, no puede agregar tareas al proyecto, aunque Olivia le haya dado permisos para agregarle tareas.
* Si el nivel de acceso de Tony le permite crear tareas, pero Olivia no otorgó permisos para agregar tareas al proyecto, no puede agregar tareas a ese proyecto, pero puede agregar tareas a otros proyectos donde se le han otorgado permisos para hacerlo.
