---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Almacenamiento de campos de texto enriquecido en la API
description: Si un objeto, como un proyecto, un problema o una tarea, contiene texto enriquecido, se almacena y se puede acceder a él como un valor de parámetro a través de la API de Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Almacenamiento de campos de texto enriquecido en la API

Si un objeto, como un proyecto, un problema o una tarea, contiene texto enriquecido, se almacena y se puede acceder a él como un valor de parámetro a través de la API de Workfront.

La solicitud de información de texto de un objeto de proyecto que contenga texto enriquecido se puede realizar utilizando el campo **parameterValues**.

Por ejemplo, una solicitud HTTP simple podría parecerse a la siguiente:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Si este proyecto de ejemplo contenía un formulario personalizado con 3 campos personalizados: calc field, párrafo text y rich 1. A continuación, la solicitud anterior devolverá una respuesta similar a la siguiente, donde el campo &quot;rich 1&quot; es un campo de parámetro de texto enriquecido y el valor de texto es &quot;**Hello** *¡Mundo!*&quot;:

```
{
	Data: {
		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,
		name: “new project with rich text”,
		objCode: “PROJ”,
		- parameterValues: {
			DE:rich 1: “{
				"blocks":[
				{
					"key":"7eibh",
					"text":"Hello Word!",
					"type":"unstyled",
					"depth":0,
					"inlineStyleRanges":[
					{
						"offset":0,
						"length":6,
						"style":"BOLD"
					},
					{
						"offset":6,
						"length":5,
						"style":"ITALIC"
					}
					],
					"entityRanges":[
					],
				"data":{
				}
				}
				],
			"entityMap":{
			}
		}”,
		DE: paragraph text: “here is some paragraph text”,
		DE: calc field: “here is a calc field entry”,
		}
	}
}
```

Para obtener más información detallada sobre cómo se almacena y se puede recuperar la información de texto enriquecido a través de la API de Adobe Workfront, consulte [Campos de texto enriquecido en la API de Adobe Workfront](../../../wf-api/general/rich-text-field-api.md).
