---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Resumen del flujo de trabajo automatizado
description: Los flujos de trabajo automatizados le permiten crear una serie de etapas de revisión secuenciales o paralelas, establecer dependencias entre estas etapas y limitar su visibilidad a ciertos usuarios. Si hay etapas interdependientes en el proceso de revisión, los flujos de trabajo automatizados mueven la prueba a través de las fases automáticamente, notificando a los revisores y aprobadores relevantes a lo largo del camino. Para obtener información sobre la configuración de un flujo de trabajo automatizado, consulte Creación de una prueba avanzada con un flujo de trabajo automatizado.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Resumen del flujo de trabajo automatizado

Los flujos de trabajo automatizados le permiten crear una serie de etapas de revisión secuenciales o paralelas, establecer dependencias entre estas etapas y limitar su visibilidad a ciertos usuarios. Si hay etapas interdependientes en el proceso de revisión, los flujos de trabajo automatizados mueven la prueba a través de las fases automáticamente, notificando a los revisores y aprobadores relevantes a lo largo del camino. Para obtener información sobre la configuración de un flujo de trabajo automatizado, consulte [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Ejemplos:**  Los flujos de trabajo automatizados ayudan a administrar procesos complejos de revisión de pruebas como

* Cuando distintos grupos o revisores necesitan revisar el contenido en un orden determinado
* Cuando hay dependencias entre la actividad de los usuarios a medida que revisan el contenido
* Cuando el contenido lo revisan regularmente los mismos grupos de personas
* Cuando desea controlar el periodo de tiempo en el que los revisores miran el contenido
* Cuando desee mantener privada alguna actividad de revisión

## Fases

Para cada fase del flujo de trabajo automatizado, puede configurar opciones como una fecha límite para la fase, un bloqueo en una fase, un revisor establecido como responsable de la toma de decisiones de la fase y una configuración de privacidad que permita que solo determinadas personas vean los comentarios del revisor en la fase.

Los escenarios se pueden activar manualmente, durante la creación de la prueba, al alcanzar una fecha y hora límite, en una fecha y hora específicas o cuando se toma una decisión en la fase principal.

Los escenarios se pueden bloquear manualmente, así como cuando se inicia la siguiente etapa o cuando se toman todas las decisiones en el escenario. También puede elegir no bloquear nunca un escenario.

Puede designar a un responsable principal de la toma de decisiones para una etapa. La decisión de esta persona hace innecesarias todas las demás decisiones de la etapa.

Del mismo modo, puede optar por requerir solo una decisión en una etapa. Al hacerlo, el proceso de revisión de la etapa se marca como completado después de que cualquiera de los destinatarios tome una decisión sobre la etapa.

Puede hacer que todos los revisores reciban notificaciones sobre su invitación para revisar el contenido cuando comience el proceso de revisión, o puede que cada revisor reciba una notificación solo cuando se active su fase.

## Etapas privadas

De forma predeterminada, los comentarios dejados por los revisores en todas las etapas son visibles para todos los que revisan el contenido y reciben notificaciones por correo electrónico y resúmenes de comentarios sobre el proceso de revisión.

Si desea evitar que ciertos grupos de revisores vean los comentarios de otros revisores, puede crear escenarios privados.

Las etapas privadas solo son visibles para los revisores agregados a esas etapas. También son visibles para los usuarios que tienen derechos de edición en la prueba o edita en todos los elementos creados en la cuenta de Adobe Workfront de su organización (Supervisor y superiores o usuarios con perfiles personalizados para los que está habilitada la edición de información de otras personas).

Los comentarios añadidos por los participantes del escenario privado no se incluyen en las notificaciones por correo electrónico ni en los resúmenes de comentarios de prueba solicitados por cualquier persona que no tenga los derechos para verlos.

## Diagrama del flujo de trabajo

El diagrama de flujo de trabajo es una representación visual del proceso de revisión de la prueba. Muestra el orden de las etapas y las dependencias entre ellas a medida que crea o ve los detalles de una prueba. Los escenarios privados se muestran con un símbolo de clave.

![intro-to-aw-example-schem.png](assets/intro-to-aw-example-diagram-350x199.png)

En pruebas en directo, las dependencias de escenario se muestran con una línea gris discontinua para etapas inactivas o una línea negra sólida para etapas activas. Los escenarios se muestran en verde si el proceso de aprobación se completó dentro de la fecha límite especificada. Las etapas que se acercan a sus fechas límite se muestran en naranja y las etapas posteriores a su fecha límite se muestran en rojo.

![workflow_2.png](assets/workflow-2-350x183.png)

## Plantillas de flujo de trabajo automatizadas

Si su organización utiliza el mismo proceso de revisión para varias pruebas, su administrador de Workfront puede crear plantillas de flujo de trabajo automatizado para facilitar la creación de pruebas. Puede elegir una plantilla Flujo de trabajo automatizado mientras configura una prueba para agregar las etapas y los revisores de esa plantilla a la prueba. Puede modificar la plantilla aplicada a la prueba según sea necesario antes y después de crear la prueba.

El administrador de Workfront puede crear un número ilimitado de plantillas según las necesidades de la empresa.

Para obtener más información sobre la creación, el uso y la administración de plantillas, consulte con el administrador de Workfront.
