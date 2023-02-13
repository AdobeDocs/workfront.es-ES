---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso,modelo,canal,diagrama,niveles,permisos
navigation-topic: access-levels
title: Funcionalidad disponible para cada tipo de objeto
description: En las tablas siguientes se muestra la funcionalidad disponible para cada tipo de objeto en los distintos niveles de acceso.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 12%

---

# Funcionalidad disponible para cada tipo de objeto

En las tablas siguientes se muestra la funcionalidad disponible para cada tipo de objeto en los distintos niveles de acceso.

También indica las acciones que los administradores de Workfront pueden deshabilitar o habilitar mediante un nivel de acceso.

## Proyectos

Solo los usuarios con una licencia del Plan pueden tener acceso completo a los proyectos.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Copiar | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; | ✓&#42; |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Vista | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Agregar un formulario personalizado | ✓ |   |   |   |   |
| Actualizar campos personalizados | ✓ | ✓ |   |   |   |
| Agregar un proceso de aprobación | ✓ |   |   |   |   |
| Aprobar un proyecto | ✓ | ✓ | ✓ |   |   |
| Agregar documento | ✓ | ✓ | ✓ |   |   |
| Añadir problema | ✓ | ✓ |   |   |   |
| Añadir  tareas | ✓ | ✓ |   |   |   |
| Enviar actualizaciones/comentarios | ✓ | ✓ | ✓ |   |   |
| Cambiar estado | ✓ |   |   |   |   |
| Horas de registro | ✓ | ✓ |   |   |   |
| Editar asignaciones | ✓ | ✓ |   |   |   |
| Administrar una línea de base | ✓ |   |   |   |   |
| Gestión de riesgos | ✓ |   |   |   |   |
| Administrar finanzas | ✓ |   |   |   |   |
| Añadir/editar gastos | ✓ | ✓ |   |   |   |
| Adjuntar plantillas | ✓ |   |   |   |   |
| Guardar como plantilla | ✓ |   |   |   |   |
| Agregar o editar un caso empresarial | ✓ |   |   |   |   |
| Editar detalles del proyecto | ✓ |   |   |   |   |
| Editar plantilla | ✓ |   |   |   |   |
| Exportar a MS Project | ✓ | ✓ | ✓ |   |   |
| Volver a calcular finanzas/cronograma | ✓ |   |   |   |   |
| Establecer propiedades de cola | ✓ |   |   |   |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Tareas

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; | ✓&#42; |   |   |   |
| Eliminar | ✓&#42; | ✓&#42; |   |   |   |
| Compartir | ✓&#42; | ✓&#42; |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Vista | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Agregar predecesores | ✓ | ✓ |   |   |   |
| Añadir  problemas | ✓ | ✓ |   |   |   |
| Editar una tarea (sin estado) | ✓ | ✓ |   |   |   |
| Cambiar el estado de una tarea | ✓ | ✓ |   |   |   |
| Agregar documentos | ✓ | ✓ | ✓ |   |   |
| Copiar una tarea | ✓ | ✓ |   |   |   |
| Mover una tarea | ✓ | ✓ |   |   |   |
| Horas de registro | ✓ | ✓ |   |   |   |
| Aceptar una asignación | ✓ | ✓ |   |   |   |
| Realizar una asignación | ✓ | ✓ | Solo en la edición en línea | Solo en la edición en línea |   |
| Adjuntar un formulario personalizado | ✓ | ✓ |   |   |   |
| Editar campos personalizados | ✓ | ✓ |   |   |   |
| Creación de un proceso de aprobación | ✓ | ✓ |   |   |   |
| Aprobar una tarea | ✓ | ✓ | ✓ |   |   |
| Editar finanzas | ✓ |   |   |   |   |
| Añadir/editar gastos | ✓ | ✓ |   |   |   |
| Ver finanzas | ✓ | ✓ | ✓ |   |   |
| Actualizaciones/comentarios | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problemas

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Editar | ✓ | ✓ | ✓ | ✓ |   |
| Eliminar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Vista | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Adjuntar formularios personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Aprobar problemas | ✓ | ✓ | ✓ | ✓ |   |
| Agregar un proceso de aprobación | ✓ | ✓ | ✓ | ✓ |   |
| Agregar documentos | ✓ | ✓ | ✓ | ✓ |   |
| Copiar problemas | ✓ | ✓ | ✓ | ✓ |   |
| Mover problemas | ✓ | ✓ | ✓ | ✓ |   |
| Horas de registro | ✓ | ✓ |   |   |   |
| Convertir un problema en un proyecto | ✓ | ✓ |   |   |   |
| Convertir un problema en una tarea a | ✓ |   |   |   |   |
| Aceptar asignaciones | ✓ | ✓ |   |   |   |
| Realización de asignaciones | ✓ | ✓ |   |   |   |
| Añadir actualizaciones y comentarios | ✓ | ✓ | ✓ | ✓ |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portafolios

