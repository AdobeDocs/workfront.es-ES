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
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1318'
ht-degree: 0%

---

# Ejemplos del campo de búsqueda externa en un formulario personalizado

Un campo de búsqueda externa en un formulario personalizado llama a una API externa y devuelve valores como opciones en un campo desplegable. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado pueden seleccionar una o más de estas opciones en la lista desplegable.

Este artículo proporciona ejemplos del uso del campo Búsqueda externa para llamar a la misma instancia de Workfront o a una API pública. También puede utilizar la Búsqueda externa para comunicarse con un sistema externo como Jira, Salesforce o ServiceNow.

Para obtener más información sobre cómo agregar un campo de búsqueda externa a un formulario personalizado y definiciones adicionales de los componentes de búsqueda externa, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configurar un campo de búsqueda externa para la misma instancia de Workfront

Puede utilizar la búsqueda externa para introducir datos de la instancia de Workfront en el formulario personalizado.

### Utilice valores de campo de Workfront nativos en la búsqueda externa

Este ejemplo muestra cómo llamar a la API de Workfront y llevar los datos del campo &quot;Consulta de estado&quot; existente al campo de búsqueda externa.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Escriba **Label** y **Name** para el campo.
1. Seleccione **Formato** para el campo.
1. Escriba la llamada de API en el campo **URL de API base**.

   * Para hacer referencia a la misma instancia de Workfront en la que se encuentra el formulario personalizado, utilice $$HOST para la dirección URL.
   * Para filtrar los resultados según la consulta a un campo diferente, agregue $$QUERY.

   **Ejemplo**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Revise las **dependencias** para los campos a los que hace referencia este campo de búsqueda en la API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo existente en la página de detalles del objeto.

   En este ejemplo, `{DE:StatusQuery}` se reemplazará por el valor del campo personalizado StatusQuery.

1. Seleccione el **método HTTP**.

   Es muy probable que esto sea **Get**.

1. Escriba la **ruta de acceso JSON** para obtener los resultados de su llamada de API.

   **Ejemplo**
   `$.data[*].name`

   >[!NOTE]
   >
   >No se necesita información de **Header** para llamar a la misma instancia de Workfront.

1. Haga clic en **Aplicar**.

   ![Configuración de la llamada API a Workfront en formulario personalizado](assets/external-lookup-to-workfront.png)

   Cuando se agrega el formulario personalizado a un objeto de Workfront (en este ejemplo, un proyecto), tiene un aspecto similar al siguiente.

   ![Formulario personalizado con campo de búsqueda externa](assets/external-lookup-project-status-example1.png)

   ![Opciones de búsqueda externa basadas en el estado](assets/external-lookup-project-status-example2.png)

### Usar valores de campo personalizados en la búsqueda externa

Este ejemplo muestra cómo llamar a la API de Workfront e introducir datos de un campo personalizado en el campo de búsqueda externa. El campo personalizado de ejemplo se denomina &quot;Colores personalizados&quot;.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Escriba **Label** y **Name** para el campo.
1. Seleccione **Formato** para el campo.
1. Escriba la llamada de URL de API en el campo **URL de API básica**.

   **Ejemplo**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Revise las **dependencias** para los campos a los que hace referencia este campo de búsqueda en la API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo existente en la página de detalles del objeto.

1. Seleccione el **método HTTP**.

   Es muy probable que esto sea **Get**.

1. Escriba la **ruta de acceso JSON** para obtener los resultados de su llamada de API.

   **Ejemplo**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * &quot;parameterValues&quot; hace referencia a cualquier campo personalizado de Workfront para el objeto en el que se encuentra.
   * Para este ejemplo, &quot;DE: Colores combinados&quot; es el campo personalizado específico que contiene los valores que desea recuperar.

   >[!NOTE]
   >
   >No se necesita información de **Header** para llamar a la misma instancia de Workfront.

1. Haga clic en **Aplicar**.

   Cuando se agrega el formulario personalizado a un objeto de Workfront, todos los valores del campo &quot;Colores combinados&quot; aparecen en la lista desplegable Campo de búsqueda externa.

## Configurar un campo de búsqueda externa para la API de Workfront Planning

Hay un punto final disponible en la API de Workfront Planning para buscar registros por ID de tipo de registro a través del método Get. Puede utilizar este extremo para hacer referencia a registros de Planning en campos de búsqueda externos.

