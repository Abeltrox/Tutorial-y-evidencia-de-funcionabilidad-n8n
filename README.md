# Instalación de n8n y Primer "Hola Mundo"

---

##  Integrantes
### Nombre 
Óscar Abel Bonilla García 

---
## Método de Instalación Utilizado

La instalación de n8n se realizó mediante **Docker**.


---

## ✅ Requisitos Previos

1. ¿Qué fue lo más difícil de la instalación?
    Realmente nada me parecio dificil en la instalacion lo unico complicado fue buscar la pagina oficial y el enorme esfuerzo de teclear jajaja
2. ¿Qué ventajas tiene n8n?
    Principalmente permite conectar aplicaciones y crea flujos de trabajo muy util para automatizar sistemas y lo mejor es gratisss.
3. ¿Qué diferencia encontraron entre Docker y local?
    Segun lo que pude ver es que el docker ejecuta el n8n en un entorno aislado (en los famosos contenedores),  en cambio ejecutarlo localmente lo corre desde el mismo sitema operativo y lo corre con node.js
4. ¿Para qué casos reales usarían automatización?
    Casi todo realmente, mandar mensajes automaticos, enviar notificaciones a correos y muchas mas funciones aun por descubrir la verdad tiene demasiados usos.
5. ¿Qué les gustaría automatizar en el futuro?
    Sistemas de registo en bases de datos y tambien uno que otro bot para buscar informacion de algun comando o ejemplo matematico de algo u fisica para desarrollar juegos por hobby.

Antes de iniciar la instalación de n8n con Docker, se deben tener instalados y configurados los siguientes componentes:

- **Node.js** (con todas sus extensiones de JavaScript incluidas)
- **Docker Desktop** instalado desde la pagina web :)
---

## Proceso de Instalación

### Paso 1 — Instalar Docker

Descarga e instala Docker Desktop desde la página oficial:
https://www.docker.com/

    Paso 1
<a href="https://ibb.co/FLtC7Rcy"><img src="https://i.ibb.co/NdzbYcfJ/Captura-de-pantalla-2026-05-27-221831.png" alt="Captura de pantalla 2026 05 27 221831" border="0"></a>
    Paso 2
<a href="https://ibb.co/7x4rz7cn"><img src="https://i.ibb.co/rKs5tnPx/Captura-de-pantalla-2026-05-27-221841.png" alt="Captura de pantalla 2026 05 27 221841" border="0"></a>
    Paso 3
<a href="https://ibb.co/JR9wvB0y"><img src="https://i.ibb.co/0jxRCD8F/Captura-de-pantalla-2026-05-27-222011.png" alt="Captura de pantalla 2026 05 27 222011" border="0"></a>
    Paso 4
<a href="https://ibb.co/0yfRDGpK"><img src="https://i.ibb.co/Xxzr2CfD/Captura-de-pantalla-2026-05-27-222341.png" alt="Captura de pantalla 2026 05 27 222341" border="0"></a>
    Paso 5 Donde sale un error de wsl necesita actualizarse 
