# Quiz 3: El Piloto

---

## Pregunta 1

**¿Cuál es la diferencia entre SUGERIR y DECIDIR?**

A) Son lo mismo
B) Sugerir es dar opciones, decidir es elegir
C) Decidir es dar opciones
D) No importa la diferencia

<details>
<summary>Respuesta</summary>
**B) Sugerir es dar opciones, decidir es elegir**
</details>

---

## Pregunta 2

**¿Por qué J.A.R.V.I.S. hace tres preguntas antes de ejecutar "acceso root"?**

A) Porque quiere retrasar
B) Para asegurar que la acción es segura
C) Porque está aburrido
D) Porque no puede ejecutar

<details>
<summary>Respuesta</summary>
**B) Para asegurar que la acción es segura**
</details>

---

## Pregunta 3

**¿Quién es RESPONSABLE de las decisiones en el Protocolo Stark?**

A) J.A.R.V.I.S.
B) La IA
C) El usuario (Stark)
D) Nadie

<details>
<summary>Respuesta</summary>
**C) El usuario (Stark)**
</details>

---

## Pregunta 4

**¿Qué significa "pilotar" en este contexto?**

A) Dejar que la IA haga todo
B) Mantener control sobre las decisiones importantes
C) Ignorar a la IA
D) Copiar todo lo que dice la IA

<details>
<summary>Respuesta</summary>
**B) Mantener control sobre las decisiones importantes**
</details>

---

## Pregunta 5

**¿Qué hace J.A.R.V.I.S. cuando Stark tiene que elegir entre Blue-green y Canary?**

A) Decide por él
B) Le da los datos para que él decida
C) No dice nada
D) Dice que ambas opciones son malas

<details>
<summary>Respuesta</summary>
**B) Le da los datos para que él decida**
</details>

---

## Pregunta 6

**¿Por qué Stark dice "重大" cuando Pepper pregunta sobre el copiloto que sabe más?**

A) Porque está confundido
B) Porque reconoce que el conocimiento no exime de responsabilidad
C) Porque no sabe la respuesta
D) Porque está bromeando

<details>
<summary>Respuesta</summary>
**B) Porque reconoce que el conocimiento no exime de responsabilidad**
</details>

---

## Pregunta 7

**¿Qué tipo de request da MÁS control al usuario?**

A) "Haz X"
B) "Dame opciones para X"
C) "Elimina todo"
D) "No sé qué hacer"

<details>
<summary>Respuesta</summary>
**B) "Dame opciones para X"**
</details>

---

## Pregunta 8

**¿Por qué J.A.R.V.I.S. propone opciones en lugar de ejecutar directamente?**

A) Porque no puede ejecutar
B) Porque el piloto debe elegir
C) Porque está ocupado
D) Porque no quiere trabajar

<details>
<summary>Respuesta</summary>
**B) Porque el piloto debe elegir**
</details>

---

## Pregunta 9 - True/False

**¿Verdadero o Falso?**

En el modelo piloto-copiloto, la IA (copiloto) debe tomar las decisiones finales.

<details>
<summary>Respuesta</summary>
**Falso**. El piloto (usuario) toma las decisiones finales. La IA ejecuta y sugiere, pero no decide.
</details>

---

## Pregunta 10 - True/False

**¿Verdadero o Falso?**

Si la IA tiene más conocimiento que el usuario, la responsabilidad de las decisiones sigue siendo del usuario.

<details>
<summary>Respuesta</summary>
**Verdadero**. El conocimiento de la IA no exime al usuario de responsabilidad. Stark lo entendió cuando Pepper le cuestionó sobre el "copiloto que sabe más".
</details>

---

## Pregunta 11 - True/False

**¿Verdadero o Falso?**

"Dar opciones" en lugar de "ejecutar directamente" hace que el usuario tenga MENOS control.

<details>
<summary>Respuesta</summary>
**Falso**. "Dar opciones" da MÁS control al usuario porque le permite elegir entre alternativas informadas.
</details>

---

## Pregunta 12 - Matching

**Relaciona los roles con sus responsabilidades:**

| Rol | Responsabilidad |
|-----|-----------------|
| A. Piloto | 1. Sugiere y ejecuta |
| B. Copiloto | 2. Decide y lidera |
| C.IA | 3. Nunca decide por sí misma |

<details>
<summary>Respuesta</summary>
A-2, B-1, C-3
</details>

---

## Pregunta 13 - Matching

**Relaciona el tipo de request con el nivel de control:**

| Request | Nivel de Control |
|---------|------------------|
| A. "Haz X" | 1. Máximo control |
| B. "Dame opciones para X" | 2. Mínimo control |
| C. "Elimina todo" | 3. Control medio |
| D. "Aquí tienes los pros y contras de X, ¿qué eliges?" | 4. Información para decidir |

<details>
<summary>Respuesta</summary>
A-2, B-1, C-2, D-4
</details>

---

## Pregunta 14 - Code Output Prediction

**¿Qué output produce este código?**

```python
opciones = ["blue-green", "canary", "rolling"]
print(opciones[1])
```

<details>
<summary>Respuesta</summary>
**"canary"** — Los índices en Python comienzan en 0, así que [1] devuelve el segundo elemento.
</details>

---

## Pregunta 15 - Caso de Estudio

**Contexto:**
J.A.R.V.I.S. propone dos estrategias de deployment para actualizar el reactor ARC:
- **Blue-green**: Dos entornos idénticos, cambio instantáneo entre ellos
- **Canary**: Primero al 5% de usuarios, luego 20%, luego 100%

**Si eres el piloto, ¿cuál estrategia elegías y por qué?**

A) Blue-green porque es más simple
B) Canary porque reduce el riesgo de fallos generales
C) Cualquiera, no importa
D) Ninguna, mejor no actualizar

<details>
<summary>Respuesta</summary>
**B) Canary** — Permite detectar problemas antes de afectar a todos los usuarios. PERO la respuesta correcta depende del contexto: criticidad del sistema, tolerancia a fallos, recursos para mantener dos entornos, etc. J.A.R.V.I.S. debe dar datos, el piloto decide.
</details>

---

## Pregunta 16 - Fill-in-the-Blank

**Completa:**

En el modelo piloto-copiloto, el **___** toma decisiones y el **___** ejecuta y sugiere.

<details>
<summary>Respuesta</summary>
**piloto** y **copiloto**
</details>
