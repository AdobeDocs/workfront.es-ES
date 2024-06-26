---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Preguntas frecuentes sobre Adobe Unified Experience
description: Algunas funciones son diferentes entre [!DNL Workfront] y Adobe Experience Cloud, y es posible que tenga algunas preguntas como [!DNL Workfront] La instancia de se migra a la experiencia unificada.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 019a1b61cd97d5d61f9a4fbf3f98eccab50809a8
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] FAQ

El [!DNL Adobe Unified Experience] para [!DNL Workfront] le permite administrar todos los [!DNL Adobe] aplicaciones en un solo lugar con un solo inicio de sesión. El [!DNL Adobe] El área de navegación se integra perfectamente con [!DNL Workfront]. Algunas funciones son diferentes y es posible que tenga algunas preguntas como [!DNL Workfront] La instancia de se migra a la experiencia unificada.

Para obtener información acerca de cómo iniciar sesión en [!DNL Adobe Unified Experience], consulte [[!DNL Adobe Unified Experience] para [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparación de [!DNL Adobe Unified Experience] y [!DNL Workfront only] experiencia

Solo los clientes que utilizan [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] puede acceder a la [!DNL Adobe Unified Experience]. Los clientes que aún no hayan migrado verán el [!DNL Workfront only] experiencia, sin la capacidad de cambiar entre [!DNL Adobe] aplicaciones.

En esta tabla se describen algunas funciones que difieren entre las dos experiencias.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] única experiencia |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menú principal] está a la izquierda ![Menú principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menú principal] está a la derecha ![Menú principal](assets/main-menu-icon.png) |
| Hay una sola URL de inicio de sesión disponible para todos los [!DNL Adobe Experience Cloud] aplicaciones | Iniciar sesión en [!DNL Workfront] con un personalizado [!DNL Workfront] URL |
| Un &quot;conmutador de organización&quot; le permite desplazarse entre [!DNL Workfront] organizaciones y entornos | El conmutador de organización no está disponible. |
| La navegación incluye un área de navegación de nivel superior para [!DNL Adobe] productos, [!DNL Adobe] notificaciones, ayuda y su perfil de usuario, además del [!DNL Workfront] barra de navegación | La navegación incluye el [!DNL Workfront] solo barra de navegación |
| Se puede acceder a la ayuda a través de [!UICONTROL Menú principal] y área de navegación superior | Se puede acceder a la ayuda a través de [!UICONTROL Menú principal] y [!DNL Workfront] barra de navegación |

{style="table-layout:auto"}

## Preguntas frecuentes

### ¿Cómo puedo determinar si estoy utilizando la experiencia unificada de Adobe o Adobe Workfront?

Para determinar si su organización está en la experiencia unificada de Adobe, examine la dirección URL que utiliza para acceder a Workfront.

| URL | Experiencia de Adobe |
|------------|------------|
| (CompanyName).my.workfront.com | Experiencia en Workfront |
| experience.adobe.com | Experiencia unificada de Adobe |

### ¿Cómo puedo obtener más información sobre la [!DNL Adobe Admin Console]?

Para obtener más información sobre [!DNL Admin Console], revise estos artículos:

* [Prepárese para la [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] descripción general](https://helpx.adobe.com/es/enterprise/using/admin-console.html)

### ¿Qué debo hacer como cliente para facilitar la migración?

Se contactará con los clientes existentes para programar las migraciones. Los compañeros de soporte del equipo de migración guiarán a los clientes a través del proceso y les aconsejarán sobre lo siguiente [!DNL Admin Console] configure y proporcione vínculos a la documentación necesaria para que el traslado sea lo más sencillo y sencillo posible.

* [[!DNL Adobe Workfront] Resumen de asistencia](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] información](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] y [!DNL Admin Console] FAQ](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### ¿Cómo lo lleva? [!DNL Adobe Admin Console] para empresas que ya tienen esto habilitado para Federated ID de forma diferente a [!DNL Workfront] ¿Se ha configurado el SSO?

[!DNL Adobe Admin Console] tiene la opción de incluir [!DNL Workfront], reemplazando SSO por IMS. Todo el aprovisionamiento de usuarios se produce en la [!DNL Admin Console]y los usuarios verán el [!DNL Adobe] pantalla de inicio de sesión para llegar a [!DNL Experience Cloud] dónde verán [!DNL Workfront] como una opción (si se les concede acceso a ella).

### AEM ¿Cómo afecta esto a los clientes que ya tienen el panel de administración de la para [!DNL Adobe Assets] - pero el SSO está configurado de forma diferente a [!DNL Workfront?]

Una [!DNL Workfront] se añade como [!DNL Admin Console] aplicación, no debería tener que hacer nada más para [!DNL Workfront] para aprovechar la configuración de SSO existente que tiene para [!DNL Adobe Assets].

### ¿Cómo afecta esto a los que están configurados con SSO?

El SSO se configura en [!DNL Admin Console] y heredado por el [!DNL Workfront] aplicación.

### Es SSO con nuestro interno [!DNL Active Directory] ¿todavía va a ser una opción con IMS?

IMS sustituye al SSO y funciona casi siempre igual. Todos los permisos de usuario se conceden y aprovisionan en [!DNL Adobe Admin Console], y el usuario verá el [!DNL Adobe] pantalla de inicio de sesión donde pueden elegir &quot;[!UICONTROL Cuenta personal]&quot; o &quot;[!UICONTROL Cuenta de empresa]&quot; para iniciar sesión (si tiene [!DNL Active Directory], la mayoría iniciará sesión con una cuenta de empresa).

### Para los que no utilizan SSO, ¿la variable [!DNL Workfront] ¿cambiar URL de inicio de sesión?

La dirección URL de inicio de sesión cambiará, pero la antigua se redirigirá a la nueva dirección URL de inicio de sesión, por lo que debe volver a entrenar a los usuarios para saber adónde ir.

### ¿Seguirán funcionando los alias que hemos configurado o son los siguientes? [!DNL Workfront] ¿Cuáles son los vínculos que cambian con esta migración?

[!DNL Workfront] hay redirecciones/alias disponibles para llegar a la página principal.

### ¿Habrá un momento en que las redirecciones estén deshabilitadas? ¿O siempre podremos escribir en my.company.workfront.com?

Siempre podrá utilizar cualquier dirección URL personalizada. Después de hacer clic en cualquiera de esos vínculos, le dirigirá a [!DNL Workfront] y mostrar una dirección URL diferente. Sin embargo, es una mejor [!DNL experience] para iniciar sesión en experience.adobe.com y marcar vínculos desde [!DNL Experience Cloud]. Menos redireccionamiento equivale a menos tiempo de retardo/tiempo de carga.

### ¿Se romperán los vínculos directos a las colas de solicitudes?

Todos los vínculos directos deben redirigirse a los nuevos patrones de URL. Sin embargo, si ha distribuido vínculos a personas, debe enviar una actualización para aprovechar el vínculo directo y evitar retrasos en el acceso a la página esperada.

### ¿Migraremos a? [!DNL Experience Cloud] a nivel mundial o podemos seleccionar para determinados usuarios (no todos nuestros usuarios utilizan incluso otros productos de Adobe)?

Todo el [!DNL Workfront] se migrará la cuenta del cliente. No se puede hacer usuario por usuario.

### Will all [!DNL Workfront] los usuarios deben iniciar sesión mediante [!DNL Experience Cloud]? ¿O solo administradores?

Sí, todos los usuarios iniciarán sesión mediante [!DNL Experience Cloud]. El inicio de sesión de IMS reemplazará el SSO. Es una experiencia muy similar, solo una pantalla de inicio de sesión diferente.

### ¿Tendrán los usuarios que vincular sus [!DNL Adobe] cuentas a su [!DNL Workfront] cuentas si ya tienen ambas?

Sí, hay un proceso para esto y se proporcionarán más detalles cuando sea el momento de que su organización pase a IMS.

### ¿Qué le sucede a la [!DNL Workfront] usuarios que no tienen un [!DNL Adobe] ¿Cuenta?

Usuarios a los que no se les ha concedido acceso en [!DNL Adobe Admin Console] para entrar en [!DNL Workfront] debe crear un &quot;[!UICONTROL cuenta personal]&quot; o un [!DNL Adobe] Cuenta de ID para poder iniciar sesión. Esto envía un correo electrónico al administrador para aprobar o rechazar su solicitud y, además, permite al administrador configurar el tipo de acceso que tiene ese usuario. Cuando inicien sesión, irán a experience.adobe.com, escribirán su dirección de correo electrónico y elegirán [!UICONTROL Cuenta personal]. Desde allí, podrán acceder a [!DNL Workfront].

### ¿Y si no tenemos ninguna? [!DNL Adobe] productos distintos de [!DNL Workfront?]

Se recomienda que su organización migre al [!DNL Adobe Unified Experience]. Recibirá una solicitud [!DNL Adobe] El ID junto con las ventajas enumeradas anteriormente.

### Tenemos usuarios externos incluidos en nuestra [!DNL Workfront] ejemplo. No queremos que tengan acceso a ningún otro producto incluido en [!DNL Adobe]. ¿Cómo limitaríamos su acceso dentro de la consola?

[!DNL Admin Console] proporciona a los administradores mucho control sobre lo que los usuarios pueden acceder y no pueden acceder. Siempre que un usuario externo desee acceder a, debe crear un [!DNL Adobe] ID, que envía un correo electrónico al administrador. El administrador puede aceptar o rechazar el acceso a un producto y definir a qué puede o no acceder para los productos propiedad de esa organización. A continuación, el [!DNL Workfront] El administrador del sistema puede entrar en el [!UICONTROL Usuarios] área de [!DNL Workfront] para crear permisos más granulares para el usuario externo.

### Los administradores de grupo se utilizan para crear personas en [!DNL Workfront]. Con el paso a [!DNL Experience Cloud], ¿seguirán siendo capaces los administradores de grupo de crear personas?

Sí, la creación de usuarios sigue siendo posible mediante [!DNL Workfront]. Estos usuarios se pueden agregar a [!DNL Experience Cloud] automáticamente. También puede configurar los administradores de grupo como propietarios de productos en la [!DNL Admin Console] para permitirles asignar [!DNL Workfront] a los usuarios.

### ¿Cuál es la fecha límite para cambiar a? [!DNL Experience Cloud]?

No hay ningún plazo en este momento para pasar a [!DNL Adobe Experience Cloud]. Estamos trabajando con los clientes para que puedan elegir cuándo están listos para realizar el cambio.

### ¿Necesitará nuestro equipo de asistencia hacer algo para este cambio?

Si el equipo de asistencia es responsable de la creación de nuevos usuarios, deberán familiarizarse con el [!DNL Admin Console] interfaces utilizadas para crear usuarios y asignar un derecho a Workfront. De lo contrario, es probable que no haya ningún cambio significativo para su equipo de soporte interno.

### ¿Cómo afecta esto a las integraciones que tenemos a través de la función API?

La ruta URL existente seguirá disponible para el tráfico API. No es necesario que haga nada para actualizar los puntos de conexión en las integraciones. Sin embargo, no se admiten inicios de sesión directos con nombre de usuario y contraseña; debe utilizar una clave de API, con la excepción de [!DNL Workfront Fusion] conectores.

### ¿Qué pasa? [!DNL Creative Cloud] ¿usuarios? ¿Cómo les afecta la migración? ¿Hay alguna ventaja para ellos?

No tiene ningún impacto en [!DNL Creative Cloud] usuarios con la migración a [!DNL Adobe Unified Experience].

### Cambiarán los inicios de sesión para [!DNL Workfront] ¿usuarios móviles?

[!DNL Workfront] los usuarios móviles no deben verse afectados por la migración a [!DNL Adobe Unified Experience].