Solo los usuarios con una licencia Plan pueden tener acceso completo a las carteras.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Vista | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Editar detalles | ✓ |   |   |   |   |
| Adjuntar formularios personalizados | ✓ |   |   |   |   |
| Editar campos personalizados | ✓ |   |   |   |   |
| Agregar y eliminar proyectos | ✓ |   |   |   |   |
| Aprobar proyectos | ✓ |   |   |   |   |
| Optimización del Portfolio | ✓ |   |   |   |   |
| Agregar documentos | ✓ | ✓ | ✓ |   |   |
| Añadir actualizaciones y comentarios | ✓ | ✓ | ✓ |   |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programas

Solo los usuarios con una licencia de Plan pueden tener acceso completo a los programas.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Vista | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Editar detalles | ✓ |   |   |   |   |
| Adjuntar formularios personalizados | ✓ |   |   |   |   |
| Editar campos personalizados | ✓ |   |   |   |   |
| Agregar y eliminar proyectos | ✓ |   |   |   |   |
| Aprobar proyectos | ✓ |   |   |   |   |
| Optimización de portafolio | ✓ |   |   |   |   |
| Agregar documentos | ✓ | ✓ | ✓ |   |   |
| Agregar actualizaciones y comentarios | ✓ | ✓ | ✓ |   |   |



&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Informes, tableros y calendarios

Los usuarios con una licencia del Plan pueden tener acceso completo a los informes. Todos los demás niveles de acceso tienen acceso de vista a los informes.

| Acción | Planificador | Trabajador | Revisor | Solicitud | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Ver informes integrados | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; | ✓ | ✓ |   |   |
| Compartir calendarios e informes públicamente | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Vista | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar | ✓ |   |   |   |   |
| Copiar | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

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
   <td>Vista</td> 
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

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documentos

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Eliminación (documentos y carpetas) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartir públicamente (externamente) | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; | ✓&#42; |   |   |   |
| Vista | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar detalles | ✓ | ✓ | ✓ | ✓ |   |
| Descargar | ✓ | ✓ | ✓ | ✓ | ✓ |
| Cierre de compra | ✓ | ✓ | ✓ | ✓ |   |
| Agregar aprobadores | ✓ | ✓ | ✓ | ✓ |   |
| Aprobar documentos | ✓ | ✓ | ✓ | ✓ | ✓ |
| Adjuntar formularios personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Mover a (objeto) | ✓ | ✓ | ✓ | ✓ |   |
| Enviar a (integración) | ✓ | ✓ | ✓ | ✓ |   |
| Añadir actualizaciones y comentarios | ✓ | ✓ | ✓ | ✓ |   |
| Cargar nueva versión | ✓ | ✓ | ✓ | ✓ |   |
| Eliminar una versión | ✓ | ✓ | ✓ | ✓ |   |
| Vista previa | ✓ | ✓ | ✓ | ✓ | ✓ |
|  Proof | ✓ | ✓ | ✓ | ✓ |   |
| Generar prueba | ✓ | ✓ |   |   |   |
| Eliminar prueba | ✓ | ✓ | ✓ | ✓ |   |
| Agregar/eliminar&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Cambiar nombre&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Vínculo (con integración) | ✓ | ✓ | ✓ | ✓ |   |
| Desvincular (con integración) | ✓ | ✓ | ✓ | ✓ |   |

{style=&quot;table-layout:auto&quot;}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Disponible sólo para carpetas de documentos, no documentos

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
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, eliminar, desactivar, iniciar sesión como o restablecer la contraseña de cualquier usuario de un grupo que administre</td> 
   <td>✓*</td> 
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

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

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
   <td>Editar equipos en los que se encuentran</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar equipos en grupos que administran</td> 
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

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Plantillas

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear | ✓&#42; |   |   |   |   |
| Eliminar | ✓&#42; |   |   |   |   |
| Compartir | ✓&#42; |   |   |   |   |
| Compartir en todo el sistema | ✓&#42; |   |   |   |   |
| Vista | ✓&#42; |   |   |   |   |
| Copiar | ✓ |   |   |   |   |
| Editar detalles de plantilla | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Datos financieros

Solo los usuarios con una licencia del Plan pueden tener acceso completo a los datos financieros.

Los tipos de licencia Solicitud y Usuario externo no se incluyen aquí porque no tienen acceso a [seleccionar objeto o área].

