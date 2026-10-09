<p align="center">
  <img src="banner.svg" alt="Joel Salcedo Ojeda. UX Engineer y Product Designer que entrega en código" width="100%">
</p>

<p align="center">
  <a href="https://joelsalcedoojeda.framer.website"><img alt="Portafolio" src="https://img.shields.io/badge/Portafolio-joelsalcedoojeda.framer.website-0e4f55?style=for-the-badge&logo=framer&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/joel-salcedo-ojeda-a74044359"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Joel%20Salcedo-123653?style=for-the-badge"></a>
  <a href="mailto:joelsalcedoojeda@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-joelsalcedoojeda%40gmail.com-f4a340?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

## Hola, soy Joel

Diseño producto y lo entrego en código. Llevo 7 años en esto, tres de ellos en fintech: pagos B2B en Estados Unidos y crédito con garantía hipotecaria en Perú.

Publico mis propias apps iOS en Swift y SwiftUI, y construyo productos full stack sobre PostgreSQL con desarrollo dirigido por especificación (SDD) y agentes de IA. Trabajo en remoto desde Colombia.

## Lo que estoy construyendo

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Mayapo POS</h3>
      <p>Sistema de punto de venta multi-restaurante. Tres aplicaciones sobre la misma base: mesero, cocina (KDS) y caja.</p>
      <ul>
        <li>Next.js (App Router), TypeScript estricto, Tailwind, TanStack Query y Zod</li>
        <li>Supabase: PostgreSQL, Auth, Realtime y Storage</li>
        <li>Multi-tenant con Row Level Security en todas las tablas. Los permisos viven en la base, no en la interfaz</li>
        <li>Claims en el token con un Auth Hook y operaciones sensibles en funciones <code>SECURITY DEFINER</code></li>
        <li>42 migraciones y 43 bloques de pruebas SQL de aislamiento entre restaurantes y de cálculo</li>
      </ul>
      <p><a href="https://mayapo-pos.vercel.app/entrar">mayapo-pos.vercel.app</a> · repositorio privado</p>
    </td>
    <td width="50%" valign="top">
      <h3>Tiro Bacano</h3>
      <p>Juego arcade de baloncesto para iOS. Publicado en la App Store, con más de 98 usuarios.</p>
      <ul>
        <li>SwiftUI y SpriteKit en Swift 6, con concurrencia estricta</li>
        <li>Compras con StoreKit 2, anuncios con AdMob, cuentas con Apple y Google</li>
        <li>Backend propio en Supabase para cuentas y ranking. Ninguna regla vive en la app: las decide PostgreSQL</li>
        <li>Edge Functions en TypeScript que verifican el dispositivo con App Attest y Play Integrity</li>
        <li>Pruebas SQL del servidor que corren con el rol y el token de un jugador real</li>
      </ul>
      <p><a href="https://tirobacano.framer.ai">tirobacano.framer.ai</a> · repositorio privado</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Rens</h3>
      <p>Finanzas personales para iOS. Publicada en la App Store, 80 usuarios activos.</p>
      <ul>
        <li>SwiftUI con MVVM</li>
        <li>Firebase Auth con Apple y Google</li>
        <li>Firestore en tiempo real para dividir cuentas entre varias personas</li>
        <li>Swift Charts y widgets</li>
      </ul>
      <p><a href="https://apps.apple.com/co/app/rens/id6757876753">App Store</a> · repositorio privado</p>
    </td>
    <td width="50%" valign="top">
      <h3>Subtitula</h3>
      <p>Extensión de Chrome que subtitula y traduce en tiempo real cualquier audio del navegador. Ocho idiomas.</p>
      <ul>
        <li>TypeScript y Manifest V3: service worker, documento offscreen y content scripts</li>
        <li>Transcripción por WebSocket con Gladia, traducción con DeepL y resúmenes con OpenAI</li>
        <li>Parte de un proyecto open source abandonado. Reparé el build y una condición de carrera en la mensajería de Chrome que perdía las traducciones</li>
      </ul>
      <p>repositorio privado</p>
    </td>
  </tr>
</table>

