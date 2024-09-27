---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,modelo,canal,diagrama,niveles,permisos
navigation-topic: access-levels
title: Funcionalidad disponible para cada tipo de objeto para varios niveles de acceso
description: En las tablas siguientes se enumeran las funciones disponibles para cada tipo de objeto en los distintos niveles de acceso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 2fa590235063e194d6277394f13b3d6be752ec4f
workflow-type: tm+mt
source-wordcount: '1953'
ht-degree: 10%

---

# Funcionalidad disponible para cada tipo de objeto para varios niveles de acceso

{{highlighted-preview}}

En las tablas siguientes se enumeran las funciones disponibles para cada tipo de objeto en los distintos niveles de acceso.

También indica qué acciones pueden deshabilitar o habilitar los administradores de Workfront mediante un nivel de acceso.

>[!NOTE]
>
>En este artículo se describe la funcionalidad disponible para los niveles de acceso en el modelo de plan de Workfront actual. Para ver la funcionalidad disponible en el nuevo modelo de plan, consulte [Funcionalidad disponible para cada tipo de objeto para los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

## Proyectos

Solo los usuarios con una licencia de planificación pueden obtener acceso completo a los proyectos.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Copiar | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; | ✓&#42; |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Ver | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Agregar un formulario personalizado | ✓ |   |   |   |   |
| Actualizar campos personalizados | ✓ | ✓ |   |   |   |
| Agregar un proceso de aprobación | ✓ |   |   |   |   |
| Aprobación de un proyecto | ✓ | ✓ | ✓ |   |   |
| Añadir documento | ✓ | ✓ | ✓ |   |   |
| Agregar problema | ✓ | ✓ |   |   |   |
| Añadir tareas | ✓ | ✓ |   |   |   |
| Proporcionar actualizaciones/comentarios | ✓ | ✓ | ✓ |   |   |
| Cambiar estado | ✓ |   |   |   |   |
| Registrar horas | ✓ | ✓ |   |   |   |
| Editar asignaciones | ✓ | ✓ |   |   |   |
| Administrar una línea base | ✓ |   |   |   |   |
| Administrar riesgos | ✓ |   |   |   |   |
| Administrar finanzas | ✓ |   |   |   |   |
| Agregar o editar gastos | ✓ | ✓ |   |   |   |
| Adjuntar plantillas | ✓ |   |   |   |   |
| Guardar como plantilla | ✓ |   |   |   |   |
| Agregar o editar un caso empresarial | ✓ |   |   |   |   |
| Editar detalles del proyecto | ✓ |   |   |   |   |
| Editar plantilla | ✓ |   |   |   |   |
| Exportar a MS Project | ✓ | ✓ | ✓ |   |   |
| Recalcular finanzas/cronología | ✓ |   |   |   |   |
| Establecer propiedades de cola | ✓ |   |   |   |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Tareas

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; | ✓&#42; |   |   |   |
| Eliminar | ✓&#42; | ✓&#42; |   |   |   |
| Compartir | ✓&#42; | ✓&#42; |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Ver | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Agregar predecesoras | ✓ | ✓ |   |   |   |
| Añadir problemas | ✓ | ✓ |   |   |   |
| Editar una tarea (excluido el estado) | ✓ | ✓ |   |   |   |
| Cambiar estado de tarea | ✓ | ✓ |   |   |   |
| Agregar documentos | ✓ | ✓ | ✓ |   |   |
| Copiar una tarea | ✓ | ✓ |   |   |   |
| Mover una tarea | ✓ | ✓ |   |   |   |
| Registrar horas | ✓ | ✓ |   |   |   |
| Aceptar una asignación | ✓ | ✓ |   |   |   |
| Realización de una asignación | ✓ | ✓ | Solo edición en línea | Solo edición en línea |   |
| Adjuntar un formulario personalizado | ✓ | ✓ |   |   |   |
| Editar campos personalizados | ✓ | ✓ |   |   |   |
| Creación de un proceso de aprobación | ✓ | ✓ |   |   |   |
| Aprobar una tarea | ✓ | ✓ | ✓ |   |   |
| Editar finanzas | ✓ |   |   |   |   |
| Agregar o editar gastos | ✓ | ✓ |   |   |   |
| Ver finanzas | ✓ | ✓ | ✓ |   |   |
| Actualizaciones/comentarios | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problemas

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Editar | ✓ | ✓ | ✓ | ✓ |   |
| Eliminar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Ver | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Adjuntar formularios personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Aprobar problemas | ✓ | ✓ | ✓ | ✓ |   |
| Agregar un proceso de aprobación | ✓ | ✓ | ✓ | ✓ |   |
| Agregar documentos | ✓ | ✓ | ✓ | ✓ |   |
| Copiar problemas | ✓ | ✓ | ✓ | ✓ |   |
| Mover problemas | ✓ | ✓ | ✓ | ✓ |   |
| Registrar horas | ✓ | ✓ |   |   |   |
| Convertir un problema en un proyecto | ✓ | ✓ |   |   |   |
| Convertir un problema en una tarea | ✓ |   |   |   |   |
| Aceptar asignaciones | ✓ | ✓ |   |   |   |
| Hacer asignaciones | ✓ | ✓ |   |   |   |
| Agregar actualizaciones y comentarios | ✓ | ✓ | ✓ | ✓ |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portafolios

Solo los usuarios con una licencia de planificación pueden tener acceso completo a las carteras.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Ver | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Editar detalles | ✓ |   |   |   |   |
| Adjuntar formularios personalizados | ✓ |   |   |   |   |
| Editar campos personalizados | ✓ |   |   |   |   |
| Agregar y quitar proyectos | ✓ |   |   |   |   |
| Aprobar proyectos | ✓ |   |   |   |   |
| optimización del Portfolio | ✓ |   |   |   |   |
| Agregar documentos | ✓ | ✓ | ✓ |   |   |
| Agregar actualizaciones y comentarios | ✓ | ✓ | ✓ |   |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programas

Solo los usuarios con una licencia de planificación pueden tener acceso completo a los programas.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Ver | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Editar detalles | ✓ |   |   |   |   |
| Adjuntar formularios personalizados | ✓ |   |   |   |   |
| Editar campos personalizados | ✓ |   |   |   |   |
| Agregar y quitar proyectos | ✓ |   |   |   |   |
| Aprobar proyectos | ✓ |   |   |   |   |
| Optimización de portafolio | ✓ |   |   |   |   |
| Agregar documentos | ✓ | ✓ | ✓ |   |   |
| Agregar Agregar actualizaciones y comentarios | ✓ | ✓ | ✓ |   |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Informes, tableros y calendarios

Los usuarios con una licencia de planificación pueden tener acceso completo a los informes. Todos los demás niveles de acceso tienen acceso de visualización a los informes.

| Acción | Planificador | Trabajador | Revisor | Solicitud | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Ver informes integrados | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; | ✓ | ✓ |   |   |
| Compartir calendarios e informes públicamente | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Ver | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar | ✓ |   |   |   |   |
| Copiar | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>Los solicitantes solo pueden ver los informes que se han compartido con ellos

## Filtros, vistas y agrupaciones

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Acción</p> </th> 
   <th> <p>Planificador</p> </th> 
   <th> <p>Trabajador</p> </th> 
   <th> <p>Revisor</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th>Usuario externo<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Crear</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartir</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartir en todo el sistema</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ver</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documentos

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Eliminar (documentos y carpetas) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir públicamente (externamente) | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; | ✓&#42; |   |   |   |
| Ver | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar detalles | ✓ | ✓ | ✓ | ✓ |   |
| Descargar | ✓ | ✓ | ✓ | ✓ | ✓ |
| Finalizar compra | ✓ | ✓ | ✓ | ✓ |   |
| Añadir aprobadores | ✓ | ✓ | ✓ | ✓ |   |
| Aprobar documentos | ✓ | ✓ | ✓ | ✓ | ✓ |
| Adjuntar formularios personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Mover a (objeto) | ✓ | ✓ | ✓ | ✓ |   |
| Enviar a (integración) | ✓ | ✓ | ✓ | ✓ |   |
| Agregar actualizaciones y comentarios | ✓ | ✓ | ✓ | ✓ |   |
| Cargar nueva versión | ✓ | ✓ | ✓ | ✓ |   |
| Eliminar una versión | ✓ | ✓ | ✓ | ✓ |   |
| Vista previa | ✓ | ✓ | ✓ | ✓ | ✓ |
| Revisión | ✓ | ✓ | ✓ | ✓ |   |
| Generar revisión | ✓ | ✓ |   |   |   |
| Eliminar revisión | ✓ | ✓ | ✓ | ✓ |   |
| Agregar/Quitar&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Cambiar nombre&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Vínculo (con integración) | ✓ | ✓ | ✓ | ✓ |   |
| Desvincular (con integración) | ✓ | ✓ | ✓ | ✓ |   |

{style="table-layout:auto"}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Disponible sólo para carpetas de documentos, no para documentos

## Usuarios

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Acción</p> </th> 
   <th> <p>Planificador</p> </th> 
   <th>Trabajador</th> 
   <th> <p>Revisor</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th> <p>Usuario externo**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Crear</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, eliminar, desactivar, iniciar sesión como o restablecer la contraseña de cualquier usuario</td> 
   <td>✓*<p><b>NOTA</b>: no puede iniciar sesión como ningún usuario que sea administrador del sistema.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Edite, elimine, desactive, inicie sesión como o restablezca la contraseña de cualquier usuario de un grupo que administre</td> 
   <td>✓*<p><b>NOTA</b>: no puede iniciar sesión como ningún usuario que sea administrador del sistema.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ver usuarios</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ver información de contacto</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Los usuarios externos solo pueden buscar otros usuarios

## Equipos

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Acción</p> </th> 
   <th> <p>Planificador</p> </th> 
   <th>Trabajador</th> 
   <th> <p>Revisor</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th> <p>Usuario externo*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Crear</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar los equipos en los que están</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar los equipos de los grupos que administran</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ver todos los equipos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ver equipos asociados a sus grupos</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Plantillas

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Ver | ✓&#42; |   |   |   |   |
| Copiar | ✓ |   |   |   |   |
| Editar detalles de plantilla | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Datos financieros

Solo los usuarios con una licencia de planificación pueden tener acceso completo a los datos financieros.

Los tipos de licencia de solicitud y usuario externo no se incluyen aquí porque no tienen acceso a estos objetos y áreas.

| Acción | Planificador | Trabajador | Revisor |
|---|---|---|---|
| Editar tarifas de facturación y de costo de rol | ✓&#42; |   |   |
| Editar tarifas de facturación y de costo de usuario | ✓&#42; |   |   |
| Ver tarifas de facturación y de costo de rol | ✓&#42; |   |   |
| Ver tarifas de facturación y de costo de usuario | ✓&#42; |   |   |
| Administrar registros de facturación | ✓ |   |   |
| Administrar gastos | ✓ | ✓ |   |
| Ver datos financieros | ✓&#42; | ✓&#42; | ✓&#42; |
| <span class="preview">Administrar tarjetas de tarifas</span> | ✓ |   |   |
| Ver información por costo en las herramientas de planificación de recursos | ✓ |   |   |
| Recursos de presupuesto en las herramientas de planificación de recursos&#42;&#42; | ✓ |   |   |
| Ver asignación de recursos en las herramientas de planificación de recursos&#42; | ✓ | ✓ | ✓ |
| Crear riesgos en los proyectos | ✓ |   |   |
| Ver riesgos en los proyectos | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requiere acceso adicional a Administración de recursos.

## Administración de recursos

Solo los usuarios con una licencia de planificación pueden tener acceso completo a [seleccionar objeto o área]. Otros tipos de licencia pueden tener acceso limitado o nulo a la administración de recursos en Workfront.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Editar prioridades y horas presupuestadas en el Planificador | ✓&#42; |   |   |   |   |
| Crear, editar y eliminar conjuntos de recursos&#42;&#42; | ✓&#42; |   |   |   |   |
| Actualizar horas planificadas en el Distribuidor de cargas de trabajo&#42;&#42;&#42; | ✓* |   |   |   |   |
| Ver las prioridades del proyecto en el Planificador de recursos | ✓&#42; |   |   |   |   |
| Ver la asignación de recursos en las herramientas de planificación de recursos | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Ver conjuntos de recursos | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Recursos de presupuesto en las herramientas de planificación de recursos&#42;&#42; | ✓ |   |   |   |   |
| Adjuntar conjuntos de recursos a proyectos, plantillas y usuarios | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requiere acceso adicional a datos financieros y permisos para las finanzas del proyecto. Si concede acceso a Administración de recursos a un usuario de Planificador que no tiene acceso a Datos financieros, el usuario puede seguir viendo las asignaciones por hora en el Planificador de recursos, pero no puede cambiar a la vista de costo ni ver el caso comercial. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) y [Compartir permisos financieros en un objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Requiere permiso para Contribute en el objeto, con la opción Realizar asignaciones habilitada en Configuración avanzada. Para obtener más información, consulte la sección [Comprender los permisos heredados y la jerarquía de objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) en el artículo [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Área del planificador de escenarios

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear/editar planes e iniciativas existentes | ✓ | ✓ | ✓ |   |   |
| Agregar o editar información de rol en planes e iniciativas&#42; | ✓ | ✓ | ✓ |   |   |
| Agregar o editar información de costos en planes e iniciativas&#42; | ✓ | ✓ | ✓ |   |   |
| Eliminar planes e iniciativas | ✓ | ✓ | ✓ |   |   |
| Ver escenarios en el menú principal ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |   |
| Ver los planes e iniciativas que creó el usuario&#42; | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

>[!NOTE]
>
>Los usuarios pueden ver un plan que otro usuario haya creado solamente si se comparte con ellos un vínculo al plan.

&#42; Para que los usuarios vean los datos financieros en un plan o iniciativa, necesitan acceso a los Datos financieros. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Área Objetivos de Workfront

| Acciones | Ver | Editar |
|---|---|---|
| Crear |   | ✓ |
| Editar/eliminar todas las metas |   | ✓ |
| Ver metas en el menú principal | ✓ | ✓ |
| Ver el área Objetivos desde un vínculo compartido | ✓ | ✓ |
| Ver todas las metas del sistema | ✓ | ✓ |
| Activar/ desactivar/ cerrar todas las metas |   | ✓ |
| Crear/editar/eliminar actividades |   | ✓ |
| Crear/editar/eliminar resultados |   | ✓ |
| Añadir una meta alineada |   | ✓ |
| Actualización del progreso de un resultado o una actividad |   | ✓ |
| Poseer un objetivo, resultado o actividad | ✓ | ✓ |
| Comentario sobre una meta | ✓ | ✓ |
| Copiar metas |   | ✓ |
| Vea la sección Lista de metas en el panel izquierdo | ✓ | ✓ |
| Vea la sección Gráficos en el panel izquierdo | ✓ | ✓ |
| Vea la sección Alineación de objetivos en el panel izquierdo | ✓ | ✓ |