| Acción | Planificador | Trabajador | Revisor |
|---|---|---|---|
| Editar facturación de funciones y tasas de coste | ✓&#42; |   |   |
| Editar la facturación y las tasas de coste de los usuarios | ✓&#42; |   |   |
| Ver facturación de funciones y tasas de coste | ✓&#42; |   |   |
| Ver la facturación y las tasas de coste de los usuarios | ✓&#42; |   |   |
| Administrar registros de facturación | ✓ |   |   |
| Administrar gastos | ✓ | ✓ |   |
| Ver datos financieros | ✓&#42; | ✓&#42; | ✓&#42; |
| Ver información por costo en las herramientas de planificación de recursos | ✓ |   |   |
| Recursos presupuestarios en las herramientas de planificación de recursos&#42;&#42; | ✓ |   |   |
| Ver la asignación de recursos en las herramientas de planificación de recursos&#42; | ✓ | ✓ | ✓ |
| Crear riesgos en proyectos | ✓ |   |   |
| Ver riesgos en proyectos | ✓ | ✓ | ✓ |

{style=&quot;table-layout:auto&quot;}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requiere acceso adicional a Administración de recursos.

## Administración de recursos

Solo los usuarios con una licencia del Plan pueden tener acceso completo a [seleccionar objeto o área]. Otros tipos de licencia pueden tener acceso limitado o no disponible a Resource Management en Workfront.

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Editar prioridades y horas presupuestadas en el Planificador | ✓&#42; |   |   |   |   |
| Crear, editar y eliminar grupos de recursos&#42;&#42; | ✓&#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| Ver las prioridades del proyecto en el planificador de recursos | ✓&#42; |   |   |   |   |
| Ver la asignación de recursos en las herramientas de planificación de recursos | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Ver grupos de recursos | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Recursos presupuestarios en las herramientas de planificación de recursos&#42;&#42; | ✓ |   |   |   |   |
| Adjuntar grupos de recursos a proyectos, plantillas y usuarios | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Con un nivel de acceso, los administradores de Workfront pueden deshabilitar o habilitar esta funcionalidad. Para obtener más información, consulte [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requiere acceso adicional a Datos financieros y permisos para las finanzas de los proyectos. Si concede acceso a la Administración de Recursos a un usuario de Planificador que no tenga acceso a Datos Financieros, el usuario podrá seguir viendo las asignaciones por hora en el Planificador de Recursos, pero no podrá cambiar a la vista Costes ni ver el Caso de Negocio. Para obtener más información, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) y [Compartir permisos financieros en un objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Requiere permiso para contribuir al objeto, con la opción para que las asignaciones estén habilitadas en Configuración avanzada. Para obtener más información, consulte la sección [Comprender los permisos heredados y la jerarquía de objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) en el artículo [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Área de Planificador de escenario

| Acción | Planificador | Trabajador | Revisor | Solicitante | Usuario externo |
|---|---|---|---|---|---|
| Crear/editar planes e iniciativas existentes | ✓ | ✓ | ✓ |   |   |
| Agregar o editar información de funciones de trabajo en planes e iniciativas&#42; | ✓ | ✓ | ✓ |   |   |
| Agregar o editar información de costo sobre planes e iniciativas&#42; | ✓ | ✓ | ✓ |   |   |
| Eliminar planes e iniciativas | ✓ | ✓ | ✓ |   |   |
| Ver escenarios en el menú principal ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ |  |   |
| Ver planes e iniciativas que el usuario creó&#42; | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Los usuarios pueden ver un plan que otro usuario creó solo si se comparte con ellos un vínculo al plan.

&#42; Para que los usuarios puedan ver los datos financieros en un plan o iniciativa, necesitan acceder a los Datos Financieros. Para obtener más información, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Área de objetivos de Workfront

| Acciones | Vista | Editar |
|---|---|---|
| Crear |   | ✓ |
| Editar / eliminar todos los objetivos |   | ✓ |
| Ver objetivos en el menú principal | ✓ | ✓ |
| Ver el área de objetivos desde un vínculo compartido | ✓ | ✓ |
| Ver todos los objetivos del sistema | ✓ | ✓ |
| Activar/desactivar/cerrar todos los objetivos |   | ✓ |
| Crear/editar/eliminar actividades |   | ✓ |
| Crear/editar/eliminar resultados |   | ✓ |
| Agregar un objetivo alineado |   | ✓ |
| Actualizar el progreso de un resultado o actividad |   | ✓ |
| Propietario de un objetivo, resultado o actividad | ✓ | ✓ |
| Comentar en un objetivo | ✓ | ✓ |
| Copiar objetivos |   | ✓ |
| Ver la sección Lista de objetivos en el panel izquierdo | ✓ | ✓ |
| Ver la sección Gráficos en el panel izquierdo | ✓ | ✓ |
| Ver la sección Alineación de objetivo en el panel izquierdo | ✓ | ✓ |

