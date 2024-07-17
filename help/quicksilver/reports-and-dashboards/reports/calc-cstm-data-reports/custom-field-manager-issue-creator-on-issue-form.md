---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Ejemplo de campo personalizado calculado: mostrar el administrador del creador de un problema en el formulario personalizado del problema"
description: Con un campo personalizado calculado, puede mostrar el nombre del administrador del creador de un problema en un formulario personalizado adjunto al problema. Con la misma instrucción, puede generar campos calculados similares para proyectos, problemas y otros objetos.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Ejemplo del campo personalizado calculado: mostrar el administrador del creador de un problema en el formulario personalizado del problema

Con un campo personalizado calculado, puede mostrar el nombre del administrador del creador de un problema en un formulario personalizado adjunto al problema. Con la misma instrucción, puede generar campos calculados similares para proyectos, problemas y otros objetos.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>plan Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados<br>Para obtener información sobre cómo conceder acceso administrativo desde el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder acceso administrativo a usuarios a ciertas áreas</a>.</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto</p> </td> 
   <td> <p>Acceso de Contribute al objeto donde se adjunta el formulario con acceso a Editar el formulario personalizado</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar el administrador del creador de un problema en el formulario personalizado del problema

Los siguientes pasos muestran cómo se puede crear un campo calculado para un formulario personalizado de problema en el que se puede capturar el nombre del administrador del usuario que creó el problema. El proceso es idéntico cuando desea capturar el nombre del administrador de un usuario que creó una tarea, un proyecto o un portafolio, por ejemplo.

1. Cree un formulario personalizado de problema y añádale un campo calculado.

   Para obtener información sobre cómo crear un formulario personalizado y agregarle campos calculados, consulte los siguientes artículos:

   * [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [Añadir datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Copie y pegue el siguiente código de modo de texto en el campo **Cálculo** del formulario personalizado:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Los cálculos de campos personalizados distinguen entre mayúsculas y minúsculas.

1. Haga clic en **Listo** y luego en **Guardar + Cerrar**.

   El administrador del usuario que creó el problema se muestra en el campo calculado cuando el formulario que contiene el campo se adjunta a un problema.
