---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Información general sobre el estado de los objetivos en los objetivos de Adobe Workfront
description: Los estados de los objetivos indican si un objetivo está activo y está registrando progresos, o si está inactivo, redactado o ya alcanzado.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Información general sobre el estado de los objetivos en los objetivos de Adobe Workfront

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>Su organización debe tener lo siguiente para utilizar la funcionalidad descrita en este artículo:
>
>* Un Pro o superior [plan de Adobe Workfront](https://www.workfront.com/plans).
>* Licencia de Adobe Workfront para objetivos además de una licencia de Workfront.
>
>Póngase en contacto con el administrador de cuentas de Workfront para obtener más información sobre una licencia de Workfront para objetivos.

Para obtener información adicional sobre el acceso a los objetivos de Workfront, consulte [Requisitos para utilizar los objetivos de Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


Los estados de los objetivos indican si un objetivo está activo y está registrando progresos, o si está inactivo, redactado o ya alcanzado.

## Consideración al actualizar estados de objetivos en objetivos de Workfront

* No puede actualizar manualmente el estado de los objetivos que ha creado o que se compartieron con usted. El estado de los objetivos se actualiza según las acciones que realice en el objetivo. Por ejemplo, al activar un objetivo, se cambia el estado Borrador a Activo.
* Existen algunas restricciones y, a veces, no se puede cambiar el estado de un objetivo a otro estado, según las siguientes reglas:

   | De/ a | Borrador | Activo | Inactivo | Cerrado |
   |---|---|---|---|---|
   | Borrador | - | Sí | No | No |
   | Activo | No | - | Sí | Sí |
   | Inactivo | No | Sí | - | No |
   | Cerrado | No | Sí | No | - |

* Abrir un objetivo cerrado también actualiza el progreso del objetivo.
* Algunas acciones que realiza en un objetivo también actualizan su estado. Para obtener información sobre cómo actualizar los estados de objetivos, consulte los siguientes artículos:

   * [Crear objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
   * [Activar objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Eliminar y desactivar objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Cierre y vuelva a abrir los objetivos en Objetivos de Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Información general sobre los estados de objetivos en los objetivos de Workfront

Para obtener información sobre la creación de objetivos de Workfront, consulte [Crear objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Para obtener información sobre la activación de objetivos, consulte [Activar objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Los objetivos pueden tener uno de los siguientes estados en los objetivos de Workfront:

* [Borrador](#draft)
* [Activo](#active)
* [Inactivo](#inactive)
* [Cerrado](#closed)

### Borrador {#draft}

* Este es el estado predeterminado de un objetivo recién creado. Para obtener información sobre la creación de objetivos, consulte [Crear objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Los objetivos de Workfront no registran los progresos realizados en un objetivo redactado.
* No se puede actualizar el progreso de un objetivo redactado.
* Los objetivos redactados no se pueden cerrar ni desactivar porque carecen de información de progreso.
* Los objetivos redactados no contribuyen al cálculo del progreso de otros objetivos y no se tienen en cuenta en gráficos.
* Los objetivos redactados se muestran en las siguientes áreas de los objetivos de Workfront:

   * Lista de metas
   * Sección Alineación de objetivos (solo como objetivo alineado)


>[!IMPORTANT]
>
>Después de cambiar el estado de un objetivo a cualquier otro estado, el objetivo nunca se puede volver a colocar en el estado Borrador.

### Activo {#active}

* Solo puede activar un objetivo redactado si lo asocia a un resultado, a una actividad o si alinea otro objetivo con él. Al activar el objetivo, su estado cambia a Activo. Para obtener información sobre la activación de objetivos, consulte [Activar objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Los objetivos de Workfront registran el progreso en los objetivos activos.
* Los objetivos activos contribuyen al cálculo del progreso de otros objetivos y se tienen en cuenta en gráficos.
* Los objetivos activos se muestran en las siguientes áreas de los objetivos de Workfront:

   * Lista de metas
   * Sección Alineación de objetivos
   * El progreso de los objetivos activos se muestra en gráficos

* Puede reactivar un objetivo Cerrado o Inactivo.

### Inactivo {#inactive}

* Puede desactivar un objetivo activo cuando el propietario haya dejado de trabajar en él de forma temporal o permanente. Puede conservarlo para información histórica. Esto actualiza el estado del objetivo a Inactivo.

   Para obtener información sobre cómo desactivar objetivos, consulte la sección &quot;Desactivar objetivos&quot; en el artículo [Eliminar y desactivar objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* No se puede desactivar un objetivo redactado o cerrado.
* Puede reactivar un objetivo inactivo y seguir trabajando en él.
* Los objetivos de Workfront no calculan el progreso en objetivos inactivos.
* No se puede actualizar el progreso de un objetivo inactivo.
* Los objetivos inactivos no contribuyen al cálculo del progreso de otros objetivos y no se tienen en cuenta en los gráficos.
* Los objetivos inactivos tienen un historial de progreso porque alguna vez fueron activos, a diferencia de los objetivos redactados.
* Los objetivos inactivos se muestran en las siguientes áreas de los objetivos de Workfront:

   * Lista de metas
   * Sección Alineación de objetivos (solo como objetivos alineados)

### Cerrado {#closed}

* Puede cerrar un objetivo cuando desee indicar que lo ha alcanzado o que ya no está trabajando en él, o que lo hará en el futuro. Para obtener información acerca de los objetivos de cierre, consulte [Cierre y vuelva a abrir los objetivos en Objetivos de Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >Si planea trabajar más adelante en un objetivo que aún no se ha alcanzado, le recomendamos que cambie el estado a Inactivo en lugar de Cerrado.

* No se pueden cerrar objetivos que nunca se han activado, como objetivos redactados.
* Puede volver a abrir un objetivo cerrado y seguir trabajando en él.
* Los objetivos de Workfront dejan de registrar el progreso en objetivos cerrados.
* No se puede actualizar el progreso de un objetivo cerrado.
* Los objetivos cerrados se muestran en la siguiente área de Objetivos de Workfront:

   * Lista de metas
   * Sección Alineación de objetivos (solo como objetivos alineados)
   * La información de objetivos cerrados también se tiene en cuenta en la sección Gráficos .
