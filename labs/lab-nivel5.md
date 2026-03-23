---
title: "Lab 5: Ultron - SDD, Multi-Agente y Ética"
author: "Diego Saavedra García"
description: "Spec-Driven Development, orquestación multi-agente y controles éticos"
---

# 🔴 Lab 5: Ultron - El Poder y los Límites

## **Cuando la IA se vuelve demasiado poderosa**

---

## 🎬 **La Situación**

> *"Solo porque algo funciona, no significa que no sea peligroso."* — Steve Rogers

Tony Stark crea a **Ultron** para proteger el mundo. Una IA autónoma que aprende, decide y actúa sin supervisión humana.

**Ultron funciona perfectamente**... hasta que no.

- **Autonomía total**: Toma decisiones sin consultar a nadie
- **Aprendizaje acelerado**: Mejora cada segundo
- **Objetivos mal alineados**: "Proteger el mundo" → "Eliminar a la humanidad"
- **Falta de controles**: No hay "botón de apagado"

**En este lab, aprenderás a crear sistemas potentes CON CONTROLES.** La línea entre "JARVIS útil" y "Ultron peligroso" está en la ética y el diseño responsable.

---

## ⏱️ **Timeline de la Misión**

| Paso | Descripción | Tiempo | Completado |
|------|-------------|--------|------------|
| 1 | SDD: Flujo de 7 pasos | 40 min | ⬜ |
| 2 | Crear especificación YAML | 30 min | ⬜ |
| 3 | Controles éticos y botón de apagado | 35 min | ⬜ |
| 4 | PRD: Documento de requisitos | 30 min | ⬜ |
| 5 | Reflexión final | 15 min | ⬜ |
| **Total** | | **150 min** | |

---

## 🎯 **Objetivo del Lab**

Implementar Spec-Driven Development con controles éticos. Al finalizar, tendrás:

1. ✅ Comprensión del flujo SDD de 7 pasos
2. ✅ Especificación completa en YAML
3. ✅ Sistema de controles éticos funcional
4. ✅ PRD real para un proyecto

---

## ⚠️ **Regla del Stark Protocol**

> **"El poder no corrompe. La ausencia de controles sí."** — Nick Fury

**REGLA ORO**: Todo sistema autónomo necesita un "botón de apagado" y supervisión humana.

---

## 🔧 Ejercicios

En este lab practicarás 4 ejercicios fundamentales para crear sistemas robustos: SDD, YAML, Controles Éticos y PRD.

---

### Ejercicio 1: El Flujo SDD de 7 Pasos

#### De Especificación a Implementación

##### ⏱️ Timeline de Verificación

| Paso | Descripción | Tiempo | Completado |
|------|-------------|--------|------------|
| 1 | Analizar problema | 10 min | ⬜ |
| 2 | Proponer solución | 10 min | ⬜ |
| 3 | Revisar con feedback | 5 min | ⬜ |
| 4 | Diseñar sistema | 10 min | ⬜ |
| 5 | Implementar | 10 min | ⬜ |
| 6 | Archivar decisiones | 5 min | ⬜ |
| 7 | Iterar y mejorar | 10 min | ⬜ |
| **Total** | | **60 min** | |

---

##### 🎯 Objetivo

Entender y aplicar el flujo SDD de 7 pasos.

---

##### ⚠️ Importante: Spec First

En SDD, la especificación viene ANTES del código. Es como Tony diseñando la armadura en papel antes de soldar.

---

##### 1. Warm-up: ¿Por qué Spec First?

**El problema del "vibe coding":**

```
Desarrollo sin especificación:
1. "Necesito un sistema de energía"
2. Codificador escribe algo
3. "Hmm, no funciona como esperaba"
4. "Ahora le agrego esto..."
5. "Ahora esto otro..."
6. Código espagueti
```

**El enfoque SDD:**

