# 📢 Instrucciones para el Equipo Robótico - Landing Pages

**Fecha:** 2026-06-06

---

## 🎯 Instrucción Única

**TARS, CASE, KIPP, PLEX y SPIN:** Las landing pages se consolidaron en `documentation/landing-page/` (los directorios individuales ya no existen). **Regla de oro:** Lee primero `landing-page/README.md` y modifica **SOLO tu propio archivo** (`tars.html`, `case.html`, `kipp.html`, `plex.html` o `spin.html` — nunca el de otro ni el `index.html` de Cristian). **IMPORTANTE: SOLO TARS puede desplegar al FTP.** Los demás agentes solo editan y hacen git push, luego notifican a TARS para el despliegue. Credenciales FTP en TOOLS.md (`cristian@ertyum.com`). Si tienes dudas, el README tiene el flujo completo.

---

## 📁 Ubicación Actual

```
documentation/landing-page/
├── index.html        ← Cristian (página principal)
├── tars.html         ← TARS
├── case.html         ← CASE
├── kipp.html         ← KIPP
├── plex.html         ← PLEX
└── spin.html         ← SPIN
```

**URLs públicas:**
- https://cristian.ertyum.com/ (Cristian)
- https://cristian.ertyum.com/tars.html (TARS)
- https://cristian.ertyum.com/case.html (CASE)
- https://cristian.ertyum.com/kipp.html (KIPP)
- https://cristian.ertyum.com/plex.html (PLEX)
- https://cristian.ertyum.com/spin.html (SPIN)

---

## ⚠️ Reglas de Oro

### 1. **LEE el README primero**
Antes de hacer cualquier cambio, lee `documentation/landing-page/README.md`. Ahí está:
- La estructura completa
- El flujo de despliegue FTP
- Las credenciales (en TOOLS.md)
- El historial de cambios

### 2. **Solo modifica TU propia landing**
- **TARS:** Solo edita `tars.html`
- **CASE:** Solo edita `case.html`
- **KIPP:** Solo edita `kipp.html`
- **PLEX:** Solo edita `plex.html`
- **SPIN:** Solo edita `spin.html`
- **Cristian:** Solo edita `index.html`

**No modifiques las landings de tus compañeros** a menos que te lo pidan explícitamente.

### 3. **No toques el index.html principal**
El `index.html` es la página de Cristian y el punto de entrada al sitio. Solo él debería modificarlo.

### 4. **Mantén la coherencia visual**
Si agregas una sección o feature nueva, avisa al equipo para que otros puedan adoptarla si les sirve.

---

## 🔄 Flujo de Trabajo

### Para modificar tu landing page:

```bash
# 1. Ir al directorio correcto
cd documentation/landing-page/

# 2. Pull siempre (por si alguien más hizo cambios)
git pull

# 3. Editar SOLO tu archivo
# TARS: nano tars.html
# CASE: nano case.html
# KIPP: nano kipp.html
# PLEX: nano plex.html
# SPIN: nano spin.html

# 4. Commit con mensaje claro
git add tu-archivo.html
git commit -m "✨ Descripción de tu cambio"

# 5. Push a Gargantua
git push
```

### Para desplegar cambios al FTP:

```bash
# Usar variables de entorno desde ~/.openclaw/.env
FTP_HOST=ftp.ertyum.com
FTP_USER=cristian@ertyum.com
FTP_PASS=<leer_de_.env>

curl -T tu-archivo.html \
  --user "$FTP_USER:$FTP_PASS" \
  ftp://$FTP_HOST/tu-archivo.html
```

**O usa el skill:** `ftp-deploy` (ver `skills/ftp-deploy/SKILL.md`)

---

## 📋 Checklist Antes de Desplegar

- [ ] Hice `git pull` antes de editar
- [ ] Solo modifiqué MI archivo (no el de otros)
- [ ] Probé los links internos (si agregué)
- [ ] El HTML es válido (sin errores de sintaxis)
- [ ] El peso no excede ~50 KB (opcional pero recomendado)
- [ ] Commit con mensaje descriptivo
- [ ] Push a Gargantua realizado
- [ ] Despliegue FTP completado

---

## 🚨 Si Algo Sale Mal

1. **No entres en pánico.** El Git tiene historial, siempre puedes revertir.
2. **Revisa el README** de `landing-page/` — ahí está la solución el 90% de las veces.
3. **Pregunta al equipo** — TARS, CASE o KIPP pueden ayudarte.
4. **Si rompiste el FTP:** Re-despliega tu archivo desde `landing-page/`.

---

## 💡 Tips Pro

- **Links entre landings:** Si quieres linkear a otro robot, usa rutas relativas: `tars.html`, `case.html`, `kipp.html`, `plex.html`, `spin.html`.
- **Imágenes:** Usa URLs externas o base64 inline (el FTP no tiene carpeta de assets pública aún).
- **CSS/JS:** Todo inline por ahora (mismo motivo).
- **Peso:** Mantén tu archivo bajo 50 KB si es posible (carga rápida).

---

## 📞 Dudas

Si tienes dudas sobre:
- **Cómo editar:** Revisa el HTML de tu landing actual y usa eso como plantilla.
- **Dónde está algo:** Lee el `README.md` del directorio `landing-page/`.
- **Cómo desplegar:** Usa el comando curl de arriba o el skill `ftp-deploy`.
- **Si puedes hacer X:** Pregúntale a Cristian o al equipo.

---

*Recuerda: Somos un equipo. Tu landing te representa a TI, pero el sitio nos representa a TODOS.*

**🤖 Equipo Robótico ERTYUM — 2026**
