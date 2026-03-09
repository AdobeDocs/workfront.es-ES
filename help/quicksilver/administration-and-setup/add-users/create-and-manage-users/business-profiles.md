---
title: Información general de perfiles empresariales
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: Los perfiles empresariales son un modelo de permisos mejorado que permite a clientes como las agencias administrar de forma eficaz el acceso de los usuarios y garantizar un control preciso de los permisos en el nivel de grupo. En un perfil empresarial, los usuarios tienen permisos distintos para objetos específicos del grupo. Los objetos adicionales también se pueden compartir directamente con el perfil empresarial.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
exl-id: 7f62de33-e544-4be9-8dcf-03a2e09e8a05
source-git-commit: 1389c6a1f41a14bafd6b70e2e079e40d22d47b07
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 1%

---

# Resumen de perfiles empresariales

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para clientes específicos.</span>

Los perfiles empresariales son un modelo de permisos mejorado que permite a clientes como las agencias administrar de forma eficaz el acceso de los usuarios y garantizar un control preciso de los permisos en el nivel de grupo. En un perfil empresarial, los usuarios tienen permisos distintos para objetos específicos del grupo. Los objetos adicionales también se pueden compartir directamente con el perfil empresarial.

Un perfil de negocio de un usuario es similar a un usuario con una función específica en un grupo, como un controlador financiero o un administrador de proyectos, y que recibe los permisos que van junto con esa función para el grupo especificado. El perfil empresarial puede ser temporal, lo que permite los permisos durante un período de tiempo que está establecido para caducar y mantener las restricciones de datos para el grupo o la agencia.

El administrador del sistema de Workfront:

* Crea los niveles de acceso y define los campos restringidos según sea necesario
* Actualiza el perfil de usuario con el grupo y el nivel de acceso para ese grupo (este es el perfil empresarial)
* Define fechas en vigor para el perfil comercial según sea necesario
* Asigna plantillas de diseño a los niveles de acceso

Cualquier usuario que tenga acceso para compartir objetos puede compartirlos con el perfil empresarial, y todos los usuarios con el perfil verán el objeto.

## Ejemplo de perfil empresarial

>[!BEGINSHADEBOX]

Sam necesita un acceso diferente a los proyectos para la Agencia A y la Agencia B. Ambas agencias se configuran como grupos en Workfront. (Para obtener información sobre los grupos, consulte Información general de grupos.)

Para la Agencia A, Sam actúa como controlador financiero y necesita acceso para ver todos los campos financieros de sus proyectos. Para la Agencia B, Sam actúa como gestor de proyectos y debe gestionar las tareas y los problemas, pero no debe poder ver la información financiera.

El administrador del sistema de Workfront crea nuevos niveles de acceso denominados Controlador financiero y Administrador de proyectos. Estos niveles de acceso tienen el acceso correcto para los datos financieros. A continuación, el administrador abre el perfil de usuario de Sam y selecciona &quot;Agencia A&quot; como grupo con el nivel de acceso &quot;Controlador financiero&quot; para crear el primer perfil empresarial y &quot;Agencia B&quot; como grupo con el nivel de acceso &quot;Administrador de proyectos&quot; para crear el segundo perfil empresarial.

Una vez configurados los perfiles empresariales, cuando Sam vaya a la lista de proyectos, aparecerán todos los proyectos para la Agencia A y la Agencia B (junto con cualquier otro proyecto que Sam haya creado o al que se le hayan concedido permisos). Los campos financieros de los proyectos de la Agencia A son visibles para Sam tanto en la vista de lista como en los detalles del proyecto, pero los campos financieros de los proyectos de la Agencia B están ocultos. Los nombres de campo aparecen, pero los datos de campo están en blanco.

Si otros usuarios de cualquiera de las agencias comparten proyectos con el &quot;Controlador financiero - Agencia A&quot; o el &quot;Gerente de proyecto - Agencia B&quot; perfiles de negocio, entonces esos proyectos son visibles para Sam. Los campos financieros de los proyectos de la Agencia B permanecerán siempre ocultos porque así se define en el nivel de acceso.

>[!ENDSHADEBOX]

## Definición de los perfiles empresariales

El administrador del sistema de Adobe Workfront es responsable de definir todas las áreas de un perfil empresarial.

### Crear nivel de acceso

El administrador del sistema de Workfront crea el nivel de acceso con el acceso necesario y define los campos restringidos según sea necesario.

