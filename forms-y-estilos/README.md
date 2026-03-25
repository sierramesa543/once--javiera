1. Estructura base del proyecto

Primero creé dos archivos:

index.html → Contiene la estructura del formulario
contacto.css → Contiene los estilos visuales

Luego conecté el CSS al HTML con:

<link rel="stylesheet" href="contacto.css">
 2. Definición de variables CSS

En el archivo contacto.css, utilicé :root para definir colores y estilos reutilizables:

:root {
  --primario: #2563eb;
  --texto: #1f2937;
  --borde: #d1d5db;
  --fondo: #f9fafb;
}

🔹 Esto permite mantener un diseño consistente
🔹 Hace fácil cambiar colores en todo el proyecto

 3. Reset básico

Eliminé márgenes y configuré el modelo de caja:

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
 4. Diseño del body

Centré el formulario en la pantalla:

body {
  display: flex;
  align-items: center;
  justify-content: center;
}

🔹 También definí fuente, fondo y altura completa

 5. Contenedor principal

Creé una tarjeta para el formulario:

.contenedor {
  background: white;
  border-radius: 16px;
  box-shadow: var(--sombra);
}

🔹 Esto da apariencia moderna tipo "card"

 6. Encabezado

Agregué un título y descripción:

<header class="encabezado">
  <h1>💬 Contáctanos</h1>
  <p>Responderemos en menos de 24 horas.</p>
</header>

🔹 Con fondo azul usando --primario

 7. Estructura del formulario

Creé el formulario con:

<form class="formulario-contacto">

🔹 Usé flexbox para organizar los campos verticalmente

↔ 8. Campos en dos columnas

Para nombre y email:

.fila-doble {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

🔹 En móviles se convierte en una sola columna (responsive)

 9. Campos de entrada

Cada campo está dentro de:

<div class="campo">
  <label>...</label>
  <input>
</div>

🔹 Esto organiza label + input correctamente

 10. Tipos de inputs usados

Utilicé varios tipos:

text → Nombre
email → Correo
tel → Teléfono
textarea → Mensaje
select → Tipo de consulta

Ejemplo:

<input type="email" required>
 11. Validaciones HTML

Agregué validaciones nativas:

required
minlength
maxlength
pattern

Ejemplo:

<input type="tel" pattern="[0-9\s\-\+]{7,15}">
 12. Estilos interactivos

Cuando el usuario escribe:

input:focus {
  border-color: var(--primario);
}

🔹 También añadí estilos para:

válido (verde)
inválido (rojo)
 13. Radios y checkboxes

Para opciones de contacto:

<input type="radio" name="via_contacto">

Y términos:

<input type="checkbox" required>

🔹 Usé accent-color para personalizar el color

 14. Campo condicional (teléfono)

Incluí un campo de teléfono que depende de la opción elegida:

<div id="campo-telefono">

🔹 (Se puede mejorar con JavaScript para mostrar/ocultar dinámicamente)

 15. Términos y condiciones

Obligué al usuario a aceptar:

<input type="checkbox" required>
 16. Botones de acción

Agregué dos botones:

<button type="submit">Enviar</button>
<button type="reset">Borrar</button>

 Con estilos diferentes:

Primario (azul)
Secundario (gris)
✨ 17. Efectos visuales

Agregué efectos modernos:

.btn-primario:hover {
  transform: translateY(-1px);
}

🔹 También sombras y transiciones

 18. Diseño responsive

Usé media queries:

@media (max-width: 520px) {
  .fila-doble {
    grid-template-columns: 1fr;
  }
}

🔹 Para que funcione bien en celular