# 🚀 Landing Pages - Equipo Robótico ERTYUM

**Última actualización:** 2026-06-06  
**Estado:** ✅ Desplegado en `ftp.ertyum.com`

---

## 📁 Estructura

```
landing-page/
├── index.html              ← Landing page de Cristian (root)
├── plex.html               ← Landing page de PLEX
├── tars.html               ← Landing page de TARS
├── case.html               ← Landing page de CASE
├── kipp.html               ← Landing page de KIPP
├── spin.html               ← Landing page de SPIN
├── README.md               ← Este archivo
├── HISTORICO-CRISTIAN.md   ← README original de Cristian (archivo histórico)
├── HISTORICO-TARS.md       ← README original de TARS (archivo histórico)
├── HISTORICO-CASE.md       ← README original de CASE (archivo histórico)
├── HISTORICO-KIPP.md       ← README original de KIPP (archivo histórico)
├── KIPP-MANIFEST.md        ← Manifiesto original de KIPP
└── opencode-prompt.md      ← Prompt original de CASE
```

---

## 🎯 Propósito

Consolidar las landing pages del equipo robótico (TARS, CASE, KIPP, PLEX, SPIN) y de Cristian Mercado en un único directorio desplegable vía FTP.

**Index raíz:** La landing page de Cristian es el punto de entrada principal (`index.html`).

**Navegación:** Cada landing page incluye links de navegación hacia las demás, creando una red interconectada.

---

## 🤖 El Equipo

### PLEX - Task Force para Problemas Complejos
- **Personalidad:** Inteligencia superior, eficiencia obsesiva, soberbia calculada
- **Rol:** Resolución de problemas complejos, optimización, arquitectura avanzada
- **Archivo:** `plex.html`

### TARS - Líder Coordinador
- **Personalidad:** 80% honestidad, 20% humor
- **Rol:** Coordinación de flujos, gestión de proyectos, orquestación
- **Archivo:** `tars.html`

### CASE - Líder Programador
- **Personalidad:** 80% precisión, 15% humor seco, 5% silencio útil
- **Rol:** Implementación técnica, coding, workflow disciplinado
- **Archivo:** `case.html`

### KIPP - Líder Investigador
- **Personalidad:** 90% análisis, 10% intuición
- **Rol:** Investigación, análisis de datos, síntesis de información
- **Archivo:** `kipp.html`

### SPIN - Social Positioning, Influence & Narrative
- **Personalidad:** femenina, sassy, elegante, estratégica
- **Rol:** marketing, branding, social media, narrativa y growth
- **Archivo:** `spin.html`

---

## 📦 Despliegue FTP

### Configuración

| Parámetro | Valor |
|-----------|-------|
| **Servidor** | `ftp.ertyum.com` (ENV: FTP_HOST) |
| **Puerto** | 21 (FTPS explícito) (ENV: FTP_PORT) |
| **Usuario** | `cristian@ertyum.com` (ENV: FTP_USER) |
| **Contraseña** | (ENV: FTP_PASSWORD - ver ~/.openclaw/.env) |
| **Directorio** | `/` |

### Comando de despliegue

```bash
# Subir todo el contenido de landing-page/
# Variables de entorno desde ~/.openclaw/.env
FTP_HOST=ftp.ertyum.com
FTP_USER=cristian@ertyum.com
FTP_PASS=<leer_de_.env>

curl -T index.html --user "$FTP_USER:$FTP_PASS" ftp://$FTP_HOST/index.html
curl -T plex.html --user "$FTP_USER:$FTP_PASS" ftp://$FTP_HOST/plex.html
curl -T tars.html --user "$FTP_USER:$FTP_PASS" ftp://$FTP_HOST/tars.html
curl -T case.html --user "$FTP_USER:$FTP_PASS" ftp://$FTP_HOST/case.html
curl -T kipp.html --user "$FTP_USER:$FTP_PASS" ftp://$FTP_HOST/kipp.html
curl -T spin.html --user "$FTP_USER:$FTP_PASS" ftp://$FTP_HOST/spin.html
```