* **URL de API básica:** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **Método HTTP:** Get
* **Ruta de acceso JSON:** `$.records[*].data.{fieldID}`

  **{fieldID}** es el campo que se mostrará en los resultados de búsqueda externa en el formulario personalizado para los usuarios finales.

Para obtener más información, consulte [API de Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

## Configurar un campo de búsqueda externa para una API pública

Puede utilizar la Búsqueda externa para llamar a una API pública externa y recuperar datos.

Este ejemplo muestra cómo llamar a una API de países (como <https://api.first.org/data/v1/countries>) para que no tenga que codificar en el código todos los nombres de países en las opciones desplegables.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Escriba **Label** y **Name** para el campo.
1. Seleccione **Formato** para el campo.
1. Escriba la llamada de URL de API en el campo **URL de API básica**.

   * Puede agregar $$QUERY para implementar el filtrado de consultas para los usuarios finales.

   **Ejemplos**
Lista todos los países: <https://api.first.org/data/v1/countries>

   Permite que el usuario busque cualquier país en el campo desplegable: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Permite que el usuario busque un país en una región: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Las regiones disponibles se definen en un campo personalizado independiente en Workfront.
   * Cuando el usuario selecciona una región en el formulario, el campo Búsqueda externa muestra solo los países de esa región (qué país está en qué región se define en la API). El usuario también puede buscar un país en la región seleccionada.

1. Revise las **dependencias** para los campos a los que hace referencia este campo de búsqueda en la API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo existente en la página de detalles del objeto.

   En este ejemplo, `{DE:Region}` se reemplazará con el valor del campo personalizado Región.

1. Seleccione el **método HTTP**.

   Es muy probable que esto sea **Get**.

1. Escriba la **ruta de acceso JSON** para obtener los resultados de su llamada de API.

   Esta opción permite extraer datos del JSON devuelto por la dirección URL de la API. Sirve para seleccionar qué valores dentro del JSON aparecerán en las opciones desplegables.

   **Ejemplo**
   `$.data[*].country`

1. (Opcional) Haga clic en **Agregar encabezado** y escriba o pegue el par clave-valor necesario para la autenticación con la API.

   >[!NOTE]
   >
   >Los campos Encabezado no son un lugar seguro para almacenar credenciales y debe tener cuidado con lo que escribe y guarda.

1. (Opcional) Seleccione **Lista desplegable de selección múltiple** para permitir que el usuario seleccione más de un valor en la lista desplegable.

1. Haga clic en **Aplicar**.

   ![Configuración de la llamada de API a la API pública en el formulario personalizado](assets/external-lookup-to-api-for-countries.png)

   Cuando se agrega el formulario personalizado a un objeto de Workfront (en este ejemplo, un proyecto), tiene un aspecto similar al siguiente.

   ![Formulario personalizado con campo de búsqueda externa](assets/external-lookup-countries-example1.png)

   ![Opciones de búsqueda externa para un país según la región](assets/external-lookup-countries-example2.png)

## Casos de uso adicionales para campos de búsqueda externos

Existen muchos otros casos de uso para crear una búsqueda externa.

**Caso de uso:** Reemplace los campos de escritura anticipada, ya que pueden causar problemas con los informes.
**Solución:** Use una llamada API a los objetos existentes en el sistema.

Ejemplo de URL de API base para plantillas, para reemplazar un campo de escritura anticipada:
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**Caso de uso:** Cree campos desplegables con más características (por ejemplo, hay ajuste de línea en el campo de búsqueda externa).
**Solución:** Use una llamada API a los objetos existentes del sistema o cree un nuevo objeto y use una llamada API a este objeto.

**Caso de uso:** defina una forma para que los usuarios mantengan sus propios campos fuera del área de formularios personalizados. Configure el campo Búsqueda externa y puede proporcionar usuarios a los objetos que componen el campo. Esta opción es adecuada para equipos y campos de alto mantenimiento.
**Solución:** Cree un nuevo objeto y use una llamada API a este objeto.

**Caso de uso:** Integración con objetos fuera de Workfront. Por ejemplo, acceder a otro sistema para obtener el nombre de cada usuario, en lugar de estar restringido en un campo de escritura anticipada.
**Solución:** Automatización de Webhook/Fusion para conectarse a otros sistemas.