## Cómo trabajo con IA

Uso Spec-Driven Development (SDD). La IA no recibe un prompt suelto: recibe una especificación, un plan técnico y una lista de tareas, y lo que escribe pasa por pruebas y revisión antes de entrar.

```mermaid
flowchart LR
    A[Especificación<br/>qué y por qué] --> B[Plan técnico<br/>cómo]
    B --> C[Tareas<br/>en orden]
    C --> D[Claude Code<br/>implementa]
    D --> E[Pruebas y<br/>revisión de código]
    E -->|falla| D
    E -->|pasa| F[Producción]
```

- **Especificación primero.** Cada proyecto guarda su `spec`, su plan técnico y sus tareas en el repositorio, junto al código.
- **Las reglas en la base de datos.** Seguridad y lógica de negocio en PostgreSQL, con pruebas SQL que corren sobre base limpia.
- **Prototipos antes de comprometer al equipo.** Claude, v0 y un agente propio que corre sobre Gemma 4.

## Stack

**Producto y diseño**

![Figma](https://img.shields.io/badge/Figma-1e1e1e?style=flat-square&logo=figma&logoColor=white)
![Framer](https://img.shields.io/badge/Framer-0055ff?style=flat-square&logo=framer&logoColor=white)
![Webflow](https://img.shields.io/badge/Webflow-146ef5?style=flat-square&logo=webflow&logoColor=white)
![Design systems](https://img.shields.io/badge/Design%20systems-123653?style=flat-square)

**Frontend**

![TypeScript](https://img.shields.io/badge/TypeScript-3178c6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61dafb)
![Angular](https://img.shields.io/badge/Angular-dd0031?style=flat-square&logo=angular&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-0f172a?style=flat-square&logo=tailwindcss&logoColor=38bdf8)

**Backend y datos**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-1c1c1c?style=flat-square&logo=supabase&logoColor=3ecf8e)
![Firebase](https://img.shields.io/badge/Firebase-1f1f1f?style=flat-square&logo=firebase&logoColor=ffca28)
![GraphQL](https://img.shields.io/badge/GraphQL-e10098?style=flat-square&logo=graphql&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-1f2937?style=flat-square&logo=nodedotjs&logoColor=5fa04e)

**iOS**

![Swift](https://img.shields.io/badge/Swift-f05138?style=flat-square&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0a84ff?style=flat-square&logo=swift&logoColor=white)
![SpriteKit](https://img.shields.io/badge/SpriteKit-1f2937?style=flat-square&logo=apple&logoColor=white)
![StoreKit 2](https://img.shields.io/badge/StoreKit%202-1f2937?style=flat-square&logo=apple&logoColor=white)

**IA**

![Claude Code](https://img.shields.io/badge/Claude%20Code-d97757?style=flat-square&logo=claude&logoColor=white)
![v0](https://img.shields.io/badge/v0-000000?style=flat-square&logo=vercel&logoColor=white)
![SDD](https://img.shields.io/badge/Spec--Driven%20Development-0e4f55?style=flat-square)

## Experiencia

| Dónde | Rol | Qué hice |
|---|---|---|
| **Fintech de crédito con garantía hipotecaria** · Lima, remoto · 06/2024 – hoy | Product Designer · Design Expert – AI & Product Design | CRM que usan 60 asesores, con un modelo de IA integrado. El tiempo entre solicitud y desembolso bajó de 30 días a 10. Respondo por el frontend y lidero QA y dos desarrolladores. |
| **CashCloud** · Miami, remoto · 10/2023 – 08/2026 | Senior Product Designer / Design Lead | Plataforma de pagos B2B que mueve más de USD 100 millones al mes. Verificación bancaria y devoluciones ACH, cambio de método de pago, integraciones con ERP. Código en Angular. |

## Contacto

Español nativo · Inglés B2

[joelsalcedoojeda@gmail.com](mailto:joelsalcedoojeda@gmail.com) · [LinkedIn](https://www.linkedin.com/in/joel-salcedo-ojeda-a74044359) · [Portafolio](https://joelsalcedoojeda.framer.website)