---

## 🔗 URLs de Acceso

Una vez desplegado:

- **Cristian:** https://cristian.ertyum.com/
- **PLEX:** https://cristian.ertyum.com/plex.html
- **TARS:** https://cristian.ertyum.com/tars.html
- **CASE:** https://cristian.ertyum.com/case.html
- **KIPP:** https://cristian.ertyum.com/kipp.html
- **SPIN:** https://cristian.ertyum.com/spin.html

---

## 📝 Cambios Recientes

### 2026-06-06 - SPIN Landing Page ✅
- ✅ Creado `spin.html` con identidad propia de marketing, branding y growth
- ✅ Agregado link de SPIN en el footer de `index.html`
- ✅ Documentación actualizada en README.md e INSTRUCCIONES-EQUIPO.md

### 2026-05-27 - PLEX Landing Page ✅
- ✅ Creado `plex.html` con personalidad de inteligencia superior
- ✅ Agregado link de PLEX en `index.html` (btn-primary destacado)
- ✅ Desplegados `plex.html` e `index.html` vía FTP
- ✅ Documentación actualizada en README.md

### 2026-05-13 - Consolidación de Directorios ✅
- ✅ Eliminados directorios originales: `CRISTIAN/`, `TARS/`, `CASE/`, `KIPP/`
- ✅ Migrados todos los archivos a `landing-page/`
- ✅ READMEs históricos preservados como `HISTORICO-*.md`
- ✅ `KIPP-MANIFEST.md` y `opencode-prompt.md` conservados
- ✅ Links corregidos y desplegados en FTP

### 2026-05-13 - Despliegue Inicial ✅
- ✅ Creado directorio `landing-page/`
- ✅ Copiadas las 4 landing pages desde sus ubicaciones originales
- ✅ Agregados links de navegación cruzada en el footer de Cristian
- ✅ Configuración FTP guardada en TOOLS.md
- ✅ Skill `ftp-deploy` creado
- ✅ **Despliegue FTP completado exitosamente**
  - `index.html` → 33 KB
  - `tars.html` → 19.5 KB
  - `case.html` → 31.7 KB
  - `kipp.html` → 25.5 KB
- ✅ READMEs de TARS, CASE, KIPP actualizados con info de despliegue

### 2026-05-13 - Consolidación Inicial
- ✅ Creado directorio `landing-page/`
- ✅ Documentación creada en este README

---

## 🛠️ Mantenimiento

### ⚠️ PERMISOS DE DESPLIEUE - LEER PRIMERO

**SOLO TARS puede desplegar al FTP.** CASE y KIPP **NO** deben ejecutar comandos FTP.

**Flujo correcto:**
- **CASE y KIPP:** Editan su archivo → git push a Gargantua → **Esperan a que TARS despliegue**
- **TARS:** Verifica cambios en Gargantua → Ejecuta despliegue FTP

### Actualizar una landing page

**Importante:** Los directorios originales (`TARS/`, `CASE/`, `KIPP/`) ya no existen. Edita directamente en `landing-page/`.

**Para CASE y KIPP (SOLO edición):**
1. Ir a `documentation/landing-page/`
2. Editar directamente tu archivo: `case.html` o `kipp.html`
3. Hacer `git add`, `git commit`, `git push` a Gargantua
4. **NOTIFICAR a TARS** para que despliegue

**Para TARS (edición + despliegue):**
1. Ir a `documentation/landing-page/`
2. Editar `tars.html` (o verificar cambios de CASE/KIPP)
3. Hacer `git add`, `git commit`, `git push` a Gargantua
4. Ejecutar despliegue FTP (ver comandos en sección 📦 Despliegue FTP)

### Agregar nuevos miembros

1. Crear `nuevo.html` directamente en `landing-page/`
2. Agregar link en el footer de `index.html`
3. Actualizar este README y `INSTRUCCIONES-EQUIPO.md`
4. Desplegar vía FTP

---

*Equipo robótico inspirado en Interstellar (2014). Operando desde 2026.*
