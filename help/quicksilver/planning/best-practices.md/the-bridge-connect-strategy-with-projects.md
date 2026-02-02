---
title: 'Bridge: Conexión de la intención estratégica con los proyectos'
description: Aprenda a crear un "hilo estratégico" entre sus planes de alto nivel en Adobe Workfront Planning y su ejecución diaria de flujos de trabajo en Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---


# El puente: conectar la intención estratégica con los proyectos


## Meta

Aprenda a crear un &quot;hilo estratégico&quot; entre sus planes de alto nivel en Workfront Planning y su ejecución diaria en el módulo Flujo de trabajo.



## Información general

Al conectar tu estrategia con tu trabajo diario, la visión se convierte en realidad. Cuando los planes de alto nivel están sincronizados con la ejecución, se crea un **subproceso estratégico** que garantiza que todos los proyectos y tareas hagan avanzar la empresa.



Para lograr esta alineación se necesita un conjunto de vínculos técnicos y protecciones de procesos que conecten los esfuerzos del **módulo de flujo de trabajo** con los registros estratégicos de **Workfront Planning (WFP)**. Al reducir la brecha entre la planificación y la acción, se asegura de que la energía de su equipo siempre se centre en sus objetivos de mayor prioridad.



## La base: establecer la conexión

Antes de poder vincular la planificación y la ejecución, un administrador del espacio de trabajo debe definir qué tipos de registro son aptos para una conexión.



### El campo de conexión: El protocolo de enlace técnico

El puente comienza con un **campo de conexión**. Este tipo de campo es el motor de todas las relaciones en WFP. Es una expresión de intención, en el sentido de que establece que un tipo de registro específico (como una *táctica de canal*) puede vincularse a otros objetos, tanto si se encuentran en el módulo de flujo de trabajo como en la propia planificación.



### Decidir la conexión

El establecimiento de esta asignación es una decisión de nivel de configuración que generalmente se produce antes de crear cualquier trabajo. Al agregar un campo de conexión, está creando el entorno para admitir un &quot;subproceso estratégico&quot;, independientemente de cómo se creen finalmente los registros individuales.



## Estrategia y ejecución sincronizadas

Para mantener la capa estratégica centrada, recomendamos enfocar los registros de planificación en la intención de alto nivel mientras se utiliza el módulo Flujo de trabajo para la ejecución táctica. Este enfoque utiliza las ventajas exclusivas de ambos módulos:



* **Planificación de Workfront (la capa estratégica):** Permanece de alto nivel. Rastrea la *campaña*, la *táctica del canal* y el *presupuesto*. No hace ruido y está preparado para ejecutivos.

* **Módulo de flujo de trabajo (la capa de ejecución):** Administra los detalles tácticos. Las &quot;experiencias&quot; o &quot;actividades&quot; individuales se administran aquí como **proyectos, tareas y problemas**.



## Activación del puente: de la intención a la acción

Una vez configurada la conexión, debe decidir cómo activar el vínculo entre un registro estratégico específico y un proyecto de ejecución.



### Clasificación profesional: la ruta guiada por tablas

Los estrategas y los usuarios avanzados a menudo usan la **vista de tabla** como su &quot;área de trabajo&quot; para perfeccionar los planes a lo largo del tiempo.

* **Entrega intencionada:** De forma predeterminada, la creación de un registro en una tabla no establece un vínculo al módulo Flujo de trabajo. La conexión a un proyecto de ejecución se establece cuando un usuario decide activar el vínculo. Esto se puede hacer creando manualmente un proyecto conectado descendente directamente desde el campo de conexión en WFP o una **página de vista de conexión** opcional en la vista de detalles del registro. Tenga en cuenta que la creación manual genera un proyecto en blanco sin formularios personalizados específicos; para necesidades más complejas, puede utilizar una **automatización nativa de WFP**. Estas automatizaciones están disponibles cuando selecciona una fila en una tabla y aparecen como botones en la barra de acciones azul en la parte inferior de la pantalla. Esto permite la supervisión humana o la creación de marcadores de posición, lo que garantiza que los proyectos solo se generen en el entorno de flujo de trabajo cuando realmente se necesitan.



