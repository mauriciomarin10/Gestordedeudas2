# Gestor de Deudas — PWA Móvil

Aplicación web progresiva (PWA) para controlar deudas financieras desde el celular.
Funciona sin conexión a internet una vez instalada.

---

## ¿Cómo instalarla en tu celular?

### iPhone / iPad (Safari)
1. Abre el archivo `index.html` en Safari (puedes subirlo a un servidor o usar una app como "Working Copy")
2. Toca el botón **Compartir** (cuadrado con flecha hacia arriba)
3. Selecciona **"Agregar a pantalla de inicio"**
4. Ponle el nombre que quieras y toca **Agregar**
5. La app aparecerá en tu pantalla de inicio como cualquier otra app

### Android (Chrome)
1. Abre el archivo `index.html` en Chrome
2. Toca el menú de tres puntos (⋮) arriba a la derecha
3. Selecciona **"Agregar a pantalla de inicio"** o **"Instalar app"**
4. Confirma y listo

### Opción más fácil: servidor local
Si tienes Python instalado, desde la carpeta del proyecto:
```bash
python3 -m http.server 8080
```
Luego abre `http://TU_IP:8080` en el navegador del celular (ambos deben estar en la misma red WiFi).

---

## Archivos del proyecto

```
gestor-deudas-pwa/
├── index.html      ← App principal
├── manifest.json   ← Configuración PWA
├── sw.js           ← Service Worker (modo offline)
├── icon-192.svg    ← Ícono app
└── icon-512.svg    ← Ícono app grande
```

---

## Funcionalidades

- Agregar deudas con nombre, capital, cuotas e interés mensual
- Cálculo automático de cuota mensual (sistema francés o capital fijo)
- Tabla de amortización cuota a cuota
- Registro de abonos libres o por cuota
- Indicadores: Activa / Por terminar / Cumplido
- Pantalla de estadísticas con gráfico de dona
- Exportar / importar datos en JSON
- Funciona 100% offline después de la primera carga
- Datos guardados localmente en el dispositivo

---

## Tecnologías

- HTML5 + CSS3 + JavaScript vanilla
- PWA con Service Worker y Web App Manifest
- localStorage para persistencia de datos
- Sin dependencias externas (excepto Google Fonts)