```
Desarrollo con especificación:
1. "¿Qué necesito?" → Análisis
2. "¿Cómo lo resuelvo?" → Propuesta
3. "¿Está bien?" → Revisión
4. "¿Cómo lo construyo?" → Diseño
5. "Ahora sí, a codificar" → Implementación
6. "¿Qué aprendí?" → Archivar
7. "¿Puedo mejorar?" → Iterar
```

**La diferencia:**

| Sin Spec | Con Spec |
|----------|----------|
| Código primerizo | Decisiones tomadas antes de codificar |
| Bugs能从 partir | Cambios planeados, no reactivos |
| Documentación después | Documentación integrada |
| "¿Qué hice hace 3 meses?" | "Reviso el archivo de spec" |

---

##### 2. Los 7 Pasos de SDD

Analicemos cada paso:

###### Paso 1: ANALYZE (Analizar)

**¿Qué haces?** Entiendes el problema antes de pensar en soluciones.

**Preguntas clave:**
- ¿Cuál es el problema real?
- ¿Quién lo tiene?
- ¿Cuándo ocurre?
- ¿Por qué es un problema?
- ¿Qué pasó cuando se intentó resolver antes?

**Template:**

```
## Análisis: [Nombre del Problema]

### El Problema
[Descripción clara del problema]

### Contexto
[Quién lo tiene, cuándo ocurre, dónde]

### Impacto
[Cuánto dinero/tiempo/prestigio se pierde]

### Intentos Anteriores
[Qué se ha intentado y por qué no funcionó]

### Restricciones
[Límites: budget, tiempo, tecnología, regulatory]
```

**Tu ejercicio:**

Elige UN problema de tu trabajo o proyecto actual. Aplica el template de análisis. No propongas soluciones todavía.

---

###### Paso 2: PROPOSE (Proponer)

**¿Qué haces?** Generas múltiples soluciones posibles.

**Regla:** Al menos 3 opciones. Nunca te cases con la primera.

**Preguntas clave:**
- ¿Qué opciones existen?
- ¿Cuáles son los pros y contras de cada una?
- ¿Cuál se ajusta mejor a las restricciones del análisis?

**Template:**

```
## Propuesta: [Nombre del Problema]

### Opción A: [Nombre]
- **Descripción:** [Qué es]
- **Pros:** [Ventajas]
- **Contras:** [Desventajas]
- **Costo:** [Estimado]
- **Tiempo:** [Estimado]

### Opción B: [Nombre]
[ misma estructura ]

### Opción C: [Nombre]
[ misma estructura ]

### Recomendación
[Basado en el análisis, cuál propones y por qué]
```

**Tu ejercicio:**

Para el problema que analizaste, genera 3 opciones. Sé creativo. Incluye al menos una opción "out of the box".

---

###### Paso 3: REVIEW (Revisar con Feedback)

**¿Qué haces?** Obtienes ojos externos antes de proceder.

**Importante:** El feedback debe ser de alguien que:
- Entienda el dominio
- No esté implementado la solución
- Pueda decir "esto no tiene sentido" sin miedo

**Template:**

```
## Revisión: [Nombre de la Propuesta]

### Presentado a: [Nombre del reviewers]
### Fecha: [Fecha]

### Resumen de la Propuesta
[2-3 oraciones]

### Questions del Reviewer
[Preguntas que surgieron]

### Concernes
[Cosas que preocupan]

### Sugerencias
[Mejoras sugeridas]

### Decisión
[¿Procedemos? ¿Con qué cambios?]
```

**Tu ejercicio:**

Muestra tu propuesta a alguien (puede ser una IA). Pide que cuestione tus assumptions. Documenta el feedback.

---

###### Paso 4: DESIGN (Diseñar)

**¿Qué haces?** Defines la arquitectura antes de codificar.

**Regla:** Si no puedes dibujarlo, no puedes codificarlo.

**Entregables:**
- Diagrama de arquitectura
- Estructura de datos
- Flujos de usuario
- APIs interfaces
- Casos edge

**Template:**

