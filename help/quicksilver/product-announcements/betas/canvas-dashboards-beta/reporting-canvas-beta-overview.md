---
content-type: reference
navigation-topic: betas
title: "Resumen del lienzo de informes beta:"
description: Información sobre el programa beta para la próxima herramienta Lienzo de informes para Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: true
source-git-commit: 2fa10260b54e4ba2e9ab661ac5a4985a91e69191
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%

---


# Resumen de Lienzo de informes beta

## Lienzo de informes

La nueva herramienta Lienzo de informes, un completo replanteamiento de los informes en Workfront, se encuentra actualmente en desarrollo. Al diseñar el lienzo de informes, hemos trabajado duro para proporcionar una experiencia que ofrezca la máxima flexibilidad junto con un diseño intuitivo y modular, de modo que los usuarios como usted puedan aprovechar de forma más eficaz sus propios datos a la hora de crear y compartir informes. A través de un nuevo tipo de informe unificado que le permite arrastrar y soltar casi todos los elementos en un lienzo ilimitado, la creación de una obra maestra de datos visuales pronto será más fácil que nunca.

Este artículo contiene información sobre la versión beta privada actual, que se limita a clientes específicos. Ahora se están implementando nuevas funciones del lienzo de informes a través de los paneles del lienzo. Consulte **Plan de desarrollo** para obtener más información.

### Plan de desarrollo

Estamos en las últimas etapas para resolver un problema de calidad de datos que observamos al principio del lienzo de informes beta. Próximamente reanudaremos el trabajo para proporcionar nuevas visualizaciones, ampliar la selección de objetos de Workfront sobre los que se pueden realizar informes y mejorar las experiencias de creación y distribución de informes, todo lo cual es integral para lograr nuestros objetivos para el lienzo de informes.

Entregaremos estas nuevas experiencias de forma incremental, a partir de la versión 23.2, a través de la nueva página Paneles de lienzo que ahora está disponible en su entorno de vista previa. Los paneles de lienzo le permiten mostrar los informes existentes junto con las nuevas funciones de creación de informes que estamos creando y servirán como nuestro entorno principal para implementar y probar nuevas funciones para el lienzo de informes. Para obtener más información sobre cómo habilitar y utilizar paneles de lienzo, consulte [Información general sobre paneles de lienzo](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Participar en la versión beta

>[!IMPORTANT]
>
>La siguiente información sobre la versión beta es para administradores que ya se han incluido en la versión beta del lienzo de informes, que ya no acepta nuevos participantes. Si desea probar las nuevas funciones del lienzo de informes a medida que se agregan, consulte **Plan de desarrollo** para obtener información sobre cómo habilitar los paneles de lienzo.

### Disponibilidad

La versión beta del lienzo de informes está disponible para todas las organizaciones que se encuentran en AWS, independientemente de la región.

### Unirse a la versión beta

La versión beta del lienzo de informes es completamente opcional, pero solo un administrador de Workfront puede aceptarla. Para registrarse como administrador del sistema:

1. Seleccione el **Creación de informes (beta)** en el menú principal de su instancia de Workfront.
1. Clic **Aceptar** para aceptar los términos y condiciones.
1. Permita que los datos de su organización se añadan al lienzo de informes (puede tardar hasta unas horas).
1. Empiece a utilizar el lienzo de informes.

Una vez que los datos de su organización se hayan agregado al lienzo de informes, otros administradores del sistema podrán optar por unirse de forma individual de la misma manera (sin esperar a que se vuelvan a agregar los datos).

Para activar a otros usuarios que no sean administradores de Workfront:

1. Seleccione el **Creación de informes (beta)** en el menú principal de su instancia de Workfront.
1. Haga clic en **Permisos del lienzo de informes**.
1. Busque y seleccione los usuarios específicos en los que desea participar.

   >[!IMPORTANT]
   >
   >Los usuarios a los que conceda acceso al lienzo de informes tendrán acceso a **todo** Los datos del sistema son de solo lectura, independientemente de sus permisos estándar para ver estos datos.

1. Haga clic en **Guardar**.
1. Añada el **Creación de informes (beta)** en la plantilla de diseño principal de cada usuario seleccionado. Para obtener más información, consulte [Personalización del menú principal mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. A continuación, cada usuario debe navegar individualmente a **Creación de informes (beta)** en el menú principal y acepte los términos y condiciones.

### Enviar comentarios

Para enviar comentarios sobre la versión beta:

1. En el lienzo de informes de Workfront, haga clic en **Enviar comentarios** botón.
1. Rellene el formulario y haga clic en **Enviar**.

## Preguntas frecuentes sobre beta

+++¿Puedo migrar mis informes heredados al lienzo de informes?

En resumen, la migración de informes heredados no estará disponible durante la versión beta. Sin embargo, es una función planificada (con algunas advertencias descritas a continuación) para el lanzamiento oficial.

Aunque la barrera para crear nuevos informes se ha reducido significativamente con el lienzo de informes, entendemos que la introducción de algunos de los informes y paneles existentes ayudará a acelerar el proceso de adopción. Como tal, queremos proporcionar las herramientas y los recursos necesarios para asegurarnos de que pueda traer cualquier elemento heredado relevante para garantizar que comience con pie derecho en el lienzo de informes. Sin embargo, dado que el lienzo de informes es un cambio tan radical en la forma en que funciona la creación de informes actual, sería imposible migrar todos los informes o tableros exactamente como hoy.

Nuestra estrategia actual para la migración en la versión oficial es permitirle hacer lo siguiente:

1. Identificar los informes y paneles relevantes

   1. Permite exportar un CSV de todos los informes y paneles del sistema, junto con cualquier información de seguimiento relevante (número de vistas, cuándo y por quién).
   1. Proporcione una exportación de los informes configurados con las entregas programadas junto con los destinatarios.

1. Seleccione los informes y paneles que desee migrar y haga clic en **Migrar**

   Se trata de una migración unidireccional. Crea una copia de los informes y paneles seleccionados en el lienzo de informes y deja el informe o panel heredado intacto en la herramienta de informes actual.

   Puede migrar el mismo informe o panel tantas veces como desee.

1. En Lienzo de informes, asegúrese de que todos los informes y paneles que seleccionó se hayan migrado.
+++

+++¿Por qué no puedo ver todos los objetos que hago normalmente?

Para ofrecer la versión beta a nuestros clientes lo antes posible, la hemos lanzado con solo un subconjunto de los muchos tipos de objetos disponibles en Workfront en la actualidad. A continuación se muestran los tipos de objetos admitidos actualmente en la versión beta:

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

+++Si algo sale mal en el lienzo de informes durante la versión beta, ¿se verán afectados los datos de mi organización?

No. La versión beta utiliza una copia de los datos de su organización que se rellenan en el lienzo de informes. Aunque esto significa que puede experimentar con seguridad durante la versión beta sin riesgo de afectar a datos importantes, también significa que la edición en línea de datos en el lienzo de informes no estará disponible hasta el lanzamiento oficial.
+++

+++¿Puedo excluirme de la versión beta una vez que me haya unido?

Un administrador de Workfront no puede excluirse de la versión beta; sin embargo, los usuarios que no son administradores del sistema pueden eliminarse haciendo lo siguiente:

1. Inicie sesión como administrador del sistema.
1. Vaya al lienzo de informes.
1. Haga clic en Lienzo de informes **permissions**.
1. Elimine los usuarios que desee excluir de la versión beta de la lista que se han incluido.
1. Haga clic en **Guardar**.
+++
