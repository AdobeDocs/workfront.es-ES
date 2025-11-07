---
title: Ejemplos del campo de búsqueda externa en un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Un campo de búsqueda externa en un formulario personalizado llama a una API externa y devuelve valores como opciones en un campo desplegable. Este artículo proporciona ejemplos del uso del campo Búsqueda externa para llamar a la misma instancia de Workfront o a una API pública.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 3838e355c16275b9e10fb92497f1698ac99c4fa4
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 79%

---

# Ejemplos del campo de búsqueda externa en un formulario personalizado

Un campo de búsqueda externa en un formulario personalizado llama a una API externa y devuelve valores como opciones en un campo desplegable. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado pueden seleccionar una o más de estas opciones en la lista desplegable.

Este artículo proporciona ejemplos del uso del campo Búsqueda externa para llamar a la misma instancia de Workfront o a una API pública. También puede utilizar la Búsqueda externa para comunicarse con un sistema externo como Jira, Salesforce o ServiceNow.

Para obtener más información sobre cómo agregar un campo de búsqueda externa a un formulario personalizado y definiciones adicionales de los componentes de búsqueda externa, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar un campo de búsqueda externa para la misma instancia de Workfront

Puede utilizar la búsqueda externa para introducir datos de la instancia de Workfront en el formulario personalizado.

<!--When someone accesses the field in the custom form, they will only see in the list of options what they have permissions to see in Workfront. For example, if you are showing a list of projects, the user would only see projects that are shared with them.-->

### Utilice valores de campo de Workfront nativos en la búsqueda externa

En este ejemplo se muestra cómo llamar a la API de Workfront y rellenar una lista de proyectos en un campo de búsqueda externa, filtrados por estado mediante el valor del campo personalizado &quot;Consulta de estado&quot; y un término de búsqueda mediante $$QUERY.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Escriba la **Etiqueta** y el **Nombre** para el campo.
1. Seleccione el **Formato** para el campo.
1. Escriba la llamada de API en el campo **URL de API base**.

   * Utilice $$HOST para hacer referencia a la misma instancia de Workfront donde está el formulario personalizado.
   * Utilice $$QUERY para filtrar dinámicamente los resultados en función de los datos introducidos por el usuario.

   **Ejemplo de llamada de API**
   `$$HOST/attask/api/v15.0/project/search?status={DE:Status Query}&description=$$QUERY`

1. Revise las **dependencias** para los campos a los que se hace referencia en la llamada de API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo disponible en el objeto. Por ejemplo, al crear un formulario personalizado para grupos que incluya un campo de búsqueda externo, los campos de dependencia pueden incluir cualquier campo disponible en un grupo.

   En este ejemplo, `{DE:Status Query}` se reemplazará dinámicamente con el valor del campo personalizado &quot;Consulta de estado&quot; para el grupo actual. Por lo tanto, cuando el formulario se adjunta al grupo A, `{DE:Status Query}` se reemplaza por el valor establecido en el campo &quot;Consulta de estado&quot; para ese grupo.

1. Seleccione el **método HTTP**.

   Es muy probable que este sea **Get**.

1. Escriba la **ruta JSON** para obtener los resultados de su llamada de API.

   **Ejemplo**
   `$.data[*].name`

   >[!NOTE]
   >
   >No se necesita información del **Encabezado** para llamar a la misma instancia de Workfront.

1. Haga clic en **Aplicar**.

   ![Configuración de la llamada de API a Workfront en formulario personalizado](assets/external-lookup-to-workfront.png)

   Cuando se añade el formulario personalizado a un objeto de Workfront (en este ejemplo, un proyecto), tiene un aspecto similar a este.

   ![Formulario personalizado con campo de búsqueda externa](assets/external-lookup-project-status-example1.png)

   ![Opciones de búsqueda externa basadas en el estado](assets/external-lookup-project-status-example2.png)

### Usar valores de campo personalizados en la búsqueda externa

Este ejemplo muestra cómo llamar a la API de Workfront e introducir datos de un campo personalizado en el campo de búsqueda externa. El campo personalizado de ejemplo se denomina “Colores personalizados”.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Escriba la **Etiqueta** y el **Nombre** para el campo.
1. Seleccione el **Formato** para el campo.
1. Escriba la llamada de URL de API en el campo **URL de API básica**.

   **Ejemplo**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Revise las **Dependencias** para los campos a los que hace referencia este campo de búsqueda en la API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo existente en la página de detalles del objeto.

1. Seleccione el **Método HTTP**.

   Es muy probable que este sea **Get**.

1. Escriba la **ruta JSON** para obtener los resultados de su llamada de API.

   **Ejemplo**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * &quot;parameterValues&quot; hace referencia a cualquier campo personalizado de Workfront para el objeto en el que se encuentra.
   * Para este ejemplo, &quot;DE:Combo Colores&quot; es el campo personalizado específico que contiene los valores que desea recuperar.

   >[!NOTE]
   >
   >No se necesita información del **Encabezado** para llamar a la misma instancia de Workfront.

