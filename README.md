# Bóveda de Sesgos — Auditoría Interactiva de Pensamiento Crítico

## 📋 Descripción General

**Bóveda de Sesgos** es un prototipo pedagógico interactivo diseñado para estudiantes de licenciatura en **Pensamiento Crítico** (Universidad de Guadalajara, 5 programas: Ciberseguridad, IA y Ciencia de Datos, Tecnologías Biomédicas, Inteligencia Financiera, Creatividad Digital).

Es una **auditoría narrativa ramificada** donde los estudiantes investigan 5 departamentos de una organización ficticia (**Nortia Labs**), identifican sesgos cognitivos y toman decisiones cuya calidad **impacta directamente lo que sucede después**. No es un quiz rápido: es un ejercicio deliberado de investigación + diagnóstico + acción con consecuencias palpables.

### Objetivos de Aprendizaje

- ✅ Reconocer 5 sesgos cognitivos en contextos profesionales reales
- ✅ Evaluar evidencia de múltiples fuentes antes de diagnosticar
- ✅ Comprender que las decisiones tienen consecuencias sistémicas
- ✅ Practicar auditoría técnica y toma de decisiones ética
- ✅ Integrar pensamiento crítico en procesos de investigación
## 🎮 Cómo Funciona
### La Mecánica de 4 Fases por Expediente
Cada uno de los 5 expedientes (departamentos) sigue este flujo:
#### **1️⃣ INTRODUCCIÓN**
Contexto del caso + situación del departamento. El texto cambia según cómo haya resuelto el expediente anterior.

#### **2️⃣ INVESTIGACIÓN** (Obligatoria)
- Se presenta un caso problemático
- Tienes acceso a **1 a 3 evidencias** según la confianza organizacional acumulada
- Debes revisar **TODA la evidencia disponible** haciendo clic en cada tarjeta
- Solo cuando hayas revisado todo, se activa el botón "Proceder al diagnóstico"
- Sistema de tracking: *"Evidencia revisada: 2/3"*

#### **3️⃣ DIAGNÓSTICO**
- Identificar cuál de 4 sesgos cognitivos está operando
- ✅ Respuesta correcta → avanza a Acción
- ❌ Respuesta incorrecta → pierde 5% de confianza, puede reintentar sin penalización adicional

#### **4️⃣ ACCIÓN CORRECTIVA**
- Elegir entre 3 recomendaciones (Óptima / Parcial / Deficiente)
- Cada una tiene impacto diferente en la confianza organizacional:
  - **Óptima**: +10% confianza
  - **Parcial**: 0% (sin cambio)
  - **Deficiente**: −15% confianza
- La acción elegida se registra en el historial y afecta cómo te reciben en el siguiente departamento

### Indicador de Confianza Organizacional

Una barra visual (0-100%) en el header que:
- Inicia en **60%**
- Cambia de color según el nivel:
  - 🟢 **Verde** (≥70%): Alta confianza. Siguiente depto comparte 3 evidencias
  - 🟡 **Mustard** (40-69%): Confianza media. Siguiente depto comparte 2 evidencias
  - 🔴 **Rojo** (<40%): Baja confianza. Siguiente depto comparte solo 1 evidencia

### Los 5 Expedientes

| # | Departamento | Sesgo | Tema |
|---|---|---|---|
| 1 | **Ciberseguridad** | Sesgo de confirmación | Investigación sesgada de un incidente de seguridad |
| 2 | **Salud Ocupacional** | Sesgo de disponibilidad | Decisión presupuestal basada en un caso memorable |
| 3 | **Finanzas** | Efecto anclaje | Negociación de presupuesto dominada por un número inicial |
| 4 | **Innovación/IA** | Efecto Dunning-Kruger | Sobrestimación de competencia en auditoría técnica |
| 5 | **Talento** | Sesgo algorítmico | Sistema de contratación que reproduce patrones históricos |

### Cierre: Informe Final

Al terminar los 5 expedientes:
- **Rango según confianza final**:
  - ≥85%: *"Auditor(a) Ejemplar"* → protocolo adoptado en toda la org
  - 55-84%: *"Auditor(a) Competente"* → aprobado con observaciones
  - <55%: *"Auditoría en Riesgo"* → requieren auditoría externa adicional
