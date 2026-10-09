<p align="center">
  <img src="banner.svg" alt="Joel Salcedo Ojeda, UX Engineer. Diseño el producto y lo construyo: interfaz, datos y backend." width="100%">
</p>

<p align="center">
  <a href="https://joelsalcedoojeda.framer.website"><img alt="Portafolio" src="https://img.shields.io/badge/Portafolio-7c3aed?style=for-the-badge&logo=framer&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/joel-salcedo-ojeda-a74044359"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0a66c2?style=for-the-badge"></a>
  <a href="mailto:joelsalcedoojeda@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-ff4d8d?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://apps.apple.com/co/app/rens/id6757876753"><img alt="Rens en la App Store" src="https://img.shields.io/badge/Rens%20en%20la%20App%20Store-0a84ff?style=for-the-badge&logo=appstore&logoColor=white"></a>
  <a href="https://tirobacano.framer.ai"><img alt="Tiro Bacano" src="https://img.shields.io/badge/Tiro%20Bacano-ea580c?style=for-the-badge"></a>
</p>

## 👋 Sobre mí

Soy **UX Engineer**: diseño producto digital y lo llevo a producción en código. Tres años en fintech, en pagos B2B para Estados Unidos y en crédito con garantía hipotecaria para Perú, liderando diseño, QA y desarrollo frontend.

Por mi cuenta construyo productos completos: aplicaciones iOS en Swift y sistemas web sobre PostgreSQL, donde la seguridad y las reglas de negocio viven en la base de datos y no en la interfaz. Trabajo con Spec-Driven Development y agentes de IA.

- 🏦 **3 años en fintech**: una plataforma de pagos que mueve más de USD 100 millones al mes y un CRM de crédito que usan 60 asesores
- 📱 **2 apps iOS propias** publicadas en la App Store
- 🧠 **IA en producto y en el proceso**: un modelo integrado al CRM y desarrollo dirigido por especificación con Claude Code
- 🌎 Remoto desde Colombia · Español nativo · Inglés B2

## 🚀 Lo que construyo

<p align="center">
  <a href="https://mayapo-pos.vercel.app/entrar"><img src="assets/mayapo.svg" alt="Mayapo POS. Punto de venta multi-restaurante" width="49%"></a>
  <a href="https://tirobacano.framer.ai"><img src="assets/tirobacano.svg" alt="Tiro Bacano. Juego arcade de baloncesto para iOS" width="49%"></a>
</p>
<p align="center">
  <a href="https://apps.apple.com/co/app/rens/id6757876753"><img src="assets/rens.svg" alt="Rens. Finanzas personales para iOS" width="49%"></a>
  <a href="#-subtitula"><img src="assets/subtitula.svg" alt="Subtitula. Subtítulos traducidos en tiempo real para Chrome" width="49%"></a>
</p>

### 🍽️ Mayapo POS