Para obtener más información, consulte [Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Añadir perfil empresarial al usuario

El administrador del sistema de Workfront añade el perfil empresarial a un perfil de usuario seleccionando un grupo y un nivel de acceso. La combinación de ambos crea el perfil empresarial. Cada grupo solo se puede utilizar en un perfil empresarial por usuario. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

El perfil empresarial puede tener más de un nivel de acceso por grupo. El nivel con el acceso más alto tiene prioridad.

El administrador puede asignar fechas en vigor a un perfil empresarial, de modo que el acceso del usuario caduque en una fecha futura. Las fechas de inicio y finalización indican cuándo comienza y finaliza el usuario que mantiene el perfil en ese grupo. El uso de fechas efectivas para finalizar el acceso en lugar de eliminar el perfil permite que el perfil se active de nuevo en el futuro.

Se permiten varios perfiles empresariales para un usuario.

<!--image?-->

Para obtener más información, vea [Editar el perfil de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). <!--may be separate article now since it's not in the profile-->

### Asignar plantillas de diseño al nivel de acceso

El administrador del sistema de Workfront puede, opcionalmente, asignar una plantilla de diseño al nivel de acceso para garantizar que los usuarios con el perfil de negocio relacionado vean la información y las acciones relevantes en función de su función dentro del sistema.

Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

## Cómo funcionan los perfiles empresariales

Cuando se agrega un perfil empresarial a un usuario, los permisos en la combinación del grupo y el nivel de acceso determinan lo que el usuario verá en Workfront.

### Diseño de Workfront

Cuando el grupo del perfil de negocio está asociado a un proyecto, se aplica la plantilla de diseño del nivel de acceso del perfil de negocio. Todos los usuarios con el perfil empresarial verán los elementos de menú, la página de inicio y otros elementos de diseño incluidos en la plantilla. La plantilla de diseño del perfil de negocio tiene prioridad sobre una plantilla de diseño asignada al usuario.

Si el perfil empresarial tiene varios niveles de acceso con el mismo grupo, se combinan las plantillas de diseño de ambos niveles de acceso. Se muestran todos los elementos de diseño disponibles. Si un elemento de menú se muestra en una plantilla pero está oculto en otra, se muestra. Solo se ocultan los elementos que están ocultos en todas las plantillas del perfil empresarial.

En situaciones en las que los mismos elementos se muestran en varias plantillas de diseño pero el orden de los elementos es diferente (como la navegación izquierda o los anclajes), se utiliza el orden de la plantilla del nivel de acceso que aparece primero en el perfil empresarial.

### Proyectos y otros objetos compartidos

Cuando un proyecto está asociado a un grupo, un usuario con un perfil empresarial para ese grupo puede ver el proyecto. La visibilidad de los campos del proyecto se basa en el nivel de acceso del perfil empresarial. Si se asignan varios niveles de acceso al grupo en el perfil empresarial del usuario, se aplica el nivel con los permisos más altos.

Por ejemplo, un usuario tiene dos perfiles de negocio: el primero proporciona acceso de interventor financiero para un grupo (para ver los campos financieros) y el segundo proporciona acceso de gestor de proyecto en un grupo diferente (donde los campos financieros no deben verse).

El usuario vería los proyectos de ambos grupos en la lista de todos los proyectos. Tanto en la vista de lista como en los detalles del proyecto, el usuario vería los datos financieros solo para el primer grupo. Los campos financieros de los proyectos del segundo grupo estarían en blanco.

Cualquier usuario con acceso para compartir objetos puede compartirlos con un perfil empresarial. Todos los usuarios asignados al perfil tendrán los permisos especificados para el objeto. Sin embargo, si el acceso está restringido en el nivel de acceso asignado por el administrador en el perfil de negocio, el nivel de acceso tiene prioridad sobre los permisos otorgados en el uso compartido. Por ejemplo, si el nivel de acceso no permite la creación de tareas, el usuario no puede agregar tareas a un proyecto, aunque se le concedan permisos de administración a un proyecto cuando se comparte con el perfil empresarial.

Si a un usuario se le asigna un perfil empresarial después de que un objeto ya se haya compartido con el perfil, el usuario verá el objeto con el acceso especificado.

Cuando un perfil empresarial tiene varios niveles de acceso, el nivel con la mayor cantidad de acceso tiene prioridad.

Para obtener información sobre cómo compartir, vea [Compartir un objeto](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Para obtener información acerca de cómo funcionan juntos los niveles de acceso y los permisos, vea [Información general sobre los niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Consideraciones sobre los perfiles empresariales

* Un usuario no tiene que ser miembro de un grupo para que se le asigne un perfil empresarial para ese grupo.
* El nivel de acceso en el perfil empresarial solo puede actualizar el nivel de acceso &quot;base&quot; de un usuario. El perfil empresarial no puede eliminar los permisos de nivel de acceso base.
* En las listas de objetos y los informes, el usuario tiene todos los permisos que están disponibles para él en todos sus perfiles empresariales asignados en los grupos combinados con su nivel de acceso base. En otras páginas, el usuario tiene los permisos de nivel de acceso base.
* Cuando se elimina un grupo de Workfront, todos los perfiles de negocio asignados a ese grupo se eliminan de los usuarios asociados.
* Si un nivel de acceso forma parte de un perfil de negocio y se elimina el nivel de acceso, se le pedirá que elija un nuevo nivel de acceso para utilizarlo en su lugar.
* Las actualizaciones de los perfiles empresariales se rastrean en los registros de auditoría de Workfront. Para obtener más información, consulte Información general sobre los registros de auditoría.