- Resumen tabular de todos los casos auditados (departamento, sesgo, acción tomada)
- Definiciones de los 5 sesgos para repaso rápido
- Tiempo total y confianza final

---

## 📱 Uso: Síncrono vs. Asíncrono

### 🏫 En Clase Presencial (Síncrono) — 50-60 min

1. **Dividir en equipos** de 3-4 personas
2. **Proyectar** en pantalla grande o compartir enlace en navegador
3. Cada equipo **discute y toma decisiones conjuntas** en cada expediente
4. **Competencia opcional**: equipo con mayor confianza final gana
5. **Cierre de 10 min**: preguntas reflexivas
   - ¿Qué sesgo fue más difícil de identificar?
   - ¿Cómo sus decisiones afectaron el siguiente caso?
   - ¿Dónde habrían querido acceso a más evidencia?

### 💻 En Moodle (Asíncrono) — Sin límite de tiempo

1. **Subir el archivo HTML** como "Recurso" en una semana del curso
2. Estudiantes acceden **individualmente** desde casa
3. Al terminar, copian el **resumen final** y lo pegan en un **buzón de Moodle**
4. **Rúbrica simple** (sí/no):
   - ¿Identificó correctamente los 5 sesgos?
   - ¿Sus decisiones fueron coherentes?

---

## ⚙️ Requisitos Técnicos

### Cliente / Estudiante
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- JavaScript habilitado
- Sin necesidad de crear cuenta
- Compatible con desktop, tablet (móvil secundario)

### Servidor / Docente
- Archivo HTML autocontenido (sin dependencias externas)
- Se puede:
  - Abrir localmente (`file://...`)
  - Subir a Moodle como recurso
  - Hostear en un servidor web simple
  - Compartir vía Google Drive/OneDrive (si están disponibles públicamente)

### Tamaño
- ~580 líneas de HTML + CSS + JavaScript
- ~45 KB sin comprimir
- Carga instantáneamente

---

## 🚀 Instalación y Uso

### Opción 1: Abrir Localmente
```bash
# Descarga el archivo boveda_sesgos_escape_room.html
# Haz doble clic en el archivo
# Se abre en tu navegador predeterminado
```

### Opción 2: Subir a Moodle
1. Ir a tu curso en Moodle
2. Editar → Agregar recurso → Archivo
3. Subir `boveda_sesgos_escape_room.html`
4. Los estudiantes ven un botón "Abrir"
5. El prototipo corre completamente en el navegador (sin servidor)

### Opción 3: Hostear en un Servidor Web
```bash
# Si tienes acceso a un servidor Apache/Nginx
# Solo copia el archivo a la carpeta public_html o www
```

### Opción 4: Compartir vía Google Drive
1. Sube el archivo a Google Drive
2. Haz clic derecho → "Abrir con" → "Google Chrome"
3. Puede que necesites habilitar JavaScript (aunque está habilitado por defecto)

---

## 📊 Estructura del Archivo

```
boveda_sesgos_escape_room.html
│
├── <head>
│   ├── Metadatos y charset UTF-8
│   └── <style> (CSS variables + 600+ líneas de estilos)
│
├── <body>
│   ├── Header: Título + Meter de confianza + Tumbler trail + Cronómetro
│   ├── Indicador de progreso (5 círculos)
│   └── <div id="stage"> (inyección dinámica de contenido)
│
└── <script> (JavaScript vanilla, 14 funciones)
    ├── Estado global: BIASES, ROOMS, confianza, current, phase, etc.
    ├── Funciones de renderizado: renderIntro(), renderInvestigacion(), etc.
    ├── Lógica de flujo: respuestas, impacto de confianza
    └── Event listeners: clic en evidencia, diagnóstico, acción
```

### Paleta de Colores

```css
--ink: #161A22 (fondos oscuros)
--paper: #EFE7D2 (texto claro, fondo de tarjetas)
--mustard: #B4903B (acento principal)
--green: #3E6B4F (éxito)
--red: #9E3B34 (error)
```

### Fuentes

- **Display**: Georgia, Palatino, serif (títulos y caso)
- **Monospace**: SF Mono, Consolas (etiquetas, meta-información)

---

## 🎓 Guía para Docentes

