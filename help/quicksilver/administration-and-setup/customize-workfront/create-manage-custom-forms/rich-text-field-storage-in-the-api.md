---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Almacenamiento de campos de texto enriquecido en la API
description: Si un objeto, como un proyecto, un problema o una tarea, contiene texto enriquecido, se almacena y se puede acceder a él como un valor de parámetro a través de la API de Workfront.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
TQID: https://experienceleague.adobe.com/lLZZugNI5odziqyz7uBMnkiVoOdGcT-jKb90j9TUG1Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 95%

---

# Almacenamiento de campo de texto enriquecido en la API

Si un objeto, como un proyecto, un problema o una tarea, contiene texto enriquecido, se almacena y se puede acceder a él como un valor de parámetro a través de la API de Workfront.

La solicitud de información de texto de un objeto de proyecto que contiene texto enriquecido se puede realizar utilizando el campo **parameterValues**.

Por ejemplo, una petición HTTP simple podría parecerse a la siguiente:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Si este proyecto de ejemplo contenía un formulario personalizado con 3 campos personalizados: campo de cálculo, texto de párrafo y 1 enriquecido. ¡Entonces la petición anterior devolvería una respuesta parecida a la siguiente, donde el campo &quot;rich 1&quot; es un campo de parámetro de texto enriquecido y el valor de texto es “**¡Hola,** *mundo!*”:

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
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
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

Para obtener información más detallada sobre cómo se almacena la información de texto enriquecido y cómo se puede recuperar mediante la API de Adobe Workfront, consulte [Campos de texto enriquecido en la API de Adobe Workfront](../../../wf-api/general/rich-text-field-api.md).
