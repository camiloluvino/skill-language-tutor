# Language Tutor — Skill

| Metadato | Valor |
| :--- | :--- |
| **Versión** | `v1.1.0` |
| **Fecha de corte** | 2026-11-03 |
| **Plataforma activa** | **Google Antigravity** / **Gemini CLI** / **Claude** |
| **Estado** | Activa en producción local |

> **Nota de diseño:** Skill universal y agnóstica al idioma para el aprendizaje y perfeccionamiento de lenguas mediante conversación (optimizada para entrada por dictado de voz / *Speech-to-Text*), combinando inmersión adaptativa por nivel CEFR (`A0` a `C2`), doble filtro de corrección y módulos bajo demanda de Síntesis y Práctica Deliberada.

---

## Capacidades Principales

- **Arquitectura Agnóstica al Idioma y Adaptativa por Nivel (CEFR `A0` a `C2`):**
  - **Nivel `A0–A1` (Arranque desde cero):** Andamiaje bilingüe, aprovechamiento de intercomprensión (puentes entre lenguas romances/germánicas) y plantillas de respuesta al final de cada turno.
  - **Nivel `A2–B1` (Consolidación):** Inmersión 100% en lengua meta, foco morfológico/sintáctico y erradicación de calcos literales.
  - **Nivel `B2–C2` (Perfeccionamiento):** Refinamiento estilístico hacia fluidez nativa, colocaciones precisas, *phrasal verbs* y matices de registro.
- **Protocolo Especializado para Dictado por Voz (*Voice-to-Text*):**
  - *Silent Correction:* Ignora la falta de puntuación y mayúsculas en la lista de errores, pero las restaura visualmente en la *Versión Corregida*.
  - *Diagnóstico Fonético:* Detecta homófonos transcritos erróneamente por el micrófono y los convierte en alertas de pronunciación.
  - *Rescate Léxico en Vivo (Code-Switching):* Permite insertar palabras o dudas en el idioma materno sin romper el flujo oral, resolviéndolas e integrándolas en la cosecha de vocabulario.
- **Ciclo Pedagógico en Tres Modos:**
  1. **Modo Conversación (Por defecto):** Respuesta cuatripartita (*Error Correction*, *Corrected Version*, *Improvement Suggestion*, *Complete Response*) con cero emojis.
  2. **Modo Síntesis (A demanda):** Detección de patrones crónicos de error, cosecha de vocabulario (*Vocabulary Harvest*), evaluación comunicativa y gancho hacia la práctica.
  3. **Modo Práctica (A demanda):** Generación de 3 ejercicios contextuales (*Contextual Drills*) basados estrictamente en los errores y temas de la sesión.

## Estructura de la Skill

- `SKILL.md`: Especificación completa del protocolo pedagógico, matriz de calibración CEFR y reglas de interacción.

## Instalación en Antigravity

Clona este repositorio directamente en tu directorio global de skills:

```bash
git clone https://github.com/camiloluvino/skill-language-tutor.git ~/.gemini/config/skills/language-tutor
```