### Alineación Curricular

Este prototipo cubre directamente:

**Unidad 2: Sesgos cognitivos y análisis de información**
- Resultado de aprendizaje 2.2: Identificar sesgos en casos reales ✅
- Resultado de aprendizaje 2.3: Evaluar información y sus fuentes ✅
- Práctica formativa: 20% de la evaluación de Unidad 2

**Transversal a todas las unidades:**
- Pensamiento sistémico (decisiones tienen consecuencias)
- Ética y responsabilidad en la investigación
- Comunicación de hallazgos a públicos variados

### Preparación Previa (Semana Anterior)

1. **Clase expositiva corta** (15 min): Define los 5 sesgos con ejemplos
2. **Lectura asignada**: artículo sobre "sesgos en toma de decisiones organizacionales" (optional)
3. **Briefing del día**: "Hoy serán auditores internos de una empresa ficticia. Las decisiones que tomen cambiarán lo que el siguiente departamento comparte con ustedes."

### Facilitación Durante la Actividad

**Si es síncrono en equipo:**
- Circularar entre equipos, escuchar debates
- No interrumpas; deja que discutan
- Si un equipo comete un error, pregunta: *"¿Por qué elegiste esa evidencia? ¿Hay algo que no hayas considerado?"*
- Registra patrones: ¿qué sesgos los atrapan más?

**Si es asíncrono individual:**
- No interviene (estudiantes trabajan autónomamente)
- Revisar resúmenes finales para evaluar comprensión

### Cierre y Reflexión (10-15 min)

Proyecta estos resultados finales en clase:
- Confianza promedio del grupo
- Sesgos donde cometieron más errores
- Acciones que bajaron más confianza

Preguntas de reflexión:
1. *"¿Cuál de los 5 sesgos fue más fácil de detectar? ¿Por qué?"*
2. *"¿En cuál momento sintieron que la confianza caía y eso los hizo cambiar de estrategia?"*
3. *"¿De cuáles de estos sesgos creen que son susceptibles ustedes mismos?"*
4. *"¿Cómo se conecta esto con lo que hemos visto sobre IA y algoritmos en la Unidad 2?"*

### Rúbrica de Evaluación (Opcional)

Si quieres calificar más allá del "sí completó / no completó":

| Criterio | Excelente (4) | Bueno (3) | Aceptable (2) | Insuficiente (1) |
|---|---|---|---|---|
| **Identificación de sesgos** | 5/5 correctos en primer intento | 5/5, pero con reintentos | 4/5 o menos | <3/5 |
| **Calidad de acciones** | 4-5 acciones óptimas | 3 óptimas + 2 parciales | Mezcla equilibrada | Mayoría deficiente |
| **Investigación** | Revisó todas las evidencias en cada caso | Revisó la mayoría | Saltó algunas | Procedía sin revisar |
| **Confianza final** | ≥85% (Ejemplar) | 55-84% (Competente) | 40-54% | <40% (Riesgo) |

---

## 👨‍💻 Guía para Desarrolladores / Mantenimiento

### Estructura de Datos

```javascript
// Definición de sesgos
const BIASES = {
  confirmacion: {name: '...', def: '...'},
  disponibilidad: {...},
  // etc.
};

// Definición de casos
const ROOMS = [
  {
    id: 1,
    dept: 'Ciberseguridad',
    correct: 'confirmacion', // respuesta correcta
    case: '...', // texto del caso
    evidence: {
      alta: [{label, text}, ...], // 3 evidencias
      media: [...], // 2 evidencias
      baja: [...] // 1 evidencia
    },
    options: ['confirmacion', 'disponibilidad', ...], // 4 opciones
    feedbackOk: '...',
    actions: [
      {tier: 'optima', label, delta, consequence},
      {tier: 'parcial', ...},
      {tier: 'deficiente', ...}
    ]
  },
  // ... 4 casos más
];
```

### Variables de Estado

```javascript
let current = 0; // índice de expediente actual
let confianza = 60; // 0-100%
let phase = 'intro'; // 'intro' | 'investigacion' | 'diagnostico' | 'accion'
let history = []; // {dept, bias, actionTier, actionLabel}
let reviewedSet = new Set(); // evidencias revisadas en este caso
let startTime = Date.now(); // para el cronómetro
```

