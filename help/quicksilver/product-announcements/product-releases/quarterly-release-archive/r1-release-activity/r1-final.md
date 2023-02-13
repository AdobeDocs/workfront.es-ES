---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Final
description: Actualmente, la siguiente funcionalidad no está disponible en Preview o Beta, pero se está liberando al entorno de producción en R1 - EDIT ME.
author: Luke
feature: Product Announcements
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# R1 Final

Actualmente, la siguiente funcionalidad no está disponible en Vista previa o Beta, pero se está liberando al entorno Producción en R1:

## Tome decisiones de aprobación para pruebas desde el área de trabajo (Workfront)

Ahora, cuando un usuario le agrega a una prueba y concede la función Aprobador o la función Revisor y Aprobador (ya sea desde la aplicación ProofHQ independiente o mediante Flujo de trabajo automatizado en Workfront ), la solicitud de aprobación se muestra en la pestaña Aprobaciones de su área de trabajo. A continuación, puede ver la prueba y tomar una decisión de aprobación sobre la prueba directamente desde Workfront.

Para obtener información sobre cómo agregar usuarios a una prueba mediante el flujo de trabajo automatizado, consulte [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) en [Compartir una prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Para obtener información sobre cómo tomar decisiones de aprobación desde el área Mi trabajo, consulte [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md) en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Informe de aprobaciones de prueba dentro de Mi área de trabajo (Workfront)

Ahora puede crear un informe basado en el objeto Proof Approval. Este informe permite informar sobre las aprobaciones de prueba de las áreas de Mi trabajo de los usuarios en las que aún no se han tomado decisiones.

Los informes de aprobación de prueba contienen la siguiente información:

* Documento presentado para su aprobación
* Nombre del aprobador
* Versión de prueba
* Identificador de revisión
* Fecha de creación de la prueba

Puede acceder a esta aprobación al crear un informe basado en un objeto, tal como se describe en [Crear un informe personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objeto Proof Approvals , consulte la [Explicación de los objetos en Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) en [Explicación de los objetos en Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Generar automáticamente una nueva versión de una prueba de documento mediante Arrastrar y soltar (Workfront)

Cuando se utiliza el método de arrastrar y soltar para añadir una nueva versión de un documento que requiera pruebas, se genera automáticamente una prueba. La prueba tiene las mismas opciones y flujos de trabajo que la prueba original o la versión anterior.

Anteriormente, al añadir una nueva versión del documento, la prueba no se generaba automáticamente en la nueva versión y tenía que volver a generar la prueba para la nueva versión.

Cuando se utiliza el menú Más documentos para cargar una nueva versión, no se genera automáticamente una prueba.

Para obtener más información, consulte la sección en

## Habilitar a todos los usuarios de prueba para acceder a ProofHQ directamente desde la interfaz de Workfront (Workfront)

Ahora puede permitir que todos los usuarios de pruebas de su sistema tengan acceso sin problemas a su cuenta de ProofHQ Premium directamente desde la interfaz de Workfront. Cuando está habilitado, todos los usuarios de pruebas ven un icono ProofHQ en la barra de navegación global que los dirige al sitio ProofHQ.

Esta opción no está activada de forma predeterminada. Para habilitar esta opción, póngase en contacto con el servicio de asistencia técnica de Workfront y solicite este acceso para todos los usuarios de prueba del sistema.

Para obtener más información, consulte [Acceso a la prueba de Workfront desde Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) en  [Acceso a la prueba de Workfront desde Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Antes de este cambio, solo el administrador de Workfront podía tener acceso directo al sitio de ProofHQ desde la interfaz de Workfront.

## Nueva opción para TLS Secure Connection for Outgoing Mail (Workfront)

Al seleccionar administrar la comunicación de Workfront mediante su propio servidor de correo electrónico, ahora puede habilitar el correo saliente para que utilice una conexión segura TLS.

Antes de esta mejora, solo podía habilitar Correo saliente a través de una conexión segura SSL.

Para obtener más información sobre la configuración del correo saliente, consulte .

## Nuevo campo para administrar correos electrónicos en el entorno de espacio aislado de vista previa

Workfront ahora deshabilita todas las comunicaciones por correo electrónico desde el entorno de espacio aislado de vista previa y el entorno de actualización personalizada. Si desea recibir notificaciones por correo electrónico de los entornos de espacio aislado de vista previa o de actualización personalizada, debe habilitar esta funcionalidad en la configuración de usuario.

Para obtener más información, consulte la siguiente información:

* [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) en [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* &quot;Recibir correos electrónicos del Simulador para pruebas de actualización personalizado&quot; en [Entorno de espacio aislado de actualización personalizado de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook para Office 365 (Workfront)

El complemento de Workfront para Outlook 365 ya está disponible. 

Para obtener más información sobre el uso del complemento, consulte [Uso del complemento de Workfront con Outlook para Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Buscar en la aplicación móvil (Workfront)

Ahora puede buscar objetos dentro de la aplicación móvil, de forma similar a como lo hace en la aplicación web. La nueva funcionalidad de búsqueda busca primero los elementos de la lista Elementos recientes , así como los objetos que se han descargado previamente en el dispositivo móvil. La lista de elementos recientes es la misma que se ve en la aplicación web.

>[!NOTE]
>
>Esta funcionalidad estará disponible la primera semana de mayo de 2017.

Para obtener más información sobre la aplicación móvil, consulte la sección &quot;Búsqueda en dispositivos móviles&quot; en  

## Ayuda mejorada en la aplicación móvil: Tutorials (Workfront)

A partir de la versión móvil de abril, verá nuevas pantallas de tutoriales que le guiarán en su experiencia móvil. Cuando inicie sesión en la aplicación móvil por primera vez y utilice una función por primera vez, verá un breve tutorial en el que se explica cómo funciona la función. El tutorial se muestra solo una vez, la primera vez que utiliza una función específica.

Para obtener más información sobre la aplicación móvil, consulte .

## Búsqueda en documentos del PDF (ProofHQ)

Ahora puede realizar búsquedas dentro de documentos de PDF, documentos de oficina y páginas web estáticas.

Para obtener más información, consulte  [Buscar contenido dentro de una prueba](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Barra de navegación global actualizada (ProofHQ)

Las cuentas de ProofHQ Premium que están integradas con Workfront ahora ven las siguientes mejoras en la barra de navegación global dentro de ProofHQ:

* Nueva imagen de perfil de usuario 
* Aspecto actualizado

## Incluir información adicional en vistas personalizadas (ProofHQ)

Ahora puede incluir la siguiente información adicional en las vistas personalizadas:

* **Datos de nivel de destinatario**\
   Puede configurar vistas personalizadas para incluir las siguientes columnas relacionadas con los datos de nivel de destinatario: Rol, Posición, Alertas de correo electrónico, Mi fecha límite, Fecha de incorporación a la prueba y Búsqueda de destinatarios.\
   Para obtener más información, consulte [Crear y administrar vistas personalizadas en la prueba de Workfront](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Datos de prueba**\
   Puede configurar vistas personalizadas para incluir las siguientes columnas relacionadas con la prueba de datos: Recuento de comentarios (todas las versiones), Tamaño en disco, Tipo de prueba, Número de archivos por versión, Datos de archivos adjuntos de comentarios (tamaño en disco, nombre de archivo) y Filtrado por subcarpeta.\
   Para obtener más información, consulte [Crear y administrar vistas personalizadas en la prueba de Workfront](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Datos de nivel de fase relacionados con flujos de trabajo automatizados**\
   Puede configurar vistas personalizadas para incluir las siguientes columnas relacionadas con etapas individuales de flujos de trabajo automatizados: Estado SOCD, Plazos de etapa, Nombre de etapa activo, Nombre de etapa siguiente, Nombre de escenario y Plantilla.\
   Para obtener más información, consulte [Crear y administrar vistas personalizadas en la prueba de Workfront](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Mejoras en los informes de prueba (anteriormente Analytics) (ProofHQ)

La función de informes (anteriormente denominada Analytics) contiene las siguientes mejoras:

* Nuevos tipos de informes predeterminados:

   * Tiempo de respuesta de la prueba
   * Porcentaje de aprobación tardía
   * Prueba de la primera actividad
   * Número de comentarios y respuestas

* Imprimir informes
* Aspecto actualizado

## Ver funcionalidad de ProofHQ en el entorno de vista previa (ProofHQ)

La funcionalidad incluida en ProofHQ estará disponible primero para su prueba en el entorno de vista previa antes de su lanzamiento en el entorno de producción.

Este nuevo flujo de trabajo de funcionalidad de lanzamiento a Vista previa antes de la producción le permitirá estar más preparado para futuras actualizaciones de su entorno ProofHQ Production.

Para obtener más información sobre el entorno de vista previa de ProofHQ, consulte [Entorno de prueba de espacio aislado de vista previa: prueba de Workfront](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
