# 📘 Apuntes del Curso de Git

Este repositorio alberga todos mis apuntes personales mientras voy aprendiendo Git paso a paso.
Por cada clase del curso, añado lo que he comprendido, los comandos clave y algunos ejemplos.
Espero que esta documentación no solo me ayude a consolidar lo aprendido, sino que también sea útil para otros.

---

## 📚 Clase 1 - ¿Qué es Git?

### 🧠 Concepto

Git es un **sistema de control de versiones**.
Esto significa que nos permite llevar un registro de todos los cambios que hacemos en nuestros archivos. Es como tener una "máquina del tiempo" para nuestros proyectos.

Con Git podemos:

- Guardar cada versión de un archivo.
- Recuperar versiones anteriores cuando lo necesitemos.
- Ver quién hizo qué cambios y cuándo.
- Colaborar en equipo sin pisarnos los cambios.

---

### 🛠️ ¿Para qué sirve?

- Es ideal para programadores, diseñadores o cualquier persona que trabaje con archivos que cambian constantemente.
- Muy útil cuando se colabora en equipo.
- También es excelente para gestionar proyectos personales.

---

### 💻 Instalación de Git

Para usar Git desde la terminal o consola, primero necesitas instalarlo.
Puedes descargarlo desde: https://git-scm.com/

---

### ⚙️ Configuración inicial de Git

Después de instalar Git, es necesario configurar tu nombre de usuario y correo electrónico.
Esto es importante porque aparecerá en los commits que realices (como una firma digital).

```bash
git config --global user.name "Gustavo"
git config --global user.email "gustavomamani2464@gmail.com"
```
## 📚 Clase 2 - ¿Cómo Iniciar un Repositorio Git?
### 🧠 Concepto
Un repositorio es un espacio donde guardamos nuestros proyectos y su historial de cambios. Al crear un repositorio con Git, este empieza a realizar un seguimiento de todos los cambios que hagas en los archivos dentro de él.

### 🛠️ Comandos Básicos
Crear un repositorio nuevo:

El comando git init es el que utilizamos para iniciar un repositorio en un directorio.

```bash
git init
```
Esto convierte la carpeta en un repositorio Git. Después de ejecutar el comando, Git empieza a hacer un seguimiento de los archivos dentro de la carpeta.
Añadir archivos al repositorio:
El siguiente paso es añadir los archivos que quieres comenzar a rastrear. Para eso, usamos el comando git add.
Para añadir un archivo individual, ejecutamos:
```bash
git add nombre_del_archivo
```
Para añadir todos los archivos del directorio, usamos:
```bash
git add 
```
Realizar el primer commit:
Después de añadir los archivos, el siguiente paso es hacer un "commit", lo cual guarda una versión de los archivos que hemos añadido.
```bash
git commit -m "Primer commit"
```
El mensaje entre comillas es importante porque describe el cambio realizado.
### 📦 Resumen
-El comando git init convierte una carpeta en un repositorio Git

-El comando git add se utiliza para añadir archivos al repositorio y que Git los rastree

-git commit guarda un "punto" en el historial de tu proyecto

## 📚 Clase 3: Comenzando con Git
### 🧠 Concepto
En esta clase, aprenderás a iniciar un proyecto con Git desde cero. Esto incluye crear un nuevo repositorio local, agregar archivos, realizar tu primer commit y comprender el flujo básico de trabajo.
## 🛠️ Pasos para iniciar un repositorio con Git
### Inicializar un repositorio
Para comenzar a usar Git en un proyecto, primero debes inicializar un repositorio en el directorio de tu proyecto:
```bash
git init
```
Este comando crea un subdirectorio oculto llamado .git que contiene todos los archivos necesarios del repositorio.
### Verificar el estado del repositorio
Para ver el estado actual de tu repositorio y los archivos que han sido modificados o añadidos:
```bash
git status
```
3. Agregar archivos al área de preparación (staging area)
Antes de realizar un commit, debes agregar los archivos que deseas incluir:
```bash
git add nombre_del_archivo
```
O para agregar todos los archivos modificados:
```bash
git add
```
### Realizar un commit
Después de agregar los archivos al área de preparación, puedes realizar un commit para guardar los cambios:
```bash
git commit -m "Mensaje descriptivo del commit"
```
Este comando guarda una instantánea de los cambios en el historial del repositorio.
### Ver el historial de commits
Para ver el historial de commits realizados en el repositorio:
```bash
git log
```
Este comando muestra una lista de commits en orden cronológico inverso.
💡 Buenas prácticas
-Mensajes de commit claros: Escribe mensajes de commit que describan claramente los cambios realizados.

-Commits frecuentes: Realiza commits con frecuencia para mantener un historial detallado de los cambios.

-Uso de .gitignore: Crea un archivo .gitignore para excluir archivos o directorios que no deseas rastrear con Git
## 📚 Clase 4 - Iniciando un Repositorio con Git y la Rama main
### 🧠 Concepto
Git nos permite crear un repositorio local desde cero en cualquier carpeta. Esto transforma esa carpeta en un proyecto que Git puede seguir y versionar.

### 🛠️ ¿Qué hace git init?
Crea un repositorio vacío en esa carpeta y añade una subcarpeta oculta llamada .git, donde se guarda todo el historial de versiones. A partir de ese momento, todos los cambios en los archivos pueden ser gestionados con Git.

