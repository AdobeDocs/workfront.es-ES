---
title: Conceder a un usuario acceso administrativo completo
description: Puede otorgar a los usuarios acceso administrativo completo a Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 1%

---

# Conceder a un usuario acceso administrativo completo

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre cómo conceder acceso completo al administrador en Adobe Admin Console:
>
>* Consulte [Cree administradores de sistema en Workfront con Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* Consulte la sección &quot;Editar detalles del usuario&quot; en el artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) en la documentación de Adobe Admin Console.
>* Póngase en contacto con su administrador de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede crear otro administrador de Workfront asignándoles el nivel de acceso del administrador del sistema. Un usuario con este nivel de acceso tiene acceso administrativo completo a todo lo que hay en Workfront, incluidos los elementos que no se crearon por sí mismo.

>[!NOTE]
>
>Esto es diferente a usar un nivel de acceso para otorgar a los usuarios acceso administrativo a ciertas áreas del sistema. Para obtener más información, consulte lo siguiente:
>
>* [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Acceso de un administrador de Workfront frente a acceso de un usuario del Plan con derechos administrativos](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) en este artículo
>


## Requisitos de acceso

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
   <td> <p>Debe ser administrador de Workfront. Para obtener más información, consulte <a href="#" class="MCXref xref selected">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Conceder acceso completo al administrador del sistema a un único usuario

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Haga clic en el nombre del usuario al que desea conceder derechos de administrador.
1. Haga clic en el menú Más ![](assets/more-icon.png)y haga clic en **Editar**.

1. En el **Editar persona** que aparece, haga clic en **Acceso**.

1. En el **nivel de acceso** lista desplegable, seleccione la **Administrador del sistema** nivel de acceso.

   Según los cambios realizados en el sistema, es posible que el nombre de este nivel de acceso haya cambiado.

1. Haga clic en **Guarde los cambios.**

   El usuario tiene derechos de administrador del sistema completos en el sistema.

## Acceso de un administrador de Workfront frente a acceso de un usuario del Plan con derechos administrativos  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Las dos tablas siguientes muestran la diferencia entre los derechos de acceso de un usuario con un nivel de acceso de administrador de Workfront y los de un usuario con una licencia de Plan con algunos derechos administrativos.

Los administradores de Workfront pueden ver todos los objetos del sistema (independientemente de quién los haya creado), crear nuevos objetos y modificar o eliminar los existentes. Tienen acceso completo a todos los objetos del sistema.

Los usuarios con una licencia Plan que pueden editar funcionalidad en un área tienen acceso completo a la funcionalidad en ese área.

