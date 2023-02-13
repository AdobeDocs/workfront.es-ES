---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Cargar documentos y pruebas desde el [!DNL Adobe Workfront plugin] a [!DNL Creative Cloud]
description: Cargar documentos y pruebas desde el [!DNL Adobe Workfront plugin] a [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Cargar documentos y pruebas desde el [!DNL Adobe Workfront plugin] a [!DNL Creative Cloud]

Puede cargar sus proyectos como documentos para una revisión y aprobación rápidas o simplemente para almacenarlos en [!DNL Adobe Workfront].

>[!NOTE]
>
>Actualmente, Premiere Pro y After Effects no admiten la carga de documentos y pruebas.


## Limitaciones de documentos

Esta sección describe las limitaciones conocidas de los documentos en la sección [!DNL Workfront for Adobe Creative Cloud plugins].

### Las nuevas versiones de los documentos solo aceptan un archivo para su carga

Porque [!DNL Workfront] los documentos no pueden contener varios archivos, ciertos ajustes deben deshabilitarse para poder cargar las nuevas versiones del documento en Workfront.

>[!NOTE]
>
>Si debe generar varios archivos, puede crear una prueba en su lugar. La nueva prueba no se asociará con el documento original.



Para volver a cambiar el conmutador a un solo archivo en [!DNL InDesign]:

1. Abra el **Definir configuración de archivo de exportación** para abrir el Navegador.

   ![](assets/file-export-settings.png)

1. Busque el tipo de recurso que desea exportar y ajuste la configuración como se describe a continuación:

   <table>
    <tr>
    <td><strong>PDF y PDF IMPRIMIR</strong>
    </td>
    <td>Anular selección <strong>Crear archivos de PDF separados</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Select <strong>Intervalos</strong> y escriba un solo número de página. 
    <p>
    <strong>Nota</strong>: Si desea cargar el documento completo, debe crear una prueba. 
    </td>
    </tr>
    <tr>
    <td><strong>ePub y EPUB FIJO</strong>
    </td>
    <td>No es necesario realizar ajustes.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>No es necesario realizar ajustes.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>Select <strong>Intervalos</strong> y escriba un solo número de página. 
    <p>
    <strong>Nota</strong>: Si desea cargar el documento completo, debe crear una prueba. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Select <strong>Intervalos</strong> y escriba un solo número de página. 
    <p>
    <strong>Nota</strong>: Si desea cargar el documento completo, debe crear una prueba. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>No es necesario realizar ajustes. 
    </td>
    </tr>
    </table>
