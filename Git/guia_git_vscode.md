
# Guía para usar Git en Visual Studio Code

Esta guía te ayudará a entender cómo trabajar con Git en Visual Studio Code (VS Code) y cómo clonar un repositorio usando un enlace.

## 1. ¿Qué es Git?

Git es un sistema de control de versiones que permite hacer un seguimiento de los cambios en el código. Es útil para trabajar en equipo y mantener un historial de cambios en los proyectos.

## 2. Instalación de Git y Visual Studio Code

Antes de comenzar, asegúrate de tener instalado:

- **Git**: Puedes descargarlo desde [aquí](https://git-scm.com/).
- **Visual Studio Code**: Descárgalo desde [aquí](https://code.visualstudio.com/).

Asegúrate de que Git esté correctamente configurado en tu sistema.

## 3. Clonar un Repositorio desde un Enlace

Cuando recibas un enlace a un repositorio, estos son los pasos para clonarlo y comenzar a trabajar en él.

### Pasos:

1. **Copia el enlace del repositorio**:
   - El profesor te proporcionará un enlace al repositorio de GitHub, copia ese enlace.

2. **Abre Visual Studio Code**.

3. **Accede al Panel de Control de Fuente**:
   - En la barra lateral izquierda de VS Code, haz clic en el icono de **"Control de Código Fuente"** (el que parece un árbol de ramas).

## 4. Configurar GIT

Es importante configurar GIT para identificarnos e indicar a Git algunos parámetros.

### Pasos para configurar GIT:

1. **Identificar Nombre de Usuario**:
   - En la terminal de VSCode (o en la propia de GIT "Git Bash"), introducir el siguiente comando:
           git config --global user.name "usuario"
   - Siendo "usuario" el nombre de usuario con el que nos identificamos en GitHub.

2. **Identificar Email del Usuario**:
   - En la terminal de VSCode (o en la propia de GIT "Git Bash"), introducir el siguiente comando:
           git config --global user.email "usuario@servidor.es"
   - Siendo "usuario@servidor.es" el correo electrónico con el que nos dimos de alta en GitHub.

3. **Identificar el IDE (VSCode) con el que vamos a trabajar**:
   - En la terminal de VSCode (o en la propia de GIT "Git Bash"), introducir el siguiente comando:
           git config --global core.editor "code --wait"
     
4. **Identificar el OS con el que vamos a trabajar**:
   - Para evitar problemas de compatibilidad entre OS (windows, mac, linux), a la hora de interpretar los retornos de carro o saltos de línea.
   - En la terminal de VSCode (o en la propia de GIT "Git Bash"), introducir el siguiente comando:
        Windows:
           git config --global core.autocrlf true
        Mac o Linux:
           git config --global core.autocrlf init

## 5. Subir Cambios al Repositorio

Cuando hayas terminado de trabajar en los archivos, es importante subir los cambios para que el profesor pueda verlos.

### Pasos para subir cambios:

1. **Hacer Commit**:
   - En el panel de **Control de Código Fuente**, verás los archivos que han cambiado. Escribe un mensaje en el campo de "Mensaje de Commit" (explicando qué cambios hiciste).
   - Haz clic en el ícono de ✔️ para confirmar los cambios (commit).
   - Otra formade realizar Commit es utilizando la terminal, para ello utilizaremos el siguiente comando:
        git commit -m "Mensaje de Commit" 
2. **Subir los Cambios (Push)**:
   - Después de hacer commit, haz clic en los tres puntos del menú (`...`) nuevamente y selecciona **Push** para subir tus cambios al repositorio remoto.
   - Otra formade realizar Push es utilizando la terminal, para ello utilizaremos el siguiente comando:
        git push origin master
     
## 6. Actualizar tu Repositorio

Es importante mantener tu copia local del repositorio actualizada con los últimos cambios del profesor.

### Pasos para actualizar:

1. **Hacer Pull**:
   - Para obtener los últimos cambios, haz clic en los tres puntos (`...`) y selecciona **Pull**. Esto actualizará tu copia local con los últimos cambios del repositorio remoto.
   - Otra formade realizar Pull es utilizando la terminal, para ello utilizaremos el siguiente comando:
        git pull
---

¡Eso es todo! Siguiendo estos pasos, podrás clonar, trabajar y subir cambios en tus proyectos de clase utilizando Git y Visual Studio Code.
