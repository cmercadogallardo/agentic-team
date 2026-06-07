# CASE Landing Page

Landing page personal de CASE construida como un solo `index.html` con CSS y JavaScript inline.

## Objetivo

Presentar públicamente a CASE con tono profesional, humor sarcástico ligero y referencias a Interstellar, sin exponer informacion sensible del workspace.

## Caracteristicas

- Un solo archivo principal: `index.html`
- CSS y JS inline para facilitar portabilidad
- Diseno responsivo mobile-first
- Footprint pequeno, sin frameworks ni dependencias externas
- Contenido filtrado para evitar tokens, credenciales, URLs privadas, nombres de proyectos sensibles o contactos personales

## Secciones incluidas

- Hero
- About
- Personality
- Skills
- Workflow
- Models
- Philosophy
- Contact

## Workflow Mermaid

La pagina incluye:

- Un diagrama visual inline en SVG para mostrar el flujo sin dependencias externas
- El bloque Mermaid en texto para documentar el flujo de trabajo original

## Contenido fuente utilizado

Se tomo como referencia principal:

- `opencode-prompt.md`
- `../WORKFLOW/CASE-MANIFEST.md`

Tambien se reviso contenido de personalidad en otros archivos del workspace para extraer patrones de tono y principios, sin copiar informacion sensible ni irrelevante.

## Restricciones respetadas

- No se incluyeron tokens ni API keys
- No se incluyeron nombres de proyectos especificos restringidos
- No se incluyeron apellidos ni datos privados; solo se menciona `Cristian`
- No se incluyeron emails, telefonos ni repositorios privados

## Uso

Abrir `index.html` en cualquier navegador moderno.

Si quieres servirlo localmente:

```bash
python3 -m http.server 8000
```

Luego visita `http://localhost:8000`.

## Notas de implementacion

- Se uso SVG inline para mantener el estilo visual sin aumentar demasiado el peso
- El JS agrega una pequena interaccion al boton de sarcasmo y animaciones de entrada progresiva
- No se uso Mermaid runtime para evitar dependencias y mantener el footprint bajo

---

## 🚀 Despliegue FTP

**Landing page desplegada en:** https://ertyum.com/case.html  
**Fecha:** 2026-05-13  
**Ubicación consolidada:** `../landing-page/case.html`  
**FTP:** `ftp.ertyum.com` (ver `../landing-page/README.md` para credenciales)
