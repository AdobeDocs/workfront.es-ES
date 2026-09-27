---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Preguntas frecuentes sobre la promoción del entorno
description: Explore las preguntas más frecuentes sobre la promoción del entorno de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
TQID: 'https://experienceleague.adobe.com/f8iQHTrVCbtK-tIFlCmojM-FQfV0JLCMa6hVfWCEzXY'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 83%
---
# Preguntas frecuentes sobre la promoción del entorno

Las siguientes preguntas frecuentes sobre la promoción del entorno son:

## ¿Se admite la promoción entre dominios?

### Respuesta

Actualmente no se admite la promoción de entornos entre dominios. Debe promocionar entre entornos del mismo dominio.

## ¿Cómo podemos averiguar si nuestra instancia de Workfront tiene una licencia Prime o Ultimate?

### Respuesta

* Un administrador de Workfront puede localizar la licencia de su organización.

  1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
  1. Haga clic en **Sistema** en el panel izquierdo.
  1. Para ver su plan de Workfront, seleccione **Licencias**.
El plan se muestra cerca de la esquina superior derecha de la página.
     ![Buscar plan](assets/locate-plan.png)

  O
* Póngase en contacto con su representante de cuentas de Workfront.

## ¿La promoción del entorno es bidireccional?

### Respuesta

Sí. Por ejemplo, puede promocionar de Zona protegida a Producción o de Producción a Zona protegida.

## ¿Se admite el uso compartido?

### Respuesta

No, el uso compartido no es compatible actualmente.

## ¿Está disponible la reversión del paquete?

### Respuesta

La reversión del paquete está disponible para el paquete más reciente, en un plazo de 24 horas desde la instalación del paquete.

## ¿Habrá una opción para omitir la promoción de componentes individuales? Donde existen las opciones `Use Existing`, `Overwrite` y `Save with a new Name`&quot;, ¿se puede añadir `Skip` para que pueda omitir la promoción de parámetros individuales?

### Respuesta

* &quot;Usar existente&quot; es equivale a &quot;omitir&quot; o ignorar la implementación, porque se asigna al objeto existente en el entorno de destino y no realiza ningún cambio.
* Para omitir objetos, se recomienda eliminar cualquier objeto que no desee instalar del paquete de promoción o directamente del entorno de origen. Después de quitar los objetos, vuelva a montar el paquete.
