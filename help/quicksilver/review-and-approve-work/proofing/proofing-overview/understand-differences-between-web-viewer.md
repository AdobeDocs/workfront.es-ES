---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Diferencias entre el visor de corrección web y el visor de corrección de escritorio
description: Conozca las diferencias entre los visores de corrección web y de escritorio.
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
TQID: https://experienceleague.adobe.com/5wUR3OHvmgjQmRtvt85iax2gbY0rC0yWsLzuLULia3M
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 872
ht-degree: 94%

---

# Diferencias entre el visor de corrección web y el visor de corrección de escritorio

Adobe Workfront ofrece dos visores de corrección diferentes:

* **Visor de corrección web:** diseñado principalmente para revisar archivos estáticos y de vídeo. Se ejecuta en Google Chrome, Firefox o Safari.
* **Visor de corrección de escritorio:** diseñado para revisar archivos interactivos, así como archivos estáticos y de vídeo. Se ejecuta como una aplicación independiente en la estación de trabajo. Para obtener más información, consulte [Explicación del visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Si su organización no puede utilizar la aplicación del visor de corrección de escritorio por motivos de seguridad, su administrador de Workfront puede configurar el sistema para que pueda revisar el contenido interactivo, incluido en un archivo ZIP, en el visor de corrección web. Para obtener más información, consulte [Configurar la revisión de contenido interactivo en el visor de corrección web](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

La siguiente lista puede ayudarle a comprender qué visor de corrección puede utilizar para revisar ciertos tipos de contenido:

* **Contenido web interactivo, URL**: si crea una revisión para el contenido web mediante una URL y desea revisar el contenido de forma interactiva, debe usar el visor de corrección de escritorio.
* **Contenido web interactivo, archivo ZIP**: si crea una revisión para contenido web con un archivo ZIP, puede usar el visor de corrección web (con algunas limitaciones) o el visor de corrección de escritorio. Para obtener información acerca de las limitaciones que implica el uso del visor de corrección web para el contenido interactivo, consulte [Configurar la revisión de contenido interactivo en el visor de corrección web](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* **Contenido estático y de vídeo**: si crea una revisión que contiene contenido estático, puede usar el visor de corrección web o el visor de corrección de escritorio.

## Pruebas estáticas

| **Característica** | **Visor de corrección web** | **Visor de corrección de escritorio** |
|---|---|---|
| Abrir pruebas estáticas | ✓ | ✓&#42; |
| Vistas únicas, de revista y continuas | ✓ | ✓&#42; |
| Panorámica | ✓ | ✓&#42; |
| Ampliación | ✓ | ✓&#42; |
| Rotar | ✓ | ✓&#42; |
| Herramienta de medición | ✓ (establecer un área de tamaño personalizado) | ✓&#42; |
| Vista en miniatura | ✓ | ✓&#42; |
| Navegador de prueba estático | ✓ | ✓&#42; |
| Búsqueda de documentos | ✓ | ✓&#42; |
| Publicar comentario en varias páginas | ✓ (disponible en todas las vistas) | ✓&#42; (disponible en todas las vistas) |
| Métodos abreviados de prueba estáticos avanzados | ✓ (para obtener más información, vea [Métodos abreviados de teclado en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;(para obtener más información, consulte [Métodos abreviados de teclado en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

{style="table-layout:auto"}

&#42; Esta funcionalidad solo funciona si el administrador de Workfront ha configurado el Visor de corrección de escritorio como el visor predeterminado para todas las revisiones.

## Pruebas de vídeo

| **Característica**  | **Visor de corrección web** | **Visor de revisiones de escritorio** |
|---|---|---|
| Abrir pruebas de vídeo | ✓ | ✓&#42; |
| Almacenamiento en búfer | ✓ | ✓&#42; |
| Revisar con el tiempo | ✓ | ✓&#42; |
| Revisar mediante fotogramas o códigos de tiempo | ✓ | ✓&#42; |
| Revisar más o menos rápido | ✓ | ✓&#42; |
| Regulación de volumen | ✓ | ✓&#42;  |
| Modo de pantalla completa | ✓ | ✓&#42;  |
| Comentarios del intervalo | ✓ | ✓&#42;  |
| Realizar pruebas de vídeo en bucle (los vídeos finalizan y comienzan automáticamente) | ✓ | ✓&#42;  |
| Métodos abreviados de vídeo avanzados | ✓ (para obtener más información, vea [Métodos abreviados de teclado en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;  |

{style="table-layout:auto"}

&#42; Esta funcionalidad solo funciona si el Visor de corrección de escritorio está configurado como el visor predeterminado para todas las revisiones.

## Pruebas interactivas

| **Característica**  | **Visor de corrección web** | **Visor de corrección de escritorio** |
|---|---|---|
| Abra pruebas interactivas creadas a partir de contenido empaquetado en un archivo ZIP | ✓ | ✓ (recomendado) |
| Abra una prueba interactiva creada a partir de una dirección URL | No compatible | ✓ |
| Ver pruebas interactivas (creadas a partir de contenido empaquetado en un archivo ZIP) en varios tamaños de pantalla | ✓ | ✓ |
| Ver pruebas interactivas (creadas a partir de contenido empaquetado en un archivo ZIP) para varios dispositivos | No compatible | ✓ |
| Revisar sitios no seguros (HTTP) | No compatible | ✓ |
| Revisar sitios protegidos por iframe (sitios protegidos contra la visualización dentro de un iFrame) | No compatible | ✓ |

{style="table-layout:auto"}

## Comentarios

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Función</th> 
   <th>Visor de revisión web </th> 
   <th>Visor de corrección de escritorio </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Añadir, eliminar y editar comentarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Añadir y eliminar respuestas</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Herramientas de marcado de rectángulo, flecha, línea, improvisación y resaltado</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Herramienta de polilínea</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Herramientas de marcado de máscara de recorte</p> </td> 
   <td>No compatible</td> 
   <td>No compatible</td> 
  </tr> 
  <tr> 
   <td> <p>Herramienta de marcado de selección de texto</p> </td> 
   <td>✓ Solo pruebas estáticas de la</td> 
   <td>✓ Solo pruebas estáticas de la</td> 
  </tr> 
  <tr> 
   <td> <p>Cambiar color de marcado</p> </td> 
   <td>✓ (32 colores disponibles) </td> 
   <td>✓ (32 colores disponibles) </td> 
  </tr> 
  <tr> 
   <td> <p>Cambiar opacidad de marcado</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Cambiar grosor de marcado</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Cortar, copiar y pegar marcas</p> </td> 
   <td> No compatible</td> 
   <td> No compatible</td> 
  </tr> 
  <tr> 
   <td> <p>Deshacer y rehacer la última operación</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Duplicar marcas</p> </td> 
   <td> No compatible</td> 
   <td> No compatible</td> 
  </tr> 
  <tr> 
   <td>Definir acciones como comentarios</td> 
   <td>✓ (Las acciones son visibles en los comentarios inmediatamente después de que se establezca la acción).</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Establecer color de marcado como predeterminado</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Resolver comentarios</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Bloquear comentarios</p> </td> 
   <td>No compatible</td> 
   <td> No compatible</td> 
  </tr> 
  <tr> 
   <td> <p>Etiquetar usuarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Habilitar comentarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ver la lista de comentarios en una vista compacta</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Ver la lista de comentarios en una vista estándar, completa o única</p> </td> 
   <td>Planificado para el futuro</td> 
   <td>Planificado para el futuro</td> 
  </tr> 
  <tr> 
   <td> <p>Buscar comentarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrar comentarios por usuario</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrar comentarios y respuestas por usuario</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ordenar comentarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Actualizaciones automáticas de comentarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Decisiones

| Función | Visor de revisión web | Visor de corrección de escritorio |
|---|---|---|
| Tomar decisiones | ✓ | ✓ |
| Personalizar decisiones | ✓ | ✓ |

{style="table-layout:auto"}

## Comparar pruebas

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Función</th> 
   <th>Visor de revisión web </th> 
   <th>Visor de corrección de escritorio </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Comparar diferentes versiones de pruebas</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>Comparar pruebas independientes</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## Operaciones de revisión

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Función</th> 
   <th>Visor de revisión web </th> 
   <th>Visor de corrección de escritorio </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Cambiar la versión de revisión </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>Crea una nueva versión</td> 
   <td> <p>Disponible solo en Workfront Proof (previsto para el futuro al revisar en Workfront)<br></p> </td> 
   <td>Disponible solo en Workfront Proof (previsto para el futuro al revisar en Workfront)</td> 
  </tr> 
  <tr> 
   <td>Revisar detalles de la prueba </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Revisar flujos de trabajo de revisión</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Editar fases del flujo de trabajo</td> 
   <td>No compatible</td> 
   <td>No compatible</td> 
  </tr> 
  <tr> 
   <td>Compartir pruebas</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Obtener URL del equipo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Cambiar las notificaciones por correo electrónico</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Descargar archivo original</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Bloquear y desbloquear pruebas y fases</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Imprimir resumen de la prueba</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Eliminar pruebas</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Administrar las pruebas desde la misma carpeta</td> 
   <td><strong>Solo disponible en Workfront Proof</strong> </td> 
   <td><strong>Solo disponible en Workfront Proof</strong> </td> 
  </tr> 
  <tr> 
   <td>Personalización de marca (logotipos personalizados)</td> 
   <td>✓</td> 
   <td> ✓<br>(Logotipo de Workfront en la página de inicio) </td> 
  </tr> 
  <tr> 
   <td>Vínculos personalizados (solo Workfront Proof)</td> 
   <td>No compatible</td> 
   <td> No compatible </td> 
  </tr> 
  <tr> 
   <td>Integraciones de Basecamp (solo Workfront Proof) </td> 
   <td>Planificado para el futuro</td> 
   <td>Planificado para el futuro</td> 
  </tr> 
  <tr> 
   <td>Indicador de presencia </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Actualizaciones automáticas de la prueba (cambios de permisos y nuevas versiones)</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

## Minivisor

| **Característica**  | **Visor de corrección web**  | **Visor de corrección de escritorio** |
|---|---|---|
| Código incrustado | Planificado para futuras pruebas de vídeo estáticas y nativas | No compatible  |

{style="table-layout:auto"}

## Traducciones

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Característica</strong> </th> 
   <th><strong>Visor de corrección web</strong> </th> 
   <th><strong>Visor de corrección de escritorio</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Idiomas de asistencia distintos del inglés</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
