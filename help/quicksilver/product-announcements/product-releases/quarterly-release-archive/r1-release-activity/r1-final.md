---
content-type: release-notes
navigation-topic: product-releases-archive
title: Final R1
description: Actividad de la versión 2018.3
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# Final R1

Las siguientes funciones no están disponibles actualmente en Vista previa o Beta, pero se lanzarán al entorno Producción en R1:

## Tomar decisiones de aprobación para pruebas desde el área de Mi trabajo (Workfront)

Ahora, cuando un usuario le agrega a una prueba y concede la función Aprobador o la función Revisor y aprobador (desde la aplicación independiente ProofHQ o mediante el uso del Flujo de trabajo automatizado en Workfront ), la solicitud de aprobación se muestra en la pestaña Aprobaciones del área Mi trabajo. A continuación, puede ver la prueba y tomar una decisión de aprobación directamente desde Workfront.

Para obtener información sobre cómo agregar usuarios a una prueba mediante el flujo de trabajo automatizado, consulte [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) en [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Para obtener información acerca de cómo tomar decisiones de aprobación en el área Mi trabajo, vea [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Informe sobre aprobaciones de revisión dentro de mi área de trabajo (Workfront)

Ahora puede crear un informe basado en el objeto Aprobación de pruebas. Este informe permite informar sobre las aprobaciones de prueba desde las áreas de Mi trabajo de los usuarios en las que aún no se han tomado decisiones.

Los informes de aprobación de pruebas contienen la siguiente información:

* Documento enviado para su aprobación
* Nombre del aprobador
* Versión de revisión
* Identificador de revisión
* Fecha de creación de revisión

Puede obtener acceso a esta aprobación al crear un informe basado en un objeto, como se describe en [Crear un informe personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objetos de aprobaciones de pruebas, consulte la sección [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) en [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Generar automáticamente una nueva versión de una revisión de documento arrastrando y soltando (Workfront)

Al utilizar el método de arrastrar y soltar para agregar una nueva versión de un documento que requiera revisión, se genera una revisión automáticamente. La prueba tiene las mismas opciones y flujos de trabajo que la prueba original o la versión anterior.

Anteriormente, cuando se agregaba una nueva versión del documento, la revisión no se generaba automáticamente en la nueva versión y había que volver a generar la revisión para la nueva versión.

Cuando se utiliza el menú Documentos más para cargar una nueva versión, no se genera una prueba automáticamente.

Para obtener más información, consulte la  sección en

## Habilitar todos los usuarios de revisión para acceder a ProofHQ directamente desde la interfaz de Workfront (Workfront)

Ahora puede permitir que todos los usuarios de revisión de su sistema tengan acceso sin problemas a su cuenta de ProofHQ Premium directamente desde la interfaz de Workfront. Cuando está habilitado, todos los usuarios de revisión ven un icono de ProofHQ en la barra de navegación global que los dirige al sitio de ProofHQ.

Esta opción no está habilitada de forma predeterminada. Para habilitar esta opción, póngase en contacto con el Soporte técnico de Workfront y solicite este acceso para todos los usuarios de revisión del sistema.

Para obtener más información, consulte [Acceder a Workfront Proof desde Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) en  [Acceder a Workfront Proof desde Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Antes de este cambio, solamente el administrador de Workfront podía tener acceso directo al sitio de ProofHQ desde la interfaz de Workfront.

## Nueva opción para la conexión segura de TLS para el correo saliente (Workfront)

Al seleccionar administrar la comunicación de Workfront mediante su propio servidor de correo electrónico, ahora puede habilitar el correo saliente para que utilice una conexión segura TLS.

Antes de esta mejora, solo podía habilitar el correo saliente a través de una conexión segura SSL.

Para obtener más información sobre la configuración del correo saliente, consulte .

## Nuevo campo para administrar correos electrónicos en el entorno de vista previa de espacio aislado

Workfront ahora deshabilita todas las comunicaciones por correo electrónico desde el entorno de vista previa de espacio aislado y el entorno de actualización personalizado. Si desea recibir notificaciones por correo electrónico desde los entornos Vista previa de espacio aislado o Actualización personalizada, debe habilitar esta funcionalidad en la configuración de usuario.

Para obtener más información, consulte la siguiente información:

* [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) en [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* &quot;Recibiendo correos electrónicos desde la zona protegida de actualización personalizada&quot; en [El entorno de la zona protegida de actualización personalizada de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook para Office 365 (Workfront)

Ya está disponible el complemento de Workfront para Outlook 365. 

Para obtener más información sobre el uso del complemento, vea [Usar el complemento de Workfront con Outlook para Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Buscar en la aplicación móvil (Workfront)

Ahora puede buscar objetos dentro de la aplicación móvil, de forma similar a como busca en la aplicación web. La nueva funcionalidad de búsqueda busca primero los elementos de la lista Elementos recientes, así como los objetos que se hayan descargado anteriormente en su dispositivo móvil. La lista de Elementos recientes es la misma lista que se ve en la aplicación web.

>[!NOTE]
>
>Esta funcionalidad estará disponible la primera semana de mayo de 2017.

Para obtener más información sobre la aplicación móvil, consulte la sección &quot;Búsqueda en dispositivos móviles&quot; en  

## Ayuda mejorada en la aplicación móvil: Tutorials (Workfront)

A partir del lanzamiento de la versión móvil en abril, verá nuevas pantallas de tutorial que le guiarán a través de su experiencia móvil. Cuando inicie sesión en la aplicación móvil por primera vez y utilice una función por primera vez, verá un breve tutorial que explica cómo funciona la función. El tutorial solo se muestra una vez, la primera vez que utilice una función específica.

Para obtener más información sobre la aplicación móvil, consulte .

## Buscar en documentos de PDF (ProofHQ)

Ahora puede realizar búsquedas en documentos de PDF, documentos de Office y páginas web estáticas.

Para obtener más información, consulte  [Buscar contenido dentro de una revisión](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Barra de navegación global actualizada (ProofHQ)

Las cuentas de ProofHQ Premium integradas con Workfront ahora ven las siguientes mejoras en la barra de navegación global dentro de ProofHQ:

* Nueva imagen de perfil de usuario 
* Aspecto y presentación actualizados

## Incluir información adicional en las vistas personalizadas (ProofHQ)

Ahora puede incluir la siguiente información adicional en las vistas personalizadas:

* **Datos De Nivel De Destinatario**\
  Puede configurar las vistas personalizadas para que incluyan las siguientes columnas relacionadas con los datos de nivel de destinatario: función, puesto, alertas de correo electrónico, mi fecha límite, fecha de adición a la prueba y búsqueda de destinatario.\
  Para obtener más información, consulte [Crear y administrar vistas personalizadas en Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Datos de revisión**\
  Puede configurar las vistas personalizadas para que incluyan las siguientes columnas relacionadas con los datos de revisión: Recuento de comentarios (todas las versiones), Tamaño en disco, Tipo de prueba, Número de archivos por versión, Datos adjuntos del comentario (tamaño en disco, nombre de archivo) y Filtrado por subcarpeta.\
  Para obtener más información, consulte [Crear y administrar vistas personalizadas en Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Datos de nivel de etapa relacionados con flujos de trabajo automatizados**\
  Puede configurar las vistas personalizadas para que incluyan las siguientes columnas relacionadas con las fases individuales de los flujos de trabajo automatizados: Estado de SOCD, Plazos de fase, Nombre de fase activo, Nombre de fase siguiente, Nombre de fase y Plantilla.\
  Para obtener más información, consulte [Crear y administrar vistas personalizadas en Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Mejoras en los informes de revisión (anteriormente Analytics) (ProofHQ)

La función de creación de informes (anteriormente conocida como Analytics) incluye las siguientes mejoras:

* Nuevos tipos de informes predeterminados:

   * Tiempo de respuesta de prueba
   * Porcentaje de aprobación tardía
   * Prueba de la primera actividad
   * Número de comentarios y respuestas

* Imprimir informes
* Aspecto y presentación actualizados

## Ver la funcionalidad de ProofHQ en el entorno de vista previa (ProofHQ)

La funcionalidad que se lanza a ProofHQ primero estará disponible para probar en el entorno de vista previa antes de lanzarse al entorno de producción.

Este nuevo flujo de trabajo de lanzamiento de la funcionalidad a Previsualización antes de Producción le permitirá estar más preparado para futuras actualizaciones de su entorno de producción de ProofHQ.

Para obtener más información sobre el entorno de vista previa de ProofHQ, consulte [Previsualizar entorno de prueba de espacio aislado- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