### 💡 Comando importante
```bash
git init
```
Este comando se ejecuta dentro de la carpeta del proyecto que queremos versionar.
### 🌱 ¿Qué es la rama main?
Cuando usamos git init, Git crea una rama principal. Antes se llamaba master, pero ahora el nombre por defecto recomendado es main. GitHub también ha adoptado main como su estándar actual
## 📚 Clase 5: Conectando tu Repositorio Local con GitHub
### 🧠 Concepto
En esta clase, vas a aprender cómo vincular tu proyecto local con un repositorio remoto en GitHub. Esto te permitirá guardar tu trabajo en la nube y colaborar con otros desarrolladores.

### 🛠️ Pasos para conectar tu repositorio local con GitHub
**Crear un repositorio en GitHub**

1. Inicia sesión en tu cuenta de GitHub.
2. Haz clic en el botón "New" o "Nuevo repositorio".
3. Asigna un nombre a tu repositorio y, si quieres, añade una descripción.
4. Puedes decidir si hacerlo público o privado.
5. Importante: No marques la opción de inicializar con un README si ya tienes archivos en tu repositorio local.
6. Haz clic en "Create repository"
7. 
## 📚 Clase 6 - Buenas prácticas en Git
### 🧠 ¿Por qué son importantes?
Seguir buenas prácticas en Git ayuda a que tu proyecto esté ordenado y sea más fácil de entender, especialmente si trabajás en equipo.

### ✅ Buenas prácticas:
Commits pequeños y claros
Hacer commits seguido, con mensajes que expliquen bien lo que cambiaste. Ej: "Agrego validación al login".

Usar ramas
Siempre crear una nueva rama para trabajar en una función o arreglo. Así no tocas la rama principal (main o master) hasta que todo esté bien.

Actualizar seguido tu repo local
Usar git pull para traer los cambios más nuevos del repositorio remoto y evitar errores o conflictos.

Revisar antes de hacer commit
Ver con git status y git diff qué vas a subir, para no incluir archivos innecesarios.

Usar .gitignore
Para que Git no suba archivos que no hacen falta (como carpetas del IDE o archivos temporales).

No subir archivos muy pesados
Evitar subir cosas como videos o imágenes grandes, que hacen lento el repo.

### 💡 Conclusión
Trabajar con orden en Git te ahorra muchos problemas. Estas prácticas ayudan a tener todo más limpio y a entender mejor el código, tanto vos como tus compañeros
**Conectar tu repositorio local con el remoto**
En tu terminal, dentro del directorio de tu proyecto local, agrega la URL del repositorio remoto:

```bash
git remote add origin https://github.com/tu_usuario/tu_repositorio.git
```
Reemplaza `tu_usuario` y `tu_repositorio` con tu nombre de usuario y el nombre del repositorio en GitHub.
**Subir tus archivos al repositorio remoto**
Si es la primera vez que subes tu proyecto, asegúrate de que todos los archivos estén comprometidos:
```bash
git add .
git commit -m "Primer commit"
```
Luego, sube los archivos a la rama principal (main):

```bash
git push -u origin main
```
Nota: Asegúrate de que tu rama principal se llame `main`. Si tu rama principal se llama `master`, considera renombrarla a `main` para seguir las prácticas actuales recomendadas.

**Verificar en GitHub**
Dirígete a tu repositorio en GitHub y verifica que los archivos se hayan subido correctamente.

### 🔑 Comandos clave
`git remote add origin <URL>`: Conecta tu repositorio local con el remoto en GitHub.

`git push -u origin main`: Sube tus archivos a la rama principal del repositorio remoto
## 🔄 Clase 7 – Cómo deshacer cambios en Git
## 🧠 ¿Por qué es importante?
En Git, es bastante común cometer errores o querer revertir algunos cambios. Saber cómo usar las herramientas adecuadas para deshacer esos cambios te ayuda a mantener un historial limpio y a colaborar de manera más efectiva.

## 🛠️ Herramientas para deshacer cambios
**git restore**
Introducido en Git 2.23, el comando git restore se utiliza para deshacer cambios en archivos específicos.
Deshacer cambios en el directorio de trabajo:
```bash
git restore archivo.txt
```
Este comando restaura archivo.txt al último commit confirmado, descartando cualquier cambio no guardado.

Deshacer cambios en el área de preparación (staging):
```bash
git restore --staged archivo.txt
```
Esto elimina archivo.txt del área de preparación, pero mantiene los cambios en el directorio de trabajo.
**git reset**
El comando git reset se usa para deshacer commits y mover el puntero de la rama a un estado anterior. Hay tres modos principales:

--soft: Deshace commits, pero mantiene los cambios en el área de preparación.
```bash
git reset --soft HEAD~1
```
--mixed (por defecto): Deshace commits y elimina los cambios del área de preparación, pero los conserva en el directorio de trabajo.
```bash
git reset HEAD~1
```
--hard: Deshace commits y elimina los cambios tanto del área de preparación como del directorio de trabajo. ¡Ten cuidado! Esta acción es irreversible.
```bash
git reset --hard HEAD~1
```
**git revert**
El comando git revert crea un nuevo commit que revierte los cambios de un commit anterior, sin alterar el historial del repositorio. Es perfecto para deshacer cambios en ramas compartidas.

Revertir el último commit:
```bash
git revert HEAD
```
Revertir un commit específico:
```bash
git revert <hash_del_commit>
```
### 📌 Conclusión
Saber cómo utilizar correctamente git revert y otras herramientas es esencial para manejar tu historial de cambios de manera efectiva.
