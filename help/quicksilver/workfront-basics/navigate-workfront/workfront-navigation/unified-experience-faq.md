---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Experiencia unificada de Adobe para preguntas más frecuentes
description: Algunas características son diferentes entre [!DNL Workfront] y Adobe Experience Cloud, y es posible que tenga algunas preguntas como [!DNL Workfront] se migra a la experiencia unificada.
author: Lisa
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Preguntas frecuentes

La variable [!DNL Adobe Unified Experience] para [!DNL Workfront] le permite administrar todas sus [!DNL Adobe] aplicaciones en un solo lugar con un solo inicio de sesión. La variable [!DNL Adobe] el área de navegación se integra perfectamente con [!DNL Workfront]. Algunas características son diferentes y es posible que tenga algunas preguntas como su [!DNL Workfront] se migra a la experiencia unificada.

Para obtener información sobre cómo iniciar sesión en la [!DNL Adobe Unified Experience], consulte [[!DNL Adobe Unified Experience] para [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparación de [!DNL Adobe Unified Experience] y [!DNL Workfront only] experiencia

Solo los clientes que usan la variable [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] puede acceder al [!DNL Adobe Unified Experience]. Los clientes que aún no hayan migrado podrán ver la variable [!DNL Workfront only] experiencia, sin la capacidad de cambiar entre [!DNL Adobe] aplicaciones.

En esta tabla se describen algunas funciones que difieren entre las dos experiencias.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] experiencia única |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menú principal] está a la izquierda ![Menú principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menú principal] está a la derecha ![Menú principal](assets/main-menu-icon.png) |
| Una sola dirección URL de inicio de sesión está disponible para todos [!DNL Adobe Experience Cloud] aplicaciones | Iniciar sesión en [!DNL Workfront] con un [!DNL Workfront] URL |
| Un &quot;conmutador de organización&quot; le permite moverse entre [!DNL Workfront] organizaciones y entornos | El &quot;conmutador de organización&quot; no está disponible |
| La navegación incluye un área de navegación de nivel superior para [!DNL Adobe] productos, [!DNL Adobe] notificaciones, ayuda y su perfil de usuario, además del [!DNL Workfront] barra de navegación | La navegación incluye el [!DNL Workfront] solo barra de navegación |
| Se puede acceder a la ayuda a través de la [!UICONTROL Menú principal] y zona de navegación superior | Se puede acceder a la ayuda a través de la [!UICONTROL Menú principal] y [!DNL Workfront] barra de navegación |

{style=&quot;table-layout:auto&quot;}

## Preguntas frecuentes

**¿Cómo puedo obtener más información sobre el [!DNL Adobe Admin Console]?**

Para obtener información sobre la variable [!DNL Admin Console], revise estos artículos:

