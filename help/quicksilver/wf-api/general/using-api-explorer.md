---
content-type: api
navigation-topic: general-api
title: Uso del Explorador de API
description: Uso del Explorador de API
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 97%

---


# Uso del Explorador de API

Al utilizar la API principal de Adobe Workfront, el Explorador de API es una herramienta de referencia heredada que cataloga las relaciones entre los recursos compatibles, los parámetros y las variables.

## Acceso al Explorador de API:

1. Use un explorador web para navegar hasta [Explorador de API](https://developer.adobe.com/workfront/api-explorer/)\
   ![Vaya al Explorador de API](assets/mceclip1-350x149.png)

1. En la parte superior derecha del Explorador de API, seleccione la **Versión de API** de Workfront que desee; de manera predeterminada, se selecciona automáticamente la versión más actual
1. El campo **Filtrar** se puede usar para filtrar los objetos enumerados por nombre y truncará en consencuencia la lista de objetos mostrados:

   ![Campos del Explorador de API](assets/mceclip2-350x147.png)

   * **Campos**: campos disponibles dentro del objeto especificado.
   * **Referencias**: variables de referencia disponibles para el objeto especificado. Una referencia es un alias para una variable. Una vez inicializada, se puede utilizar una referencia indistintamente con el nombre de la variable. Una referencia utiliza memoria inicializada.
   * **Colecciones**: colecciones disponibles para el objeto. Las colecciones son variables que representan una relación &quot;uno a varios&quot; entre el objeto y el recurso.
   * **Buscar**: recursos de búsqueda disponibles para el objeto. Los resultados de una búsqueda se basan en los parámetros de consulta especificados por el recurso de búsqueda en la solicitud de API.
   * **Acciones**: acciones compatibles con el objeto. Las acciones pueden ser procedimientos simples o complejos que se ejecutan con un recurso o un conjunto de recursos. Una acción determinada también puede afectar a los recursos relacionados.

1. Abra una pestaña y, a continuación, haga clic en el ID de objeto para ver las variables aplicables.\
   ![Ver variables](assets/approval-350x89.png)\
   Según el objeto seleccionado, pueden aplicarse las siguientes variables:

   | Variable | Definición |
   |---|---|
   | Nombre de campo | Nombre de un campo utilizado en una operación dentro de la API de Workfront. |
   | Tipo de campo | Tipo de valores que se pueden introducir en un campo específico de una tabla de datos. Los posibles valores de tipo de campo incluyen string, double, int y dateTime. |
   | Tipo enumerado | El tipo de valores que se pueden utilizar para identificar un tipo de datos. |
   | Valores posibles | Valores aceptables para el objeto. |
   | Tipo de atributo ObjCode | Atributos que se pueden utilizar para modificar la clase de objeto. |
   | URL | Ruta de entrada que permite a la aplicación comunicarse con la API de Workfront. |
   | Argumentos | Las variables del objeto que se pueden pasar entre la aplicación y Workfront. |
   | Tipo de resultado | Tipos de datos permitidos que se pueden devolver desde un método. |