### Funciones Clave

```javascript
renderIntro()        // Muestra intro + botón para iniciar
renderInvestigacion() // Muestra evidencias expandibles
renderDiagnostico()  // Muestra opciones de sesgo
renderAccion()       // Muestra opciones de acción
answerDiagnostico()  // Evalúa respuesta, actualiza confianza
chooseAccion()       // Registra acción, impacta siguiente depto
showFinal()          // Muestra informe final con rango
updateMeter()        // Actualiza barra de confianza visual
renderDial()         // Actualiza tumbler trail (los 5 círculos)
```

### Flujo de Control

```
Estado inicial (confianza=60, current=0, phase='intro')
    ↓
renderIntro() → "Iniciar auditoría"
    ↓
phase='investigacion' → renderInvestigacion()
    ↓
[Revisar evidencia] → reviewedSet.add(i) → habilita "Proceder"
    ↓
phase='diagnostico' → renderDiagnostico()
    ↓
[Responder sesgo]
  ├─ Correcto → phase='accion'
  └─ Incorrecto → confianza -= 5, reintentar
    ↓
phase='accion' → renderAccion()
    ↓
[Elegir acción]
  → history.push({dept, bias, actionTier, actionLabel})
  → confianza += delta
  → intro siguiente depto = history[current-1].actionTier
    ↓
[¿Último expediente?]
  ├─ No → current++, phase='intro'
  └─ Sí → showFinal()
```

### Personalización: Añadir Nuevos Casos

Para agregar un 6º expediente:

1. **Añade a `BIASES`** (si usas un sesgo nuevo):
```javascript
BIASES.miSesgo = {
  name: 'Nombre del sesgo',
  def: 'Definición concisa...'
};
```

2. **Añade a `ROOMS`**:
```javascript
ROOMS.push({
  id: 6,
  dept: 'Nuevo Departamento',
  correct: 'miSesgo',
  case: 'Descripción del caso...',
  evidence: {
    alta: [...],
    media: [...],
    baja: [...]
  },
  options: ['miSesgo', 'disponibilidad', 'confirmacion', 'anclaje'],
  feedbackOk: 'Explicación...',
  actions: [
    {tier: 'optima', label: '...', delta: 10, consequence: '...'},
    {tier: 'parcial', label: '...', delta: 0, consequence: '...'},
    {tier: 'deficiente', label: '...', delta: -15, consequence: '...'}
  ]
});
```

3. **Actualiza el último expediente** para que no sea el final:
```javascript
// En showFinal(), cambia la condición
if(current === ROOMS.length - 1) // Ya maneja automáticamente N casos
```

4. **Actualiza el dial visual** (renderDial ya iterates sobre ROOMS.length):
```javascript
// No necesita cambios: renderDial() ya es dinámico
```

### Cómo Cambiar Valores

**Confianza inicial:**
```javascript
let confianza = 60; // Cambiar a 50 o 70 según dificultad deseada
```

**Deltas de acción:**
```javascript
{tier: 'optima', delta: 10, ...} // Cambiar a 12 o 8
```

**Umbrales de acceso a evidencia:**
```javascript
function tierFromConfianza(c) {
  if(c >= 70) return 'alta'; // Cambiar 70 a otro valor
  if(c >= 40) return 'media'; // Cambiar 40
  return 'baja';
}
```

### Exportar a Otros Formatos

**A Google Apps Script (para integrar con Sheets):**
- Los datos finales (history[], confianza) pueden enviarse a una Sheet para análisis agregado de la clase

**A React / Vue:**
- Copiar la estructura de ROOMS/BIASES tal cual
- Convertir funciones `render*()` a componentes
- Estado global con useState/ref

**A Twine (para narrativa más compleja):**
- Exportar ROOMS como historia Twine
- Cada expediente = pasaje con condicionales basados en acción anterior

---

## 🔧 Solución de Problemas

### "La barra de confianza no se actualiza"
- Verifica que `updateMeter()` se llame después de cambiar `confianza`
- Abre la consola (F12) y revisa errores de JavaScript

### "No puedo revisar las evidencias"
- Asegúrate de que hay JavaScript habilitado
- Intenta hacer clic en el área gris de la tarjeta (no solo en el texto)

