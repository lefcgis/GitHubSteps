# Manejo de GitHub 🎁

¡Bienvenido/a! Esta es una guía práctica, visual y optimizada para aprender a **crear, conectar y actualizar repositorios en GitHub** utilizando Git desde la terminal.

Esta iniciativa ha sido diseñada para el uso del público en general.

---

## 👥 Autores y Comunidad
* **Luis Ferrer 👨‍💻**
* **Víctor Medina**

📥 **Organización:** #Innovación | #WalshPerú

---

## 🐣 Sección: Modo Pollito (Conceptos Básicos desde Cero)

Si el lenguaje técnico te suena a chino, no te preocupes. Vamos a explicar qué estamos haciendo usando una analogía muy simple: **"La Carpeta Mágica y el Archivador en la Nube"**.

Imagina que estás escribiendo un libro o desarrollando un proyecto:
* **Tu Computadora (Local):** Es tu escritorio de trabajo real.
* **Git:** Es un fotógrafo invisible que toma fotos de tus documentos cada vez que tú se lo pides, para que si te equivocas borrando algo, puedas regresar en el tiempo.
* **GitHub (Remoto):** Es un archivador de seguridad gigante que está en la nube. Sirve para que tu trabajo no se pierda si tu computadora se daña y para compartirlo con tu equipo.

### El Ciclo de Vida de un Archivo en Git (Los 3 Estados)
Antes de enviar cualquier cosa a internet, tus archivos pasan por tres estaciones:
1. **Directorio de Trabajo (Working Directory):** Modificas tus archivos (están "sucios" o sin guardar en la foto).
2. **Área de Preparación (Staging Area / `git add`):** Pones los archivos en una "caja abierta". Le dices a Git: *"Oye, prepárame estos archivos para la foto"*.
3. **Repositorio Local (`git commit`):** Cierras la caja con llave y le pones una etiqueta. Ya guardaste el historial en tu máquina.
4. **Repositorio Remoto (`git push`):** Envías la caja por correo directamente a GitHub.

---

## 🚀 I. Crear y Subir un Repositorio por Primera Vez ✨🏆

Sigue estos pasos cuando tengas una carpeta nueva en tu computadora y quieras subirla a GitHub por primera vez.


### Paso 1: Inicializar el entorno
```bash
git init
```
💡 Modo Pollito: Le da "superpoderes" a tu carpeta actual. Git creará un ojo invisible (una carpeta oculta llamada .git) para empezar a vigilar qué archivos entran y salen.


### Paso 2: Revisar qué ha cambiado
```bash
git status
```
💡 Modo Pollito: Es una radiografía. Te mostrará en color rojo los archivos nuevos o modificados que Git todavía no tiene guardados en su memoria.


### Paso 3: Preparar los archivos
```bash
git add .
```
⚠️ Nota: El punto (.) significa "AGREGAR TODO". Si solo quieres agregar un archivo específico, usa git add nombre_del_archivo.txt.  
💡 Modo Pollito: Metes todos tus archivos rojos a la caja de preparación. Si vuelves a ejecutar git status, ahora saldrán en color verde.


### Paso 4: Registrar la foto (Tu primer guardado)
```bash
git commit -m "Mi primer commit: Estructura inicial del proyecto"
```
💡 Modo Pollito: Cierras la caja y le pones una etiqueta descriptiva obligatoria (-m). Consejo de oro: Escribe mensajes claros que expliquen qué cambiaste, evita usar cosas como "asdasd" o "cambios".


### Paso 5: Conectar tu computadora con GitHub
```bash
git remote add origin [https://github.com/tu_usuario/tu_repositorio.git](https://github.com/tu_usuario/tu_repositorio.git)
```
⚠️ Nota de corrección: Recuerda incluir siempre la palabra add para enlazar un servidor remoto por primera vez.  
💡 Modo Pollito: Construye un puente digital. Le dices a tu computadora: "A partir de ahora, tu destino en internet (origin) será esta URL de GitHub".


### Paso 6: Lanzar los archivos a la nube
```bash
git push -u origin main
```
💡 Modo Pollito: Empujas la caja a través del puente hacia la rama principal (main). El comando -u hace que la computadora recuerde el camino para que la próxima vez solo tengas que escribir git push.


## 🔄 II. Actualizar un Repositorio Existente 🔄⚡
Utiliza este flujo en tu día a día cuando tú u otra persona ya hayan creado el repositorio y solo necesites subir tus nuevos avances diarios.

### Paso 0: Traer lo último de internet (¡Súper Importante!)
```bash
git pull origin main
```
💡 Modo Pollito: Antes de que tú escribas una sola línea de código, descarga lo que otros miembros del equipo hayan subido a GitHub. Evita los famosos "conflictos de código".


### Paso 1: Verificar el estado actual
```bash
git status
```


### Paso 2: Seleccionar los nuevos cambios
```bash
git add .
```


### Paso 3: Sellar el paquete con un mensaje descriptivo
```bash
git commit -m "Actualización: Se añade sección explicativa para principiantes"
```


### Paso 4: Enviar los cambios modificados a GitHub
```bash
git push origin main
```


🛠️ Tabla de Comandos Rápidos (Acordeón para Emergencias)
Comando	¿Qué hace?	¿Cuándo usarlo?
git init	Crea un repositorio Git local.	Solo una vez al iniciar el proyecto.
git status	Muestra el estado de tus archivos (Rojo/Verde).	Todo el tiempo, antes de cada paso.
git add .	Empaqueta los cambios para la foto.	Después de modificar código.
git commit -m "mensaje"	Toma la foto del código con una nota.	Cuando termines una idea o tarea lógica.
git pull	Descarga los cambios de GitHub a tu PC.	Siempre al iniciar tu jornada de trabajo.
git push	Sube tus fotos guardadas a GitHub.	Al final del día o al terminar una función.

🛠️ Desarrollado con fines educativos e innovadores. ¡El control de versiones es el mejor amigo del desarrollador!
