---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Preguntas frecuentes sobre Adobe Unified Experience
description: Algunas características son diferentes entre  [!DNL Workfront]  y Adobe Experience Cloud, y es posible que tenga algunas preguntas a medida que su instancia de  [!DNL Workfront] se migra a la experiencia unificada.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: b4c1f9c29dd6ad1e07acc741ab52e95a7bae7f67
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 0%

---

# Preguntas frecuentes sobre [!DNL Adobe Unified Experience]

[!DNL Adobe Unified Experience] para [!DNL Workfront] le permite administrar todas sus aplicaciones de [!DNL Adobe] en un solo lugar con un único inicio de sesión. El área de navegación [!DNL Adobe] se integra perfectamente con [!DNL Workfront]. Algunas características son diferentes y es posible que tenga algunas preguntas a medida que migre la instancia de [!DNL Workfront] a la experiencia unificada.

Para obtener información acerca de cómo iniciar sesión en [!DNL Adobe Unified Experience], vea [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparación de la experiencia [!DNL Adobe Unified Experience] y [!DNL Workfront only]

Solo los clientes que usen [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] pueden tener acceso a [!DNL Adobe Unified Experience]. Los clientes que aún no hayan migrado verán la experiencia [!DNL Workfront only], sin la posibilidad de cambiar entre [!DNL Adobe] aplicaciones.

En esta tabla se describen algunas funciones que difieren entre las dos experiencias.

| [!DNL Adobe Unified Experience] | Experiencia de solo [!DNL Workfront] |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menú principal] se encuentra a la izquierda ![Menú principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menú principal] está a la derecha ![Menú principal](assets/main-menu-icon.png) |
| Hay disponible una sola URL de inicio de sesión para todas las aplicaciones de [!DNL Adobe Experience Cloud] | Inicie sesión en [!DNL Workfront] con una dirección URL [!DNL Workfront] personalizada |
| Un &quot;conmutador de organización&quot; le permite desplazarse entre [!DNL Workfront] organizaciones y entornos | El conmutador de organización no está disponible. |
| La navegación incluye un área de navegación de nivel superior para [!DNL Adobe] productos, [!DNL Adobe] notificaciones, ayuda y su perfil de usuario, además de la barra de navegación de [!DNL Workfront] | La navegación solo incluye la barra de navegación [!DNL Workfront] |
| Se puede acceder a la ayuda a través del [!UICONTROL Menú principal] y del área de navegación superior | Se puede acceder a la ayuda a través del [!UICONTROL Menú principal] y la barra de navegación de [!DNL Workfront] |
| El visor de revisión se abre en una nueva pestaña | El visor de revisión se abre en Workfront |
| La URL utilizada para acceder a Workfront es `experience.adobe.com` | La URL utilizada para acceder a Workfront es `(CompanyName).my.workfront.com` |
| El formato de la fecha (como MM/DD/AAAA) se basa en las preferencias del navegador. | El formato de fecha (como MM/DD/AAAA) se basa en la configuración del lenguaje de experiencia unificado. Si el usuario no ha actualizado la configuración de idioma, se utiliza la configuración de `en-US`. |

{style="table-layout:auto"}

## Preguntas frecuentes

### ¿Cómo puedo determinar si estoy utilizando la experiencia unificada de Adobe o Adobe Workfront?

Para determinar si su organización está en la experiencia unificada de Adobe, examine la dirección URL que utiliza para acceder a Workfront.

| URL | Experiencia de Adobe |
|------------|------------|
| (CompanyName).my.workfront.com | Experiencia en Workfront |
| experience.adobe.com | Experiencia unificada de Adobe |

### ¿Cómo puedo obtener más información sobre [!DNL Adobe Admin Console]?

Para obtener información acerca de [!DNL Admin Console], consulte estos artículos:

* [Prepararse para  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] descripción general](https://helpx.adobe.com/es/enterprise/using/admin-console.html)

### ¿Qué debo hacer como cliente para facilitar la migración?

Se contactará con los clientes existentes para programar las migraciones. Los compañeros de soporte del equipo de migración guiarán a los clientes a través del proceso, les aconsejarán sobre la configuración de [!DNL Admin Console] y proporcionarán los vínculos a la documentación necesaria para que el movimiento sea lo más sencillo y sencillo posible.

* [[!DNL Adobe Workfront] Resumen de asistencia](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] información](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] y [!DNL Admin Console] preguntas más frecuentes](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### ¿Cómo administra [!DNL Adobe Admin Console] para las empresas que ya lo tienen habilitado para Federated ID de forma distinta a la configuración del SSO de [!DNL Workfront]?

[!DNL Adobe Admin Console] tiene la opción de incluir [!DNL Workfront], reemplazando SSO por IMS. Todo el aprovisionamiento de usuarios se realiza en [!DNL Admin Console] y los usuarios verán la pantalla de inicio de sesión de [!DNL Adobe] para llegar a [!DNL Experience Cloud], donde verán [!DNL Workfront] como una opción (si se les concede acceso a él).

### AEM ¿Cómo afecta esto a los clientes que ya tienen el panel de administración de para [!DNL Adobe Assets], pero el SSO está configurado de forma diferente a [!DNL Workfront?]?

Una vez agregado [!DNL Workfront] como aplicación [!DNL Admin Console], no debería tener que hacer nada más para [!DNL Workfront] para aprovechar la configuración de SSO existente que tiene para [!DNL Adobe Assets].

### ¿Cómo afecta esto a los que están configurados con SSO?

SSO se configura en [!DNL Admin Console] y la aplicación [!DNL Workfront] lo hereda.

### ¿El SSO con nuestro(a) [!DNL Active Directory] interno todavía será una opción con IMS?

IMS sustituye al SSO y funciona casi siempre igual. Todos los permisos de usuario se han concedido y aprovisionado en [!DNL Adobe Admin Console], y el usuario verá la pantalla de inicio de sesión de [!DNL Adobe] en la que podrá elegir &quot;[!UICONTROL Cuenta personal]&quot; o &quot;[!UICONTROL Cuenta de la compañía]&quot; para iniciar sesión (si tiene [!DNL Active Directory], la mayoría iniciará sesión con una cuenta de la compañía).

### Para los que no utilizan SSO, ¿cambia la dirección URL de inicio de sesión de [!DNL Workfront]?

La dirección URL de inicio de sesión cambiará, pero la antigua se redirigirá a la nueva dirección URL de inicio de sesión, por lo que debe volver a entrenar a los usuarios para saber adónde ir.

### ¿Seguirán funcionando los alias que hemos configurado o los vínculos [!DNL Workfront] están cambiando con esta migración?

Hay [!DNL Workfront] redirecciones/alias disponibles para llegar a la página principal.

### ¿Habrá un momento en que las redirecciones estén deshabilitadas? ¿O siempre podremos escribir en my.company.workfront.com?

Siempre podrá utilizar cualquier dirección URL personalizada. Después de hacer clic en cualquiera de esos vínculos, se le dirigirá a [!DNL Workfront] y se mostrará una dirección URL diferente. Sin embargo, es mejor [!DNL experience] iniciar sesión en experience.adobe.com y marcar vínculos desde [!DNL Experience Cloud]. Menos redireccionamiento equivale a menos tiempo de retardo/tiempo de carga.

### ¿Se romperán los vínculos directos a las colas de solicitudes?

Todos los vínculos directos deben redirigirse a los nuevos patrones de URL. Sin embargo, si ha distribuido vínculos a personas, debe enviar una actualización para aprovechar el vínculo directo y evitar retrasos en el acceso a la página esperada.

### ¿Migraremos a [!DNL Experience Cloud] globalmente o podemos seleccionar para determinados usuarios (no todos nuestros usuarios utilizan incluso otros productos de Adobe)?

Se migrará toda la cuenta de cliente [!DNL Workfront]. No se puede hacer usuario por usuario.

### ¿Todos los usuarios de [!DNL Workfront] tendrán que iniciar sesión a través de [!DNL Experience Cloud]? ¿O solo administradores?

Sí, todos los usuarios iniciarán sesión mediante [!DNL Experience Cloud]. El inicio de sesión de IMS reemplazará el SSO. Es una experiencia muy similar, solo una pantalla de inicio de sesión diferente.

### ¿Tendrán los usuarios que vincular sus cuentas de [!DNL Adobe] a sus cuentas de [!DNL Workfront] si ya tienen ambas?

Sí, hay un proceso para esto y se proporcionarán más detalles cuando sea el momento de que su organización pase a IMS.

### ¿Qué les sucede a los usuarios de [!DNL Workfront] que no tienen una cuenta de [!DNL Adobe]?

Los usuarios a los que no se les ha concedido acceso en [!DNL Adobe Admin Console] para entrar a [!DNL Workfront] deben crear una &quot;[!UICONTROL cuenta personal]&quot; o una cuenta de identificador de [!DNL Adobe] para poder iniciar sesión. Esto envía un correo electrónico al administrador para aprobar o rechazar su solicitud y, además, permite al administrador configurar el tipo de acceso que tiene ese usuario. Cuando inicien sesión, irán a experience.adobe.com, escribirán su dirección de correo electrónico y elegirán [!UICONTROL Cuenta personal]. Desde allí, podrán acceder a [!DNL Workfront].

### ¿Qué sucede si no tenemos [!DNL Adobe] productos distintos de [!DNL Workfront?]?

Se recomienda que su organización migre a [!DNL Adobe Unified Experience]. Recibirá un ID de [!DNL Adobe] junto con los beneficios enumerados anteriormente.

### Se han incluido usuarios externos en nuestra instancia [!DNL Workfront]. No queremos que tengan acceso a ningún otro producto incluido en [!DNL Adobe]. ¿Cómo limitaríamos su acceso dentro de la consola?

[!DNL Admin Console] proporciona a los administradores mucho control sobre lo que los usuarios pueden y no pueden acceder. Siempre que un usuario externo desee acceder, deberá crear un ID de [!DNL Adobe], que enviará un mensaje de correo electrónico al administrador. El administrador puede aceptar o rechazar el acceso a un producto y definir a qué puede o no acceder para los productos propiedad de esa organización. A continuación, el administrador del sistema [!DNL Workfront] puede entrar en el área de [!UICONTROL Usuarios] de [!DNL Workfront] para obtener permisos más granulares para el usuario externo.

### Los administradores de grupo se usan para crear personas en [!DNL Workfront]. Con el cambio a [!DNL Experience Cloud], ¿los administradores de grupo aún podrán crear personas?

Sí, la creación de usuarios aún es posible a través de [!DNL Workfront]. Estos usuarios se pueden agregar automáticamente a [!DNL Experience Cloud]. También puede configurar los administradores de grupo como propietarios de producto en [!DNL Admin Console] para que puedan asignar [!DNL Workfront] a los usuarios.

### ¿Cuál es la fecha límite para cambiar a [!DNL Experience Cloud]?

No hay ninguna fecha límite en este momento para pasar a [!DNL Adobe Experience Cloud]. Estamos trabajando con los clientes para que puedan elegir cuándo están listos para realizar el cambio.

### ¿Necesitará nuestro equipo de asistencia hacer algo para este cambio?

Si el equipo de soporte es responsable de la creación de nuevos usuarios, deberán familiarizarse con las interfaces de [!DNL Admin Console] utilizadas para crear usuarios y asignar un derecho a Workfront. De lo contrario, es probable que no haya ningún cambio significativo para su equipo de soporte interno.

### ¿Cómo afecta esto a las integraciones que tenemos a través de la función API?

La ruta URL existente seguirá disponible para el tráfico API. No es necesario que haga nada para actualizar los puntos de conexión en las integraciones. Sin embargo, no se admitirá el inicio de sesión directo mediante nombre de usuario y contraseña; debe utilizar una clave de API, con la excepción de los conectores [!DNL Workfront Fusion].

### ¿Qué hay de [!DNL Creative Cloud] usuarios? ¿Cómo les afecta la migración? ¿Hay alguna ventaja para ellos?

No afecta a [!DNL Creative Cloud] usuarios con la migración a [!DNL Adobe Unified Experience].

### ¿Cambiarán los inicios de sesión de [!DNL Workfront] usuarios móviles?

[!DNL Workfront] usuarios móviles no deberían verse afectados por la migración a [!DNL Adobe Unified Experience].
