
# Proyecto Final: Control de Servidores y Dispositivos en Red

Este proyecto final permite a los alumnos aplicar sus conocimientos de HTML, CSS, Bootstrap y JavaScript para construir una aplicación web que administre servidores y dispositivos en red. A lo largo del proyecto, se implementará una interfaz visual atractiva con Bootstrap y funcionalidades interactivas con JavaScript.

## Objetivos del Proyecto
- Crear una interfaz de usuario usando **Bootstrap** para mejorar el diseño y la usabilidad.
- Utilizar **JavaScript** para añadir interactividad, como agregar y gestionar servidores y dispositivos en la red.
- Consolidar conocimientos sobre manipulación del DOM y eventos.

## Estructura del Proyecto

1. **Agregar Servidor**: Formulario para añadir un servidor a la red especificando su nombre y tipo.
2. **Lista de Servidores**: Visualización dinámica de los servidores agregados.
3. **Administración de Dispositivos en Red**: Formulario para agregar dispositivos, asignar IPs y definir su estado.
4. **Lista de Dispositivos**: Visualización de los dispositivos, con la opción de cambiar su estado entre "Activo" e "Inactivo".

## Instrucciones Paso a Paso

### Paso 1: Configuración de Bootstrap
Incluye Bootstrap en el archivo HTML para estilizar la interfaz. Agrega el siguiente enlace en la sección `<head>`:

```html
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
```

### Paso 2: Estructura HTML
En el cuerpo del archivo HTML (`<body>`), crea secciones que contengan:

1. **Encabezado**: Con un título y una breve descripción de la aplicación.
2. **Formulario para Agregar Servidor**: Incluye campos para el nombre del servidor y el tipo de servidor. Agrega un botón que ejecute la función `agregarServidor()` al hacer clic.
3. **Lista de Servidores**: Un área donde se mostrará la lista de servidores agregados. Actualiza esta lista dinámicamente usando JavaScript.
4. **Formulario para Agregar Dispositivo**: Incluye campos para el nombre del dispositivo y la dirección IP, con un botón que ejecute la función `agregarDispositivo()`.
5. **Lista de Dispositivos**: Un área para mostrar los dispositivos en red, cada uno con su estado actual y un botón para cambiar entre "Activo" e "Inactivo".

### Paso 3: JavaScript
En el archivo JavaScript o en una sección `<script>` dentro del HTML, agrega las siguientes funciones:

- **agregarServidor()**: Agrega un servidor al array `servidores` y actualiza la lista en la interfaz.
- **mostrarServidores()**: Recorre el array `servidores` y muestra cada servidor en la lista de servidores.
- **agregarDispositivo()**: Agrega un dispositivo al array `dispositivos`, asignándole un estado inicial de "Activo".
- **mostrarDispositivos()**: Muestra cada dispositivo en la lista de dispositivos, incluyendo su nombre, IP y estado.
- **cambiarEstadoDispositivo(index)**: Cambia el estado de un dispositivo entre "Activo" e "Inactivo" al hacer clic en el botón correspondiente.

### Ejemplo de Código
Aquí tienes un ejemplo de cómo estructurar la función `agregarServidor()`:

```javascript
function agregarServidor() {
    const nombreServidor = document.getElementById("nombre-servidor").value;
    const tipoServidor = document.getElementById("tipo-servidor").value;
    
    if (nombreServidor && tipoServidor) {
        let servidor = { nombre: nombreServidor, tipo: tipoServidor };
        servidores.push(servidor);
        mostrarServidores();
        document.getElementById("nombre-servidor").value = "";
        document.getElementById("tipo-servidor").value = "";
    } else {
        alert("Por favor, completa todos los campos.");
    }
}
```

### Notas Adicionales
- Asegúrate de validar todos los campos de entrada para mejorar la experiencia del usuario.
- Utiliza clases de Bootstrap como `.card`, `.list-group`, y `.btn` para estructurar y dar estilo a los elementos de la interfaz.

¡Buena suerte con el proyecto!
