---
filename: api-changes-search
content-type: api
keywords: objeto, estado, búsqueda, práctica, respuesta
navigation-topic: api-navigation-topic
title: "Cambios de la API principal: respuestas de búsqueda de estado"
description: Cambios en la forma en que Workfront almacena los objetos de estado.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# Cambios en la API principal: Respuestas de búsqueda de estado

Se han realizado cambios en la forma en que Workfront almacena los objetos de estado. Estos cambios no afectan a cómo se realizan las solicitudes de búsqueda de estado, pero afectarán a la respuesta devuelta por las solicitudes de API que incluyen una búsqueda de objetos de estado al devolver una lista incompleta de estados de grupo.

## Prácticas recomendadas

Para obtener de forma fiable la lista completa de estados disponibles para un grupo, se consideran prácticas recomendadas las siguientes solicitudes.

>[!NOTE]
>
>Se recomiendan estas estructuras de solicitud para todos los usuarios independientemente de si se han realizado o no cambios en la búsqueda de estado en el clúster.

Para Estado De Grupo De Proyecto:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Para Estado Del Grupo De Tareas:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Para Estado De Grupo De Problemas:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Los tres extremos aceptan el **includeHidden=true** para recuperar los estados ocultos de proyecto, tarea o problema de un grupo determinado. Modelar las consultas de búsqueda de estado después de estos ejemplos de prácticas recomendadas garantizará que toda la información de estado del grupo se incluya en cada respuesta.

A continuación se muestra un ejemplo de una consulta de búsqueda de estado realizada a un grupo de tareas que incluye un estado bloqueado de nivel de sistema **Custom_1** y un estado desbloqueado **Personalizado_2**:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

El uso de este formato garantiza que la respuesta incluya todo lo siguiente:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Explicación de los cambios realizados en la consulta de búsqueda de estado heredada

En el sistema heredado, una consulta de búsqueda de estado copiaría todos los estados del sistema disponibles para todos los grupos incluidos en una consulta. La respuesta heredada entonces incluiría todos los estados del sistema y los estados de nivel de grupo disponibles para cada grupo en la consulta.

Por ejemplo, esta consulta (que no sigue las prácticas recomendadas actuales):

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Tendría la siguiente respuesta en el sistema heredado, que incluye todos los estados de objetos:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

Sin embargo, tras las actualizaciones realizadas sobre la forma en que se almacenan y utilizan los estados, los estados no se copian para los grupos y los hereda cada grupo en el sistema. Como resultado, la consulta de la API de búsqueda solo lee los estados que están directamente asociados con un grupo en particular, por lo que la respuesta incluye los estados bloqueado por el sistema y desbloqueado, pero solo para los grupos que se crearon después de agregar el estado en cuestión.

Si no se utilizan los métodos de prácticas recomendadas actualizados para realizar consultas de búsqueda de estado después de actualizar el sistema heredado, se devolverá una lista incompleta de los estados de grupo en la respuesta.

A continuación, se muestra un ejemplo de lo que devuelve esta estructura de solicitud obsoleta después de actualizar el sistema heredado:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Tenga en cuenta que esta respuesta solo incluye estados específicos del grupo y excluye los estados que se declararon en el nivel del sistema:

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
