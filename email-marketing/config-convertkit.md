# CONFIGURACIÓN — ConvertKit & Mailchimp

**ISCD — Information Security Consulting and Development**

---

## CONVERTKIT

### 1. Formularios de Opt-In

#### Landing Page Principal
```
Nombre: Landing - Desarrollo con IA
URL: https://iscd.ec/curso-ia
```

#### Form Embed
```html
<!-- Widget ConvertKit -->
<form action="https://app.convertkit.com/forms/XXXXXXXX/interactions.js" method="post" class="ck_form">
  <input type="email" name="email_address" placeholder="Tu email" required>
  <input type="text" name="first_name" placeholder="Tu nombre">
  <button type="submit">Descargar guía gratuita</button>
</form>
```

#### Campo oculto (UTM tracking)
```html
<input type="hidden" name="tags" value="curso-ia">
<input type="hidden" name="utm_source" value="{utm_source}">
<input type="hidden" name="utm_medium" value="{utm_medium}">
```

---

### 2. Tags para Segmentación

| Tag | Descripción | Trigger |
|-----|-------------|---------|
| `lead-curso-ia` | Interesado en el curso | Formulario de opt-in |
| `estudiante-espe` | Estudiante ESPE | Campo universidad = ESPE |
| `estudiante-uide` | Estudiante UIDE | Campo universidad = UIDE |
| `empresa` |来自企业 | Campo empresa no vacío |
| `freelancer` | Freelancer | Campo empresa vacío + freelance checked |
| `descargó-guía` | Descargó lead magnet | Completó opt-in |
| `abrió-email-1` | Abrió email #1 | Automation trigger |
| `click-cta-1` | Clickeó CTA #1 | Automation trigger |
| `no-abrió-email-1` | No abrió email #1 | Automation trigger |
| `compró-curso` | Compró el curso | Payment confirmed |
| `cupo-reservado` | Reservó cupo | Depósito confirmado |

---

### 3. Sequences / Automations

#### Sequence Principal: "Curso IA - 5 Emails"

| # | Email | Enviar | Condición |
|---|-------|--------|-----------|
| 1 | Anuncio | Día 1 | Tag: `lead-curso-ia` |
| 2 | Problema + Solución | Día 3 | Si abrió #1 |
| 3 | Venta Principal | Día 5 | Si abrió #1 o #2 |
| 4 | Urgencia | Día 7 | Si noció #3 |
| 5 | Cierre | Día 9 | Si noció #4 |

#### Automation: Re-engagement
```
Trigger: No abre email en 72h
Action: Enviar variant con diferente subject
```

#### Automation: Abandoned Cart
```
Trigger: Visitó checkout pero no pagó
Wait: 2 horas
Action: Email de recuperación
```

---

### 4. Broadcasts

| Broadcast | Asunto | Segmento | Fecha |
|-----------|--------|----------|-------|
| Anuncio inicio | [Subject Email 1] | Todos los leads | Día 1 |
| Recordatorio | Recordatorio del email 1 | No abrieron | Día 2 |
| Venta final | Urgencia última | Abiertos sin compra | Día 7 |

---

## MAILCHIMP

### 1. Audience / List

```
Nombre: ISCD - Curso IA
Default from name: ISCD
Reply-to: hola@iscd.ec
```

#### Merge Fields

| Field | Tag | Type | Description |
|-------|-----|------|-------------|
| First Name | FNAME | Text | Nombre del suscriptor |
| Last Name | LNAME | Text | Apellido |
| Company | COMPANY | Text | Empresa (opcional) |
| Universidad | UNIV | Dropdown | ESPE, UIDE, OTHER |
| Rol | ROL | Dropdown | Estudiante, Dev, Manager |
| Interés | INTERES | Checkbox | Curso IA, Consulting, Both |

---

### 2. Tags (Mailchimp)

| Tag | Descripción | Color |
|-----|-------------|-------|
| lead-curso-ia | Interesado en curso | Blue |
| estudiantes | Estudiantes | Green |
| empresas | Empresas | Purple |
| freelancers | Freelancers | Orange |
| comprados | Compraron | Red |
| no-interesado | Sin interés | Gray |

---

### 3. Customer Journeys

#### Journey: "Curso IA - Secuencia 5 Días"

```
TRIGGER: Tag "lead-curso-ia" added

DAY 1:
└─ Send Email: "Email 1 - Anuncio"
   └─ Wait 2 days

DAY 3:
└─ IF Opened Email 1
   └─ Send Email: "Email 2 - Problema"
   └─ Wait 2 days
   
   IF Not Opened
   └─ Send Email: "Email 1 - Variant B"
   └─ Wait 1 day

DAY 5:
└─ Send Email: "Email 3 - Venta Principal"
└─ Wait 2 days

DAY 7:
└─ Send Email: "Email 4 - Urgencia"
└─ Wait 2 days

DAY 9:
└─ Send Email: "Email 5 - Cierre"
```

---

### 4. Landing Pages

```
URL: https://iscd.ec/curso-ia
Tipo: Product/Services
```

#### Popup / Exit Intent
```
Display: Exit intent + 5s delay
Content: "Antes de ir...Descarga la guía gratuita"
```

---

## UTM TRACKING

### URLs con UTM

| Email | Campaña | Source | Medium | Content |
|-------|---------|--------|--------|---------|
| 1 | curso-ia | email | newsletter | email-1 |
| 2 | curso-ia | email | newsletter | email-2 |
| 3 | curso-ia | email | newsletter | email-3 |
| 4 | curso-ia | email | newsletter | email-4 |
| 5 | curso-ia | email | newsletter | email-5 |

### Ejemplo URL completa
```
https://wa.me/593996812371?text=Quiero%20info
&utm_source=email&utm_medium=newsletter&utm_campaign=curso-ia&utm_content=email-1
```

---

## INTEGRACIÓN WHATSAPP (Click to Chat)

### Links por email

| Email | Link WhatsApp |
|-------|---------------|
| 1 | wa.me/593996812371?text=Hola%2C%20quiero%20información%20del%20curso%20Desarrollo%20con%20IA |
| 2 | wa.me/593996812371?text=Quiero%20más%20info%20del%20curso |
| 3 | wa.me/593996812371?text=Quiero%20reservar%20mi%20lugar%20en%20el%20curso |
| 4 | wa.me/593996812371?text=Datos%20para%20reservar%20mi%20lugar |
| 5 | wa.me/593996812371?text=Quiero%20el%20último%20cupo%20disponible |

---

## EXPORT/IMPORT

### ConvertKit Export
1. Ir a **Audience** → **Export**
2. Seleccionar formato CSV
3. Incluir: email, name, tags, created_at

### Mailchimp Export
1. Ir to **Audience** → **Export**
2. Seleccionar formato CSV
3. Incluir: merge fields y tags

---

**© 2026 ISCD — Information Security Consulting and Development**