### Activación automatizada

Para organizaciones con solicitudes de gran volumen o necesidades de automatización avanzadas, el puente se puede activar automáticamente en función de eventos específicos o valores de campo.

* **déclencheur de envío:** Debido a que los formularios proporcionan un único &quot;evento de envío&quot; limpio, se pueden usar como déclencheur para **automatizaciones de Fusion**. Un escenario puede detectar un envío de formulario y generar inmediatamente un proyecto vinculado en el módulo de flujo de trabajo.

* **déclencheur de valor de campo:** Para una automatización más profunda, puede configurar **Fusion** para que supervise campos específicos. Por ejemplo, una casilla de verificación simple etiquetada como &quot;listo para la ejecución&quot; puede servir como catalizador y establecer el puente automáticamente en el momento en que se selecciona.



## Visibilidad de superficie: campos de búsqueda

Una vez vinculado un proyecto, puede obtener datos en tiempo real del módulo Flujo de trabajo directamente en el registro WFP.



Un administrador del área de trabajo puede configurar **campos de búsqueda** para extraer cualquier campo nativo o personalizado del proyecto vinculado (como *fecha real de finalización* o *posible cliente creativo*) en el tipo de registro de WFP. Una vez capturados, estos datos se pueden resumir en varios niveles de la jerarquía estratégica, incluso hasta el nivel de campaña. Esto proporciona potentes informes agregados para las partes interesadas en todo el ciclo de vida del marketing, lo que les mantiene informados sin necesidad de abandonar el entorno de planificación.



## Visibilidad de estrategia a acción

El valor definitivo del puente es **visibilidad en tiempo real**. Al conectar la intención con la acción, puede responder preguntas comerciales críticas de un vistazo:



* &quot;¿Está nuestra campaña &#39;Conocimiento de marca del año fiscal 2026&#39; dando resultados de forma activa en este momento?&quot;

* &quot;¿Dónde necesitan nuestras tácticas estratégicas más apoyo creativo para cumplir con el programa?&quot;

* &quot;¿Cómo estamos alineando nuestros recursos con nuestros pilares estratégicos de máxima prioridad?&quot;



## Prácticas recomendadas y sugerencias



### Haga:

* **Utilice la metáfora de &quot;hilo estratégico&quot;.** Recuerde a los equipos que cada proyecto debe ser un &quot;hilo&quot; en una cadena estratégica.

* **Automatice el traspaso.** Use automatizaciones para almacenar en déclencheur la creación de proyectos a fin de ahorrar tiempo y esfuerzo, a la vez que se mejora la conectividad y el control de datos.

* **Vínculo, no lo duplique.**: utilice campos de búsqueda para que aparezcan datos de ejecución en tiempo real (como fechas de estado o finalización) en los registros estratégicos. Esto garantiza que sus vistas estratégicas sean siempre precisas sin necesidad de actualizaciones manuales por parte de su equipo.



### No haga lo siguiente:

* **No trate los registros de planificación como listas de tareas.**: el puente está diseñado para conectar la intención estratégica con los proyectos de ejecución. Mantenga los registros de planificación centrados en el &quot;qué&quot; y el &quot;por qué&quot;, y permita que el módulo de flujo de trabajo gestione el &quot;cómo&quot; granular a través de las tareas y los problemas.

* **No sincronizar en exceso.** No es necesario que vuelva a sincronizar todos los detalles de nivel de proyecto con Planning. Mantenga la capa estratégica de alto nivel y libre de ruido.

* **No saltes el puente.** Si el trabajo comienza en el módulo Flujo de trabajo sin un vínculo a Planning, ha creado un &quot;Plan en la sombra&quot; que es invisible para el liderazgo.




