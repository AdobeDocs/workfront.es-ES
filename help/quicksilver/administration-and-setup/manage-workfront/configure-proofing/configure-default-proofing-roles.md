---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurar roles de corrección predeterminados
description: Como administrador de Adobe Workfront, puede configurar las funciones de revisión predeterminadas para los usuarios y usuarios invitados que acceden a las pruebas creadas en Workfront. Cualquier persona que añada usuarios a una prueba puede ajustar estas funciones para ellos.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
TQID: https://experienceleague.adobe.com/1bEnBH5l58juHFYsg1bfR-LMcQ-wGgKNkeGAGQlNbJs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 505
ht-degree: 99%

---

# Configurar funciones de revisión predeterminadas

Como administrador de Adobe Workfront, puede configurar las funciones de revisión predeterminadas para los usuarios y usuarios invitados que acceden a las pruebas creadas en Workfront. Cualquier persona que añada usuarios a una prueba puede ajustar estas funciones para ellos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Configurar funciones de revisión predeterminadas

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Haga clic en **Revisión y aprobación** cerca de la parte inferior de la lista que aparece a la izquierda.
1. En la sección **Funciones de los destinatarios designados de una prueba de documento**, seleccione la función predeterminada de los usuarios y usuarios invitados que se añaden al flujo de trabajo de una prueba.

   Consulte más adelante [Derechos asociados con las funciones de revisión](#rights-associated-with-proofing-roles) para obtener una lista de cada función de revisión y los derechos asociados con ella.

   >[!NOTE]
   >
   >* Esta configuración solo se aplica a los usuarios que se crean en el sistema de Workfront después de establecer la función; no a los usuarios existentes.
   >* La persona que añade usuarios a la prueba puede ajustar esta función, tal como se describe en [Añadir usuarios a una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) en [Compartir una prueba dentro de Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. En la sección **Funciones de los no destinatarios que abren una prueba de documento**, seleccione la función predeterminada de los usuarios y usuarios invitados que pueden acceder a una prueba, pero que no se han añadido al flujo de trabajo de una prueba.

   Esta situación se produce cuando usuarios e invitados tienen acceso a un documento para el que se ha creado una prueba: aunque no se hayan añadido al flujo de trabajo de la prueba, pueden abrir la prueba.

   **Ejemplos:** a continuación se muestran algunos ejemplos de cómo usar esta configuración:

   * Seleccione **Solo lectura** para limitar toda la actividad de prueba, como añadir comentarios y tomar decisiones a quienes se les ha pedido que lo hagan.
   * Seleccione **Revisor** porque desea que cualquier abonado del equipo pueda añadir marcas y comentarios en una prueba.

1. Haga clic en **Guardar**.

## Derechos asociados con las funciones de revisión {#rights-associated-with-proofing-roles}

En la tabla siguiente se muestra cada función y los derechos asociados con ella:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Ver una prueba</strong> </p> </th> 
   <th> <p><strong>Añadir marcas</strong> </p> </th> 
   <th> <p><strong>Añadir comentarios</strong> </p> </th> 
   <th> <p><strong>Editar comentarios propios si no hay respuestas</strong> </p> </th> 
   <th> <p><strong>Tomar una decisión</strong> </p> </th> 
   <th> <p><strong>Eliminar los comentarios de otros</strong> </p> </th> 
   <th>Resolver comentarios</th> 
   <th>Aplicar acciones a los comentarios</th> 
   <th> <p><strong>Editar la prueba</strong> </p> </th> 
   <th>Compartir la prueba con otros usuarios</th> 
   <th>Crear nueva versión</th> 
   <th> <p><strong>Ver solicitudes de aprobación en el área de inicio</strong> </p> </th> 
   <th>Añadir nuevos revisores</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Solo lectura</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisor</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aprobador</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisor y aprobador</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autor</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Moderador</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Los usuarios de los nuevos planes de Workfront pueden otorgar funciones de autor o moderador a cualquier usuario del sistema. Los usuarios de los planes heredados pueden conceder funciones de autor o moderador a cualquier usuario con una licencia de prueba en el sistema.