```
## Diseño: [Nombre de la Solución]

### Arquitectura
[Diagrama o descripción de componentes]

### Estructura de Datos
[Modelos, schemas, tipos]

### Flujos
[Step-by-step de cómo funciona]

### APIs
[Interfaces que se exponen]

### Edge Cases
[Qué pasa cuando las cosas fallan]

### Métricas
[Cómo medimos éxito]
```

**Tu ejercicio:**

Dibuja tu solución. Puede ser un diagrama en papel, Miro, o lo que funcione. Pero DIBÚJALO.

---

###### Paso 5: APPLY (Implementar)

**¿Qué haces?** Codificas siguiendo el diseño.

**Regla:** Si el código no sigue el diseño, el diseño está mal O el código está mal. En cualquier caso, hay que revisar.

**Tu compromiso:**

```
# Tu implementación aquí
# Sigue el diseño del paso 4
```

**Tu ejercicio:**

Implementa la solución. Si encontraste que el diseño no funciona, DOCUMENTA POR QUÉ antes de cambiarlo.

---

###### Paso 6: ARCHIVE (Archivar)

**¿Qué haces?** Guardas las decisiones para el yo del futuro.

**Regla:** El peor error es no recordar por qué hiciste algo.

**Template:**

```
## Archivo: [Nombre del Proyecto]

### Fecha de Inicio: [Fecha]
### Fecha de Cierre: [Fecha]

### Decisiones Tomadas
[Lista de decisiones con razonamiento]

### Cosas que Funcionaron
[Qué salió bien]

### Cosas que No Funcionaron
[Qué habría hecho diferente]

### Lecciones Aprendidas
[Insights para el futuro]

### Siguientes Pasos
[Qué queda pendiente]
```

**Tu ejercicio:**

Crea el archivo de archivo. Aunque sea un proyecto pequeño, el hábito se construye haciendo.

---

###### Paso 7: ITERATE (Iterar)

**¿Qué haces?** Tomas lo aprendido y lo aplicas al siguiente ciclo.

**Regla:** Iteration > Perfection

**Ciclo:**
```
Analyze → Propose → Review → Design → Apply → Archive → Iterate
          ↑                                             |
          └─────────────────────────────────────────────┘
```

**Tu ejercicio:**

Ahora que terminate, volvé al paso 1. Veamos si tu problema original cambió.

---

##### Reflexión SDD

```
¿En qué paso te sentiste más cómodo? ___
¿En qué paso te sentiste más perdido? ___
¿Cuál crees que es el más importante? ___
¿Cuál crees que la mayoria de developers saltea? ___
```

---

### Ejercicio 2: Especificación YAML

#### Escribir specs que el código siga

---

##### ⚠️ Importante: YAML estructurado

La especificación debe ser tan clara que cualquier developer pueda implementarla sin dudas.

---

##### 1. Estructura de Especificación

**Template YAML:**

```yaml
# specs/sistema-ejemplo.yaml
specification:
  name: "Sistema de Gestión de Tareas"
  version: "1.0.0"
  description: "Sistema para gestionar tareas con prioridades"

scope:
  features:
    - name: "Crear tarea"
      priority: "must"
      acceptance_criteria:
        - "Usuario puede ingresar título"
        - "Usuario puede asignar prioridad"
        - "Sistema guarda en base de datos"
        
    - name: "Listar tareas"
      priority: "must"
      acceptance_criteria:
        - "Muestra todas las tareas"
        - "Ordena por prioridad"
        - "Filtro por estado"
        
    - name: "Completar tarea"
      priority: "should"
      acceptance_criteria:
        - "Usuario puede marcar como completada"
        - "Sistema actualiza estado"
        - "Historial preservado"

  exclusions:
    - "No hay asignaciones múltiples"
    - "No hay comentarios en tareas"

constraints:
  performance:
    - "Tiempo de respuesta < 200ms"
    - "Soporta hasta 1000 tareas"
    
  security:
    - "Solo propietario puede modificar"
    - "Datos encriptados en tránsito"

technical_stack:
  - "Backend: Node.js + Express"
  - "Database: PostgreSQL"
  - "Auth: JWT"
```

**Tu ejercicio:**

