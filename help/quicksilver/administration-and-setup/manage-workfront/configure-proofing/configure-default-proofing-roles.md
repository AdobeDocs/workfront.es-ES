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
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 2%

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
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo total a un usuario</a>.</p> </td> 
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

1. Haga clic en **Revisar y aprobar** cerca de la parte inferior de la lista que aparece a la izquierda.
1. En la sección **Roles de los destinatarios designados de una revisión de documento**, seleccione el rol predeterminado de los usuarios y usuarios invitados que se agregan al flujo de trabajo de una revisión.

   Consulte [Derechos asociados con funciones de revisión](#rights-associated-with-proofing-roles) a continuación para obtener una lista de cada función de revisión y los derechos asociados con ella.

   >[!NOTE]
   >
   >* Esta configuración solo se aplica a los usuarios que se crean en el sistema de Workfront después de establecer la función; no a los usuarios existentes.
   >* La persona que agrega usuarios a la revisión puede ajustar esta función, tal como se describe en [Agregar usuarios a una revisión](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) en [Compartir una revisión en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. En la sección **Roles de no destinatarios que abren una revisión de documento**, seleccione el rol predeterminado para los usuarios y usuarios invitados que pueden acceder a una revisión, pero que no se agregan al flujo de trabajo de la revisión.

   Esta situación se produce cuando los usuarios e invitados tienen acceso a un documento para el que se ha creado una prueba: incluso si no se han añadido al flujo de trabajo de la prueba, pueden abrir la prueba.

   **Ejemplos:** Estos son algunos ejemplos de cómo usar esta configuración:

   * Selecciona **Solo lectura** para limitar toda la actividad de revisión, como agregar comentarios y tomar decisiones a quienes se les pidió hacerlo.
   * Selecciona **Revisor** porque desea que cualquier miembro del equipo pueda agregar marcas y comentarios en una revisión.

1. Haga clic en **Guardar**.

## Derechos asociados a funciones de revisión {#rights-associated-with-proofing-roles}

En la tabla siguiente se muestra cada función y los derechos asociados a ella:

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
   <th> <p><strong>Ver una revisión</strong> </p> </th> 
   <th> <p><strong>Agregar marcas</strong> </p> </th> 
   <th> <p><strong>Agregar comentarios</strong> </p> </th> 
   <th> <p><strong>Editar sus propios comentarios si no hay respuestas</strong> </p> </th> 
   <th> <p><strong>Tomar una decisión</strong> </p> </th> 
   <th> <p><strong>Eliminar comentarios de otros</strong> </p> </th> 
   <th>Resolver comentarios</th> 
   <th>Aplicar acciones a comentarios</th> 
   <th> <p><strong>Editar la revisión</strong> </p> </th> 
   <th>Compartir la prueba con otros usuarios</th> 
   <th>Crear nueva versión</th> 
   <th> <p><strong>Ver solicitudes de aprobación en el área de inicio</strong> </p> </th> 
   <th>Añadir nuevos revisores</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Sólo lectura</strong> </p> </td> 
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
   <td> <p>✓ <strong></strong> </p> </td> 
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
>Los usuarios con nuevos planes de Workfront pueden otorgar funciones de autor o moderador a cualquier usuario del sistema. Los usuarios con planes heredados pueden conceder funciones de autor o moderador a cualquier usuario con una licencia de revisión en el sistema.
