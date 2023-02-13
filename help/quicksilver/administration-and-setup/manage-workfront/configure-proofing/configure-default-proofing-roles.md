---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuración de las funciones de prueba predeterminadas
description: Como administrador de Adobe Workfront, puede configurar las funciones de prueba predeterminadas para los usuarios y los usuarios invitados que accedan a las pruebas creadas en Workfront. Cualquier persona que agregue usuarios a una prueba puede ajustar estas funciones para ellos.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Configuración de las funciones de prueba predeterminadas

Como administrador de Adobe Workfront, puede configurar las funciones de prueba predeterminadas para los usuarios y los usuarios invitados que accedan a las pruebas creadas en Workfront. Cualquier persona que agregue usuarios a una prueba puede ajustar estas funciones para ellos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
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

## Configuración de las funciones de prueba predeterminadas

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Haga clic en **Revisión y aprobación** cerca de la parte inferior de la lista que aparece a la izquierda.
1. En el **Funciones para los destinatarios designados de una prueba de documento** , seleccione la función predeterminada para los usuarios y usuarios invitados que se agregan al flujo de trabajo de una prueba.

   Consulte [Derechos asociados a funciones de prueba](#rights-associated-with-proofing-roles) a continuación para obtener una lista de cada función de prueba y los derechos asociados a ella.

   >[!NOTE]
   >
   >* Esta configuración solo se aplica a los usuarios creados en el sistema Workfront después de establecer la función. no a los usuarios existentes.
   >* La persona que agrega usuarios a la prueba puede ajustar esta función, tal como se describe en [Agregar usuarios a una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) en [Compartir una prueba en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. En el **Funciones para los usuarios que no son destinatarios y que abren una prueba de documento** , seleccione la función predeterminada para los usuarios y usuarios invitados que pueden acceder a una prueba, pero que no se agregan al flujo de trabajo de la prueba.

   Esta situación se produce cuando usuarios e invitados tienen acceso a un documento para el que se ha creado una prueba: aunque no se hayan agregado al flujo de trabajo de la prueba, pueden abrir la prueba.

   **Ejemplos:** Estos son ejemplos de cómo puede utilizar esta configuración:

   * Seleccione **Solo lectura** para limitar toda la actividad de prueba, como agregar comentarios y tomar decisiones a los que se les ha pedido que lo hagan.
   * Seleccione **Revisor** porque desea que cualquier miembro del equipo pueda añadir marcas y comentarios en una prueba.

1. Haga clic en **Guardar**.

## Derechos asociados a funciones de prueba {#rights-associated-with-proofing-roles}

La tabla siguiente muestra cada función y los derechos asociados a ella:

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
   <th> <p><strong>Agregar marcas</strong> </p> </th> 
   <th> <p><strong>Añadir comentarios</strong> </p> </th> 
   <th> <p><strong>Editar sus propios comentarios si no hay respuestas</strong> </p> </th> 
   <th> <p><strong>Tomar una decisión</strong> </p> </th> 
   <th> <p><strong>Suprimir los comentarios de otros</strong> </p> </th> 
   <th>Resolver comentarios</th> 
   <th>Aplicar acciones a los comentarios</th> 
   <th> <p><strong>Editar la prueba</strong> </p> </th> 
   <th>Comparta la prueba con otros usuarios</th> 
   <th>Crear nueva versión</th> 
   <th> <p><strong>Ver solicitudes de aprobación en el área principal</strong> </p> </th> 
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
>Los usuarios de nuevos planes de Workfront pueden otorgar funciones de autor o moderador a cualquier usuario del sistema. Los usuarios de planes heredados pueden otorgar funciones de autor o moderador a cualquier usuario con una licencia de prueba en el sistema.