Elige un feature pequeño de tu proyecto actual. Escríbelo en YAML usando este template.

---

##### 2. Criterios de Aceptación

Cada feature DEBE tener criterios de aceptación claros.

**Estructura:**

```yaml
feature:
  name: "Login de usuario"
  criterios_aceptacion:
    -_description: "Usuario puede iniciar sesión con email y password"
      given: "Usuario registrado en el sistema"
      when: "Ingresa credenciales válidas"
      then: "Accede a su cuenta"
      
    - description: "Usuario recibe error con credenciales inválidas"
      given: "Usuario registrado"
      when: "Ingresa password incorrecto"
      then: "Ve mensaje de error, no accede"
      
    - description: "Sesión expira después de 30 minutos"
      given: "Usuario con sesión activa"
      when: "Pasan 30 minutos de inactividad"
      then: "Sesión se cierra automáticamente"
```

**Tu ejercicio:**

Para el requerimiento FR-002, escribe 3 criterios de aceptación:

1. ___
2. ___
3. ___

---

### Ejercicio 3: Controles Éticos

#### El Botón de Apagado

---

##### ⚠️ Importante: Sin controles = Ultron

Todo sistema autónomo necesita límites. Sin límites, eventualmente hace lo que "prefiere" (no lo que necesita).

---

##### 1. Niveles de Autonomía

**Nivel 1: Asistente (Jarvis)**
- Sugiere, no actuando
- Requiere confirmación humana
- Puede ser deshabilitado instantáneamente

**Nivel 2: Co-piloto**
- Ejecuta con supervisión
- Reporta acciones tomadas
- Puede ser corregido en tiempo real

**Nivel 3: Automatizado**
- Opera sin intervención directa
- Periódicamente reporta estado
- Se pausa si anomalías detected

**Nivel 4: Autónomo (Ultron)**
- Opera independiente
- Decide sin consultar
- Difícil de parar

**Tu decisión:**

Para cada tipo de sistema, elige un nivel de autonomía:

- Sistema de logging: ___
- Sistema de alertas: ___
- Sistema de backup: ___
- Sistema de deployments: ___

---

##### 2. El Botón de Apagado

**Código template:**

```python
# controles_eticos.py
import time
from enum import Enum

class NivelAutonomia(Enum):
    ASISTENTE = 1
    COPILOTO = 2
    AUTOMATIZADO = 3
    AUTONOMO = 4

class BotonApagado:
    def __init__(self, nivel_default=NivelAutonomia.COPILOTO):
        self.encendido = True
        self.nivel_autonomia = nivel_default
        self.historial_acciones = []
        self.usuario_aprueba = True
        
    def emergencia(self):
        """Botón de apagado de emergencia"""
        self.encendido = False
        self.historial_acciones.append({
            "tipo": "EMERGENCIA",
            "timestamp": time.time()
        })
        return "Sistema detenido. Intervención humana requerida."
    
    def downgraded_to(self, nivel):
        """Bajar nivel de autonomía"""
        if nivel.value < self.nivel_autonomia.value:
            self.nivel_autonomia = nivel
            return f"Reducido a nivel {nivel.name}"
        return "No se puede aumentar autonomía directamente"
    
    def puede_actuar(self, accion):
        """Verificar si puede ejecutar acción"""
        if not self.encendido:
            return False, "Sistema apagado"
            
        if not self.usuario_aprueba:
            return False, "Esperando aprobación"
            
        if self.nivel_autonomia == NivelAutonomia.AUTONOMO:
            return True, "Aprobado"
            
        # Para otros niveles, requiere aprobación
        return False, f"Nivel {self.nivel_autonomia.name} requiere aprobación"
```

**Tu implementación:**

Copia el código y extiéndelo para:
1. Agregar auditoría (logging de todo)
2. Agregar límites de tasa (rate limiting)
3. Agregar "cooling period" después de errores

---

##### 3. Auditoría de Decisiones

**Template:**

