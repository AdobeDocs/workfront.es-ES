---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Información general sobre modelos
description: Los modelos proporcionan componentes básicos para ayudarle a crear un sistema de gestión del trabajo que crezca con usted.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Información general sobre modelos

Los modelos proporcionan componentes básicos para ayudarle a crear un sistema de gestión del trabajo que crezca con usted. Los administradores del sistema pueden examinar el catálogo de modelos e instalar plantillas de proyecto listas para usar. Otros usuarios pueden examinar el catálogo y solicitar la instalación de un modelo. Para obtener más información, consulte [Examine el catálogo de modelos y solicite la instalación de modelos](../../administration-and-setup/blueprints/browse-catalog.md).

Cada modelo está dirigido a un departamento y a un nivel de madurez específico para ayudarle a implementar las mejores prácticas comprobadas en su sistema con mayor rapidez. Los niveles de vencimiento detallados a continuación se indican en la tarjeta del catálogo del modelo y en los detalles.

**[!UICONTROL Administrado]:** Las plantillas de proyecto gestionadas ayudan a respaldar la adopción de un nuevo proceso empresarial antes de que las actividades y los resultados se acepten completamente como un procedimiento estándar. Contienen tareas para garantizar que se sigue cada paso del nuevo proceso.

**[!UICONTROL Integrado]:** Las plantillas de proyecto integradas suponen que las funciones empresariales se admiten mediante un procedimiento operativo estándar. Los colaboradores del proceso conocen los pasos y tareas que deben completar para seguir el proceso. Las plantillas de proyecto para admitir este proceso contienen menos tareas para rastrear solo hitos y otros entregables clave necesarios para la generación de informes.

## Buscar el modelo adecuado

Puede examinar los modelos por caso de uso, nivel de vencimiento, estado de instalación y escribir con los filtros en el lado derecho del catálogo. Una vez que haya encontrado un modelo que le interese, puede ver los detalles en la página de detalles.

### Tipos de modelos

El tipo de modelo muestra lo que se incluye en el modelo. El tipo se muestra en la parte inferior de la tarjeta de modelo del catálogo. Tenga en cuenta que un modelo puede tener más de un tipo.

Están disponibles los siguientes tipos de modelos:

* Plantillas de proyecto: Incluye objetos estándar asociados a una plantilla de proyecto (tareas, problemas, funciones y equipos) y algunas preferencias relacionadas con esos objetos. Para obtener más información, consulte [Configuración de un modelo](../../administration-and-setup/blueprints/configure-template-package.md).
* Estructuras organizativas: Incluye objetos asociados a la estructura de una organización (empresas, grupos, funciones y equipos). Para obtener más información, consulte [Configuración de un modelo](../../administration-and-setup/blueprints/configure-template-package.md).
* Tableros: Incluye uno o más tableros para un caso de uso específico, como los servicios de implementación.

<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Para revisar los modelos actuales, consulte [Lista de modelos disponibles](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Ver  detalles

Cada modelo contiene una página de detalles. Desde esta página puede:

* Ver un resumen del contenido del flujo de trabajo
* Lea un breve resumen del modelo
* Ver el historial de instalación (haga clic en **[!UICONTROL Consulte Detalles]** para ver la lista completa de objetos instalados con el modelo)
* Consulte las descripciones de funciones, equipos, empresas y grupos
* Ver un ejemplo visual del modelo específico, como una plantilla de proyecto (puede obtener una vista previa de la imagen completa en el explorador o descargarla)

![[!UICONTROL Detalles del modelo] página](assets/blueprint-details-page-2022.png)

## Instalación de un modelo

El administrador del sistema puede realizar la instalación directamente en el entorno de producción o en entornos de entorno limitado. Para obtener más información, consulte [Instalación de un modelo](../../administration-and-setup/blueprints/blueprints-install.md) o [Configuración de un modelo](../../administration-and-setup/blueprints/configure-template-package.md).

Después de la instalación, es posible que no esté seguro de las mejores próximas acciones que realizar. Para obtener más información, consulte [Acciones que deben realizarse después de instalar un modelo](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Notas adicionales sobre modelos y plantillas

Los modelos no sustituyen la funcionalidad de las plantillas de proyecto en [!DNL Adobe Workfront]. Los modelos son una forma de crear nuevas plantillas más rápido para organizar más trabajo en [!DNL Workfront].

No se puede copiar ni editar un modelo. Sin embargo, una vez que haya instalado la solución desde un modelo, puede modificar la plantilla de proyecto, las funciones de trabajo o los equipos que se crean a partir del modelo del mismo modo que normalmente actualiza esos registros en el [!DNL Workfront] interfaz. Además, al instalar un modelo, la plantilla se almacena en la variable [!UICONTROL Plantillas] área de [!DNL Workfront] y el modelo original permanece en el [!UICONTROL Planes] . No es necesario realizar una copia de la plantilla antes de comenzar a adaptarla a sus necesidades.

Los modelos no eliminan ni reemplazan nada configurado en su entorno. Si tiene intención de reemplazar una plantilla existente instalando un modelo que cree una plantilla nueva, le recomendamos que desactive la versión anterior para evitar confusiones entre los planificadores que crean proyectos a partir de plantillas.
