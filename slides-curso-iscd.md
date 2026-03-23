---
marp: true
theme: default
paginate: true
backgroundColor: #0f1419
color: #e6edf3
style: |
  section {
    background-color: #0f1419;
    font-family: 'Inter', -apple-system, sans-serif;
    padding: 40px 60px;
  }
  h1 {
    color: #58a6ff;
    font-size: 2.5em;
    font-weight: 700;
    margin-bottom: 0.3em;
  }
  h2 {
    color: #58a6ff;
    font-size: 1.8em;
    font-weight: 600;
    border-bottom: 2px solid #238636;
    padding-bottom: 10px;
    margin-bottom: 20px;
  }
  h3 {
    color: #f0883e;
    font-size: 1.3em;
    margin-top: 15px;
  }
  p, li {
    font-size: 1.1em;
    line-height: 1.6;
  }
  strong {
    color: #ffa657;
  }
  code {
    background: #21262d;
    padding: 2px 8px;
    border-radius: 4px;
    font-size: 0.95em;
  }
  section.title {
    text-align: center;
    justify-content: center;
  }
  section.title h1 {
    font-size: 3em;
    color: #ffffff;
  }
  section.title p {
    font-size: 1.4em;
    color: #8b949e;
  }
  .columns {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 40px;
  }
  .badge {
    display: inline-block;
    background: #238636;
    color: white;
    padding: 4px 12px;
    border-radius: 20px;
    font-size: 0.85em;
    font-weight: 600;
    margin: 5px 5px 5px 0;
  }
  .badge-blue { background: #1f6feb; }
  .badge-purple { background: #8957e5; }
  .badge-orange { background: #db6d28; }
  .highlight {
    background: linear-gradient(90deg, #238636 0%, #1f6feb 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: 700;
  }
  footer {
    font-size: 0.7em;
    color: #8b949e;
  }
  section::after {
    color: #8b949e;
    font-size: 0.8em;
  }
  ul li::marker {
    color: #238636;
  }
  blockquote {
    border-left: 4px solid #238636;
    background: #161b22;
    padding: 15px 20px;
    margin: 20px 0;
    border-radius: 0 8px 8px 0;
  }
  table {
    width: 100%;
    border-collapse: collapse;
    margin: 20px 0;
  }
  th {
    background: #21262d;
    color: #58a6ff;
    padding: 12px 15px;
    text-align: left;
  }
  td {
    padding: 12px 15px;
    border-bottom: 1px solid #30363d;
  }
  tr:hover {
    background: #161b22;
  }
---

<!-- _class: title -->
<!-- _paginate: false -->

# 🚀 Desarrollo con IA
## **De 0 a Producción**

---

<!-- _class: lead -->

# El Mercado Cambió

### Lo que era habilidad → ahora es commodity

- ~~Escribir código sin asistencia~~ → **Prompting efectivo**
- ~~Git push y rezar~~ → **Code Review automatizado**
- ~~Prototipos que nunca escalan~~ → **Spec-Driven Development**
- ~~Stack overflow copy-paste~~ → **Agentes que razonan**

> **El developer del 2026 no compite contra la IA... compite con developers que SABEN usar IA.**

---

# El Problema

## El 90% de los cursos enseñan *qué* hacer

<div class="columns">

**Faltan:**
- :x: Arquitectura con IA
- :x: Persistencia de contexto
- :x: Metodologías AI-First
- :x: De producción en mente

**Sobran:**
- :warning: Tutoriales de 2 horas
- :warning: "Prompts mágicos"
- :warning: Promesas vacías

</div>

---

<!-- _class: lead -->

# La Solución

## **3 jornadas intensivas para transformar tu stack**

```
┌─────────────────────────────────────────────────────────┐
│  DÍA 1          │  DÍA 2          │  DÍA 3            │
│  Fundamentos     │  Agentes        │  Producción       │
├──────────────────┼─────────────────┼───────────────────┤
│ • LLMs           │ • AI-First IDEs │ • TDD con IA      │
│ • Prompts        │ • Engram Cloud  │ • CI/CD           │
│ • SDD + PRD      │ • Multi-Agente  │ • Code Review     │
│ • Labs           │ • Labs          │ • Releases        │
└──────────────────┘└─────────────────┴───────────────────┘
```

**Modalidad:** Online por Zoom · Certificación ISCD

---

# Programa: Día 1 - Fundamentos

## *Domina las bases del desarrollo con IA*

### Mañana (3 horas)
| Tema | Descripción |
|------|-------------|
| **LLMs** | Modelos, tokens, limitaciones, pricing |
| **Context Window** | Memoria vs contexto, estrategias |
| **Prompts Engineering** | Patterns, few-shot, chain-of-thought |

### Tarde (3 horas)
| Tema | Descripción |
|------|-------------|
| **PRD** | Product Requirements Document con IA |
| **SDD** | Spec-Driven Development |
| **Lab 1** | Práctica con Engram + SDD |

---

# Programa: Día 2 - Agentes

## *Construye sistemas multi-agente*

### Mañana (3 horas)
| Tema | Descripción |
|------|-------------|
| **AI-First IDEs** | Cursor, Copilot, Windsurf, Claude Code |
| **Engram Cloud** | Memoria persistente para IA |
| **Agentic Patterns** | ReAct, Tool-use, Memory |

### Tarde (3 horas)
| Tema | Descripción |
|------|-------------|
| **Multi-Agente** | Orchestration, comunicación |
| **Human in Loop** | Gates, approval, fallback |
| **Lab 2** | Sistema multi-agente con Engram |

---

# Programa: Día 3 - Producción

## *Lleva tu código a producción profesional*

### Mañana (3 horas)
| Tema | Descripción |
|------|-------------|
| **TDD con IA** | Red-Green-Refactor potenciado |
| **Unit Testing** |覆盖率, edge cases |
| **Integration Testing** | Contratos, mocks |

### Tarde (3 horas)
| Tema | Descripción |
|------|-------------|
| **CI/CD** | Pipelines con IA |
| **Code Review** | Procesos AI-Augmented |
| **Lab 3** | Release completo con CI/CD |

---

# 🔧 Herramientas del Curso

## Stack tecnológico que dominarás

<div class="columns">

### **Memoria & Contexto**
- **Engram Cloud** — Memoria persistente multi-sesión
- **Context Management** — Optimización de tokens
- **Embedding** — Búsqueda semántica

### **Metodología**
- **SDD** — Spec-Driven Development
- **PRD** — Product Requirements Document
- **TDD** — Test-Driven Development

### **AI-First IDEs**
- Cursor, Claude Code, Windsurf, Copilot
- **200 prompts** categorizados por dominio

### **Producción**
- CI/CD con GitHub Actions
- Code Review automatizado
- Release management

</div>

---

# 🏆 Diferenciadores

## Por qué este curso es diferente

<span class="badge">Engram Cloud</span>
<span class="badge-blue">SDD + PRD</span>
<span class="badge-purple">Human in Loop</span>

### Lo que nos hace únicos:

| Diferenciador | Beneficio |
|--------------|-----------|
| **Memoria Persistente** | La IA "recuerda" entre sesiones |
| **Spec-Driven** | Diseña antes de codificar |
| **Metodología** | No solo herramientas, proceso |
| **200 Prompts** | Plantillas listas para producción |
| **Labs Prácticos** | Aprendizaje haciendo, no mirando |
| **Certificado ISCD** | Reconocimiento profesional |

---

# 🎯 Diferenciadores - Detalle

## Value Proposition en acción

### **Antes vs Después del curso:**

```
ANTES                          DESPUÉS
─────────────────────────────────────────────────────
ChatGPT random                Prompts estructurados
Código que "funciona"         Spec → Test → Code
Perdido en contexto           Engram Cloud memory
Prototipos descartables       Producción desde día 1
Developer junior              AI-First Developer
─────────────────────────────────────────────────────
```

### **ROI Esperado:**
- ⏱️ 40-60% reducción en tiempo de desarrollo
- 📈 3x más features en mismo sprint
- 🐛 70% menos bugs en producción
- 🔄 Iteraciones 5x más rápidas

---

# 👥 Audiencias

## ¿Para quién es este curso?

### **Perfil A: Estudiantes** 🎓
- Universitarios de últimos semestres
- Recién graduados en CS/Software
- Bootcamp graduates

<span class="badge-orange">Skills que el mercado exige</span>

---

### **Perfil B: Empresas** 🏢
- Equipos de desarrollo
- CTOs planificando 2026
- Startups escalando

<span class="badge-orange">Productividad + calidad</span>

---

### **Perfil C: Recruiters/HR** 💼
- Tech recruiters
- Headhunters de IT
- HR managers

<span class="badge-orange">Evaluar candidatos AI-Ready</span>

---

# 👨‍🏫 Instructores

## Expertos con experiencia real

<div class="columns">

### **Luis Jaramillo**
![ISCD Logo](https://iscd.ec/logo.png)
**CEO & Arquitecto de Ciberseguridad**
- 15+ años en seguridad ofensiva
- Profesor titular ESPE
- Fundador ISCD

### **Diego Saavedra**
![placeholder](data:image/svg+xml;base64,PHBV)
**FullStack Dev & Ethical Hacking**
- GDE & MVP
- SDD Practitioner
- GDE en Angular, Firebase

</div>

### Contacto:
- **WhatsApp:** +593 99 681 2371
- **YouTube:** @ISCDcanal

---

# 💬 Testimonios

## Lo que dicen nuestros estudiantes

> *"El módulo de SDD cambió completamente mi forma de abordar proyectos. Pasé de coder a architect."*
> 
> — **Carlos M.**, FullStack Developer

---

> *"La técnica de Engram Cloud para memoria persistente es revolutionary. Mi workflow con Claude mejoró 10x."*
> 
> — **María G.**, Backend Engineer @ Startup

---

> *"Como recruiter, este curso me dio las herramientas para evaluar candidatos AI-Ready. Transformó mi hiring process."*
> 
> — **Juan P.**, Tech Recruiter

---

# 📋 Info Práctica

## Detalles del curso

| Aspecto | Detalle |
|---------|---------|
| **Duración** | 3 jornadas (18 horas totales) |
| **Modalidad** | Online por Zoom |
| **Formato** | Teoría + Labs prácticos |
| **Idioma** | Español |
| **Materiales** | Slides, templates, 200 prompts |
| **Certificado** | Digital ISCD |

### Horarios:
- **Mañana:** 9:00 - 12:00 (hora Ecuador)
- **Tarde:** 14:00 - 17:00 (hora Ecuador)

---

# 💰 Inversión

## Planes disponibles

| Plan | Incluye | Precio |
|------|---------|--------|
| **Individual** | Curso + Labs + Templates | Consultar |
| **Corporativo** | 5+ devs + Workshop privado | Consultar |
| **VIP** | Todo + Mentoría 1:1 + Soporte | Consultar |

### **Early Bird** 🎁
*Primeros 10 inscriptos: 20% OFF*

---

<!-- _class: lead -->

# 🚀 ¿Listo para Transformar tu Carrera?

## **Reserva tu cupo ahora**

---

# Próximos Pasos

## Tu camino hacia AI-First Development

```
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│   RESERVA   │───▶│   PRE-CURSO │───▶│   3 DÍAS    │───▶│  CERTIFÍCATE │
│   TU CUPO   │    │   MATERIAL  │    │  INTENSIVO  │    │   + CV      │
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
```

### Contáctanos:

- **WhatsApp:** +593 99 681 2371
- **YouTube:** @ISCDcanal
- **Email:** [contacto@iscd.ec](mailto:contacto@iscd.ec)

---

<!-- _class: lead -->

# **ISCD**
## Information Security Consulting and Development

*Formando la próxima generación de developers AI-First*

---

<!-- _paginate: false -->

# Anexo: Temario Detallado

## Día 1 - Fundamentos

### Módulo 1.1: LLM Foundations
- Tipos de modelos (GPT, Claude, Gemini)
- Tokens y pricing
- Limitations y edge cases
- Picking the right model

### Módulo 1.2: Prompt Engineering
- Zero-shot, Few-shot, Chain-of-thought
- Role prompting
- Structured output
- Error handling

### Módulo 1.3: PRD & SDD
- Product Requirements Document
- Spec-Driven Development workflow
- From spec to code

---

# Anexo: Temario Detallado (cont.)

## Día 2 - Agentes

### Módulo 2.1: AI-First IDEs
- Cursor features avanzados
- Claude Code workflows
- Windsurf patterns
- Copilot extensions

### Módulo 2.2: Engram Cloud
- Setup y configuración
- Memory patterns
- Context optimization
- Multi-session persistence

### Módulo 2.3: Multi-Agent Systems
- Agentic patterns (ReAct, Tool-use)
- Orchestration patterns
- Human in the Loop design
- Fallback strategies

---

# Anexo: Temario Detallado (cont.)

## Día 3 - Producción

### Módulo 3.1: TDD con IA
- Red-Green-Refactor potenciado
- Test generation strategies
- Coverage analysis
- Mutation testing

### Módulo 3.2: CI/CD con IA
- GitHub Actions + AI
- Automated code review
- Quality gates
- Performance benchmarking

### Módulo 3.3: Releases
- Semantic versioning
- Changelog automation
- Release notes with AI
- Rollback strategies

---

# Anexo: Prompts Library Preview

## 200 prompts categorizados

### Categories:
1. **Architecture** (25) — System design, patterns
2. **Code Review** (30) — PR reviews, refactoring
3. **Testing** (25) — Unit, integration, e2e
4. **Debugging** (20) — Error analysis, fixes
5. **Documentation** (20) — README, API docs
6. **Security** (25) — Audit, hardening
7. **Performance** (20) — Optimization, profiling
8. **DevOps** (35) — CI/CD, Docker, Kubernetes

---

# Anexo: Requisitos

## Qué necesitas para el curso

### Hardware:
- :computer: Laptop/PC con mínimo 8GB RAM
- :headphones: Auriculares + micrófono
- :tv: Segunda pantalla (recomendado)

### Software:
- :globe: Navegador actualizado (Chrome/Firefox)
- :floppy_disk: Cuenta Engram Cloud (incluida)
- :gear: Git + IDE de tu preferencia
- :video_game: Zoom Desktop App

### Conocimientos previos:
- :white_check_mark: Programación básica
- :white_check_mark: Git fundamentals
- :white_check_mark: Terminal/CLI basics

---

# Anexo: FAQ

## Preguntas frecuentes

### ¿Necesito experiencia previa con IA?
No. El curso cubre desde fundamentos. Experiencia en programación es suficiente.

### ¿Las sesiones quedan grabadas?
Sí, tendrás acceso a las grabaciones por 6 meses.

### ¿Hay soporte post-curso?
Plan VIP incluye 1 mes de soporte. Plan Individual tiene acceso a comunidad.

### ¿El certificado tiene validez internacional?
El certificado ISCD es reconocido en la industria de seguridad de Ecuador y LATAM.

### ¿Puedo facturar a empresa?
Sí, emitimos facturas para empresas con RUC.

---

<!-- _class: lead -->
<!-- _paginate: false -->

# **¡Únete a la revolución AI-First!**

## ISCD · @ISCDcanal · +593 99 681 2371

