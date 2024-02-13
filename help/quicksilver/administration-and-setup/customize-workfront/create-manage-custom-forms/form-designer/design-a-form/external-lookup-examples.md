---
title: Ejemplos del campo Búsqueda externa en un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Un campo de búsqueda externa en un formulario personalizado llama a una API externa y devuelve valores como opciones en un campo desplegable. Este artículo proporciona ejemplos del uso del campo Búsqueda externa para llamar a la misma instancia de Workfront o a una API pública.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: a082f010dbd78235aaad41a80d87d772ca77ff89
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Ejemplos del campo Búsqueda externa en un formulario personalizado

Un campo de búsqueda externa en un formulario personalizado llama a una API externa y devuelve valores como opciones en un campo desplegable. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado pueden seleccionar una o más de estas opciones en la lista desplegable.

Este artículo proporciona ejemplos del uso del campo Búsqueda externa para llamar a la misma instancia de Workfront o a una API pública. También puede utilizar la búsqueda externa para comunicarse con un sistema externo como Jira, Salesforce o ServiceNow.

Para obtener más información sobre cómo agregar un campo de búsqueda externa a un formulario personalizado y definiciones adicionales de los componentes de búsqueda externos, consulte [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configure un campo de búsqueda externa para la misma instancia de Workfront

Puede utilizar la búsqueda externa para introducir datos de la instancia de Workfront en el formulario personalizado.

Este ejemplo muestra cómo llamar a la API de Workfront y llevar los datos del campo &quot;Consulta de estado&quot; existente al campo de búsqueda externa.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Introduzca el **Etiqueta** y **Nombre** para el campo.
1. Seleccione el **Formato** para el campo.
1. Introduzca la llamada de URL de API en la **URL de API básica** field.

   * Puede agregar $$HOST para hacer referencia a la misma instancia.
   * Puede agregar $$QUERY para filtrar los resultados en función de la consulta a un campo diferente.

   **Ejemplo**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Revise la **Dependencias** para los campos a los que hace referencia este campo de búsqueda en la API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo existente en la página de detalles del objeto.

   En este ejemplo, la variable `{DE:StatusQuery}` se reemplazará por el valor del campo personalizado StatusQuery.

1. Seleccione el **Método HTTP**.

   Es muy probable que así sea **Obtener**.

1. Introduzca el **Ruta de JSON** para obtener los resultados de su llamada de API.

   **Ejemplo**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Header** no se requiere información para una llamada a la misma instancia de Workfront.

1. Clic **Aplicar**.

   ![Configuración de la llamada de API a Workfront en formulario personalizado](assets/external-lookup-to-workfront.png)

   Cuando se agrega el formulario personalizado a un objeto de Workfront (en este ejemplo, un proyecto), tiene un aspecto similar al siguiente.

   ![Formulario personalizado con campo de búsqueda externo](assets/external-lookup-project-status-example1.png)

   ![Opciones de búsqueda externa basadas en el estado](assets/external-lookup-project-status-example2.png)

## Configurar un campo de búsqueda externa para una API pública

Puede utilizar la búsqueda externa para llamar a una API pública externa y recuperar datos.

Este ejemplo muestra cómo llamar a una API de países (como <https://api.first.org/data/v1/countries>) para que no tenga que codificar obligatoriamente todos los nombres de países en las opciones desplegables.

1. Abra el formulario personalizado.
1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. Introduzca el **Etiqueta** y **Nombre** para el campo.
1. Seleccione el **Formato** para el campo.
1. Introduzca la llamada de URL de API en la **URL de API básica** field.

   * Puede agregar $$QUERY para implementar el filtrado de consultas para los usuarios finales.

   **Ejemplos**
Enumera todos los países: <https://api.first.org/data/v1/countries>

   Permite al usuario buscar cualquier país en el campo desplegable: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Permite al usuario buscar un país en una región: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Las regiones disponibles se definen en un campo personalizado independiente en Workfront.
   * Cuando el usuario selecciona una región en el formulario, el campo Búsqueda externa muestra solo los países de esa región (qué país está en la región definida en la API). El usuario también puede buscar un país en la región seleccionada.

1. Revise la **Dependencias** para los campos a los que hace referencia este campo de búsqueda en la API.

   Un campo de dependencia puede ser cualquier campo personalizado o nativo existente en la página de detalles del objeto.

   En este ejemplo, la variable `{DE:Region}` se reemplazará por el valor del campo personalizado Región.

1. Seleccione el **Método HTTP**.

   Es muy probable que así sea **Obtener**.

1. Introduzca el **Ruta de JSON** para obtener los resultados de su llamada de API.

   Esta opción permite extraer datos del JSON devuelto por la dirección URL de la API. Sirve para seleccionar qué valores dentro del JSON aparecerán en las opciones desplegables.

   **Ejemplo**
   `$.data[*].country`

1. (Opcional) Haga clic en **Añadir encabezado** y escriba o pegue el par clave-valor necesario para la autenticación con la API.

   >[!NOTE]
   >
   >Los campos Encabezado no son un lugar seguro para almacenar credenciales y debe tener cuidado con lo que escribe y guarda.

1. (Opcional) Seleccione **Lista desplegable de selección múltiple** para permitir que el usuario seleccione más de un valor en la lista desplegable.

1. Clic **Aplicar**.

   ![Configuración de la llamada de API a la API pública en formato personalizado](assets/external-lookup-to-api-for-countries.png)

   Cuando se agrega el formulario personalizado a un objeto de Workfront (en este ejemplo, un proyecto), tiene un aspecto similar al siguiente.

   ![Formulario personalizado con campo de búsqueda externo](assets/external-lookup-countries-example1.png)

   ![Opciones de búsqueda externa para un país según la región](assets/external-lookup-countries-example2.png)

