---
title: Registros de auditoría
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede realizar un seguimiento de los cambios de usuario activados en el sistema durante los últimos 90 días mediante registros de auditoría.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 3%

---

# Registros de auditoría

<!--Audited: 01/2024-->

Como administrador de Adobe Workfront, puede realizar un seguimiento de los cambios de usuario activados en el sistema durante los últimos 90 días mediante los registros de auditoría que se describen a continuación.

Para obtener instrucciones sobre cómo ver y filtrar lo que desea ver en estos registros de auditoría, consulte [Ver y exportar registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Información que puede encontrar en un registro de auditoría

En cada entrada de registro de auditoría se registran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Fecha y hora</td> 
   <td>Cuando se produjo la acción.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de registro</td> 
   <td>Tipo de registro de auditoría, como nivel de acceso o formulario personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nombre de usuario</td> 
   <td> <p>Nombre del usuario que realizó la acción.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acción</td> 
   <td> Acciones realizadas por el usuario, como Cambiar, Crear y Eliminar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objeto</td> 
   <td> Nombre del objeto afectado como resultado de la acción. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Detalles</td> 
   <td>Detalles adicionales sobre la acción. Pase el ratón sobre el texto para leer el mensaje completo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dirección IP</td> 
   <td> <p>Dirección IP del usuario que realizó la acción en el momento de la acción.</p> <p>La dirección IP no está disponible para algunas acciones del sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de registros de auditoría y las acciones que los almacenan en déclencheur

* [Nivel de acceso](#access-level)
* [Empresa](#company)
* [Condición](#condition)
* [Campo personalizado](#custom-field)
* [Formularios personalizados](#custom-forms)
* [Sección personalizada](#custom-section)
* [Tasa de cambio](#exchange-rate)
* [Grupo](#group)
* [Roles](#job-roles)
* [Intento de inicio de sesión](#login-attempt)
* [Prioridad](#priority)
* [Preferencia del proyecto](#project-preference)
* [Gravedad](#severity)
* [Estado](#status)
* [Preferencias de tareas y problemas](#tasks-issues-preferences)
* [Usuario](#user)

### Nivel de acceso {#access-level}

El sistema genera una entrada de registro de nivel de acceso cuando un usuario realiza una de las siguientes acciones:

* Crea un nivel de acceso
* Elimina un nivel de acceso
* Cambia un nivel de acceso:

   * Modifica el tipo de licencia
   * Cambia los permisos a Proyectos, Tareas, Problemas, Portfolio, Programas, Informes, Documentos, Usuarios o Plantillas

     >[!NOTE]
     >
     >El sistema no registra ningún cambio de permiso en los datos financieros o en los siguientes tipos de acceso: Ver y Editar.
     >
     >Por ejemplo, si un usuario cambia el tipo de acceso del Planificador de Ver a Editar, el sistema no muestra la información contenida en el menú desplegable Ajustar la configuración.

### Compañía {#company}

El sistema genera una entrada de registro de auditoría de la compañía cuando un usuario realiza una de las siguientes acciones:

* Crea una empresa
* Cambia una compañía:

   * Cambiarle el nombre
   * Agrega o quita miembros
   * Agrega, edita o elimina el valor en su campo Grupo
   * Agrega o edita una tarifa de facturación de compañía para un rol
   * Quita una tarifa de facturación de la compañía para un rol
   * La establece como la compañía principal de la organización
   * Adjunta o quita un formulario personalizado

* Elimina una compañía

Para obtener más información sobre los estados, vea [Información general sobre los estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condición {#condition}

El sistema genera una entrada de registro de auditoría de condiciones cuando un usuario realiza una de las siguientes acciones:

* Crea una condición
* Cambia una condición:

   * Cambia el nombre
   * Cambia el color
   * La establece como predeterminada
   * Cambia o quita la descripción de la condición
   * Oculta o muestra la condición

* Elimina una condición

Para obtener más información acerca de cómo configurar los roles, vea [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Campo personalizado {#custom-field}

El sistema genera una entrada de registro de auditoría de campo personalizado cuando un usuario realiza una de las siguientes acciones:

* Crea un campo personalizado
* Cambia un campo personalizado:

   * Cambia el nombre, etiqueta, instrucciones o formato
   * Cambia el tipo de visualización

     Esta opción solo está disponible si el campo es de uno de los siguientes tipos: línea única, párrafo, lista desplegable, casilla de verificación o botón de opción

   * Cambia el tamaño del campo

     Esto solo está disponible si el campo es de uno de los siguientes tipos: línea única, párrafo, texto con formato

   * Agrega, quita u oculta una opción de campo
   * Edita una etiqueta de opción de campo o un valor
   * Configura la opción de campo que se va a seleccionar o no seleccionar de forma predeterminada
   * Configura un campo desplegable para permitir varias selecciones o una sola
   * Configura un campo de fecha para mostrar o no la hora del día
   * Edita el hipervínculo o cambia el valor en un campo de texto descriptivo

* Elimina un campo personalizado
* Comparte un campo personalizado

### Formularios personalizados {#custom-forms}

El sistema genera una entrada de registro de auditoría de Forms personalizada cuando un usuario realiza una de las siguientes acciones:

* Crea un formulario personalizado
* Cambia un formulario personalizado:

   * Cambia el nombre o la descripción
   * Activa o desactiva la opción
   * Agrega o quita un campo o sección
   * Para una sección personalizada, cambia una configuración en Configuración adicional
   * Cambia un campo a obligatorio o no obligatorio
   * Cambia un cálculo en un campo personalizado
   * Oculta o muestra la fórmula asociada a un campo calculado en el texto de desplazamiento Instrucciones
   * Activa o desactiva la actualización de cálculos anteriores
   * Agrega o cambia lógica de omisión o de visualización

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Elimina un formulario personalizado
* Comparte un formulario personalizado

### Sección personalizada {#custom-section}

El sistema genera una entrada de registro de auditoría de sección personalizada cuando un usuario realiza una de las siguientes acciones en un formulario personalizado:

* Crea una sección personalizada
* Cambia el nombre o la descripción de una sección personalizada
* Elimina una sección personalizada

Para obtener información acerca de las secciones personalizadas de los formularios personalizados, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### tarifa de cambio {#exchange-rate}

El sistema genera una entrada de registro de auditoría de tasa de cambio cuando un usuario realiza una de las siguientes acciones:

* Crea un tipo de cambio
* Cambia un tipo de cambio:

   * Agrega una moneda
   * Cambia la tasa de la moneda
   * Establece la moneda como la moneda base (predeterminada) para todos los proyectos e informes del sistema

* Elimina una tasa de cambio

Para obtener más información acerca de cómo configurar tasas de cambio, vea [Configurar tasas de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Grupo {#group}

El sistema genera una entrada de registro de auditoría de grupo cuando un usuario realiza una de las siguientes acciones:

* Crea un grupo
* Elimina un grupo
* Cambia un grupo:

   * Agrega o quita usuarios
   * Agrega o quita subgrupos

### Roles {#job-roles}

El sistema genera una entrada de registro de auditoría de funciones de trabajo cuando un usuario realiza una de las siguientes acciones:

* Crea un rol
* Cambia un rol:

   * Cambia el nombre
   * Agrega, cambia o quita la descripción
   * Agrega, cambia o quita el costo por hora (costo/hora)
   * Agrega, cambia o elimina la tarifa de facturación (factura/hora)

* Elimina un rol

Para obtener más información acerca de cómo configurar los roles, consulte [Crear y administrar los roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Intento de inicio de sesión {#login-attempt}

El sistema genera una entrada de registro de auditoría de intento de inicio de sesión cuando un usuario realiza una de las siguientes acciones:

* Inicia sesión, cierra la sesión o falla al intentar iniciar sesión en Workfront (en un explorador y en la aplicación móvil)
* Inicia sesión, cierra la sesión o falla en un intento de inicio de sesión en cualquier integración de Workfront (como Workfront para Slack y Workfront para Salesforce)
* Inicia sesión o cierra sesión en la API de Workfront

Inicio de sesión Los registros de intentos no registran cuándo un administrador de Workfront utiliza la función Iniciar sesión como.

>[!NOTE]
>
>Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Consulte al administrador de red o de TI si necesita más información.

### Prioridad {#priority}

El sistema genera una entrada de registro de auditoría de prioridad cuando un usuario realiza una de las siguientes acciones:

* Crea una prioridad
* Cambia una prioridad:

   * Cambia el nombre
   * Cambia el color
   * La establece como predeterminada
   * Agrega, cambia o quita la descripción de la prioridad
   * Oculta o muestra la prioridad

* Elimina una prioridad

Para obtener más información acerca de la configuración de prioridades, vea [Crear y personalizar prioridades](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Preferencia del proyecto {#project-preference}

El sistema genera una entrada de registro de auditoría Preferencias del proyecto cuando un usuario realiza una de las siguientes acciones:

* Crea un trimestre personalizado
* Cambia una preferencia de proyecto:

   * Lo bloquea o desbloquea
   * Cambia una de sus configuraciones
   * Lo habilita, deshabilita o edita
   * Edita un cálculo de escala de tiempo

* Elimina un trimestre personalizado

Para obtener más información acerca de las preferencias del proyecto, vea [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Gravedad {#severity}

El sistema genera una entrada de registro de auditoría de gravedad cuando un usuario realiza una de las siguientes acciones:

* Crea una gravedad del problema
* Cambia la gravedad de un problema:

   * Cambia el nombre
   * Cambia el color
   * La establece como predeterminada
   * Cambia o elimina la descripción de la gravedad
   * Oculta o muestra la gravedad

* Elimina una gravedad del problema

Para obtener más información acerca de cómo configurar los roles, consulte [Crear o personalizar gravedades de problemas](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Estado {#status}

El sistema genera una entrada de registro de auditoría de estado cuando un usuario realiza una de las siguientes acciones:

* Crea un estado en el nivel de sistema o grupo
* Cambia un estado en el sistema o en el nivel de grupo:

   * Cambiarle el nombre
   * Lo convierte en un estado predeterminado
   * Lo bloquea o desbloquea
   * Lo oculta o no lo oculta
   * Cambia el color o la descripción

* Elimina un estado en el sistema o en el nivel de grupo

Para obtener más información sobre los estados, vea [Información general sobre los estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Preferencias de tareas y problemas {#tasks-issues-preferences}

El sistema genera una entrada de registro de auditoría Preferencias de tareas y problemas cuando un usuario cambia una preferencia de tareas y problemas de una de las siguientes maneras:

* Bloquea o desbloquea una preferencia
* Cambia la configuración de una preferencia
* Cambia una configuración de Access para tareas, problemas o solicitudes

Para obtener más información acerca de las preferencias de tareas y problemas, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Usuario {#user}

El sistema genera una entrada de registro de auditoría de usuario cuando un usuario realiza una de las siguientes acciones:

* Crea un usuario

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Consulte al administrador de red o de TI si necesita más información.

* Elimina un usuario
* Cambia el nivel de acceso, la empresa, el equipo o el grupo de un usuario
* Activa un usuario
* Desactiva un usuario