>[!NOTE]
>
>Los usuarios con una licencia Plan designados como administradores de grupo pueden realizar algunas de las acciones permitidas para los administradores de Workfront. Solo pueden realizar estas acciones para los grupos que administran, sus subgrupos y los usuarios de estos grupos y subgrupos. Para obtener más información, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Acceso al área de configuración](#access-to-the-setup-area)
* [Acceso a objetos](#access-to-objects)

### Acceso al área de configuración {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área/objeto</th> 
   <th>Administrador de Workfront </th> 
   <th>Usuario con licencia Plan y algunos derechos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Preferencias de proyecto: Proyectos</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias de proyecto: Tareas y problemas</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias de proyecto: Estados</td> 
   <td>Acceso completo</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Preferencias de proyecto: Prioridades</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias de proyecto: Versiones</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Preferencias de proyecto: Tipos de Cambio</td> 
   <td>Acceso completo</td> 
   <td>Acceso completo</td> 
  </tr> 
  <tr> 
   <td>Procesos: Aprobaciones</td> 
   <td> <p>Acceso completo</p> </td> 
   <td>Acceso completo</td> 
  </tr> 
  <tr> 
   <td>Procesos: Rutas de Milestone</td> 
   <td>Acceso completo</td> 
   <td>Acceso completo</td> 
  </tr> 
  <tr> 
   <td>Formularios personalizados</td> 
   <td>Acceso completo</td> 
   <td> <p>Administre los formularios personalizados que crearon o los formularios personalizados que compartieron con ellos.</p> <p>Adjunte los formularios personalizados que hayan creado o los formularios personalizados que hayan compartido con ellos a los objetos que administran o a los que tienen permisos de contribución.</p> </td> 
  </tr> 
  <tr> 
   <td>Papelera de reciclaje: Eliminado recientemente</td> 
   <td>Acceso completo</td> 
   <td> <p>Los usuarios que sean administradores de grupos pueden restaurar proyectos asignados a los Grupos que administran, así como tareas, problemas o documentos asociados a esos proyectos.</p> </td> 
  </tr> 
  <tr> 
   <td>Papelera de reciclaje: Restaurado recientemente</td> 
   <td>Acceso completo</td> 
   <td>Los usuarios que son administradores de grupos pueden ver los elementos que han restaurado recientemente.</td> 
  </tr> 
  <tr> 
   <td>Roles</td> 
   <td>Acceso completo</td> 
   <td> <p>Modifique pero no elimine las funciones de trabajo existentes.</p> <p>Añada nuevas funciones de trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td>Equipos</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para crear equipos.</p> <p>Agregue equipos existentes a usuarios al crear o editar usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td>Grupos</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para crear Grupos.</p> <p>Solo los administradores de grupos pueden administrar la pertenencia a grupos, subgrupos y estados de nivel de grupo para los grupos que administran. </p> </td> 
  </tr> 
  <tr> 
   <td>Compañías</td> 
   <td>Acceso completo</td> 
   <td>Acceso completo</td> 
  </tr> 
  <tr> 
   <td>Iniciar sesión como</td> 
   <td>Acceso completo </td> 
   <td> <p>Si el acceso administrativo de grupo está habilitado en su nivel de acceso y están designados como administradores de grupo, pueden iniciar sesión como los usuarios del grupo que administran y sus subgrupos. No pueden iniciar sesión como administrador del sistema.<br>Para obtener más información sobre cómo habilitar el acceso administrativo de grupo para los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Horarios</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para editar programas.</p> <p>Acceso para agregar programaciones existentes a otros usuarios a nivel de usuario. </p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas y horas: Perfiles de parte de horas</td> 
   <td>Acceso completo</td> 
   <td> <p>Acceso para asignar perfiles de parte de horas existentes a usuarios a nivel de usuario.</p> <p>Los usuarios que sean administradores de grupo pueden crear Perfiles de parte de horas para los grupos que administran y sus subgrupos. </p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas y horas: Tipos de hora</td> 
   <td>Acceso completo</td> 
   <td> <p>Acceso para asignar tipos de hora a los usuarios a nivel de usuario.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas y horas: Preferencias</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: Notificaciones: Notificaciones de eventos</td> 
   <td>Activar/Desactivar todo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: Notificaciones: Notificaciones de recordatorio</td> 
   <td>Acceso completo</td> 
   <td>Acceso completo</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: Notificaciones: Plantillas de correo electrónico</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para editar plantillas de correo electrónico.</p> <p>Acceso para agregar plantillas de correo electrónico existentes a las notificaciones de recordatorio.</p> </td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: Recordatorios automáticos</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: Invitaciones</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para editar las invitaciones por correo electrónico.</p> <p>Acceso para reenviar invitaciones de correo electrónico a usuarios no registrados solo desde la pestaña Personas .</p> </td> 
  </tr> 
  <tr> 
   <td>Correo electrónico: Configuración</td> 
   <td>Acceso completo</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Tarjetas de puntuación</td> 
   <td>Acceso completo</td> 
   <td> <p>Acceso completo</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de gastos</td> 
   <td>Acceso completo</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de riesgos</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Niveles de acceso</td> 
   <td> <p>Acceso completo para modificar todos los niveles de acceso.</p> <p>Los niveles de acceso del administrador del sistema y del usuario externo no se pueden modificar de forma predeterminada.</p> </td> 
   <td> <p>No hay acceso para editar los niveles de acceso.</p> <p>Asigne un nivel de acceso a otros usuarios que sea menor o igual que el de ellos a nivel de usuario.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Plantillas de diseño</td> 
   <td>Acceso completo</td> 
   <td> <p>Acceso para asignar plantillas de diseño existentes a otros usuarios a nivel de usuario. </p> <p>Los usuarios designados como administradores de grupo pueden crear plantillas de diseño para los grupos y subgrupos que administran.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Actualizar fuentes</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para modificar las fuentes de actualización.</p> <p>Acceso para añadir campos de los que realizar un seguimiento en Actualizar fuentes al editar Forms personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Filtros</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para crear filtros en el área Configuración.</p> <p>Acceso para crear nuevos filtros en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Vistas</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para crear vistas en el área Configuración.</p> <p>Acceso para crear nuevas vistas en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Agrupaciones</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para crear agrupaciones en el área Configuración.</p> <p>Acceso para crear nuevas agrupaciones en una lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaz: Controles de lista</td> 
   <td>Acceso completo</td> 
   <td> <p>Sin acceso</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Proveedores de nube</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para configurar los proveedores de Cloud.</p> <p>Acceso para vincular documentos a y desde proveedores de nube desde la pestaña Documentos , después de que los proveedores de nube se hayan integrado con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Asignación de metadatos</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Documentos: Integración de SharePoint</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para configurar una integración con SharePoint.</p> <p>Acceso para vincular documentos a y desde SharePoint desde la pestaña Documents , después de configurar la integración de SharePoint con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Integración personalizada</td> 
   <td>Acceso completo</td> 
   <td> <p>No hay acceso para configurar una integración personalizada.</p> <p>Acceso para vincular documentos a y desde proveedores de terceros desde la pestaña Documents , después de que los proveedores de terceros se hayan integrado con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Sistema: Marcas</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Información del cliente</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Inicio de sesión único (SSO)</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Actualizar usuarios para SSO</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Inicio</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Diagnóstico</td> 
   <td>Acceso completo</td> 
   <td>Sin acceso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Preferencias</td> 
   <td>Acceso completo</td> 
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
   <th>Usuario con licencia Plan y algunos derechos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendarios</td> 
   <td>Acceso completo</td> 
   <td>Administre los calendarios que crean y los calendarios que comparten con ellos.</td> 
  </tr> 
  <tr> 
   <td>Paneles</td> 
   <td>Acceso completo</td> 
   <td>Administre los tableros que crean y los tableros se comparten con ellos.</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Acceso completo</td> 
   <td>Administre los documentos que cargan o los documentos que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td>Acceso completo</td> 
   <td>Administre los problemas que crean o los problemas que se han compartido con ellos.</td> 
  </tr> 
  <tr> 
   <td>Portafolios</td> 
   <td>Acceso completo</td> 
   <td>Administre portafolios que crean o portafolios compartidos con ellos. </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td>Acceso completo</td> 
   <td>Administre los programas que crean o los programas que comparten con ellos.</td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Acceso completo</td> 
   <td>Administre los proyectos que crean o los proyectos que comparten con ellos.</td> 
  </tr> 
  <tr> 
   <td>Informes</td> 
   <td>Acceso completo</td> 
   <td>Administre los informes que crean o los informes que comparten con ellos. Ver, copiar y editar informes del sistema.</td> 
  </tr> 
  <tr> 
   <td>Tareas</td> 
   <td>Acceso completo</td> 
   <td>Administre las tareas que crean o las tareas compartidas con</td> 
  </tr> 
  <tr> 
   <td>Plantillas</td> 
   <td>Acceso completo</td> 
   <td>Administre las plantillas que crean o las plantillas compartidas con ellas</td> 
  </tr> 
  <tr> 
   <td>Plantillas de horas</td> 
   <td>Acceso completo</td> 
   <td>Acceso completo</td> 
  </tr> 
  <tr> 
   <td>Usuarios</td> 
   <td>Acceso completo</td> 
   <td> <p>Acceso limitado</p> <p>No pueden asignar grupos a usuarios para los que no sean administradores de grupos ni grupos que no sean públicos.</p> <p>No pueden asignar un nivel de acceso a los usuarios que sea superior al de su propio nivel de acceso.</p> <p>Si el acceso administrativo de grupo está habilitado en su nivel de acceso y están designados como administradores de grupo en un grupo, pueden restablecer la contraseña de e iniciar sesión como los usuarios del grupo que administran y sus subgrupos. No pueden restablecer la contraseña de ni iniciar sesión como administrador del sistema.<br>Para obtener más información sobre cómo habilitar el acceso administrativo de grupo para los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
