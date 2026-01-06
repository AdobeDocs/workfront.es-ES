---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Resumen del estado de las metas en Adobe Workfront Goals
description: Los estados de la meta indican si una meta está activa y registra progreso actualmente, o si está inactiva, está esbozada o ya se ha alcanzado.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 90%

---

# Información general sobre el estado de las metas en Adobe Workfront Goals

<!--Audited: 4/2025-->

>[!NOTE]
>
>Su empresa puede optar por seguir utilizando los objetivos de Adobe Workfront si compró este paquete anteriormente. Debe hablar con el representante de su cuenta para obtener más detalles.
>
>Adobe Workfront Goals ya no se puede adquirir.
>
>Para obtener información adicional sobre el acceso a Workfront Goals, consulte [Requisitos para usar Workfront Goals](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).

<!--Old:

>[!IMPORTANT]
>
>Your organization must have the following to use the functionality described in this article:
>
>* For the new plan and license structure:
>
>   * The Ultimate Workfront plan 
>    
>* For the current plan and license structure: 
>
>   * A Pro or higher Workfront plan
>   * An Adobe Workfront Goals license in addition to a Workfront license.
>
>Contact your Workfront account manager to learn about a Workfront Goals license.    
> 
>For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).   -->

## Consideración al actualizar estados de las metas en Workfront Goals

* No puede actualizar manualmente el estado de las metas que ha creado o que se han compartido con usted. El estado de las metas se actualiza según las acciones que realice en la meta. Por ejemplo, al activar una meta, el estado Borrador cambia a Activo.
* Existen algunas restricciones y, a veces, no se puede cambiar el estado de una meta a otro estado, según las siguientes reglas:

  | Desde/Hasta | Borrador | Activo | Inactivo | Cerrado |
  |---|---|---|---|---|
  | Borrador | - | Sí | No | No |
  | Activo | No | - | Sí | Sí |
  | Inactivo | No | Sí | - | No |
  | Cerrado | No | Sí | No | - |

* Al abrir una meta cerrada también se actualiza su progreso.
* Ciertas acciones que realiza en una meta también actualizan su estado. Para obtener información sobre cómo actualizar los estados de objetivos, consulte los siguientes artículos:

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
* Workfront Goals no registra el progreso en un objetivo en borrador.
* No puede actualizar el progreso de un objetivo en borrador.
* No puede cerrar ni desactivar las metas esbozadas porque carecen de información de progreso.
* Las metas redactadas no contribuyen al cálculo del progreso de otras metas y no se tienen en cuenta en los gráficos.
* Las metas en borrador se muestran en las siguientes áreas de Workfront Goals:

   * Lista de metas
   * Sección de alineación de metas (solo como un objetivo alineado)


>[!IMPORTANT]
>
>Después de cambiar el estado de una meta a cualquier otro estado, la meta nunca podrá volver a colocarse en estado de Borrador.

### Activo {#active}

* Puede activar un objetivo en borrador solo cuando lo asocia con un resultado, una actividad o alinea otro objetivo con él. Al activar la meta, su estado cambia a Activo. Para obtener información sobre cómo activar metas, consulte [Activar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
* Workfront Goals registra el progreso de las metas activas.
* Las metas activas contribuyen al cálculo del progreso de otras metas y se tienen en cuenta en los gráficos.
* Las metas activas se muestran en las siguientes áreas de Workfront Goals:

   * Lista de metas
   * Sección Alineación de metas
   * El progreso de las metas activas se muestra en gráficos

* Puede volver a activar una meta cerrada o inactiva.

### Inactivo {#inactive}

* Puede desactivar una meta activa cuando el propietario haya dejado de trabajar en ella de forma temporal o permanente. Puede guardarla para obtener información histórica. Esto actualiza el estado de la meta a Inactiva.

  Para obtener información acerca de cómo desactivar metas, consulte la sección “Desactivar metas” en el artículo [Eliminar y desactivar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* No se puede desactivar una meta esbozada o cerrada.
* Puede reactivar una meta inactiva y continuar trabajando en ella.
* Workfront Goals no calcula el progreso de las metas inactivas.
* No se puede actualizar el progreso de una meta inactiva.
* Las metas inactivas no contribuyen al cálculo del progreso de otras metas y no se tienen en cuenta en los gráficos.
* Las metas inactivas tienen un historial de progreso porque en el pasado estaban activas, a diferencia de las metas esbozadas.
* Las metas inactivas se muestran en las siguientes áreas de Workfront Goals:

   * Lista de metas
   * Sección Alineación de metas (solo como metas alineadas)

### Cerrado {#closed}

* Puede cerrar una meta cuando desee indicar que la ha conseguido o que ya no está trabajando en ella, ni lo hará en el futuro. Para obtener información sobre cómo cerrar metas, consulte [Cerrar y volver a abrir metas en Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Si planea trabajar más adelante en una meta que aún no se ha alcanzado, le recomendamos que cambie el estado a Inactiva en lugar de a Cerrada.

* No puede cerrar metas que nunca se han activado, como las metas esbozadas.
* Puede volver a abrir una meta cerrada y continuar trabajando en ella.
* Workfront Goals deja de registrar el progreso de las metas cerradas.
* No se puede actualizar el progreso de una meta cerrada.
* Las metas cerradas se muestran en la siguiente área de Workfront Goals:

   * Lista de metas
   * Sección Alineación de metas (solo como metas alineadas)
   * La información de las metas cerradas también se tiene en cuenta en la sección Gráficos.
