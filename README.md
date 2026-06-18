# POB Digital - MVP (OCASA Life Sciences)

Dos pantallas estáticas, cada una pensada para servirse como sitio independiente en Render y accederse por QR.

## Contenido
- `pob-planificados/index.html` -> Pantalla **Retiros Planificados** (QR1)
- `pob-ejecutados/index.html` -> Pantalla **Resultado POB / Ejecutados** (QR2)

Ambas son archivos autónomos: HTML + CSS + JS + datos embebidos. No requieren backend, build ni dependencias.

## Deploy en Render (Static Site desde GitHub)

Se crean **dos** Static Sites (uno por pantalla) para que cada una tenga su URL independiente.

### Sitio 1 - Planificados
1. New + -> Static Site -> conectar este repo.
2. Configuración:
   - **Name:** pob-planificados (o el que prefieras)
   - **Branch:** main
   - **Root Directory:** `pob-planificados`
   - **Build Command:** (vacío)
   - **Publish Directory:** `.`
3. Create Static Site -> queda en `https://pob-planificados.onrender.com`

### Sitio 2 - Ejecutados
Igual que el anterior, con **Root Directory:** `pob-ejecutados`
-> queda en `https://pob-ejecutados.onrender.com`

## Después del deploy
Con las dos URLs finales se generan los dos códigos QR (uno por pantalla).
