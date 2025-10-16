---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Ejemplo del campo personalizado calculado: mostrar el administrador del creador de un problema en el formulario personalizado del problema'
description: Con un campo personalizado calculado, puede mostrar el nombre del administrador del creador de un problema en un formulario personalizado adjunto al problema. Con la misma instrucción, puede generar campos calculados similares para proyectos, problemas y otros objetos.
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 97%

---

# Ejemplo del campo personalizado calculado: mostrar el administrador del creador de un problema en el formulario personalizado del problema

Con un campo personalizado calculado, puede mostrar el nombre del administrador del creador de un problema en un formulario personalizado adjunto al problema. Con la misma instrucción, puede generar campos calculados similares para proyectos, problemas y otros objetos.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>paquete de Adobe Workfront</p> </td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront</p> </td> 
   <td>
      <p>Estándar</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configuraciones de nivel de acceso</p></td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto</p> </td> 
   <td> <p>Acceso de aportación al objeto donde se adjunta el formulario con acceso a Editar el formulario personalizado</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar el administrador del creador de un problema en el formulario personalizado del problema

Los siguientes pasos muestran cómo se puede crear un campo calculado para un formulario personalizado de problema en el que se puede capturar el nombre del administrador del usuario que creó el problema. El proceso es idéntico a cuando desea capturar el nombre del administrador de un usuario que creó una tarea, un proyecto o un portafolio, por ejemplo.

1. Cree un formulario personalizado de problema y añádale un campo calculado.

   Para obtener información sobre cómo crear un formulario personalizado y añadirle campos calculados, consulte los siguientes artículos:

   * [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Copie y pegue el siguiente código de modo de texto en el campo **Cálculo** del formulario personalizado:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Los cálculos de campos personalizados distinguen entre mayúsculas y minúsculas.

1. Haga clic en **Listo**, luego **Guardar + Cerrar**.

   El administrador del usuario que creó el problema se muestra en el campo calculado cuando el formulario que contiene el campo se adjunta a un problema.