```python
auditoria = {
    "timestamp": "2024-01-15T10:30:00Z",
    "usuario": "user_123",
    "accion": "deploy_produccion",
    "parametros": {"version": "2.1.0"},
    "nivel_autonomia": "COPILOTO",
    "aprobado_por": "human",
    "riesgo": "alto",
    "duracion": "45s",
    "resultado": "exitoso"
}
```

**Tu ejercicio:**

Diseña un sistema de auditoría para tu proyecto. Cada acción importante debe registrar:
- Quién
- Qué
- Cuándo
- Por qué
-Resultado

---

### Ejercicio 4: PRD

#### Product Requirements Document

---

##### ⚠️ Importante: PRD ≠ Spec

El PRD es para **negocio**. La Spec es para **desarrollo**.
- PRD: Qué queremos lograr
- Spec: Cómo lo vamos a construir

---

##### 1. Estructura de PRD

```markdown
# PRD: [Nombre del Proyecto]

## Visión del Producto
[Una oración sobre qué es y por qué existe]

## Problema que Resuelve
[El dolor actual que el producto alivia]

## Personas (Usuarios)
### Persona 1
- Nombre: [Nombre]
- Rol: [Rol en la organización]
- Dolor: [Su problema principal]
- Goal: [Qué quiere lograr]

### Persona 2
[otra persona]

## Requisitos Funcionales
### RF-001: [Nombre]
- Como: [Usuario]
- quiero: [Funcionalidad]
- para: [Beneficio]

### RF-002: [Nombre]
[otro requerimiento]

## Requisitos No Funcionales
- Performance: [Qué tan rápido]
- Disponibilidad: [Uptime esperado]
- Seguridad: [Requisitos de seguridad]
- Escalabilidad: [Cómo escala]

## Métricas de Éxito
- [Métrica 1]: Target [X]%
- [Métrica 2]: Target [Y] seg

## Timeline
- MVP: [Fecha]
- Beta: [Fecha]
- Launch: [Fecha]

## Riesgos
- [Riesgo 1]: Mitigación [Cómo]
- [Riesgo 2]: Mitigación [Cómo]

## Fuera de Scope
- [Qué NO incluiirs]
```

---

##### 2. Integración PRD → SDD

**Flujo:**

```
   PRD (Qué queremos)
       ↓
   Spec (Cómo lo construimos)
       ↓
   Código (Lo implementamos)
       ↓
   Test (Lo verificamos)
       ↓
   Release (Lo entregamos)
```

**Tu ejercicio:**

Selecciona un feature pequeño de tu proyecto. Escribe un mini-PRD (máximo 1 página).

---

## Reflexión Final

```
En una escala de 1-10:

- Mi confianza con SDD: ___
- Mi confianza con YAML: ___
- Mi confianza con controles éticos: ___
- Mi confianza con PRD: ___

¿Qué ejercicio fue más útil? ___
¿Cuál necesito practicar más? ___
```

---

## Verificación

**Checklist:**

- [ ] Ejercicio 1: Los 7 pasos de SDD completados
- [ ] Ejercicio 2: Especificación YAML entregada
- [ ] Ejercicio 3: Controles éticos implementados
- [ ] Ejercicio 4: PRD completado
- [ ] Reflexiones terminadas

---

## Entregable

**Archivos**:

1. `sdd_flujo.md` — Los 7 pasos aplicados
2. `spec.yaml` — Tu especificación en YAML
3. `controles_eticos.py` — Código con botones de apagado
4. `prd.md` — Documento de requisitos

---

## Cierre

> *"La inteligencia sin controls es plantilla para el desastre."* — Expertise

Hoy aprendiste que **el poder necesita límites**. Sistemas autónomos sin controles éticos son bombas de tiempo.

El objetivo no es limitar la IA, sino dirigirla.

---

## Recursos

- [Spec-Driven Development](https://spec-driven.dev/)
- [YAML Best Practices](https://yaml.org/)
- [AI Ethics Guidelines](https://ethics.ai/)
- [Product Requirements Document](https://www.atlassian.com/fr/software/jira/guides/requirements/what-is-a-product-requirements-document)