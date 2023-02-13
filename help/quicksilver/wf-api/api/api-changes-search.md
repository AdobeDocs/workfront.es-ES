---
filename: api-changes-search
content-type: api
keywords: objeto,estado,búsqueda,mejor,práctica,respuesta
navigation-topic: api-navigation-topic
title: '''Cambios en la API principal: Respuestas de búsqueda de estado'
description: Cambios en la forma en que Workfront almacena los objetos de estado.
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# Cambios en las API principales: Respuestas de búsqueda de estado

Se han realizado cambios en la forma en que Workfront almacena los objetos de estado. Estos cambios no afectan a cómo se realizan las solicitudes de búsqueda de estado, pero sí afectan a la respuesta que devuelven las solicitudes de API que incluyen una búsqueda de objetos de estado devolviendo una lista incompleta de estados de grupo.

## Prácticas recomendadas

Para obtener de forma fiable la lista completa de los estados disponibles para un grupo, las siguientes solicitudes se consideran prácticas recomendadas.

>[!NOTE]
>
>Estas estructuras de solicitud se recomiendan para todos los usuarios independientemente de si se han realizado o no cambios en la búsqueda de estado en el clúster.

Para el estado del grupo de proyectos:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Para el estado del grupo de tareas:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Para el estado del grupo de problemas:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Los tres extremos aceptan la variable **includeHidden=true** para recuperar los estados ocultos de proyecto/tarea/problema de un grupo determinado. Al modelar las consultas de búsqueda de estado después de estos ejemplos de prácticas recomendadas, se asegurará de que toda la información de estado de grupo se incluya en cada respuesta.

Este es un ejemplo de una consulta de búsqueda de estado que se realiza a un grupo de tareas que incluye un estado bloqueado a nivel de sistema **Personalizado_1** y un estado desbloqueado **Personalizado_2**:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

El uso de este formato garantiza que la respuesta incluya lo siguiente:

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

## Explicación de los cambios realizados en la consulta de búsqueda de estado heredado

En el sistema heredado, una consulta de búsqueda de estado copiaría todos los estados del sistema disponibles para todos los grupos incluidos en una consulta. La respuesta heredada entonces incluiría todos los estados del sistema y los estados de nivel de grupo disponibles para cada grupo en la consulta.

Por ejemplo, esta consulta (que no sigue las prácticas recomendadas actuales):

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Tendría la siguiente respuesta en el sistema heredado, que incluye todos los estados de objeto:

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

Sin embargo, tras las actualizaciones realizadas en la forma en que se almacenan y usan los estados, estos no se copian para grupos y cada grupo los hereda a nivel del sistema. Como resultado, la consulta de la API de búsqueda solo lee los estados que están directamente asociados a un grupo en particular, por lo que la respuesta incluye los estados bloqueados y desbloqueados del sistema, pero solo para los grupos que se crearon después de agregar el estado en cuestión.

Si no se utilizan los métodos de prácticas recomendadas actualizados para realizar consultas de búsqueda de estado después de actualizar el sistema heredado, se devolverá una lista incompleta de estados de grupo en la respuesta.

Este es un ejemplo de lo que devuelve esta estructura de solicitud obsoleta después de actualizar el sistema heredado:

>**Ejemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Tenga en cuenta que esta respuesta solo incluye estados específicos de grupo y excluye aquellos estados declarados a nivel de sistema:

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
