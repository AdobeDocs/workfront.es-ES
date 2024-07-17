---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Información general sobre el estado de las metas en Adobe Workfront Goals
description: Los estados de objetivo indican si una meta está activa y registra progreso actualmente, o si está inactiva, está redactada o ya se ha alcanzado.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 4%

---

# Información general sobre el estado de las metas en Adobe Workfront Goals

Su organización debe tener lo siguiente para utilizar la funcionalidad descrita en este artículo:

* Para el nuevo plan y la estructura de licencias:

   * Un plan definitivo

     O

     Licencia adicional para objetivos de Adobe Workfront para los planes Prime o Select Adobe Workfront. Para obtener más información, consulte [plan de Adobe Workfront](https://www.workfront.com/plans).

* Para el plan y la estructura de licencias actuales:

   * A Pro o superior
   * Una licencia de Adobe Workfront Goals además de una licencia de Workfront.

Póngase en contacto con el administrador de cuentas de Workfront para obtener más información sobre una licencia de Workfront Goals.

Los estados de objetivo indican si una meta está activa y registra progreso actualmente, o si está inactiva, está redactada o ya se ha alcanzado.

## Consideración al actualizar estados de objetivos en Workfront Goals

* No puede actualizar manualmente el estado de las metas que ha creado o que se han compartido con usted. El estado de las metas se actualiza según las acciones que realice en la meta. Por ejemplo, al activar un objetivo, el estado del borrador cambia a Activo.
* Existen algunas restricciones y, a veces, no se puede cambiar el estado de un objetivo a otro estado, según las siguientes reglas:

  | Desde/ hasta | Borrador | Activo | Inactivo | Cerrado |
  |---|---|---|---|---|
  | Borrador | - | Sí | No | No |
  | Activo | No | - | Sí | Sí |
  | Inactivo | No | Sí | - | No |
  | Cerrado | No | Sí | No | - |

* Abrir una meta cerrada también actualiza el progreso de la meta.
* Ciertas acciones que realiza en una meta también actualizan su estado. Para obtener información sobre cómo actualizar los estados de objetivos, consulte los siguientes artículos:

   * [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md)
   * [Activar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md)
   * [Eliminar y desactivar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Cerrar y volver a abrir metas en Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Información general sobre los estados de objetivos en Workfront Goals

Para obtener información sobre cómo crear metas de Workfront Goals, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

Para obtener información sobre cómo activar metas, consulte [Activar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

Las metas pueden tener uno de los siguientes estados en Workfront Goals:

* [Borrador](#draft)
* [Activo](#active)
* [Inactivo](#inactive)
* [Cerrado](#closed)

### Borrador {#draft}

* Este es el estado predeterminado de una meta recién creada. Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
* Los objetivos de Workfront no registran el progreso en un objetivo esbozado.
* No se puede actualizar el progreso de un objetivo esbozado.
* No puede cerrar ni desactivar las metas esbozadas porque carecen de información de progreso.
* Los objetivos redactados no contribuyen al cálculo del progreso de otros objetivos y no se tienen en cuenta en los gráficos.
* Los objetivos esbozados se muestran en las siguientes áreas de Workfront Goals:

   * Lista de metas
   * Sección Alineación de metas (solo como una meta alineada)


>[!IMPORTANT]
>
>Después de cambiar el estado de una meta a cualquier otro estado, la meta nunca podrá volver a colocarse en estado de Borrador.

### Activo {#active}

* Solo puede activar una meta esbozada cuando la asocia a un resultado, a una actividad o cuando le alinea otra meta. Al activar la meta, su estado cambia a Activo. Para obtener información sobre cómo activar metas, consulte [Activar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
* Workfront Goals registra el progreso de las metas activas.
* Las metas activas contribuyen al cálculo del progreso de otras metas y se tienen en cuenta en los gráficos.
* Los objetivos activos se muestran en las siguientes áreas de Workfront Goals:

   * Lista de metas
   * Sección Alineación de metas
   * El progreso de las metas activas se muestra en gráficos

* Puede volver a activar una meta cerrada o inactiva.

### Inactivo {#inactive}

* Puede desactivar un objetivo activo cuando el propietario haya dejado de trabajar en él de forma temporal o permanente. Puede guardarlo para obtener información histórica. Esto actualiza el estado de la meta a Inactiva.

  Para obtener información acerca de cómo desactivar metas, consulte la sección &quot;Desactivar metas&quot; en el artículo [Eliminar y desactivar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* No se puede desactivar un objetivo esbozado o cerrado.
* Puede reactivar una meta inactiva y continuar trabajando en ella.
* Workfront Goals no calcula el progreso de las metas inactivas.
* No se puede actualizar el progreso de un objetivo inactivo.
* Las metas inactivas no contribuyen al cálculo del progreso de otras metas y no se tienen en cuenta en los gráficos.
* Las metas inactivas tienen un historial de progreso porque, en el pasado, estaban activas, a diferencia de las metas esbozadas.
* Los objetivos inactivos se muestran en las siguientes áreas de Workfront Goals:

   * Lista de metas
   * Sección Alineación de metas (solo como metas alineadas)

### Cerrado {#closed}

* Puede cerrar un objetivo cuando desee indicar que lo ha conseguido o que ya no está trabajando en él, ni lo hará en el futuro. Para obtener información sobre cómo cerrar metas, vea [Cerrar y volver a abrir metas en Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Si planea trabajar más adelante en un objetivo que aún no se ha alcanzado, le recomendamos que cambie el estado a Inactivo en lugar de a Cerrado.

* No puede cerrar metas que nunca se han activado, como las metas esbozadas.
* Puede volver a abrir una meta cerrada y continuar trabajando en ella.
* Workfront Goals deja de registrar el progreso de las metas cerradas.
* No se puede actualizar el progreso de una meta cerrada.
* Las metas cerradas se muestran en la siguiente área de las metas de Workfront:

   * Lista de metas
   * Sección Alineación de metas (solo como metas alineadas)
   * La información de las metas cerradas también se tiene en cuenta en la sección Gráficos.