* [Prepare para el [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferencias de administración basadas en plataformas ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] información general](https://helpx.adobe.com/es/enterprise/using/admin-console.html)

**¿Qué debo hacer como cliente para facilitar la migración?**

Se contactará con los clientes existentes para programar migraciones. Los compañeros de soporte del equipo de migración guiarán a los clientes a través del proceso, aconsejarán sobre [!DNL Admin Console] configure y proporcione vínculos a la documentación necesaria para que el movimiento sea lo más sencillo y sencillo posible.

* [[!DNL Adobe Workfront] Información general sobre la asistencia](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] información](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] and [!DNL Admin Console] Preguntas frecuentes](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

**Cómo maneja [!DNL Adobe Admin Console] para empresas que ya tienen esto habilitado para Federated ID de forma distinta a [!DNL Workfront] ¿SSO está configurado?**

[!DNL Adobe Admin Console] tiene la opción de incluir [!DNL Workfront], reemplazando SSO por IMS. Todo el aprovisionamiento de usuarios se produce en la variable [!DNL Admin Console]y los usuarios verán la variable [!DNL Adobe] pantalla de inicio de sesión para llegar a [!DNL Experience Cloud] donde verán [!DNL Workfront] como opción (si se les concede acceso a él).

**¿Cómo afecta esto a los clientes que ya tienen el panel de administración de AEM para [!DNL Adobe Assets] - pero el SSO está configurado de forma diferente que[!DNL Workfront?]**

Una vez [!DNL Workfront] se añade como [!DNL Admin Console] aplicación, no debe hacer nada más por [!DNL Workfront] para aprovechar la configuración de SSO existente que tiene para [!DNL Adobe Assets].

**¿Cómo afecta esto a los que están configurados con SSO?**

SSO se configura en la variable [!DNL Admin Console] y heredado por el [!DNL Workfront] aplicación.

**Es SSO con nuestra [!DNL Active Directory] ¿seguirá siendo una opción con IMS?**

IMS es un reemplazo para SSO y funciona principalmente igual. Todos los permisos de usuario se conceden y aprovisionan en [!DNL Adobe Admin Console], y el usuario verá la variable [!DNL Adobe] pantalla de inicio de sesión donde puede elegir &quot;[!UICONTROL Cuenta personal]&quot; o &quot;[!UICONTROL Cuenta de la empresa]&quot; para iniciar sesión (si tiene [!DNL Active Directory], la mayoría iniciará sesión con una cuenta de empresa).

**Para aquellos que no utilizan SSO, ¿realiza la variable [!DNL Workfront] cambio de dirección URL de inicio de sesión?**

La dirección URL de inicio de sesión cambiará; sin embargo, la antigua dirección URL redireccionará a la nueva dirección URL de inicio de sesión, por lo que debe volver a entrenar a los usuarios a dónde ir.

**¿Seguirán funcionando los alias que hemos configurado, o son los [!DNL Workfront] ¿los vínculos cambian con esta migración?**

[!DNL Workfront] los redireccionamientos y alias están disponibles para llegar a la página principal.

**¿Habrá algún momento en que se deshabiliten las redirecciones? ¿O siempre podremos escribir my.company.workfront.com?**

Siempre podrá usar direcciones URL personalizadas. Después de hacer clic en cualquiera de estos vínculos, le redirigirá a [!DNL Workfront] y muestran una dirección URL diferente. Sin embargo, es mejor [!DNL experience] para iniciar sesión en experience.adobe.com y marcar vínculos desde [!DNL Experience Cloud]. Menos redireccionamiento es igual a menos tiempo de retraso/tiempo de carga.

**¿Se romperán los vínculos directos a las colas de solicitud?**

Todos los vínculos directos deben redirigir a los nuevos patrones de URL. Sin embargo, si ha distribuido vínculos a personas, debe enviar una actualización para aprovechar el vínculo directo y evitar retrasos en el acceso a la página esperada.

**¿Migraremos a [!DNL Experience Cloud] globalmente, ¿o podemos seleccionar para ciertos usuarios (no todos nuestros usuarios usan incluso otros productos de Adobe)?**

Todo [!DNL Workfront] se migrará la cuenta de cliente. No se puede hacer usuario por usuario.

**Will all [!DNL Workfront] los usuarios deben iniciar sesión mediante [!DNL Experience Cloud]? ¿O solo administradores?**

Sí, todos los usuarios iniciarán sesión mediante [!DNL Experience Cloud]. El inicio de sesión de IMS sustituirá a SSO. Es una experiencia muy similar, solo una pantalla de inicio de sesión diferente.

**¿Los usuarios tendrán que vincular su [!DNL Adobe] cuentas en sus [!DNL Workfront] cuentas si ya tienen ambas?**

Sí, hay un proceso para esto, y se proporcionarán más detalles cuando sea hora de que su organización se traslade a IMS.

**Qué le sucede a la variable [!DNL Workfront] usuarios que no tengan un [!DNL Adobe] cuenta?**

Usuarios a los que no se ha concedido acceso en [!DNL Adobe Admin Console] para entrar [!DNL Workfront] debe crear un[!UICONTROL cuenta personal]&quot; o [!DNL Adobe] Cuenta de ID para poder iniciar sesión. Esto envía un correo electrónico al administrador para aprobar o rechazar su solicitud y, además, permite al administrador configurar el tipo de acceso que tiene. Cuando inicien sesión, irán a experience.adobe.com, introducirán su dirección de correo electrónico y elegirán [!UICONTROL Cuenta personal]. Desde allí, podrán acceder a [!DNL Workfront].

**¿Y si no tenemos ninguno? [!DNL Adobe] productos distintos de[!DNL Workfront?]**

Aún se recomienda que su organización migre a la variable [!DNL Adobe Unified Experience]. Recibirá una [!DNL Adobe] ID junto con los beneficios enumerados anteriormente.

**Tenemos usuarios externos incluidos en nuestra [!DNL Workfront] instancia. No queremos que tengan acceso a ningún otro producto incluido en [!DNL Adobe]. ¿Cómo limitaríamos su acceso dentro de la consola?**

[!DNL Admin Console] proporciona a los administradores mucho control sobre lo que los usuarios pueden y no pueden acceder. Siempre que un usuario externo desee acceder, debe crear un [!DNL Adobe] ID, que envía un correo electrónico al administrador. A continuación, el administrador puede aceptar o rechazar el acceso a un producto y definir a qué puede acceder o no a los productos propiedad de esa organización. A continuación, el [!DNL Workfront] El administrador del sistema puede entrar en la [!UICONTROL Usuarios] área de [!DNL Workfront] para crear permisos más granulares para el usuario externo.

**Los administradores de grupo se utilizan para crear personas en [!DNL Workfront]. Con el desplazamiento a [!DNL Experience Cloud], ¿seguirán los administradores de grupo siendo capaces de crear personas?**

Sí, la creación de usuarios sigue siendo posible a través de [!DNL Workfront]. Estos usuarios se pueden agregar a [!DNL Experience Cloud] automáticamente. También puede configurar sus administradores de grupo como propietarios de productos en la variable [!DNL Admin Console] para permitirles asignar [!DNL Workfront] a los usuarios.

**¿Cuál es la fecha límite para cambiar a [!DNL Experience Cloud]?**

Actualmente no hay plazo para pasar a [!DNL Adobe Experience Cloud]. Estamos trabajando con los clientes para permitirles elegir cuándo están listos para realizar el cambio.

**¿Necesitará nuestro equipo de asistencia hacer algo para este cambio?**

Si el equipo de asistencia es responsable de la creación de nuevos usuarios, deberán familiarizarse con la variable [!DNL Admin Console] interfaces utilizadas para crear usuarios y asignar un derecho a Workfront. De lo contrario, es probable que no haya ningún cambio significativo para su equipo de asistencia interna.

**¿Cómo afecta esto a las integraciones que tenemos a través de la función de API?**

La ruta de URL existente seguirá estando disponible para el tráfico de API. No es necesario que haga nada para actualizar los extremos de las integraciones. Sin embargo, no se admitirá el inicio de sesión directo mediante nombre de usuario y contraseña: debe utilizar una clave de API, con la excepción de [!DNL Workfront Fusion] conectores.

**¿Qué pasa con [!DNL Creative Cloud] usuarios? ¿Cómo les afecta la migración? ¿Hay alguna ventaja para ellos?**

No hay ningún impacto en [!DNL Creative Cloud] usuarios con la migración a [!DNL Adobe Unified Experience].

**Los inicios de sesión cambiarán para [!DNL Workfront] usuarios móviles?**

[!DNL Workfront] los usuarios móviles no deben verse afectados por la migración a [!DNL Adobe Unified Experience].
