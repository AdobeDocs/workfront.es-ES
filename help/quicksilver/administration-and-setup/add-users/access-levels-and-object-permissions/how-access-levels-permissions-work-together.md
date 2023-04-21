---
title: Cómo funcionan juntos los niveles de acceso y los permisos
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,modelo,canal,diagrama,niveles,permisos
navigation-topic: access-levels
description: El administrador de Adobe Workfront determina el nivel de acceso que debe tener cada usuario. Ese nivel de acceso define lo que los usuarios pueden ver y hacer con los tipos de objetos y las áreas del sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 2%

---

# Cómo funcionan juntos los niveles de acceso y los permisos

El administrador de Adobe Workfront determina el nivel de acceso que debe tener cada usuario. Ese nivel de acceso define lo que los usuarios pueden ver y hacer con los tipos de objetos y las áreas del sistema.

Además, los usuarios obtienen acceso a objetos individuales cuando otros usuarios comparten y conceden determinados permisos sobre esos objetos.

Por lo tanto, las actividades que un usuario puede realizar con un objeto se definen mediante una combinación de su nivel de acceso y los permisos que se les otorgan para ese proyecto.

![](assets/security-model-hierachy.png)

Por ejemplo, si el nivel de acceso indica que puede crear tareas, pero los permisos que recibe en un proyecto específico no le permiten añadir tareas, no puede agregar tareas en el proyecto aunque pueda crear tareas en otro lugar de Workfront.

Este artículo explica cómo funciona esta combinación.

## Nivel de acceso

El nivel de acceso que un administrador de Workfront asigna a cada usuario es necesario para iniciar sesión en Workfront.

Los niveles de acceso predeterminados son:

* Administrador del sistema (adjunto a la licencia del Plan)
* Planificador (adjunto a la licencia del Plan)
* Trabajador (adjunto a la licencia de trabajo)
* Revisor (adjunto a la licencia de revisión)
* Solicitante (adjunto a la licencia de solicitud)
* Usuario externo (adjunto a la licencia de correo electrónico externo)

La licencia de Workfront para cada nivel de acceso predeterminado determina lo que está disponible y se puede configurar en el nivel de acceso. Para obtener información sobre las licencias de Workfront, consulte [Información general sobre las licencias de Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Para los usuarios asignados a él, un nivel de acceso define lo que pueden ver y hacer con los siguientes tipos de objetos y áreas en Workfront:

* Proyectos
* Tareas
* Problemas
* Portafolios
* Informes, tableros y calendarios
* Filtros, vistas y agrupamientos
* Documentos
* Otros usuarios
* Plantillas
* Datos financieros
* Administración de recursos
* Planificador de escenarios
* Workfront Goals

En un nivel de acceso personalizado, puede configurar las opciones de estos objetos y áreas para cambiar la cantidad de acceso que los usuarios tienen a ellos. Según la licencia asociada con el nivel de acceso, así como el tipo de objeto o área, puede configurar el nivel de acceso para que no permita acceso, acceso a la vista o acceso a la edición a un objeto o área.

>[!IMPORTANT]
>
>Se recomienda dejar los niveles de acceso integrados sin cambios para poder consultarlos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. (Puede hacerlo para todos los niveles de acceso excepto para el administrador del sistema y el usuario externo).

Para obtener una explicación detallada de cada uno de los niveles de acceso predeterminados, consulte [Niveles de acceso integrados en Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Para obtener instrucciones sobre la asignación de un nivel de acceso a un usuario, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Permisos

Al compartir un objeto con alguien del sistema, un usuario puede conceder al destinatario cualquiera de los siguientes permisos para el objeto.

* **Ver**: Este nivel de permiso permite que el destinatario comparta el objeto de una de las siguientes maneras:

   * Todo el sistema para que todos los usuarios puedan verlo (no disponible para todos los objetos)
   * Con usuarios externos que no tienen una licencia de Workfront (no disponible para todos los objetos)
   * Con una dirección de correo electrónico (solo disponible para documentos)

* **Contribute**: (no disponible para todos los objetos)
* **Administrar**: Cuando alguien comparte un objeto, los derechos del destinatario al objeto están determinados por una combinación del nivel de acceso del destinatario y los permisos al objeto que concedió el usuario que comparte. El menor grado de acceso disponible en esa combinación es el que determina lo que el destinatario puede hacer con el objeto.

   >[!INFO]
   >
   >**Ejemplo:** Si el nivel de acceso del destinatario no permite la edición de proyectos, esa persona no puede editar ni eliminar un proyecto aunque la persona que comparte haya concedido permisos para administrarlo.
   >
   >O bien, si el nivel de acceso del destinatario permite la edición del proyecto, pero el usuario que comparte solo concede permisos de visualización a un proyecto, el usuario no puede editar ni eliminar el proyecto.

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

>[!NOTE]
>
>* Si un usuario comparte un objeto con ciertos permisos y ese objeto tiene cualquier objeto secundario debajo de él, el destinatario hereda los mismos permisos para esos objetos secundarios.
>* Si un nivel de acceso impide que los usuarios eliminen determinados objetos, no impide que eliminen objetos secundarios contenidos en ellos.
>


## Más escenarios de ejemplo

Cuando Olivia comparte un proyecto de Workfront con Tony, el acceso de Tony a él está determinado por una combinación de dos cosas:

* Nivel de acceso de Tony, asignado por el administrador de Workfront
* Permisos de Tony para el proyecto, especificados por Olivia

Las acciones de Tony en el proyecto pueden ser restringidas aún más en el proyecto, pero no pueden ser ilimitadas más allá de lo que está permitido en su nivel de acceso:

* Si el nivel de acceso de Tony no le permite crear tareas, no puede agregar tareas al proyecto, aunque Olivia le haya dado permisos para agregarle tareas.
* Si el nivel de acceso de Tony le permite crear tareas, pero Olivia no otorgó permisos para agregar tareas al proyecto, no puede agregar tareas a ese proyecto, pero puede agregar tareas a otros proyectos donde se le han otorgado permisos para hacerlo.
