---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Añadir opciones de revisión avanzadas con la API de Adobe Workfront
description: Añadir opciones de revisión avanzadas con la API de Adobe Workfront
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
TQID: https://experienceleague.adobe.com/EQ1zHPVOqW-2yZU8pvPTmBJ-q-PMKotGBuDB1G7hc7A
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 614
ht-degree: 100%

---

# Añada opciones avanzadas de revisión al crear pruebas a través de la API de Adobe Workfront

Al crear revisiones en la API de Workfront, es posible añadir opciones de revisión avanzadas.

Use uno de los siguientes flujos de trabajo para añadir opciones de revisión a una prueba mediante la API:

* (Recomendado) Cree una prueba sencilla con la API de Workfront y, a continuación, añada opciones de revisión avanzadas a la prueba con la API de ProofHQ

* Crear una revisión con opciones de revisión avanzadas con JSON en la API de Workfront

## Crear una prueba con las API de Workfront y ProofHQ (recomendado) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

En esta sección se describe cómo crear una prueba con opciones de revisión avanzadas con la API de Workfront mediante una combinación de las API de Workfront y ProofHQ.

La API de ProofHQ incluye diversas acciones que no están disponibles para las pruebas en la API de Workfront. Con estas acciones es posible modificar o configurar la prueba con más precisión que la que hay disponible en la API de Workfront.

Para obtener información general sobre la API de ProofHQ, consulte la [Información general sobre ProofHQ](../../proofhq-api/general/overview.md). También se puede consultar la [Documentación de ProofHQ](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* La API de Workfront es una API completa de REST. La API de ProofHQ es una API de SOAP.
>* Las pruebas creadas en la API de ProofHQ no se vinculan automáticamente a Workfront. Por lo tanto, se recomienda crear pruebas en la API de Workfront antes de actualizarlas con la API de ProofHQ.
>

### Creación de pruebas con opciones avanzadas de revisión

1. Creación de una prueba con la acción `Document createProof` en la API de Workfront.

   >[!NOTE]
   >
   >Al crear la prueba, establezca `{}` como el valor del parámetro `advancedProofingOptions`.

1. Una vez creada la prueba, use la API de ProofHQ para añadir opciones avanzadas.

### Ejemplos

En esta sección se muestran algunas actualizaciones de ejemplo que se pueden realizar con la API de ProofHQ.

**Ejemplos:**

* [Se puede descargar una prueba, contiene un mensaje y se comparte públicamente](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Actualice una fase para que no sea privada ni obligatoria y requiera solamente una aprobación](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Añadir dos destinatarios a una prueba sin responsable de toma de decisiones principal](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Se puede descargar una prueba, contiene un mensaje y se comparte públicamente**

La documentación de este punto final se encuentra en la página [updateProof de la API de ProofHQ](https://api.proofhq.com/home/proofs/updateproof.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**Actualice una fase para que no sea privada ni obligatoria y requiera solamente una aprobación**

La documentación de este punto final se encuentra en la página [updateWorkflowProofStage de la API de ProofHQ](https://api.proofhq.com/updateworkflowproofstage.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**Añadir dos destinatarios a una prueba sin responsable de toma de decisiones principal**

La documentación de este punto final se encuentra en la página [addWorkflowProofReviewers de la API de ProofHQ](https://api.proofhq.com/addworkflowproofreviewers.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Creación de una prueba con JSON en la API de Workfront

En esta sección se describe la creación de pruebas con opciones avanzadas de revisión mediante la API de Workfront, utilizando JSON como valor de parámetro en la API de Workfront

### Creación de pruebas con opciones avanzadas de revisión

Es posible crear pruebas con la API de Workfront mediante la acción `Document createProof`. Esta acción acepta el parámetro `advancedProofingOptions`, que tiene el tipo de valor `string`. Para incluir opciones de revisión avanzadas en la acción `createProof`, es necesario escribir las opciones en el parámetro `advancedProofingOptions` en formato JSON.

>[!NOTE]
>
>Puede resultar difícil predecir los campos que se incluirán en el JSON advancedProofingOptions. Es posible que quiera examinar los datos de red de su organización mientras utiliza la revisión avanzada en Workfront, así como basar el JSON en los campos y valores que suela usar la organización.
>
>Como puede resultar difícil predecir estos campos, se recomienda crear una prueba con la API de Workfront y actualizarla con la API de ProofHQ. Para obtener más información, consulte [Creación de pruebas con las API de Workfront y ProofHQ (recomendado)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) en este artículo

### Ejemplo

En este ejemplo se muestran los campos y el formato que se pueden utilizar al crear el JSON para el parámetro `advancedProofingOptions`. El archivo JSON `advancedProofingOptions` puede tener más o menos campos que los que se muestran aquí.

**Ejemplo:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
