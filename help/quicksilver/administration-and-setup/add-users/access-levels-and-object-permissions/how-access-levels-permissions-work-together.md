---
title: Cómo funcionan juntos los niveles de acceso y los permisos
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,modelo,canal,diagrama,niveles,permisos
navigation-topic: access-levels
description: El administrador de Adobe Workfront determina el nivel de acceso que debe tener cada usuario. Ese nivel de acceso define lo que los usuarios pueden ver y hacer con los tipos de objetos y las áreas del sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 51%

---

# Funcionamiento conjunto de los niveles de acceso y los permisos

>[!NOTE]
>
>La información de este artículo hace referencia a los niveles de acceso heredados. Para obtener información acerca de los niveles de acceso actuales, vea [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

El administrador de Adobe Workfront determina el nivel de acceso que debe tener cada usuario. Ese nivel de acceso define lo que los usuarios pueden ver y hacer con los tipos de objetos y las áreas del sistema.

Los usuarios también obtienen acceso a objetos individuales cuando otros usuarios comparten y conceden determinados permisos sobre esos objetos.


![Jerarquía del modelo de seguridad](assets/security-model-hierachy.png)

Por ejemplo, si el nivel de acceso indica que puede crear tareas, pero los permisos que recibe en un proyecto específico no le permiten agregarle tareas, no puede agregar tareas en el proyecto aunque pueda crear tareas en cualquier otra parte de Workfront.

Este artículo explica cómo funciona esta combinación.

## Nivel de acceso

El nivel de acceso asignado a cada usuario por un administrador de Workfront es necesario para iniciar sesión en Workfront.

Los niveles de acceso predeterminados son:

* Administrador del sistema (adjunto a la licencia de planificación)
* Planificador (adjunto a la licencia de planificación)
* Trabajador (adjunto a la licencia de trabajo)
* Revisor (adjunto a la licencia de revisión)
* Solicitante (adjunto a la licencia de solicitud)
* Usuario externo (adjunto a la licencia de correo electrónico externo)

La licencia de Workfront para cada nivel de acceso predeterminado determina qué está disponible y qué se puede configurar en el nivel de acceso. Para obtener información sobre las licencias de Workfront, consulte [Descripción general de las licencias de Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Para los usuarios asignados a él, un nivel de acceso define lo que pueden ver y hacer con los siguientes tipos de objetos y áreas en Workfront:

* Proyectos
* Tareas
* Problemas
* Portafolios
* Informes, paneles de control y calendarios
* Filtros, vistas y agrupaciones
* Documentos
* Otros usuarios
* Plantillas
* Datos financieros
* Administración de recursos
* Planificador de escenarios
* Workfront Goals

En un nivel de acceso personalizado, puede establecer la configuración de estos objetos y áreas para cambiar el nivel de acceso que tienen los usuarios a ellos. Según la licencia asociada al nivel de acceso, así como el tipo de objeto o área, puede configurar el nivel de acceso para que no permita el acceso, el acceso de visualización o el acceso de edición a un objeto o área.

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que no modifique los niveles de acceso integrado para poder consultarlos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. (Puede hacerlo para todos los niveles de acceso, excepto para el Administrador del sistema y el Usuario externo).

Para obtener una explicación detallada de cada uno de los niveles de acceso predeterminados, vea [Niveles de acceso integrados](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Para obtener instrucciones sobre cómo asignar un nivel de acceso a un usuario, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Permisos

Al compartir un objeto con alguien en el sistema, un usuario puede otorgar al destinatario cualquiera de los siguientes permisos para el objeto.

* **Visualización**: este nivel de permiso permite al destinatario compartir el objeto de una de las siguientes maneras:

   * En todo el sistema para que todos los usuarios puedan verlo (no disponible para todos los objetos)
   * Con usuarios externos sin licencia de Workfront (no disponible para todos los objetos)
   * Con una dirección de correo electrónico (disponible solo para documentos)

* **Contribución**: (no disponible para todos los objetos)
* **Administración**: cuando alguien comparte un objeto, los derechos del destinatario sobre el objeto están determinados por una combinación del nivel de acceso del destinatario y los permisos para el objeto que concedió el que comparte. El grado más bajo de acceso disponible en esa combinación es lo que determina lo que el destinatario puede hacer con el objeto.

  >[!INFO]
  >
  >**Ejemplo:** Si el nivel de acceso del destinatario no permite la edición del proyecto, esa persona no podrá editar ni eliminar un proyecto aunque el que comparte haya concedido permisos para administrarlo.
  >
  >O bien, si el nivel de acceso del destinatario permite la edición del proyecto, pero el usuario que comparte ha concedido permisos de solo visualización a un proyecto, el usuario no puede editar ni eliminar el proyecto.

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

>[!NOTE]
>
>* Si un usuario comparte un objeto con ciertos permisos y ese objeto tiene objetos secundarios debajo, el destinatario hereda los mismos permisos para esos objetos secundarios.
>* Si un nivel de acceso restringe a los usuarios de eliminar ciertos objetos, esto no impide que eliminen objetos secundarios contenidos en esos objetos.
>

## Más escenarios de ejemplo

Cuando Olivia comparte un proyecto de Workfront con Tony, el acceso de Tony a este está determinado por una combinación de dos cosas:

* Nivel de acceso de Tony, asignado por el administrador de Workfront
* Los permisos de Tony para el proyecto, especificados por Olivia

Las acciones de Tony en el proyecto pueden restringirse aún más en el proyecto, pero no pueden ser ilimitadas más allá de lo permitido en su nivel de acceso:

* Si el nivel de acceso de Tony no le permite crear tareas, no puede añadir tareas al proyecto , incluso si Olivia le dio permisos para añadir tareas.
* Si el nivel de acceso de Tony le permite crear tareas, pero Olivia no concedió permisos para añadir tareas al proyecto, no puede añadir tareas a ese proyecto, pero puede añadir tareas a otros proyectos en los que se le han concedido permisos para hacerlo.
