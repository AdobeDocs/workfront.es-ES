---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Añadir opciones de corrección avanzadas con la API de Adobe Workfront
description: Añadir opciones de corrección avanzadas con la API de Adobe Workfront
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---


# Añada opciones avanzadas de revisión al crear una prueba a través de la API de Adobe Workfront

Al crear una prueba en la API de Workfront, puede añadir opciones de prueba avanzadas.

Utilice uno de los siguientes flujos de trabajo para añadir opciones de prueba a una prueba mediante la API:

* (Recomendado) Cree una prueba sencilla con la API de Workfront y luego añada opciones de prueba avanzadas a la prueba con la API de ProofHQ

* Cree una prueba con opciones de prueba avanzadas con JSON en la API de Workfront

## Cree una prueba con las API de Workfront y ProofHQ (recomendado) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

En esta sección se describe cómo crear una prueba con opciones de prueba avanzadas a través de la API de Workfront, utilizando una combinación de las API de Workfront y ProofHQ.

La API de ProofHQ incluye diversas acciones que no están disponibles para las pruebas en la API de Workfront. Con estas acciones, puede modificar o configurar la prueba con más precisión de la que está disponible en la API de Workfront.

Para obtener una descripción general de la API de ProofHQ, consulte la [Información general de ProofHQ](../../proofhq-api/general/overview.md). También puede consultar la [Documentación de ProofHQ](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* La API de Workfront es una API completa de REST. La API de ProofHQ es una API de SOAP.
>* Las pruebas creadas en la API de ProofHQ no se vinculan automáticamente a Workfront. Por lo tanto, se recomienda crear pruebas en la API de Workfront antes de actualizarlas con la API de ProofHQ.
>

### Creación de una prueba con opciones avanzadas de revisión

1. Cree una prueba con la variable `Document createProof` acción en la API de Workfront.

   >[!NOTE]
   >
   Al crear la prueba, establezca `{}` como el valor de `advancedProofingOptions` parámetro.

1. Una vez creada la prueba, utilice la API de ProofHQ para agregar opciones avanzadas.

### Ejemplos

Esta sección muestra algunas actualizaciones de ejemplo que puede realizar con la API de ProofHQ.

**Ejemplos:**

* [Una prueba se puede descargar, tiene un mensaje y se comparte públicamente](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Actualice una fase para que no sea privada, no obligatoria y requiera solo una aprobación](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Añadir dos destinatarios a una prueba sin el responsable principal de la toma de decisiones](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Una prueba se puede descargar, tiene un mensaje y se comparte públicamente**

La documentación de este extremo se encuentra en la [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) página.

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

**Actualice una fase para que no sea privada, no obligatoria y requiera solo una aprobación**

La documentación de este extremo se encuentra en la [API de ProofHQ updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) página.

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

**Añadir dos destinatarios a una prueba sin el responsable principal de la toma de decisiones**

La documentación de este extremo se encuentra en la [API de ProofHQ addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) página.

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

## Cree una prueba con JSON en la API de Workfront

En esta sección se describe cómo crear una prueba con opciones de prueba avanzadas a través de la API de Workfront, utilizando JSON como valor de parámetro en la API de Workfront

### Creación de una prueba con opciones avanzadas de revisión

Puede crear pruebas a través de la API de Workfront utilizando `Document createProof` acción. Esta acción acepta la variable `advancedProofingOptions` parámetro, que tiene el tipo de valor `string`. Para incluir opciones de revisión avanzadas en su `createProof` acción, debe introducir las opciones en la variable `advancedProofingOptions` en formato JSON.

>[!NOTE]
>
Puede ser difícil predecir los campos que se incluirán en el JSON advancedProofingOptions. Es posible que desee examinar los datos de red de su organización mientras utiliza la revisión avanzada en Workfront y basar el JSON en los campos y valores que suele utilizar su organización.
>
Dado que estos campos pueden ser difíciles de predecir, se recomienda crear una prueba con la API de Workfront y luego actualizarla con la API de ProofHQ. Para obtener más información, consulte [Cree una prueba con las API de Workfront y ProofHQ (recomendado)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) en este artículo

### Ejemplo

Este ejemplo muestra los campos y el formato que puede utilizar al crear su JSON para la `advancedProofingOptions` parámetro. Su `advancedProofingOptions` El archivo JSON puede tener más o menos campos de los que se muestran aquí.

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
