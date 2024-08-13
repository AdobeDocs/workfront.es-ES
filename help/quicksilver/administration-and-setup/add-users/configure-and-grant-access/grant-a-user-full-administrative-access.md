---
title: Conceder a un usuario acceso administrativo completo
description: Puede otorgar a los usuarios acceso administrativo completo a Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 1%

---

# Conceder a un usuario acceso administrativo completo

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre cómo conceder acceso de administrador completo en Adobe Admin Console, consulte [Administrar administradores del sistema en Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede crear otro administrador de Workfront asignándole el nivel de acceso de administrador del sistema. Un usuario con este nivel de acceso tiene acceso administrativo completo a todo lo que hay en Workfront, incluidos los elementos que no creó él mismo.

>[!NOTE]
>
>Esto es diferente a usar un nivel de acceso para otorgar a los usuarios acceso administrativo a ciertas áreas del sistema. Para obtener más información, consulte lo siguiente:
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
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener más información, consulte <a href="#" class="MCXref xref selected">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Conceder acceso completo de administrador del sistema a un solo usuario

{{step-1-to-users}}

1. Haga clic en el nombre del usuario al que desea conceder derechos de administrador.
1. Haga clic en el menú Más ![](assets/more-icon.png) y luego haga clic en **Editar**.

1. En el cuadro **Editar persona** que aparece, haga clic en **Acceder**.

1. En la lista desplegable **nivel de acceso**, seleccione el nivel de acceso **Administrador del sistema**.

   Según los cambios realizados en el sistema, el nombre de este nivel de acceso podría haber cambiado.

1. Haga clic en **Guardar cambios.**

   Ahora el usuario tiene derechos completos de administrador del sistema en el sistema.

## Acceso de un administrador de Workfront frente a acceso de un usuario de Plan con derechos administrativos  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Las dos tablas siguientes muestran la diferencia entre los derechos de acceso de un usuario con un nivel de acceso de administrador de Workfront y los de un usuario con una licencia de Plan con algunos derechos administrativos.

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
   <th>administrador de Workfront </th> 
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
   <td>Preferencias del proyecto: tasas de cambio</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Procesos: aprobaciones</td> 
   <td> <p>Acceso total</p> </td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Procesos: Rutas de hitos</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Formularios personalizados</td> 
   <td>Acceso total</td> 
   <td> <p>Administrar formularios personalizados que hayan creado o formularios personalizados compartidos con ellos</p> <p>Adjuntar formularios personalizados que hayan creado o formularios personalizados compartidos con ellos a objetos para los que tengan permisos de administración o de contribución.</p> </td> 
  </tr> 
  <tr> 
   <td>Papelera de reciclaje: Eliminado recientemente</td> 
   <td>Acceso total</td> 
   <td> <p>Los usuarios que sean administradores de grupos pueden restaurar los proyectos asignados a los grupos que administran, así como las tareas, problemas o documentos asociados con esos proyectos.</p> </td> 
  </tr> 
  <tr> 
   <td>Papelera de reciclaje: restaurada recientemente</td> 
   <td>Acceso total</td> 
   <td>Los usuarios que son administradores de grupos pueden ver los elementos que han restaurado recientemente.</td> 
  </tr> 
  <tr> 
   <td>Roles</td> 
   <td>Acceso total</td> 
   <td> <p>Modifique pero no elimine los roles existentes.</p> <p>Agregar nuevos roles.</p> </td> 
  </tr> 
  <tr> 
   <td>Equipos</td> 
   <td>Acceso total</td> 
   <td> <p>No hay acceso para crear equipos.</p> <p>Agregar equipos existentes a usuarios al crear o editar usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td>Grupos</td> 
   <td>Acceso total</td> 
   <td> <p>No tiene acceso para crear grupos.</p> <p>Solo los administradores de grupo pueden administrar los estados de pertenencia a grupos, subgrupos y de nivel de grupo para los grupos que administran. </p> </td> 
  </tr> 
  <tr> 
   <td>Compañías</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Iniciar sesión como</td> 
   <td>Acceso total </td> 
   <td> <p>Si el acceso administrativo a su grupo está habilitado en su nivel de acceso y se les designa como administrador de grupo, pueden iniciar sesión como los usuarios del grupo que administran y sus subgrupos. No pueden iniciar sesión como administrador del sistema.<br>Para obtener más información acerca de cómo habilitar el acceso administrativo de grupo para los usuarios, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Horarios</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para editar Horarios.</p> <p>Acceso para agregar programaciones existentes a otros usuarios, en el nivel de usuario. </p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas y horas: perfiles de hoja de horas</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso para asignar perfiles de hojas de horas existentes a usuarios, en el nivel de usuario.</p> <p>Los usuarios que sean administradores de grupos pueden crear perfiles de hoja de horas para los grupos que administren y sus subgrupos. </p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas y horas: tipos de horas</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso para asignar tipos de horas a usuarios, en el nivel de usuario.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas y horas: Preferencias</td> 
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
   <td> <p>No tiene acceso para editar plantillas de correo electrónico.</p> <p>Acceso para agregar plantillas de correo electrónico existentes a notificaciones de recordatorio.</p> </td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: recordatorios automáticos</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: invitaciones</td> 
   <td>Acceso total</td> 
   <td> <p>No hay acceso para editar las invitaciones por correo electrónico.</p> <p>Acceso para reenviar invitaciones por correo electrónico a usuarios no registrados solo desde la pestaña Personas.</p> </td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: configuración</td> 
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
   <td> <p>Acceso completo para modificar todos los niveles de acceso.</p> <p>Los niveles de acceso Administrador del sistema y Usuario externo no se pueden modificar de forma predeterminada.</p> </td> 
   <td> <p>No tiene acceso para editar los niveles de acceso.</p> <p>Asigne a otros usuarios un nivel de acceso inferior o igual al suyo en el nivel de usuario.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: plantillas de diseño</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso para asignar plantillas de diseño existentes a otros usuarios, en el nivel de usuario. </p> <p>Los usuarios designados como administradores de grupo pueden crear plantillas de diseño para los grupos y subgrupos que administren.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Actualizar fuentes</td> 
   <td>Acceso total</td> 
   <td> <p>No hay acceso para modificar Actualizar fuentes.</p> <p>Acceso para añadir campos de los que realizar un seguimiento en las fuentes de actualización al editar Forms personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Filtros</td> 
   <td>Acceso total</td> 
   <td> <p>No tiene acceso para crear filtros en el área de configuración.</p> <p>Acceso para crear nuevos filtros en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: vistas</td> 
   <td>Acceso total</td> 
   <td> <p>No tiene acceso para crear vistas en el área de configuración.</p> <p>Acceso para crear vistas nuevas en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Agrupaciones</td> 
   <td>Acceso total</td> 
   <td> <p>No tiene acceso para crear agrupaciones en el área de configuración.</p> <p>Acceso para crear nuevas agrupaciones en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: controles de lista</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Proveedores de nube</td> 
   <td>Acceso total</td> 
   <td> <p>No hay acceso para configurar proveedores en la nube.</p> <p>Acceso para vincular documentos a y desde proveedores de la nube desde la pestaña Documentos, después de que los proveedores de la nube se hayan integrado con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Asignación de metadatos</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Documentos: Integración de SharePoint</td> 
   <td>Acceso total</td> 
   <td> <p>No tiene acceso para configurar una integración de SharePoint.</p> <p>Acceso para vincular documentos desde y hacia SharePoint desde la pestaña Documentos, después de configurar la integración de SharePoint con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Integración personalizada</td> 
   <td>Acceso total</td> 
   <td> <p>Sin acceso para configurar una integración personalizada.</p> <p>Acceso para vincular documentos a proveedores de terceros y desde ellos desde la pestaña Documentos, después de que los proveedores de terceros se hayan integrado con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Sistema: marca</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Información del cliente</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: inicio de sesión único (SSO)</td> 
   <td>Acceso total</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Actualizar usuarios para SSO</td> 
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
   <td>Sistema: Preferencias</td> 
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
   <th>administrador de Workfront </th> 
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
   <td>Administre los tableros que crean y los que se comparten con ellos.</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Acceso total</td> 
   <td>Administre los documentos que cargan o los que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td>Acceso total</td> 
   <td>Administre los problemas que crean o los problemas compartidos con ellos.</td> 
  </tr> 
  <tr> 
   <td>Portafolios</td> 
   <td>Acceso total</td> 
   <td>Administre los portafolios que creen o los que se hayan compartido con ellos. </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td>Acceso total</td> 
   <td>Administre los programas que crean o los programas que comparten con ellos.</td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Acceso total</td> 
   <td>Gestionar los proyectos que creen o los proyectos compartidos con ellos.</td> 
  </tr> 
  <tr> 
   <td>Informes</td> 
   <td>Acceso total</td> 
   <td>Administrar los informes que crean o los informes que se comparten con ellos. Ver, copiar y editar informes del sistema.</td> 
  </tr> 
  <tr> 
   <td>Tareas</td> 
   <td>Acceso total</td> 
   <td>Administrar las tareas que creen o las tareas compartidas con</td> 
  </tr> 
  <tr> 
   <td>Plantillas</td> 
   <td>Acceso total</td> 
   <td>Administrar las plantillas que crean o las plantillas compartidas con ellos</td> 
  </tr> 
  <tr> 
   <td>Hojas de horas</td> 
   <td>Acceso total</td> 
   <td>Acceso total</td> 
  </tr> 
  <tr> 
   <td>Usuarios</td> 
   <td>Acceso total</td> 
   <td> <p>Acceso limitado</p> <p>No pueden asignar grupos a usuarios para los que no son administradores de grupos ni a grupos que no son públicos.</p> <p>No pueden asignar a los usuarios un nivel de acceso superior a su propio nivel de acceso.</p> <p>Si el acceso administrativo de grupo está habilitado en su nivel de acceso y está designado como administrador de grupo en un grupo, puede restablecer la contraseña de e iniciar sesión como los usuarios del grupo que administra y sus subgrupos. No pueden restablecer la contraseña de ni iniciar sesión como administrador del sistema.<br>Para obtener más información acerca de cómo habilitar el acceso administrativo de grupo para los usuarios, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
