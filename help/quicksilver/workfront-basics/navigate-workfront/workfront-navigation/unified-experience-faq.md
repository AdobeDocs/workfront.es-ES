---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Preguntas frecuentes sobre Adobe Unified Experience
description: Algunas características son diferentes entre  [!DNL Workfront]  y Adobe Experience Cloud, y es posible que tenga algunas preguntas a medida que su instancia de  [!DNL Workfront] se migra a la experiencia unificada.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 90%

---

# Preguntas frecuentes sobre [!DNL Adobe Unified Experience]

[!DNL Adobe Unified Experience] para [!DNL Workfront] le permite administrar todas sus aplicaciones de [!DNL Adobe] en un solo lugar con un único inicio de sesión. El área de navegación de [!DNL Adobe] se integra perfectamente con [!DNL Workfront]. Algunas características son diferentes y es posible que tenga algunas preguntas a medida que migre la instancia de [!DNL Workfront] a la experiencia unificada.

Para obtener información acerca de cómo iniciar sesión en [!DNL Adobe Unified Experience], consulte [[!DNL Adobe Unified Experience] para [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparación de la experiencia de [!DNL Adobe Unified Experience] y [!DNL Workfront only]

Solo los clientes que usen [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] pueden tener acceso a [!DNL Adobe Unified Experience]. Los clientes que aún no hayan migrado verán la experiencia de [!DNL Workfront only], sin la posibilidad de cambiar entre aplicaciones de [!DNL Adobe].

En esta tabla se describen algunas funciones que difieren entre las dos experiencias.

| [!DNL Adobe Unified Experience] | Experiencia de solo [!DNL Workfront] |
| ---- | ----|
| El [!UICONTROL [!DNL Workfront] Menú principal] se encuentra a la izquierda ![Menú principal](assets/main-menu-icon-left-nav.png) | El [!UICONTROL [!DNL Workfront] Menú principal] se encuentra a la derecha ![Menú principal](assets/main-menu-icon.png) |
| Hay disponible una sola URL de inicio de sesión para todas las aplicaciones de [!DNL Adobe Experience Cloud] | Inicie sesión en [!DNL Workfront] con una dirección URL de [!DNL Workfront] personalizada |
| Un “conmutador de organización” le permite desplazarse entre organizaciones y entornos de [!DNL Workfront] | El “conmutador de organización” no está disponible. |
| La navegación incluye un área de navegación de nivel superior para productos de [!DNL Adobe], notificaciones de [!DNL Adobe], ayuda y su perfil de usuario, además de la barra de navegación de [!DNL Workfront] | La navegación solo incluye la barra de navegación de [!DNL Workfront] |
| Se puede acceder a la ayuda a través del [!UICONTROL Menú principal] y del área de navegación superior | Se puede acceder a la ayuda a través del [!UICONTROL Menú principal] y la barra de navegación de [!DNL Workfront] |
| El visor de corrección se abre en una nueva ficha | El visor de corrección se abre en Workfront |
| La URL utilizada para acceder a Workfront es `experience.adobe.com` | La URL utilizada para acceder a Workfront es `(CompanyName).my.workfront.com` |
| El formato de fecha (como MM/DD/AAAA) se basa en la configuración del lenguaje de experiencia unificado. Si el usuario no ha actualizado la configuración de idioma, se utiliza la configuración de `en-US`. | El formato de la fecha (como MM/DD/AAAA) se basa en las preferencias del navegador. |

{style="table-layout:auto"}

## Preguntas frecuentes

### ¿Cómo puedo determinar si estoy utilizando Adobe Unified Experience o Adobe Workfront?

Para determinar si su organización está en Adobe Unified Experience, examine la URL que utiliza para acceder a Workfront.

| URL | Adobe Experience |
|------------|------------|
| (CompanyName).my.workfront.com | Experiencia de Workfront |
| experience.adobe.com | Adobe Unified Experience |

### ¿Cómo puedo obtener más información sobre [!DNL Adobe Admin Console]?

Para obtener información acerca de [!DNL Admin Console], consulte estos artículos:

* [Prepararse para  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] Información general](https://helpx.adobe.com/es/enterprise/using/admin-console.html)

### ¿Qué debo hacer como cliente para facilitar la migración?

Se contactará con los clientes existentes para programar las migraciones. Los compañeros de soporte del equipo de migración guiarán a los clientes a través del proceso, les aconsejarán sobre la configuración de [!DNL Admin Console] y les proporcionarán vínculos a la documentación necesaria para que el traslado sea lo más sencillo y libre de complicaciones posible.

* [[!DNL Adobe Workfront] Información general sobre asistencia](https://experienceleague.adobe.com/es/docs/customer-one/using/workfront/overview)
* [[!DNL Workfront Admin Console] información](https://experienceleague.adobe.com/es/docs/customer-one/using/workfront/landing)
* [[!DNL Adobe Business Platform] y [!DNL Admin Console] preguntas más frecuentes](https://experienceleague.adobe.com/es/docs/customer-one/using/workfront/faq)

### ¿Cómo administra [!DNL Adobe Admin Console] para las compañías que ya lo tienen habilitado para Federated ID de forma distinta a la configuración del SSO de [!DNL Workfront]?

[!DNL Adobe Admin Console] tiene la opción de incluir [!DNL Workfront], reemplazando el SSO con el sistema Identity Management de Adobe (IMS). Todo el aprovisionamiento de usuarios se realiza en [!DNL Admin Console] y los usuarios verán la pantalla de inicio de sesión de [!DNL Adobe] para llegar a [!DNL Experience Cloud], donde verán [!DNL Workfront] como una opción (si se les concede acceso a este).

### ¿Cómo afecta esto a los clientes que ya tienen el panel de administración AEM para [!DNL Adobe Assets], pero tienen SSO configurado de forma diferente a [!DNL Workfront?]?

Una vez añadido [!DNL Workfront] como aplicación de [!DNL Admin Console], no debería tener que hacer nada más para que [!DNL Workfront] aproveche la configuración de SSO existente que tiene para [!DNL Adobe Assets].

### ¿Cómo afecta esto a los que están configurados con SSO?

SSO se configura en [!DNL Admin Console] y la aplicación [!DNL Workfront] lo hereda.

### ¿El SSO con nuestro [!DNL Active Directory] interno todavía será una opción con el sistema Identity Management de Adobe (IMS)?

IMS sustituye el sistema SSO y funciona prácticamente igual. Todos los permisos de usuario se han concedido y aprovisionado en [!DNL Adobe Admin Console], y el usuario verá la pantalla de inicio de sesión de [!DNL Adobe] en la que podrá elegir “[!UICONTROL Cuenta personal]” o “[!UICONTROL Cuenta de compañía]” para iniciar sesión (si tienen [!DNL Active Directory], la mayoría de usuarios iniciarán sesión con una cuenta de compañía).

### Para aquellos que no utilicen SSO, ¿cambia la dirección URL de inicio de sesión de [!DNL Workfront]?

La dirección URL de inicio de sesión cambiará, pero la antigua se redirigirá a la nueva dirección URL de inicio de sesión, por lo que será necesario volver a instruir a los usuarios para que sepan a dónde deben ir.

### ¿Seguirán funcionando los alias que hemos configurado o los vínculos [!DNL Workfront] van a cambiar con esta migración?

Existen redirecciones o alias de [!DNL Workfront] que permiten acceder a la página principal.

### ¿Habrá algún momento en que se deshabiliten los redireccionamientos? ¿O siempre podremos escribir my.company.workfront.com?

Siempre podrá utilizar cualquier dirección URL personalizada. Después de hacer clic en cualquiera de esos vínculos, se le dirigirá a [!DNL Workfront] y se mostrará una dirección URL diferente. Sin embargo, resulta una mejor [!DNL experience] iniciar sesión en experience.adobe.com y marcar vínculos como favoritos desde [!DNL Experience Cloud]. Menos redireccionamientos equivale a menos tiempo de retardo/tiempo de carga.

### ¿Se romperán los vínculos directos a las colas de solicitudes?

Todos los vínculos directos deben redirigirse a los nuevos patrones de URL. Sin embargo, si ha distribuido vínculos a personas, debe enviar una actualización para aprovechar el vínculo directo y evitar retrasos en el acceso a la página prevista.

### ¿Migraremos a [!DNL Experience Cloud] globalmente o podemos seleccionarlo para determinados usuarios (no todos nuestros usuarios utilizan otros productos de Adobe)?

Se migrará toda la cuenta de cliente de [!DNL Workfront] entera. No se puede hacer usuario a usuario.

### ¿Todos los usuarios de [!DNL Workfront] tendrán que iniciar sesión a través de [!DNL Experience Cloud]? ¿O solo los administradores?

Sí, todos los usuarios iniciarán sesión mediante [!DNL Experience Cloud]. El inicio de sesión de Adobe Identity Management System (IMS) reemplazará el SSO. Es una experiencia muy similar que solo tiene una pantalla de inicio de sesión diferente.

### ¿Tendrán los usuarios que vincular sus cuentas de [!DNL Adobe] a sus cuentas de [!DNL Workfront] si ya tienen ambas?

Sí, hay un proceso para esto y se proporcionarán más detalles cuando llegue el momento en que su organización se pase a IMS.

### ¿Qué les sucede a los usuarios de [!DNL Workfront] que no tienen una cuenta de [!DNL Adobe]?

Los usuarios a los que no se les ha concedido acceso en [!DNL Adobe Admin Console] para entrar a [!DNL Workfront] deben crear una &quot;[!UICONTROL personal account]&quot; o una cuenta de ID de [!DNL Adobe] para poder iniciar sesión. Esto envía un correo electrónico al administrador para aprobar o rechazar su solicitud y, además, le permite a este configurar el tipo de acceso que tiene ese usuario. Cuando inicien sesión, irán a experience.adobe.com, escribirán su dirección de correo electrónico y elegirán [!UICONTROL Personal Account]. Desde allí, podrán acceder a [!DNL Workfront].

### ¿Qué sucede si no tenemos productos [!DNL Adobe] distintos de [!DNL Workfront?]?

Recomendamos igualmente que su organización migre a la [!DNL Adobe Unified Experience]. Recibirá un ID de [!DNL Adobe] junto con los beneficios mencionados anteriormente.

### Se han incluido usuarios externos en nuestra instancia de [!DNL Workfront]. No queremos que tengan acceso a los otros productos incluidos en [!DNL Adobe]. ¿Cómo podemos limitar su acceso dentro de la consola?

[!DNL Admin Console] proporciona a los administradores mucho control con respecto a lo que los usuarios pueden y no pueden acceder. Siempre que un usuario externo desee acceso, deberá crear un ID de [!DNL Adobe], lo cual enviará un mensaje de correo electrónico al administrador. El administrador puede aceptar o rechazar el acceso a un producto y definir a qué pueden o no acceder los usuarios con respecto a los productos que son propiedad de esa organización. A continuación, el administrador del sistema de [!DNL Workfront] puede entrar en el área [!UICONTROL Users] de [!DNL Workfront] para obtener permisos más granulares para el usuario externo.

### Los administradores de grupo se usan para crear personas en [!DNL Workfront]. Con el cambio a [!DNL Experience Cloud], ¿los administradores de grupo aún podrán crear personas?

Sí, la creación de usuarios se sigue pudiendo hacer a través de [!DNL Workfront]. Estos usuarios se pueden añadir automáticamente a [!DNL Experience Cloud]. También puede configurar los administradores de grupo como propietarios de producto en [!DNL Admin Console] para que puedan asignar [!DNL Workfront] a los usuarios.

### ¿Cuál es la fecha límite para cambiar a [!DNL Experience Cloud]?

No hay ninguna fecha límite en este momento para cambiar a [!DNL Adobe Experience Cloud]. Estamos trabajando con los clientes para que puedan elegir cuándo estarán listos para realizar el cambio.

### ¿Necesitará nuestro equipo de soporte hacer algo con respecto a este cambio?

Si el equipo de soporte es responsable de la creación de nuevos usuarios, deberán familiarizarse con las interfaces de [!DNL Admin Console] utilizadas para crear usuarios y asignar un derecho a Workfront. De lo contrario, es probable que no haya ningún cambio significativo que afecte a su equipo de soporte interno.

### ¿Cómo afecta esto a las integraciones que tenemos a través de la función API?

La ruta URL existente seguirá disponible para el tráfico de la API. No es necesario que haga nada para actualizar los puntos finales en las integraciones. Sin embargo, no se admitirá el inicio de sesión directo mediante nombre de usuario y contraseña; con la excepción de los conectores de [!DNL Workfront Fusion], se debe utilizar una clave de API.

### ¿Qué pasará con los usuarios de [!DNL Creative Cloud]? ¿Cómo les afecta la migración? ¿Existe alguna ventaja para ellos?

Los usuarios de [!DNL Creative Cloud] no se verán afectados por la migración a [!DNL Adobe Unified Experience].

### ¿Cambiarán los inicios de sesión para los usuarios móviles de [!DNL Workfront]?

Los usuarios móviles de [!DNL Workfront] no deberían verse afectados por la migración a [!DNL Adobe Unified Experience].

### JumpSeat no funciona con [!DNL Adobe Unified Experience]. ¿Cómo puedo resolver esto?

JumpSeat funciona con [!DNL Adobe Unified Experience], pero requiere una actualización de configuración. Con el panel de administración de JumpSeat, cambie la dirección URL de la aplicación de `workfront.com` a `.workfront.adobe.com`
