---
title: Información general sobre tipos de registros centralizados
description: Los tipos de registros centralizados se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Resumen de tipos de registros centralizados


Los tipos de registros centralizados se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Adobe Workfront Planning.

## Descripción general de los tipos de registros centralizados

Al implementar Workfront Planning para una organización de varios equipos con flujos de trabajo comunes, es posible que necesite definir una estructura y metadatos coherentes para los tipos de registro clave (como Campañas o Entregables) que se pueden agregar a los espacios de trabajo de cada equipo para capturar y administrar su trabajo.

Además, es posible que necesite el trabajo de cada equipo para llegar a un nivel central y más global.

En este flujo de trabajo, se puede garantizar que los equipos capturan su trabajo de forma coherente y desbloquean la visibilidad entre equipos, sin necesidad de añadir a todos los miembros de la organización a un espacio de trabajo.

Para utilizar tipos de registros centralizados, haga lo siguiente:

1. Configure un tipo de registro para que esté centralizado.

   Para obtener más información, consulte [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Añada un tipo de registro existente de uno centralizado.

   Para obtener más información, vea [Agregar tipos de registros existentes](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).




· Hay disponible una nueva configuración &quot;Permitir agregar el tipo de registro en otros espacios de trabajo&quot; en Configuración avanzada para tipos de registros.

· Si está activado, el administrador del espacio de trabajo puede seleccionar usuarios con licencia estándar, equipos, grupos, funciones o empresas que pueden añadir el tipo de registro en los espacios de trabajo que administran.

· El administrador del espacio de trabajo que está editando la configuración se agregará automáticamente a la lista de usuarios seleccionados de forma predeterminada

o El administrador del espacio de trabajo puede quitar su propio nombre después de agregar al menos otra entidad

o Debe haber al menos 1 usuario/equipo/... seleccionado para guardar la configuración

o Una vez agregado el tipo de registro en al menos 1 espacio de trabajo, se pueden eliminar todos los usuarios seleccionados

§ Esto se hace para evitar que se agregue el tipo de registro global en nuevos espacios de trabajo, pero para mantenerlo en los espacios de trabajo que ya lo están utilizando.

· En la fase 1, todos los registros de los tipos de registros conectados se comparten automáticamente con cualquier espacio de trabajo donde se haya agregado el tipo de registro.

· Una vez habilitado el tipo de registro como espacio de trabajo cruzado, se añade un campo &quot;Workspace&quot; generado por el sistema al tipo de registro

o Muestra el espacio de trabajo desde el que se ha creado cada registro.

o Este campo es de solo lectura y no se puede eliminar.

o Se puede ocultar en los campos de vista.

o El campo del espacio de trabajo se puede utilizar para filtrar, agrupar y ordenar, así como en cualquier configuración de vista, como otros campos.


Tipos de registros de Cross-Workspace en espacios de trabajo locales

· Al intentar agregar un nuevo tipo de registro a su espacio de trabajo, los administradores de espacio de trabajo local ven una opción para seleccionar de la lista de tipos de registro globales disponibles para ellos

· Cuando seleccionan uno de los tipos de registros globales, se añade inmediatamente al espacio de trabajo

· Es posible mover el tipo de registro global a cualquier sección y posición dentro del espacio de trabajo local


Permisos para el tipo de registro global en espacios de trabajo locales

Dentro de los espacios de trabajo locales, los miembros obtienen el siguiente acceso al tipo de registro global:

· En la fase 1, los gestores de espacios de trabajo locales obtienen permiso de contribución. Esto significa que:

o Los administradores de espacio de trabajo local pueden:

§ Agregar el tipo de registro global

§ Agregar, editar o eliminar cualquier registro del tipo de registro global, independientemente del área de trabajo desde la que se agregó el registro.

§ Eliminar el tipo de registro global de su espacio de trabajo local

o Los administradores de espacio de trabajo local no pueden:

§ Agregar, editar, eliminar campos

§ Actualizar el aspecto y la etiqueta del tipo de registro

§ Consulte configuración avanzada para el tipo de registro

§ Administrar automatizaciones

§ Administrar formularios de solicitud

§ Ajustar el uso compartido del tipo de registro para el ámbito de su espacio de trabajo

§ Deshabilite la configuración del tipo de registro global en la configuración avanzada.

· Los colaboradores del espacio de trabajo local obtienen permiso de contribución para el tipo de registro global y pueden agregar y administrar registros en él

· Los visualizadores de Workspace locales obtienen permiso de visualización para el tipo de registro global

· Tan pronto como se añade un registro al tipo de registro global desde cualquiera de los espacios de trabajo locales, el campo Workspace muestra ese nombre de espacio de trabajo

o Por ahora no es posible editar ni cambiar el campo del espacio de trabajo

· Todos los registros agregados a espacios de trabajo locales se acumulan y se muestran en el espacio de trabajo principal, y todos los miembros del espacio de trabajo principal obtienen acceso de visualización al mismo.

· Los registros agregados en espacios de trabajo locales no se muestran en otros espacios de trabajo locales utilizando el mismo tipo de registro global y sus miembros no tienen acceso a los registros.



Acceso a Conexiones:

· Ámbito de MVP

o Los tipos de registro conectados al tipo de registro global serán visibles para los espacios de trabajo locales donde se agrega el tipo de registro global para que puedan utilizar los campos de conexión para etiquetar


Comportamiento de API

Si el usuario intenta crear registros en un tipo de registro global mediante API sin proporcionar el ID de espacio de trabajo, el sistema comprueba si el usuario tiene acceso para crear registros en el espacio de trabajo principal (donde se crea el tipo de registro global)

· Si es así, el registro se crea en el espacio de trabajo principal

· Si no es así, el usuario recibe un error de validación que indica que no tiene acceso al espacio de trabajo principal y que debe proporcionar el ID del espacio de trabajo donde tiene acceso para crear.