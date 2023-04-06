---
content-type: reference
navigation-topic: betas
title: 'Reporting Canvas beta: descripción general'
description: Información sobre el programa beta para la próxima herramienta de lienzo de informes para Adobe Workfront
author: Nolan
feature: Product Announcements
exl-id: cc0adf28-08ab-4330-b901-219ab687f02f
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Reporting Canvas beta: información general

## Lienzo de informes

La nueva herramienta de lienzo de informes, que se ha reinventado completamente para crear informes en Workfront, está en desarrollo. Al diseñar el Lienzo de informes, hemos trabajado duro para proporcionar una experiencia que ofrezca la máxima flexibilidad, junto con un diseño intuitivo y modular, de modo que los usuarios como usted puedan aprovechar de manera más eficaz sus propios datos al crear y compartir informes. Con un nuevo tipo de informe unificado que le permite arrastrar y soltar casi todos los elementos en un lienzo ilimitado, la creación de una obra maestra de datos visuales será más fácil que nunca.

Este artículo contiene información sobre la versión beta privada actual, que está limitada a clientes específicos. Las nuevas funciones del lienzo de informes ahora se implementan a través de los paneles de lienzo. Consulte **Plan de desarrollo** más abajo para obtener más información.

### Plan de desarrollo

Estamos en las fases finales de resolución de un problema de calidad de datos que observamos al principio de la versión beta del lienzo de informes. Pronto reanudaremos el trabajo para proporcionar nuevas visualizaciones, expandir la selección de objetos de Workfront informables y mejorar las experiencias de creación y distribución de informes, todas las cuales son esenciales para lograr nuestros objetivos para el Lienzo de informes.

Las nuevas experiencias se distribuirán gradualmente, a partir de la versión 23.2, a través de la nueva página Tableros de lienzo que ahora está disponible en su entorno de vista previa. Los paneles de lienzo le permiten mostrar los informes existentes junto con las nuevas funciones de informes que estamos creando, y servirán como entorno principal para implementar y probar nuevas funciones para el lienzo de informes. Para obtener más información sobre cómo habilitar y usar paneles de lienzo, consulte [Información general sobre los paneles de lienzo](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Participar en la versión beta

>[!IMPORTANT]
>
>La información beta siguiente es para administradores que ya se han incluido en la versión beta del lienzo de informes, que ya no aceptan nuevos participantes. Si desea probar las nuevas funciones del lienzo de informes a medida que se agregan, consulte **Plan de desarrollo** más arriba para obtener información sobre cómo habilitar los paneles de lienzo.

### Disponibilidad

La versión beta del lienzo de informes está disponible para todas las organizaciones que estén en AWS, independientemente de la región.

### Únase a la versión beta

La versión beta del lienzo de informes es completamente opcional, pero solo puede seleccionarla un administrador de Workfront. Para activar como administrador del sistema:

1. Seleccione el **Informes (beta)** en el menú Principal de la instancia de Workfront.
1. Haga clic en **Accept** aceptar los términos y condiciones.
1. Permita que los datos de su organización se agreguen al lienzo de informes (puede tardar hasta unas pocas horas).
1. Empiece a usar el Lienzo de informes.

Una vez que los datos de su organización se han agregado al Lienzo de informes, otros administradores de sistemas pueden optar por unirse de forma individual de la misma manera (sin esperar a que se vuelvan a agregar los datos).

Para incluir a otros usuarios que no son administradores de Workfront:

1. Seleccione el **Informes (beta)** en el menú Principal de la instancia de Workfront.
1. Haga clic en **Permisos del lienzo de informes**.
1. Busque y seleccione los usuarios específicos que desea participar.

   >[!IMPORTANT]
   >
   >Los usuarios que conceda acceso al lienzo de informes tendrán acceso a **all** datos del sistema con capacidad de solo lectura, independientemente de sus permisos estándar para ver estos datos.

1. Haga clic en **Guardar**.
1. Agregue la variable **Informes (beta)** en la plantilla de diseño principal de cada usuario seleccionado. Para obtener más información, consulte [Personalización del menú principal mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Cada usuario debe navegar individualmente a la variable **Informes (beta)** en el menú principal y acepte los términos y condiciones.

### Enviar comentarios

Para enviar comentarios sobre la versión beta:

1. En Lienzo de informes en Workfront, haga clic en el botón **Enviar comentarios** botón.
1. Complete el formulario y haga clic en **Submit**.

## Preguntas frecuentes sobre Beta

+++¿Puedo migrar mis informes heredados a Lienzo de informes?

En resumen, la migración de informes heredados no estará disponible durante la versión beta. Sin embargo, se trata de una característica planificada (con algunas advertencias descritas a continuación) para el lanzamiento oficial.

Aunque la barrera para crear nuevos informes se ha reducido significativamente con el Lienzo de informes, entendemos que incorporar algunos de sus informes y tableros existentes ayudará a acelerar el proceso de adopción. Como tal, queremos proporcionar las herramientas y los recursos necesarios para garantizar que puede traer cualquier elemento heredado relevante para garantizar que comienza con el pie derecho en el Lienzo de informes. Sin embargo, como el Lienzo de informes es un cambio tan radical en la forma en que funciona la actual creación de informes, sería imposible migrar todos los informes o tableros exactamente como es hoy.

Nuestra estrategia actual para la migración en la versión oficial es permitirle hacer lo siguiente:

1. Identificar los informes y los tableros que sean relevantes

   1. Permite exportar un CSV de todos los informes y tableros del sistema junto con cualquier información de seguimiento relevante (número de vistas, cuándo y quién lo realizó).
   1. Proporcione una exportación de informes que estén configurados con envíos programados junto con los destinatarios.

1. Seleccione los informes y tableros que desee migrar y, a continuación, haga clic en **Migrar**

   Esta es una migración unidireccional. Crea una copia de los informes y tableros seleccionados en el Lienzo de informes, dejando el tablero o informe preexistente intacto en la herramienta de informes actual.

   Puede migrar el mismo informe o tablero tantas veces como desee.

1. En Lienzo de informes, asegúrese de que se han migrado todos los informes y tableros seleccionados.
+++

+++¿Por qué no puedo ver todos los objetos que normalmente hago?

Para ofrecer la versión beta a nuestros clientes lo antes posible, la hemos lanzado con solo un subconjunto de los muchos tipos de objetos disponibles en Workfront hoy en día. A continuación se muestran los tipos de objeto admitidos actualmente en la versión beta:

* Asignación
* Documento
* Aprobación de documento
* Gasto
* Hora
* Problema
* Nota
* Portafolio
* Proyecto
* Programar
* Tarea
* Hoja de horas
* Elemento de trabajo
+++

+++Si algo sale mal en el Lienzo de informes durante la fase beta, ¿se verán afectados los datos de mi organización?

No. La versión beta utiliza una copia de los datos de su organización que se rellenan en el Lienzo de informes. Aunque esto significa que es seguro experimentar durante la versión beta sin riesgo de afectar a los datos importantes, también significa que la edición en línea de datos en el lienzo de informes no estará disponible hasta el lanzamiento oficial.
+++

+++¿Puedo desactivar la versión beta una vez que me haya unido?

Un administrador de Workfront no puede desactivar la versión beta; sin embargo, los administradores que no sean del sistema pueden eliminarse haciendo lo siguiente:

1. Inicie sesión como administrador del sistema.
1. Vaya al lienzo de informes.
1. Haga clic en Lienzo de informes **permissions**.
1. Elimine de la lista los usuarios que desee excluir de la versión beta que hayan elegido.
1. Haga clic en **Guardar**.
+++