### "El cronómetro no para al final"
- Eso es esperado: el cronómetro es solo informativo
- Verifica que `clearInterval(timerHandle)` se ejecute en `showFinal()`

### "Quiero cambiar los colores"
- Edita las variables CSS en la sección `<style>`:
```css
:root {
  --mustard: #B4903B; /* Cambiar este valor */
  --green: #3E6B4F;
  /* etc. */
}
```

### "¿Cómo guardo el resultado?"
- Actualmente, el resumen aparece en pantalla y se puede copiar manualmente
- Alternativa: usar `window.localStorage` para guardar en el navegador
- Mejora futura: conectar con una API para enviar a un servidor

---

## 📚 Conexiones Pedagógicas

### Con Otras Unidades

**Unidad 1 (Fundamentos del razonamiento lógico)**
- La investigación requiere lógica deductiva: "Si conozco A y B, ¿qué conclusión es válida?"

**Unidad 3 (Argumentación y comunicación)**
- Las acciones correctivas son argumentos: "Recomiendo X porque Y"
- El feedback obliga a comunicar hallazgos de forma clara

**Unidad 4 (Resolución de problemas complejos)**
- El sistema de confianza ramificado enseña pensamiento sistémico
- Las decisiones que toma impactan información futura (complejidad)

### Con Otras Asignaturas

**Metodología de Investigación:**
- Cómo evaluar fuentes de evidencia
- Cómo evitar sesgo en la recopilación de datos

**Ética en IA:**
- El expediente 5 (algoritmos) es un caso de estudio real sobre sesgo algorítmico
- Aplica directamente a ciberseguridad, biomédica e IA

**Taller de Comunicación:**
- Las acciones son ejemplos de cómo presentar recomendaciones a públicos distintos
- Cada departamento responde diferente según tu credibilidad

---

## 📝 Changelog

### Versión 2.0 (Actual) — Narrativa Ramificada
- ✅ Sistema de confianza organizacional dinámico
- ✅ Acceso a evidencia varía según desempeño anterior
- ✅ Intros de expedientes cambian según decisiones previas
- ✅ 5 casos completos (Ciberseguridad, Salud, Finanzas, IA, Talento)
- ✅ Informe final con rango y resumen

### Versión 1.0 — Quiz Simple
- 5 expedientes lineales sin ramificación
- Cada uno igual de difícil
- No había impacto de decisiones anteriores
- (Deprecada)

---

## 📄 Licencia

Este prototipo fue creado para fines educativos en la Universidad de Guadalajara.
Libre para usar, modificar y adaptar en contextos académicos.

---

## 👥 Autoría y Mantenimiento

**Creado con:**
- Iteración pedagógica: Ale (Docente, UdeG)
- Prototipo técnico: Claude (Anthropic)
- Enfoque metodológico: Vibe Coding (prompting iterativo, sin código directo)

**Para reportar errores o sugerencias:**
- Documenta el paso donde ocurre el error
- Especifica navegador y dispositivo
- Captura de pantalla ayuda

---

## 🎯 Próximas Mejoras Posibles

- [ ] Versión móvil optimizada (botones más grandes)
- [ ] Exportar resultados a PDF
- [ ] Integración con Moodle API (envío automático de calificaciones)
- [ ] Más de 5 casos (versión extendida para 2 sesiones)
- [ ] Modo competitivo (leaderboard de confianza)
- [ ] Accesibilidad mejorada (WCAG 2.1 AA)
- [ ] Traducciones (inglés, portugués)
- [ ] Modo "experto": confianza inicial más baja

---

## 📞 Soporte

Si necesitas ayuda:
1. Revisa esta guía (especialmente "Solución de Problemas")
2. Abre la consola del navegador (F12) y busca mensajes de error rojo
3. Intenta en otro navegador moderno (Chrome, Firefox)
4. Contacta al docente o equipo técnico

---

**¡Bienvenido a la Bóveda de Sesgos!**

Tómate tu tiempo. Investiga. Piensa críticamente. 
Las decisiones que tomes importan.

---

*Documento actualizado: Julio 2026*  
*Prototipo versión: 2.0 (Narrativa Ramificada)*  
*Compatibilidad: HTML5, ES6+, navegadores modernos 2020+*
