---
content-type: api
navigation-topic: general-api
title: Uso del Explorador de API
description: Uso del Explorador de API
author: Becky
feature: Workfront API
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---


# Uso del Explorador de API

Al utilizar la API principal de Adobe Workfront, API Explorer es una herramienta de referencia heredada que cataloga las relaciones entre los recursos, parámetros y variables admitidos.

## Acceda al Explorador de API:

1. Utilice un explorador web para navegar hasta la página [Explorador de API](https://one.workfront.com/s/api-explorer)\
   ![](assets/mceclip1-350x149.png)

1. En la parte superior derecha del Explorador de API, seleccione el elemento Workfront deseado **Versión de API**, de forma predeterminada se selecciona la versión más actual de forma automática
1. La variable **Filtro** , se puede utilizar para filtrar los objetos enumerados por su nombre y truncará la lista de objetos mostrados en consecuencia:

   ![](assets/mceclip2-350x147.png)

   * **Campos**: Campos disponibles dentro del objeto especificado.
   * **Referencias**: Variables de referencia disponibles para el objeto especificado. Una referencia es un alias para una variable. Una vez inicializada, una referencia se puede utilizar de forma intercambiable con el nombre de la variable. Una referencia utiliza memoria inicializada.
   * **Colecciones**: Colecciones disponibles para el objeto . Las colecciones son variables que representan una relación &quot;uno a varios&quot; entre el objeto y el recurso.
   * **Buscar**: Recursos de búsqueda disponibles para el objeto . Los resultados de una búsqueda se basan en los parámetros de consulta especificados por el recurso de búsqueda en la solicitud de API.
   * **Acciones**: Acciones compatibles con el objeto. Las acciones pueden ser procedimientos simples o complejos que se ejecutan en un recurso o conjunto de recursos. Una acción determinada también puede afectar a los recursos relacionados.

1. Abra una ficha y, a continuación, haga clic en el ID de objeto para ver las variables aplicables.\
   ![](assets/approval-350x89.png)\
   Según el objeto seleccionado, se pueden aplicar las siguientes variables:

   | Variable | Definición |
   |---|---|
   | Nombre de campo | Nombre de un campo utilizado en una operación dentro de la API de Workfront. |
   | Tipo de campo | Tipo de valores que se pueden introducir en un campo específico de una tabla de datos. Los valores posibles de tipo de campo incluyen string, double, int, dateTime. |
   | Tipo enumerado | Tipo de valores que se pueden utilizar para identificar un tipo de datos. |
   | Valores posibles | Valores aceptables para el objeto. |
   | Tipo de atributo ObjCode | Atributos que se pueden utilizar para modificar la clase object. |
   | Dirección URL | Ruta de entrada que permite a la aplicación comunicarse con la API de Workfront. |
   | Argumentos | Las variables del objeto que se pueden pasar entre la aplicación y Workfront. |
   | Tipo de resultado | Tipos de datos permitidos que se pueden devolver desde un método. |
