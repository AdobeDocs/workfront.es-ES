---
title: Conceder a un usuario acceso administrativo completo
description: Puede otorgar a los usuarios acceso administrativo completo a Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 95%

---

# Conceder a un usuario acceso administrativo completo

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica solo a las organizaciones que aún no se han incorporado a Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe llevar a cabo esta acción mediante Adobe Admin Console.
>
>Para obtener instrucciones sobre cómo conceder acceso de administrador completo en Adobe Admin Console, consulte [Administrar administradores del sistema en Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede crear otro administrador de Workfront asignándole el nivel de acceso de administrador del sistema. Un usuario con este nivel de acceso tiene acceso administrativo completo a todo lo que hay en Workfront, incluidos los elementos que no creó él mismo.

>[!NOTE]
>
>Esto es diferente a usar un nivel de acceso para otorgar a los usuarios acceso administrativo a ciertas áreas del sistema. Para obtener más información, consulte los artículos:
>
>* [Conceder a los usuarios acceso administrativo a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Acceso de un administrador de Workfront frente a acceso de un usuario de Plan con derechos administrativos](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) en este artículo
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront. </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conceder acceso completo de administrador del sistema a un solo usuario

{{step-1-to-users}}

1. Haga clic en el nombre del usuario al que desea conceder derechos de administrador.
1. Haga clic en el menú **Más** ![](assets/more-icon.png) que se encuentra a la derecha del nombre de usuario y luego haga clic en **Editar**.

   Se muestra el cuadro **Editar persona**.
1. Haga clic en **Acceso** en el panel izquierdo.
1. En la lista desplegable **Nivel de acceso**, seleccione el nivel de acceso **Administrador del sistema**.

   Según los cambios realizados en el sistema, el nombre de este nivel de acceso podría haber cambiado.

1. Haga clic en **Guardar cambios.**

   Ahora el usuario tiene derechos completos de administrador del sistema en el sistema.

## Acceso de un administrador de Workfront frente a acceso de un usuario de Plan con derechos administrativos  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Las dos tablas siguientes muestran la diferencia entre los derechos de acceso de un usuario con un nivel de acceso de administrador del sistema de Workfront y los de un usuario con una licencia de planificación con algunos derechos administrativos.

Los administradores de Workfront pueden ver todos los objetos del sistema (independientemente de quién los haya creado), crear nuevos y modificar o eliminar los existentes. Tienen acceso completo a todos los objetos del sistema.

Los usuarios con una licencia de planificación que pueden editar la funcionalidad en una área tienen acceso completo a la funcionalidad de esa área.

>[!NOTE]
>
>Los usuarios con una licencia de planificación designados como administradores de grupo pueden realizar algunas de las acciones permitidas para los administradores de Workfront. Solo se les permite realizar estas acciones en los grupos que administran, sus subgrupos y los usuarios de estos grupos y subgrupos. Para obtener más información, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Acceso al área de Configuración](#access-to-the-setup-area)
* [Acceso a objetos](#access-to-objects)

### Acceso al área de Configuración {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área/objeto</th> 
   <th>Administrador de Workfront </th> 
   <th>Usuario con licencia de planificación y algunos derechos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Preferencias de proyecto: proyectos</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias de proyecto: tareas y problemas</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias de proyecto: estados</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Preferencias del proyecto: prioridades</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias del proyecto: gravedades</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias del proyecto: tipos de cambio</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Procesos: aprobaciones</td> 
   <td> <p>Acceso total</p> </td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Procesos: ver rutas de hitos</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Formularios personalizados</td> 
   <td>Acceso total</td> 
   <td> <p>Administrar formularios personalizados que hayan creado o formularios personalizados compartidos con ellos.</p> <p>Adjuntar formularios personalizados que hayan creado o formularios personalizados compartidos con ellos a objetos para los que tengan permisos de administración o de aportación.</p> </td> 
  </tr> 
  <tr> 
   <td>Papelera de reciclaje: eliminados recientemente</td> 
   <td>Acceso total</td> 
   <td> <p>Los usuarios que son administradores de grupos pueden restaurar los proyectos asignados a los grupos que administran, así como las tareas, problemas o documentos asociados con esos proyectos.</p> </td> 
  </tr> 
  <tr> 
   <td>Papelera de reciclaje: restaurados recientemente</td> 
   <td>Acceso total</td> 
   <td>Los usuarios que son administradores de grupos pueden ver los elementos que han restaurado recientemente.</td> 
  </tr> 
  <tr> 
   <td>Roles</td> 
   <td>Acceso total</td> 
   <td> <p>Modificar pero no eliminar las funciones existentes.</p> <p>Añadir nuevas funciones.</p> </td> 
  </tr> 
  <tr> 
   <td>Equipos</td> 
   <td>Acceso total</td> 
   <td> <p>No hay acceso para crear equipos.</p> <p>Añadir equipos existentes a usuarios al crear o editar usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td>Grupos</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para crear grupos.</p> <p>Solo los administradores de grupo pueden administrar los estados de pertenencia a grupos, subgrupos y nivel de grupo de los grupos que administran. </p> </td> 
  </tr> 
  <tr> 
   <td>Compañías</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Iniciar sesión como</td> 
   <td>Acceso total </td> 
   <td> <p>Si el acceso administrativo a su grupo está habilitado en su nivel de acceso y se les designa como administrador de grupos, pueden iniciar sesión como los usuarios del grupo que administran y sus subgrupos. No pueden iniciar sesión como administrador del sistema.<br>Para obtener más información sobre cómo habilitar el acceso administrativo de grupo para los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Horarios</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para editar Horarios.</p> <p>Acceso para añadir programaciones existentes a otros usuarios en el nivel de usuario. </p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas y horas: perfiles de hojas de horas</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso para asignar perfiles de hojas de horas existentes a usuarios en el nivel de usuario.</p> <p>Los usuarios con la función de administradores de grupos pueden crear perfiles de plantilla de horas para los grupos que administren y sus subgrupos. </p> </td> 
  </tr> 
  <tr> 
   <td>Plantilla de horas y horas: tipos de horas</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso para asignar tipos de horas a usuarios, en el nivel de usuario.</p> </td> 
  </tr> 
  <tr> 
   <td>Plantilla de horas y horas: preferencias</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: notificaciones: notificaciones de eventos</td> 
   <td>Activar/ desactivar todo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: notificaciones: notificaciones de recordatorio</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: notificaciones: plantillas de correo electrónico</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para editar plantillas de correo electrónico.</p> <p>Acceso para añadir plantillas de correo electrónico existentes a notificaciones de recordatorio.</p> </td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: recordatorios automáticos</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: invitaciones</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para editar invitaciones por correo electrónico.</p> <p>Acceso para reenviar invitaciones por correo electrónico a usuarios no registrados solo desde la pestaña Personas.</p> </td> 
  </tr> 
  <tr> 
   <td>Configuración de correo electrónico</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Tarjetas de puntuación</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso total</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de gastos</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de riesgos</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Niveles de acceso</td> 
   <td> <p>Acceso total para modificar todos los niveles de acceso.</p> <p>Los niveles de acceso de administrador del sistema y usuario externo no se pueden modificar de forma predeterminada.</p> </td> 
   <td> <p>Sin acceso para editar los niveles de acceso.</p> <p>Asigne a otros usuarios un nivel de acceso inferior o igual al que tengan en el nivel de usuario.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: plantillas de diseño</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso para asignar plantillas de diseño existentes a otros usuarios en el nivel de usuario. </p> <p>Los usuarios designados como administradores de grupos pueden crear plantillas de diseño para los grupos y subgrupos que administren.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Actualizar fuentes</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para modificar Actualizar fuentes.</p> <p>Acceso para añadir campos de los que realizar un seguimiento en Actualizar fuentes al editar Formularios personalizados.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Filtros</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para crear filtros en el área de configuración.</p> <p>Acceso para crear nuevos filtros en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Vistas</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para crear vistas en el área de configuración.</p> <p>Acceso para crear vistas nuevas en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Agrupaciones</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para crear agrupaciones en el área de configuración.</p> <p>Acceso para crear nuevas agrupaciones en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Controles de lista</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Proveedores de servicios en la nube</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para configurar proveedores de servicios en la nube.</p> <p>Acceso para vincular documentos a y desde proveedores de servicios en la nube desde la pestaña Documentos, después de que los proveedores de servicios en la nube se hayan integrado con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Asignación de metadatos</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Documentos: Integración con SharePoint</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para configurar una integración de SharePoint.</p> <p>Acceso para vincular documentos a y desde SharePoint desde la pestaña Documentos, después de configurar la integración de SharePoint con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Integración personalizada</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para configurar una integración personalizada.</p> <p>Acceso para vincular documentos a y desde proveedores de terceros desde la pestaña Documentos, después de que estos proveedores se hayan integrado con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Sistema: Personalización de marca</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Información del cliente</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Inicio de sesión único (SSO)</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Actualización de usuarios para SSO</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Kick-Starts</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: diagnóstico</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: preferencias</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
 </tbody> 
</table>

### Acceso a objetos {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área/objeto</th> 
   <th>Administrador de Workfront </th> 
   <th>Usuario con licencia de planificación y algunos derechos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendarios</td> 
   <td>Acceso total</td> 
   <td>Administre los calendarios que crean y los que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Paneles</td> 
   <td>Acceso total</td> 
   <td>Administre los paneles de control que crean y los que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Acceso total</td> 
   <td>Administre los documentos que cargan o los que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td>Acceso total</td> 
   <td>Administre los problemas que crean o los que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Portafolios</td> 
   <td>Acceso total</td> 
   <td>Administre los portafolios que crean o los que se han compartido con ellos. </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td>Acceso total</td> 
   <td>Administre los programas que crean o los que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Acceso total</td> 
   <td>Administre los proyectos que crean o los que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Informes</td> 
   <td>Acceso total</td> 
   <td>Administre los informes que crean o los que se han compartido con ellos. Consulte, copie y edite informes del sistema.</td> 
  </tr> 
  <tr> 
   <td>Tareas</td> 
   <td>Acceso total</td> 
   <td>Administre las tareas que crean o las que se han compartido con</td> 
  </tr> 
  <tr> 
   <td>Plantillas</td> 
   <td>Acceso total</td> 
   <td>Administre las plantillas que crean o las que se han compartido con ellos</td> 
  </tr> 
  <tr> 
   <td>Hojas de horas</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Usuarios</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso limitado</p> <p>No pueden asignar grupos a usuarios para los que no son administradores de grupos ni a grupos que no son públicos.</p> <p>No pueden asignar a los usuarios un nivel de acceso que sea superior a su propio nivel de acceso.</p> <p>Si el acceso administrativo de su grupo está habilitado en su nivel de acceso y está designado como administrador de grupos en un grupo, puede restablecer la contraseña de los usuarios del grupo que administra y de sus subgrupos e iniciar sesión como tal. No pueden restablecer la contraseña de ni iniciar sesión como administrador del sistema.<br>Para obtener más información sobre cómo habilitar el acceso administrativo de grupo para los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
