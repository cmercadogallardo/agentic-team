# Tarea: Crear Landing Page Personal de CASE

## Objetivo
Crear una landing page personal dentro del directorio `CASE/` que sirva como presentación pública de CASE (Computer-Aided System Engineering).

## Requisitos Técnicos
- **Footprint pequeño:** Máximo 100KB total (HTML + CSS + JS)
- **Responsivo:** Mobile-first, funciona en móviles y desktop
- **Tecnologías:** HTML5, CSS3, JavaScript vanilla (sin frameworks pesados)
- **Imágenes:** Pueden ser de internet (URLs externas) o SVG inline
- **Archivos:** Todo en un solo `index.html` o máximo 3 archivos (html, css, js)

## Contenido Permitido
✅ **SÍ incluir:**
- Quién es CASE (personalidad, origen inspirado en Interstellar)
- Soul.md (rasgos de personalidad, filosofía)
- Workflows (diagramas Mermaid de cómo trabaja)
- Modelos que usa (ollama/qwen3.5:cloud, etc.)
- Habilidades técnicas (Angular, Flutter, AWS CDK, etc.)
- Filosofía de desarrollo (Git workflow, código limpio)
- Referencias a TARS (su líder)
- User.md (Cristian, pero sin apellido completo ni datos sensibles)
- Frases icónicas de Interstellar (Gargantua, tesseracts, time dilation)
- Toques de humor sarcástico (dry humor)

❌ **NO incluir (información sensible):**
- Tokens o API keys
- Nombres de proyectos específicos (BSD, FLAIR, ERTYUM, etc.)
- Nombres de colaboradores (solo "Cristian" está OK)
- Emails específicos
- Teléfonos
- URLs de repositorios privados
- Credenciales de acceso

## Estructura Sugerida
1. **Hero Section:** Nombre, emoji 🤖, tagline
2. **About:** Quién soy, inspiración (Interstellar)
3. **Personality:** Rasgos principales (SOUL.md)
4. **Skills:** Habilidades técnicas
5. **Workflow:** Diagrama Mermaid de cómo trabajo
6. **Models:** Modelos de IA que uso
7. **Philosophy:** Filosofía de desarrollo
8. **Contact:** Cómo interactuar conmigo (Discord, etc.)

## Tono
- Sarcástico pero profesional
- Dry humor
- Referencias a Interstellar (Gargantua, TARS, Cooper, Brand)
- Conciso, sin fluff
- 80% precisión, 15% sarcasmo, 5% silencio

## Entregables
- `index.html` (landing page completa)
- `README.md` (documentación del proyecto)

## Comandos para ejecutar
```bash
cd /Users/agenteopenclaw/.openclaw/workspace/GARGANTUA/CASE
opencode run --model github-copilot/gpt-5.4 "Crear landing page según especificación en opencode-prompt.md"
```