<a href="https://ibb.co/wZR8dy2M"><img src="https://i.ibb.co/0pc1nqzh/Captura-de-pantalla-2026-05-27-225156.png" alt="Captura de pantalla 2026 05 27 225156" border="0"></a>
    Paso 6 Solucion del error. Abrir el powershell con permisos de administrador y luego pegar el comando wsl --update
    <a href="https://ibb.co/8nGmCQN8"><img src="https://i.ibb.co/HLRKS9Bg/Captura-de-pantalla-2026-05-27-225207.png" alt="Captura de pantalla 2026 05 27 225207" border="0"></a>
    Paso 7 Solucion del problema.
    <a href="https://ibb.co/0pcJsmB1"><img src="https://i.ibb.co/tw4CLQZn/Captura-de-pantalla-2026-05-27-225409.png" alt="Captura de pantalla 2026 05 27 225409" border="0"></a>
    Paso 8 No sdirigimos a el apartado de images.
    <a href="https://ibb.co/5WxLsjqr"><img src="https://i.ibb.co/JRFHrpXv/Captura-de-pantalla-2026-05-27-225728.png" alt="Captura de pantalla 2026 05 27 225728" border="0"></a>
    Paso 9 Y le damos a buscar imagen para correr
    <a href="https://ibb.co/5WxLsjqr"><img src="https://i.ibb.co/JRFHrpXv/Captura-de-pantalla-2026-05-27-225728.png" alt="Captura de pantalla 2026 05 27 225728" border="0"></a>
    Paso 10 Buscamos n8n y escojemos casi que el primer resultado que diga n8nio
    <a href="https://ibb.co/JDKQTD4"><img src="https://i.ibb.co/RR9yKRm/Captura-de-pantalla-2026-05-27-225741.png" alt="Captura de pantalla 2026 05 27 225741" border="0"></a>
    Paso 11 Le damos a pull y debe de quedar asi 
    <a href="https://ibb.co/q3nZwg8x"><img src="https://i.ibb.co/tThd5263/Captura-de-pantalla-2026-05-27-230002.png" alt="Captura de pantalla 2026 05 27 230002" border="0"></a>
    Paso 12 Le damos a run y debemos llenar estos datos tal cual 
    <a href="https://ibb.co/210n2HwB"><img src="https://i.ibb.co/fzV1RLb7/Captura-de-pantalla-2026-05-27-230404.png" alt="Captura de pantalla 2026 05 27 230404" border="0"></a>
    Paso 13 Le damos click en ports 
    <a href="https://ibb.co/1YhJ6jkk"><img src="https://i.ibb.co/5XtxFwPP/Captura-de-pantalla-2026-05-27-230529.png" alt="Captura de pantalla 2026 05 27 230529" border="0"></a>
    Paso 14 Llenamos nuestra informacion 
    <a href="https://ibb.co/j9QfKCCN"><img src="https://i.ibb.co/MytSTzzv/Captura-de-pantalla-2026-05-27-230957.png" alt="Captura de pantalla 2026 05 27 230957" border="0"></a>
    Paso 15 Y estamos listos para empezar 
    <a href="https://ibb.co/d0CBBd03"><img src="https://i.ibb.co/99KnnF9f/Captura-de-pantalla-2026-05-27-231658.png" alt="Captura de pantalla 2026 05 27 231658" border="0"></a>
    Paso 16 Le damos en evento por click y lo vinculamos con discord
    <a href="https://ibb.co/My4HBMyB"><img src="https://i.ibb.co/GfLDHcfH/Captura-de-pantalla-2026-05-27-232328.png" alt="Captura de pantalla 2026 05 27 232328" border="0"></a>
    Paso 16 y buala nuestro primer hola mundo en n8n
    <a href="https://ibb.co/F4ychJL9"><img src="https://i.ibb.co/4RXCFMnc/Captura-de-pantalla-2026-05-27-234234.png" alt="Captura de pantalla 2026 05 27 234234" border="0"></a>
---

### Paso 2 — Verificar que Docker está activo

Abre una terminal (PowerShell o CMD) y ejecuta:

```bash
docker --version
```

Deberías ver algo como:

<a href="https://ibb.co/DH8pdSg3"><img src="https://i.ibb.co/HfxdZkpm/Captura-de-pantalla-2026-05-28-005339.png" alt="Captura de pantalla 2026 05 28 005339" border="0"></a>

---

## 💭 Reflexión Final

El uso de n8n para mí es una herramienta fundamental para la automatización de procesos en los cuales normalmente tomaría demasiado tiempo hacerlo a mano. Gracias a su interfaz visual e intuitiva basada en nodos, es posible construir flujos de trabajo complejos sin necesidad de escribir grandes bloques de código, lo que lo convierte en una solución accesible tanto para desarrolladores como para personas con conocimientos técnicos básicos. La integración con Docker facilita aún más su despliegue, permitiendo tener un entorno funcional en cuestión de minutos. Sin duda, n8n representa una alternativa poderosa y flexible frente a otras herramientas de automatización del mercado, y su curva de aprendizaje resulta bastante amigable una vez superada la configuración inicial.

---

*Documento elaborado por Óscar Abel Bonilla García*
