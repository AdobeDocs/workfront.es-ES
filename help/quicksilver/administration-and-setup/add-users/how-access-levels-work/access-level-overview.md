---
title: Información general sobre nuevos niveles de acceso
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso, nivel, sistema, administrador, estándar, light, colaborador
navigation-topic: access-levels
description: Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront. El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: dcc4657d4af4edbbe7971acd385a67b2ad50a058
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 98%

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

Si necesita un nivel de acceso personalizado, puede copiar el nivel de acceso integrado y ajustar la cantidad de acceso que desee que permita para los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, consulte [Creación o modificación de niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que no modifique los niveles de acceso integrado para poder consultarlos después de configurar los usuarios.

### Nivel de acceso de administrador del sistema

Adjunto a la licencia estándar, este nivel de acceso integrado está diseñado para un usuario a cargo de la administración del sistema de Adobe Workfront. Este nivel de acceso integrado no puede modificarse.

Los usuarios con nivel de acceso de administrador del sistema pueden hacer de todo dentro de Workfront. Pueden ver y editar todos los objetos de Workfront y la información introducida en Workfront por todos los demás usuarios.

También tienen acceso a todo el área de Configuración, donde pueden cambiar cualquier ajuste en el nivel del sistema, y pueden acceder a todas las áreas en el menú principal.

Para obtener más información, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Nivel de acceso estándar

Este nivel de acceso, que también se adjunta a la licencia estándar, está diseñado para los usuarios que:

* Planifican, crean y llevan el seguimiento de todos los proyectos en un solo lugar
* Automatizan los procesos rutinarios
* Administran los recursos
* Llevan el seguimiento y colaboran en las solicitudes
* Llevan el seguimiento y crean informes sobre las finanzas del proyecto
* Inician las solicitudes de trabajo entrantes
* Colaboran en proyectos, tareas y problemas

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado estándar y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, consulte [Creación o modificación de niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para los objetos del nivel de acceso estándar:

| Tipo de objeto de Workfront | Sin acceso | Acceso de visualización | Acceso de edición |
|---|---|---|---|
| Proyectos |   |   | ✓ |
| Tareas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portafolios |   |   | ✓ |
| Programas |   |   | ✓ |
| Informes (incluidos informes de paneles de control y calendarios) |   |   | ✓ |
| Filtros, vistas y agrupaciones |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuarios |   |   | ✓ |
| Plantillas |   |   | ✓ |
| Datos financieros |   |   | ✓ |
| Administración de recursos |   |   | ✓ |
| Planificador de escenarios |   |   | ✓ (La configuración predeterminada es Sin acceso). |
| Tableros |   |   | ✓ |
| Inicio |   |   | ✓ |
| Metas |   |   | ✓ |

{style="table-layout:auto"}

### Nivel de acceso Light

Adjuntado a la licencia básica, este nivel de acceso está diseñado para los usuarios que:

* Ven todos los elementos y actualizaciones vinculados al trabajo
* Aprueban proyectos, tareas y problemas
* Ven paneles de control e informes
* Rastree el tiempo en las tareas y los problemas y apruebe las hojas de horas
* Crean y administran problemas

Usuarios con el nivel de acceso Light:

* Se pueden asignar elementos de trabajo pero no se pueden completar.
* Puede acceder a solicitudes y documentos en el menú principal.
* Tienen una capacidad limitada para crear objetos: no pueden crear proyectos, portafolios, programas o informes.

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado Light y ajustar la cantidad de acceso que se permiten en los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

Los siguientes son los ajustes de acceso más altos disponibles para los objetos del nivel de acceso Light:

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
   <td>Informes (incluidos informes de paneles de control y calendarios)</td> 
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
   <td>✓ (La configuración predeterminada es Sin acceso).</td> 
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

Adjunto a la licencia de colaborador, este nivel de acceso está diseñado para los usuarios que:

* Envían solicitudes
* Llevan el seguimiento de solicitudes
* Actualizan y revisan solicitudes
* Aprueban solicitudes

Los usuarios con este nivel de acceso integrado:

* Puede realizar solicitudes y actualizarlas
* Puede cargar y aprobar documentos
* Pueden aprobar proyectos, tareas y problemas
* Puede revisar el estado de los problemas que han enviado
* Pueden ser asignados a elementos de trabajo pero no pueden completarlos
* Solo pueden acceder a las solicitudes desde el menú principal. Para obtener más información acerca de las colas de solicitudes, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Puede crear una versión personalizada del nivel de acceso integrado colaborador y ajustar la cantidad de acceso que permite para los distintos tipos de objetos de Workfront. Para obtener información sobre cómo crear un nivel de acceso personalizado, consulte [Creación o modificación de niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalles de acceso**

A continuación se muestran las opciones de acceso más altas disponibles para los objetos del nivel de acceso colaborador:

| Tipo de objeto de Workfront | Sin acceso | Acceso de visualización | Acceso de edición |
|---|---|---|---|
| Proyecto |   | ✓ |   |
| Tarea |   | ✓ |   |
| Problema |   |   | ✓ |
| Portafolios |   | ✓ |   |
| Programas |   | ✓ |   |
| Informes (incluidos informes de paneles de control y calendarios) |   | ✓ (solo la pestaña Detalles) |   |
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

>[!IMPORTANT]
>
>A partir de la versión 24.7, los colaboradores tienen acceso de visualización a programas y portafolios de forma predeterminada.
>
> 
>Los colaboradores incorporados antes de la versión 24.7 seguirán sin tener acceso a los programas y los portafolios de forma predeterminada. Puede actualizar su acceso para verlos manualmente si es necesario.

### Nivel de acceso de usuario externo

Este nivel de acceso no está adjunto a una licencia de Workfront de pago. Es el nivel de acceso más restrictivo, diseñado principalmente para colaboradores como consultores externos que no inician sesión en Workfront, pero que necesitan revisar, descargar o ver documentos ocasionalmente.

Usuarios con nivel de acceso de usuario externo:

* Solo pueden ver documentos e informes de calendario que se han compartido con ellos
* Vea los usuarios que comparten documentos e informes de calendario con ellos
* Aprobar los documentos que se comparten con ellos

No se pueden asignar usuarios externos a elementos de trabajo.

No es posible modificar este nivel de acceso.

>[!IMPORTANT]
>
>El usuario externo solo está disponible si la opción “Colaborar con personas sin cuentas de Workfront mediante el uso de su dirección de correo electrónico” está activada en el área Preferencias del sistema en Configuración. Para obtener más información, consulte [Configurar las preferencias de seguridad del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Detalles de acceso**

Las siguientes son las opciones de acceso más altas disponibles para los objetos en el nivel de acceso de usuario externo.

| Tipo de objeto de Workfront | Sin acceso | Acceso de visualización | Acceso de edición |
|---|---|---|---|
| Proyecto | ✓ |   |   |
| Tarea | ✓ |   |   |
| Problema | ✓ |   |   |
| Portafolios | ✓ |   |   |
| Programas | ✓ |   |   |
| Informes (incluidos informes de paneles de control y calendarios) |   | ✓ (Solo para informes de calendario; no se permite compartir informes) |   |
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


## Funcionamiento conjunto de los niveles de acceso y los permisos

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

![Jerarquía del modelo de seguridad](assets/security-model-hierachy-copy.png)

### Conceder permisos mediante el uso compartido de objetos

Los usuarios obtienen acceso a objetos individuales cuando otros usuarios comparten y conceden determinados permisos sobre dichos objetos.

>[!NOTE]
>
>* Si un usuario comparte un objeto con ciertos permisos y ese objeto tiene objetos secundarios debajo, el destinatario hereda los mismos permisos para esos objetos secundarios.
>* Si un nivel de acceso restringe a los usuarios de eliminar ciertos objetos, esto no impide que eliminen objetos secundarios contenidos en esos objetos.

Un usuario puede conceder al destinatario cualquiera de los siguientes permisos al objeto individual:

* **Visualización**: este nivel de permiso permite al destinatario compartir el objeto de una de las siguientes maneras:

   * En todo el sistema para que todos los usuarios puedan verlo (no disponible para todos los objetos)
   * Con usuarios externos sin licencia de Workfront (no disponible para todos los objetos)
   * Con una dirección de correo electrónico (disponible solo para documentos y calendarios)

* **Contribución**: (no disponible para todos los objetos)
* **Administración**: cuando alguien comparte un objeto, los derechos del destinatario sobre el objeto están determinados por una combinación del nivel de acceso del destinatario y los permisos para el objeto que concedió el que comparte. El grado más bajo de acceso disponible en esa combinación es lo que determina lo que el destinatario puede hacer con el objeto.

### Escenarios de ejemplo

#### **Escenario 1**

Si el nivel de acceso del destinatario no permite la edición del proyecto, esa persona no puede editar ni eliminar un proyecto aunque el usuario que comparte haya concedido permisos para administrarlo.

O bien, si el nivel de acceso del destinatario permite la edición del proyecto, pero el usuario que comparte ha concedido permisos de solo visualización a un proyecto, el usuario no puede editar ni eliminar el proyecto.

#### **Escenario 2**

Cuando Olivia comparte un proyecto de Workfront con Tony, el acceso de Tony a este está determinado por una combinación de dos cosas:

* Nivel de acceso de Tony, asignado por el administrador de Workfront
* Los permisos de Tony para el proyecto, especificados por Olivia

Las acciones de Tony en el proyecto pueden restringirse aún más en el proyecto, pero no pueden ser ilimitadas más allá de lo permitido en su nivel de acceso:

* Si el nivel de acceso de Tony no le permite crear tareas, no puede añadir tareas al proyecto , incluso si Olivia le dio permisos para añadir tareas.
* Si el nivel de acceso de Tony le permite crear tareas, pero Olivia no concedió permisos para añadir tareas al proyecto, no puede añadir tareas a ese proyecto, pero puede añadir tareas a otros proyectos en los que se le han concedido permisos para hacerlo.
