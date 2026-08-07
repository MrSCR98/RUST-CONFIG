# 📂 **RUST-CONFIG**  
Mi configuración personalizada de **Rust**: gráficos, comandos, sensibilidad, teclas y más.

## 📍 **Dónde encontrar los archivos de configuración de Rust**  
Los archivos de configuración se encuentran en la siguiente carpeta:

```cmd
C:\Program Files (x86)\Steam\steamapps\common\Rust\cfg
```

## ⚙️ **Instrucciones para usar mi configuración**  
Para utilizar mi configuración en el juego, reemplaza los archivos existentes de la carpeta `cfg` con mis archivos (recuerda hacer una copia de seguridad por si alguna cosa no te gusta o tenías algo que no querías perder):

### 1. **`client.cfg`**  
Este archivo contiene configuraciones relacionadas con:  
- Calidad de gráficos  
- Configuración de la interfaz de usuario  
- Sensibilidad del mouse  
- Otras configuraciones generales del cliente.

### 2. **`keys.cfg`**  
Este archivo guarda tus **teclas personalizadas** y **bindeos**.  
Modifica este archivo para cambiar tus teclas asignadas, añadir nuevos bindeos o eliminarlos.

### 3. **`keys_default.cfg`**  
Este archivo tiene las **teclas predeterminadas** que usa **Rust**.  
Úsalo como referencia si deseas restablecer cualquier tecla a su configuración original.

### 4. **`favorites.cfg`**  
Aquí se almacenan los **servidores** que has agregado a tus **favoritos**.

---

### ✨ **Recuerda**:  
- **Haz una copia de seguridad** de tus archivos originales antes de realizar cualquier cambio, por si no te gusta alguna cosa o necesitas recuperarlo.  
- **Cierra el juego** antes de reemplazar los archivos de configuración para evitar problemas.

---

## 🚀 **Parámetros de lanzamiento recomendados**

Estos se colocan en las opciones de lanzamiento de Steam (Clic derecho sobre Rust > Propiedades > General > Parámetros de lanzamiento):

- **Todos:**
  ```cmd
  -"effects.maxgibs -1" -graphics.shadowmode "1" -gc.incremental_milliseconds "1"
  ```

- **No escombros:**
  ```cmd
  effects.maxgibs -1
  ```

- **Corrige el retraso al disparar:**
  ```cmd
  gc.incremental_milliseconds 1
  ```

---

## 🧾 **Comandos en el juego**

### ✅ Funcionan:

- **Ver armas más pequeñas (+ de FOV 70):**
  ```cmd
  graphics.vm_fov_scale false
  ```

- **Zoom bind FOV 90 a FOV 70:**
  ```cmd
  bind mouse3 ~graphics.fov 90;graphics.fov 70
  ```

- **Ver FPS y ping:**
  ```cmd
  global.perf 5
  ```

- **Cambiar calidad del agua:**
  ```cmd
  bind j ~water.quality 0;water.quality 2
  ```

- **Cambiar calidad de objetos:**
  ```cmd
  bind k ~mesh.quality 0;mesh.quality 200
  ```

- **Remover (Servidor Modificado):**
  ```cmd
  bind z chat.say "/remove"
  ```

- **Aceptar TP (Servidor Modificado):**
  ```cmd
  bind x chat.say "/tpa"
  ```

### ❌ No funcionan:

- **No retroceso tiro a tiro:**
  ```cmd
  player.recoilcomp true
  ```

- **Ver debajo del agua (viejo):**
  ```cmd
  bind k ~water.quality +2;water.quality -2
  ```

- **Ver debajo del agua (nuevo):**
  ```cmd
  bind j meta.if_true "water.quality 2";+meta.if_false "water.quality -1
  ```

- **Saltar más:**
  ```cmd
  physics.steps 60
  ```

## ➕ **Miras**

- **Base**
```cmd
RUST-FceIG-V4T
```

graphicssettings.shadowcascades "1" :(

graphics.shaderlod "3" :(

COSAS: https://wiki.facepunch.com/rust/