1. Haga clic en **Aplicar**.

   Cuando se añade el formulario personalizado a un objeto de Workfront, todos los valores del campo &quot;Colores combinados&quot; aparecen en la lista desplegable del campo de búsqueda externa.

## Configurar un campo de búsqueda externa para la API de Workfront Planning

Hay un punto final disponible en la API de Workfront Planning para buscar registros por ID de tipo de registro a través del método Get. Puede utilizar este extremo para hacer referencia a registros de Planning en campos de búsqueda externos.

* **URL de API básica:** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **Método HTTP:** Get
* **Ruta de acceso JSON:** `$.records[*].data.{fieldID}`

  **{fieldID}** es el campo que se mostrará en los resultados de búsqueda externa en el formulario personalizado para los usuarios finales.

Para obtener más información, consulte [API de Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

## Configurar un campo de búsqueda externa para una API pública

Puede utilizar la Búsqueda externa para llamar a una API pública externa y recuperar datos.

Este ejemplo muestra cómo llamar a una API de países (como <https://api.first.org/data/v1/countries>) para no tener que codificar todos los nombres de los países en las opciones desplegables.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Escriba la **Etiqueta** y el **Nombre** para el campo.
1. Seleccione el **Formato** para el campo.
1. Escriba la llamada de URL de API en el campo **URL de API básica**.

   * Puede añadir $$QUERY para implementar el filtrado de consultas para los usuarios finales.

   **Ejemplos**
Enumera todos los países: <https://api.first.org/data/v1/countries>

   Permite que el usuario busque cualquier país en el campo desplegable: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Permite que el usuario busque un país en una región: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Las regiones disponibles se definen en un campo personalizado independiente en Workfront.
   * Cuando el usuario selecciona una región en el formulario, el campo Búsqueda externa muestra solo los países de esa región (qué país está en qué región se define en la API). El usuario también puede buscar un país en la región seleccionada.

1. Revise las **dependencias** para los campos a los que hace referencia este campo de búsqueda en la API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo existente en la página de detalles del objeto.

   En este ejemplo, `{DE:Region}` se reemplazará con el valor del campo personalizado Región.

1. Seleccione el **método HTTP**.

   Es muy probable que este sea **Get**.

1. Escriba la **ruta JSON** para obtener los resultados de su llamada de API.

   Esta opción permite extraer datos del JSON devuelto por la URL de la API. Sirve para seleccionar qué valores dentro del JSON aparecerán en las opciones desplegables.

   **Ejemplo**
   `$.data[*].country`

1. (Opcional) Haga clic en **Añadir encabezado** y escriba o pegue el par clave-valor necesario para la autenticación con la API.

   >[!NOTE]
   >
   >Los campos Encabezado no son un lugar seguro para almacenar credenciales y debe tener cuidado con lo que escribe y guarda.

1. (Opcional) Seleccione **Lista desplegable de selección múltiple** para permitir que el usuario seleccione más de un valor en la lista desplegable.

1. Haga clic en **Aplicar**.

   ![Configuración de la llamada de API a la API pública en el formulario personalizado](assets/external-lookup-to-api-for-countries.png)

   Cuando se añade el formulario personalizado a un objeto de Workfront (en este ejemplo, un proyecto), tiene un aspecto similar a este.

   ![Formulario personalizado con campo de búsqueda externa](assets/external-lookup-countries-example1.png)

   ![Opciones de búsqueda externa para un país según la región](assets/external-lookup-countries-example2.png)

## Casos de uso adicionales para campos de búsqueda externos

Existen muchos otros casos de uso para crear una búsqueda externa.

**Caso de uso:** reemplace los campos de escritura anticipada, ya que pueden causar problemas con la creación de informes.
**Solución:** use una llamada de API a los objetos existentes en el sistema.

Ejemplo de URL de API base para plantillas, para reemplazar un campo de escritura anticipada:
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**Caso de uso:** cree campos desplegables con más funciones (por ejemplo, hay salto de línea en el campo Búsqueda externa).
**Solución:** use una llamada de API a los objetos existentes del sistema o cree un nuevo objeto y use una llamada de API a este objeto.

**Caso de uso:** defina una forma para que los usuarios mantengan sus propios campos fuera del área de formularios personalizados. Configure el campo Búsqueda externa y puede proporcionar usuarios a los objetos que componen el campo. Esta opción es adecuada para campos y equipos de alto mantenimiento.
**Solución:** cree un nuevo objeto y use una llamada de API a este objeto.

**Caso de uso:** integración con objetos fuera de Workfront. Por ejemplo, acceder a otro sistema para obtener el nombre de cada usuario, en lugar de estar restringido en un campo de escritura anticipada.
**Solución:** automatización de webhook/Fusion para conectarse a otros sistemas.

