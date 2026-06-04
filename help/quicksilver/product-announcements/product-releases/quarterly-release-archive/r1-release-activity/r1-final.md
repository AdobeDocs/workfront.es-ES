---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versión R1 final
description: Actividad de la versión 2018.3
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
TQID: https://experienceleague.adobe.com/FQZ7CAhTWmVPgaSkVIedTDIRaXtt2ekNZq5x7kjTvxc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c18d9e03-ac7d-4811-9c92-3e92ddc70ade
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1195
ht-degree: 100%

---

# Versión R1 final

Las siguientes funcionalidades no están disponibles actualmente en Vista previa o Beta, pero se lanzarán al entorno de producción en la versión R1:

## Tomar decisiones de aprobación para pruebas desde el área de Mi trabajo (Workfront)

Ahora, cuando un usuario le añade a una prueba y concede la función Aprobador o la función Revisor y aprobador (desde la aplicación independiente ProofHQ o mediante el uso del flujo de trabajo automatizado en Workfront), la solicitud de aprobación se muestra en la pestaña Aprobaciones del área Mi trabajo. A continuación, será posible consultar la prueba y tomar una decisión de aprobación directamente desde Workfront.

Para obtener información sobre cómo añadir usuarios a una prueba mediante el flujo de trabajo automatizado, consulte [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) en [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Para obtener información sobre cómo tomar decisiones de aprobación en el área Mi trabajo, consulte [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Informar sobre aprobaciones de revisión dentro del área Mi trabajo (Workfront)

Ahora puede crear un informe basado en el objeto Aprobación de pruebas. Este informe permite informar sobre las aprobaciones de pruebas desde las áreas Mi trabajo de los usuarios en las que aún no se han tomado decisiones.

Los informes de aprobación de pruebas contienen la siguiente información:

* Documento enviado para su aprobación
* Nombre del aprobador
* Versión de la prueba
* Identificador de revisión
* Fecha de creación de la prueba

Puede acceder a esta aprobación al crear un informe basado en un objeto, como se describe en [Crear un informe personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objetos de aprobaciones de pruebas, consulte la sección [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) de [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Generar automáticamente una nueva versión de una prueba de documento arrastrando y soltando (Workfront)

Al utilizar el método de arrastrar y soltar para añadir una nueva versión de un documento que requiera revisión, se genera una prueba automáticamente. La prueba tiene las mismas opciones y flujos de trabajo que la prueba original o la versión anterior.

Anteriormente, cuando se añadía una nueva versión del documento, la prueba no se generaba automáticamente en la nueva versión y había que volver a generarla para la nueva versión.

Cuando se utiliza el menú Más de Documentos para cargar una nueva versión, no se genera una prueba automáticamente.

Para obtener más información, consulte la sección en

## Habilitar todos los usuarios de revisión para acceder a ProofHQ directamente desde la interfaz de Workfront (Workfront)

Ahora puede habilitar que todos los usuarios de revisión del sistema tengan acceso sin problemas a su cuenta de ProofHQ Premium directamente desde la interfaz de Workfront. Cuando está habilitado, todos los usuarios de revisión ven un icono de ProofHQ en la barra de navegación global que los dirige al sitio de ProofHQ.

Esta opción no está habilitada de forma predeterminada. Para habilitar esta opción, póngase en contacto con el soporte técnico de Workfront y solicite este acceso para todos los usuarios de revisión del sistema.

Para obtener más información, consulte [Acceder a Workfront Proof desde Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) en [Acceder a Workfront Proof desde Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Antes de este cambio, solo la persona con la función de administrador de Workfront podía tener acceso directo al sitio de ProofHQ desde la interfaz de Workfront.

## Nueva opción de conexión segura TLS para el correo saliente (Workfront)

Al seleccionar la opción de administrar la comunicación de Workfront mediante su propio servidor de correo electrónico, ahora puede habilitar el correo saliente para que utilice una conexión segura TLS.

Antes de esta mejora, solo podía habilitar el correo saliente a través de una conexión segura SSL.

Para obtener más información sobre la configuración del correo saliente, consulte.

## Nuevo campo para administrar correos electrónicos en el entorno de zona protegida de vista previa

Workfront ahora deshabilita todas las comunicaciones por correo electrónico desde el entorno de zona protegida de vista previa y el entorno de actualización personalizada. Si desea recibir notificaciones por correo electrónico desde los entornos Zona protegida de vista previa o Actualización personalizada, debe habilitar esta funcionalidad en la configuración de usuario.

Para obtener más información, consulte el artículo:

* [Entorno de zona protegida de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) en [Entorno de zona protegida de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* “Recepción de correos electrónicos desde la zona protegida de actualización personalizada” en [Entorno de zona protegida de actualización personalizada de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook para Office 365 (Workfront)

Ya está disponible el complemento de Workfront para Outlook 365. 

Para obtener más información sobre el uso del complemento, consulte [Usar el complemento de Workfront con Outlook para Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Buscar en la aplicación móvil (Workfront)

Ahora puede buscar objetos dentro de la aplicación móvil, de forma similar a como busca en la aplicación web. La nueva funcionalidad de búsqueda busca primero los elementos de la lista de elementos recientes, así como los objetos que se hayan descargado anteriormente en el dispositivo móvil. La lista de elementos recientes es la misma lista que se ve en la aplicación web.

>[!NOTE]
>
>Esta funcionalidad estará disponible la primera semana de mayo de 2017.

Para obtener más información sobre la aplicación móvil, consulte la sección “Búsqueda en dispositivos móviles” en  

## Ayuda mejorada en la aplicación móvil: tutoriales (Workfront)

A partir del estreno de la versión móvil de abril, se verán nuevas pantallas de tutorial que guiarán a través de la experiencia móvil. Al iniciar sesión en la aplicación móvil por primera vez y utilizar una función por primera vez, aparecerá un breve tutorial explicando cómo funciona la función. El tutorial solo se mostrará una vez, la primera que se utilice una función específica.

Para obtener más información sobre la aplicación móvil, consulte .

## Búsqueda en documentos PDF (ProofHQ)

Ya es posible realizar búsquedas en documentos PDF y de Office, así como en páginas web estáticas.

Para obtener más información, consulte  [Búsqueda de contenido dentro de una prueba](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Barra de navegación global actualizada (ProofHQ)

Las cuentas de ProofHQ Premium integradas con Workfront ya ven las siguientes mejoras en la barra de navegación global, dentro de ProofHQ:

* Nueva imagen de perfil de usuario 
* Apariencia actualizada

## Incluir información adicional en las vistas personalizadas (ProofHQ)

Ya es posible incluir la siguiente información adicional en las vistas personalizadas:

* **Datos de nivel de destinatario**\
  Configure las vistas personalizadas para que incluyan las siguientes columnas relacionadas con los datos de nivel de destinatario: Función, Puesto, Alertas de correo electrónico, Mi fecha límite, Fecha de adición a la prueba y Búsqueda de destinatario.\
  Para obtener más información, consulte [Creación y administración de vistas personalizadas en pruebas de Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Datos de revisión**\
  Configure las vistas personalizadas para que incluyan las siguientes columnas relacionadas con los datos de revisión: Recuento de comentarios (todas las versiones), Tamaño en disco, Tipo de prueba, Número de archivos por versión, Datos adjuntos del comentario (tamaño en disco y nombre de archivo) y Filtrado por subcarpeta.\
  Para obtener más información, consulte [Creación y administración de vistas personalizadas en pruebas de Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Datos de nivel de fase relacionados con flujos de trabajo automatizados**\
  Configure las vistas personalizadas para que incluyan las siguientes columnas relacionadas con las fases individuales de los flujos de trabajo automatizados: Estado de SOCD, Plazos de fase, Nombre de fase activa, Nombre de fase siguiente, Nombre de fase y Plantilla.\
  Para obtener más información, consulte [Creación y administración vistas personalizadas en pruebas de Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Mejoras en los informes de revisión (anteriormente, análisis) (ProofHQ)

La función de creación de informes (anteriormente conocida como análisis) incluye las siguientes mejoras:

* Nuevos tipos de informes predeterminados:

   * Tiempo de respuesta de la prueba
   * Porcentaje de aprobación tardía
   * Tiempo de la primera actividad de prueba
   * Número de comentarios y respuestas

* Imprimir informes
* Apariencia actualizada

## Ver la funcionalidad de ProofHQ en el entorno de vista previa (ProofHQ)

Las funcionalidades que se publiquen para ProofHQ primero estarán disponibles para probarse en el entorno de vista previa antes de publicarse en el entorno de producción.

Este nuevo flujo de trabajo de publicación de la funcionalidad como vista previa antes de producción permitirá estar preparado para futuras actualizaciones del entorno de producción de ProofHQ.

Para obtener más información sobre el entorno de vista previa de ProofHQ, consulte [Entorno de prueba de zona protegida de vista previa: Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