Sistema de punto de venta multi-restaurante. Tres aplicaciones sobre una misma base de datos: mesero, cocina (KDS) y caja. **[mayapo-pos.vercel.app](https://mayapo-pos.vercel.app/entrar)**

<table>
  <tr><td width="140" valign="top"><b>Arquitectura</b></td><td>Multi-tenant desde el primer día. El token lleva restaurante, sede y rol mediante un Auth Hook, y cada política de Row Level Security lee esos claims.</td></tr>
  <tr><td width="140" valign="top"><b>Seguridad</b></td><td>RLS forzado en todas las tablas, con denegación por defecto. Las operaciones sensibles (anular una orden, cerrar caja, cambiar un precio) pasan por funciones <code>SECURITY DEFINER</code>. Auditoría de solo inserción.</td></tr>
  <tr><td width="140" valign="top"><b>Datos</b></td><td>42 migraciones versionadas. Dinero en pesos enteros con <code>numeric</code>, precios congelados al entrar a la orden y día operativo por sede.</td></tr>
  <tr><td width="140" valign="top"><b>Calidad</b></td><td>43 bloques de pruebas SQL de aislamiento entre restaurantes y de cálculo, que corren sobre una base limpia.</td></tr>
  <tr><td width="140" valign="top"><b>Stack</b></td><td><code>Next.js</code> <code>TypeScript</code> <code>PostgreSQL</code> <code>Supabase</code> <code>TanStack Query</code> <code>Zod</code> <code>Tailwind</code></td></tr>
</table>

### 🏀 Tiro Bacano

Juego arcade de baloncesto para iOS. Publicado en la App Store, con más de 98 usuarios. **[tirobacano.framer.ai](https://tirobacano.framer.ai)**

<table>
  <tr><td width="140" valign="top"><b>Cliente</b></td><td>SwiftUI con SpriteKit embebido, en Swift 6 con concurrencia estricta. Compras con StoreKit 2 y cuentas con Apple y Google.</td></tr>
  <tr><td width="140" valign="top"><b>Servidor</b></td><td>Backend propio para cuentas y ranking, pensado para iPhone y Android. Ninguna regla vive en la app: qué partida cuenta y quién gana lo decide PostgreSQL.</td></tr>
  <tr><td width="140" valign="top"><b>Integridad</b></td><td>Edge Functions en TypeScript que verifican el dispositivo con App Attest y Play Integrity antes de aceptar una partida.</td></tr>
  <tr><td width="140" valign="top"><b>Calidad</b></td><td>Pruebas SQL del servidor que se ejecutan con el rol y el token de un jugador real, más pruebas unitarias en la app.</td></tr>
  <tr><td width="140" valign="top"><b>Stack</b></td><td><code>Swift 6</code> <code>SwiftUI</code> <code>SpriteKit</code> <code>StoreKit 2</code> <code>PostgreSQL</code> <code>Edge Functions</code> <code>App Attest</code></td></tr>
</table>

### 💸 Rens

Finanzas personales para iOS. Publicada en la App Store, con 80 usuarios activos. **[Ver en la App Store](https://apps.apple.com/co/app/rens/id6757876753)**

Registro de gastos e ingresos con almacenamiento local primero, presupuestos por categoría y metas de ahorro. Las cuentas compartidas se dividen entre varias personas en tiempo real sobre Firestore.

`Swift` `SwiftUI` `MVVM` `Firebase Auth` `Firestore` `Swift Charts` `WidgetKit`

### 💬 Subtitula

Extensión de Chrome que subtitula y traduce en tiempo real cualquier audio del navegador, en ocho idiomas.

Parte de un proyecto open source abandonado que ya no compilaba. Reparé el build y resolví una condición de carrera en la mensajería de Chrome: varios listeners respondían mensajes ajenos y la traducción se perdía en el camino de vuelta.

`TypeScript` `Chrome Extensions MV3` `WebSockets` `Gladia` `DeepL` `OpenAI`

## ⚙️ Cómo trabajo

**Ingeniería dirigida por especificación (SDD).** El agente de IA nunca recibe un prompt suelto. Recibe documentos versionados en el repositorio, implementa una tarea a la vez y no avanza hasta pasar las puertas de calidad.

```mermaid
flowchart TB
    subgraph CTX["Contexto permanente del agente"]
        direction LR
        C1["CLAUDE.md<br/>stack, comandos, arquitectura<br/>y reglas no negociables"]
        C2["DECISIONES.md<br/>cada decisión con su razón"]
    end
    subgraph DOC["Documentos por funcionalidad"]
        direction LR
        S["spec.md<br/>qué y por qué"] --> P["plantecnico.md<br/>modelo de datos, contrato,<br/>seguridad y pruebas"]
        P --> T["task.md<br/>tareas numeradas"]
    end
    CTX --> A
    DOC --> A["Claude Code<br/>implementa una tarea"]
    A --> GPuertas de<br/>calidad
    G -->|falla| A
    G -->|pasa| M["Commit pequeño<br/>y tarea cerrada"]
    M -->|siguiente tarea| A
    M --> R["Producción"]
```

**Los artefactos**

| Artefacto | Responde | Contenido |
|---|---|---|
| `spec.md` | Qué y por qué | Contexto y objetivo, alcance, funcionalidades, restricciones transversales, riesgos asumidos y puntos abiertos |
| `plantecnico.md` | Cómo | Decisiones estructurales numeradas, modelo de datos, contrato de funciones, cómo se cumple cada regla de seguridad, plan de pruebas y supuestos confirmados |
| `task.md` | En qué orden | Tareas numeradas (`T-S3.4`) agrupadas por paso, con casilla de estado y una sección «Dónde quedamos» para retomar la siguiente sesión |
| `CLAUDE.md` | Con qué reglas | Stack, comandos, arquitectura y reglas no negociables que el agente lee antes de escribir código |
| `DECISIONES.md` | Por qué quedó así | Registro de decisiones técnicas, cada una con su razón. 34 en Mayapo POS |

**Puertas de calidad.** Una tarea no está hecha hasta que pasa la suya.

| Capa | Condición |
|---|---|
| Web | `tsc --noEmit` en modo estricto y ESLint sin errores. Los tipos de la base se regeneran desde el esquema después de cada migración |
| iOS | Debug y Release compilan, sin warnings nuevos y con las pruebas unitarias en verde |
| Base de datos | Pruebas SQL en verde sobre una base recreada desde cero: aislamiento entre tenants, permisos por rol y cálculo |
| Seguridad | Asesor de seguridad de Supabase sin avisos WARN ni ERROR. Una prueba de catálogo verifica que el rol `authenticated` solo ejecuta las funciones de su lista |

**Principios de arquitectura**

- **Infraestructura como código.** Nada se crea a mano en el panel: si no está en `supabase/`, no existe. Una migración aplicada no se edita, se crea otra.
- **La API son funciones.** El esquema interno no está expuesto. Las apps llaman funciones `SECURITY DEFINER` con `grant` explícito y nunca tocan tablas.
- **Denegación por defecto.** RLS habilitado y forzado en toda tabla, con políticas que leen los claims del JWT y no parámetros que mande el cliente.
- **Pruebas como el cliente real.** Se ejecutan con el rol `authenticated` y un JWT simulado, dentro de una transacción que se deshace al terminar.
- **Secretos fuera del bundle.** La llave de servicio vive solo en el servidor, detrás de `server-only`: un import equivocado rompe la compilación en vez de filtrarla.
- **Validación en cada borde.** Formularios, respuestas de API y variables de entorno pasan por Zod.

## 🧰 Stack

**Frontend**

<p>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178c6?style=flat-square&logo=typescript&logoColor=white">
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white">
  <img alt="React" src="https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61dafb">
  <img alt="Angular" src="https://img.shields.io/badge/Angular-dd0031?style=flat-square&logo=angular&logoColor=white">
  <img alt="Tailwind CSS" src="https://img.shields.io/badge/Tailwind%20CSS-0ea5e9?style=flat-square&logo=tailwindcss&logoColor=white">
  <img alt="TanStack Query" src="https://img.shields.io/badge/TanStack%20Query-ff4154?style=flat-square&logo=reactquery&logoColor=white">
  <img alt="Zod" src="https://img.shields.io/badge/Zod-3068b7?style=flat-square&logo=zod&logoColor=white">
</p>

**Backend y datos**

<p>
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white">
  <img alt="Supabase" src="https://img.shields.io/badge/Supabase-1c1c1c?style=flat-square&logo=supabase&logoColor=3ecf8e">
  <img alt="Row Level Security" src="https://img.shields.io/badge/Row%20Level%20Security-0f766e?style=flat-square">
  <img alt="Edge Functions" src="https://img.shields.io/badge/Edge%20Functions-1c1c1c?style=flat-square&logo=deno&logoColor=white">
  <img alt="Firebase" src="https://img.shields.io/badge/Firebase-dd2c00?style=flat-square&logo=firebase&logoColor=white">
  <img alt="Drizzle ORM" src="https://img.shields.io/badge/Drizzle%20ORM-1a1a1a?style=flat-square&logo=drizzle&logoColor=c5f74f">
  <img alt="GraphQL" src="https://img.shields.io/badge/GraphQL-e10098?style=flat-square&logo=graphql&logoColor=white">
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-3c873a?style=flat-square&logo=nodedotjs&logoColor=white">
</p>

**iOS**

<p>
  <img alt="Swift 6" src="https://img.shields.io/badge/Swift%206-f05138?style=flat-square&logo=swift&logoColor=white">
  <img alt="SwiftUI" src="https://img.shields.io/badge/SwiftUI-0a84ff?style=flat-square&logo=swift&logoColor=white">
  <img alt="SpriteKit" src="https://img.shields.io/badge/SpriteKit-111827?style=flat-square&logo=apple&logoColor=white">
  <img alt="StoreKit 2" src="https://img.shields.io/badge/StoreKit%202-111827?style=flat-square&logo=apple&logoColor=white">
  <img alt="WidgetKit" src="https://img.shields.io/badge/WidgetKit-111827?style=flat-square&logo=apple&logoColor=white">
  <img alt="App Attest" src="https://img.shields.io/badge/App%20Attest-111827?style=flat-square&logo=apple&logoColor=white">
</p>

**IA aplicada**

<p>
  <img alt="Claude Code" src="https://img.shields.io/badge/Claude%20Code-d97757?style=flat-square&logo=claude&logoColor=white">
  <img alt="Spec-Driven Development" src="https://img.shields.io/badge/Spec--Driven%20Development-7c3aed?style=flat-square">
  <img alt="v0" src="https://img.shields.io/badge/v0-000000?style=flat-square&logo=vercel&logoColor=white">
  <img alt="Gemma" src="https://img.shields.io/badge/Gemma-4285f4?style=flat-square&logo=google&logoColor=white">
</p>

**Low-code y diseño**

<p>
  <img alt="OutSystems sobre .NET" src="https://img.shields.io/badge/OutSystems%20sobre%20.NET-c8102e?style=flat-square">
  <img alt="Figma" src="https://img.shields.io/badge/Figma-1e1e1e?style=flat-square&logo=figma&logoColor=white">
  <img alt="Framer" src="https://img.shields.io/badge/Framer-0055ff?style=flat-square&logo=framer&logoColor=white">
  <img alt="Webflow" src="https://img.shields.io/badge/Webflow-146ef5?style=flat-square&logo=webflow&logoColor=white">
</p>

## 💼 Experiencia

| Periodo | Rol | Resultado |
|---|---|---|
| 06/2024 – hoy | **Product Designer · Design Expert, AI & Product Design**<br/>Fintech de crédito con garantía hipotecaria · Lima, remoto | Entré como UX Designer y pasé al cargo actual en 01/2026. Diseñé y entregué el CRM que usan 60 asesores de ventas, riesgos y cobranza, con un modelo de IA integrado. El tiempo entre solicitud y desembolso de un crédito bajó de 30 días a 10. Respondo por el frontend, reviso el contrato GraphQL con backend y lidero QA y dos desarrolladores. Otra compañía compró el proyecto para operarlo en México. |
| 10/2023 – 08/2026 | **Senior Product Designer / Design Lead**<br/>CashCloud · Miami, remoto | Entré como UI Designer a diseñar una versión mobile y quince meses después dirigía todo el diseño del producto. Plataforma de pagos B2B que usan cientos de empresas y mueve más de USD 100 millones al mes. Verificación bancaria y devoluciones ACH, cambio de método de pago sobre transacciones emitidas, despacho físico de cheques e integraciones con ERP. Cerca de 100 entrevistas con clientes. Código en Angular bajo cumplimiento SOC 2. |
| 02/2023 – 10/2023 | **Diseñador UI/UX**<br/>Inlaze · Bogotá | CRM de afiliados desde la idea hasta la primera versión en producción, un producto que la compañía no tenía. Con él los afiliados pasaron a gestionar y cobrar sus comisiones. Design system construido desde cero. |
| 01/2022 – 12/2022 | **Diseñador UX/UI Freelance**<br/>Montería | 10 proyectos digitales de punta a punta para clientes de ecommerce y otros sectores, con entrega documentada a desarrollo y acompañamiento durante la implementación. |
| 06/2019 – 12/2021 | **Desarrollador Web y Diseñador UX**<br/>Vitola SAS · Colombia | Ecommerce a medida diseñado y desarrollado desde cero, que llevó el catálogo de 17 puntos de venta físicos a un solo canal digital. Único responsable del diseño UX/UI y del desarrollo frontend. |

## 🎓 Formación

- **Licenciatura en Informática y Medios Audiovisuales** · Universidad de Córdoba · 2017 – 2022
- **The Complete Full-Stack Web Development Bootcamp** (61,5 h) · Udemy · 2025
- **UX/UI Design, UX Research, UX Writing, Product Design** · LinkedIn Learning · 2023

## 📫 Hablemos

<p align="center">
  <a href="mailto:joelsalcedoojeda@gmail.com"><img alt="joelsalcedoojeda@gmail.com" src="https://img.shields.io/badge/joelsalcedoojeda%40gmail.com-ff4d8d?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/joel-salcedo-ojeda-a74044359"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0a66c2?style=for-the-badge"></a>
  <a href="https://joelsalcedoojeda.framer.website"><img alt="Portafolio" src="https://img.shields.io/badge/Portafolio-7c3aed?style=for-the-badge&logo=framer&logoColor=white"></a>
</p>
