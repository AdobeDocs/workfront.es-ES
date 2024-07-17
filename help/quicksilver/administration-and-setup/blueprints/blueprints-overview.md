---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Información general de modelos
description: Los modelos son conjuntos de objetos de Workfront que se ocupan de casos de uso comunes en Workfront. Puede descargar e instalar un modelo y, a continuación, configurar los objetos para su caso de uso específico.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: 0da724e975cfb1f0f7e36cffdc545c6223a14a76
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# Información general de modelos

<!--Audited: 01/2024-->

Los modelos son conjuntos de objetos de Workfront que se ocupan de casos de uso comunes en Workfront. Puede descargar e instalar un modelo y, a continuación, configurar los objetos para su caso de uso específico.

![](assets/blueprints-main-page-catalog.png)

>[!INFO]
>
>Ejemplos:
>
>* **Configuración de la organización de recursos humanos**
>
>   Este modelo contiene la configuración de estructuras organizativas para ampliarlas a un departamento de recursos humanos.
>
>* **Agregar nueva lista de comprobación de TI de empleado**
>
>   Este modelo contiene una plantilla para organizar las actividades de incorporación de nuevos empleados. El uso de esta plantilla permite a los equipos de TI operar de forma eficiente, lo que conduce a una nueva experiencia positiva para los empleados y a un camino más rápido hacia la productividad.
>
>* **Conceptos básicos de instancias heredadas | Lista de comprobación**
>
>    Este modelo contiene una plantilla de proyecto (o lista de comprobación) que puede revisar con una breve lista de preguntas, recursos y vínculos para comprender claramente cómo se ha configurado la instancia de Workfront. Utilícelo cuando haya heredado recientemente una instancia de Workfront y necesite instrucciones sobre por dónde empezar.
>
>Para revisar los modelos actuales, vea [Lista de modelos disponibles](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).


Los modelos proporcionan componentes básicos que le ayudarán a crear un sistema de administración del trabajo que crezca con usted. Los administradores del sistema pueden examinar el catálogo de modelos e instalar plantillas de proyecto, tableros y estructuras organizativas listos para usar. Otros usuarios pueden examinar el catálogo y solicitar la instalación de un modelo. Para obtener más información, vea [Examinar el catálogo de modelos y solicitar la instalación de los modelos](../../administration-and-setup/blueprints/browse-catalog.md).

Cada modelo está dirigido a un departamento y a un nivel de madurez específico para ayudarle a implementar las prácticas recomendadas comprobadas en su sistema más rápido. Los niveles de vencimiento detallados a continuación se indican en la tarjeta del catálogo de modelos y detalles.

* **[!UICONTROL Administrado]:** Las plantillas de proyecto administradas ayudan a admitir la adopción de un nuevo proceso empresarial antes de que las actividades y los entregables se acepten completamente como un procedimiento estándar. Contienen tareas para garantizar que se sigue cada paso del nuevo proceso.

* **[!UICONTROL Integrado]:** Las plantillas de proyecto integradas suponen que las funciones empresariales son compatibles mediante un procedimiento operativo estándar. Los colaboradores del proceso conocen los pasos y las tareas que deben completar para seguir el proceso. Las plantillas de proyecto compatibles con este proceso contienen menos tareas para realizar el seguimiento de hitos y otros resultados clave necesarios para la creación de informes.

## Encuentre el modelo correcto

Puede examinar los modelos por caso de uso, nivel de madurez, estado de instalación y tipo con los filtros a la derecha del catálogo. Una vez que haya encontrado un modelo que le interesa, puede ver los detalles en la página de detalles.

### Tipos de modelos

El tipo de modelo muestra lo que se incluye en el modelo. El tipo se muestra en la parte inferior de la tarjeta de modelo del catálogo. Tenga en cuenta que un modelo puede tener más de un tipo.

Están disponibles los siguientes tipos de modelos:

* **Plantillas de proyecto**: incluye objetos estándar asociados a una plantilla de proyecto (tareas, problemas, funciones y equipos) y algunas preferencias relacionadas con esos objetos. Para obtener más información, consulte [Configurar un modelo](../../administration-and-setup/blueprints/configure-template-package.md).
* **Estructuras organizativas**: incluye objetos asociados con la estructura de una organización (compañías, grupos, roles y equipos). Para obtener más información, consulte [Configurar un modelo](../../administration-and-setup/blueprints/configure-template-package.md).
* **Paneles**: incluye uno o más paneles para un caso de uso específico, como los servicios de implementación.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Para revisar los modelos actuales, vea [Lista de modelos disponibles](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Ver detalles

Cada modelo contiene una página de detalles. Desde esta página, puede:

* Ver un resumen del contenido del flujo de trabajo
* Lea un breve resumen del modelo
* Ver el historial de instalación (haga clic en **[!UICONTROL Ver detalles]** para ver la lista completa de objetos instalados con el modelo)
* Consulte descripciones de funciones, equipos, empresas y grupos
* Vea un ejemplo visual del modelo específico, como una plantilla de proyecto (puede previsualizar la imagen completa en el explorador o descargarla)

![[!UICONTROL Detalles de modelo] página](assets/blueprint-details-page-2022.png)

## Instalar un modelo

Un administrador de Workfront puede instalar un modelo directamente en cualquier entorno (entornos de producción, vista previa o zona protegida). Para obtener más información, consulta [Instalar un modelo](../../administration-and-setup/blueprints/blueprints-install.md) o [Configurar un modelo](../../administration-and-setup/blueprints/configure-template-package.md).

Después de la instalación, es posible que no esté seguro de cuáles son las mejores acciones siguientes que debe realizar. Para obtener más información, consulte [Acciones que se deben realizar después de instalar un modelo](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Notas adicionales sobre modelos y plantillas

Los modelos no reemplazan la funcionalidad de plantillas de proyecto en [!DNL Adobe Workfront]. Los modelos son una forma de crear nuevas plantillas más rápido para organizar más trabajo en [!DNL Workfront].

No puede copiar ni editar un modelo. Sin embargo, una vez que haya instalado la solución desde un modelo, puede modificar la plantilla de proyecto, los roles de trabajo o los equipos creados a partir del modelo de la misma manera que suele actualizar esos registros en la interfaz [!DNL Workfront]. Además, al instalar un modelo, la plantilla se almacena en el área [!UICONTROL Plantillas] de [!DNL Workfront] y el modelo original permanece en el área [!UICONTROL Modelos]. No es necesario que realice una copia de la plantilla antes de empezar a adaptarla a sus necesidades.

Los modelos no eliminan ni reemplazan nada configurado en su entorno. Si tiene intención de reemplazar una plantilla existente mediante la instalación de un modelo que cree una nueva plantilla, le recomendamos que desactive la versión anterior para evitar confusiones entre los planificadores que crean proyectos a partir de plantillas.
