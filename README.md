# Catalogo-de-Libros-

# DevBooks — Catálogo de libros para programadores

## Información del reto

* **Duración:** 45–60 minutos
* **Modalidad:** Equipos
* **Tecnologías:** HTML5 + Bootstrap 5
* **Entrega:** Repositorio de código

### Objetivo

Aplicar **Bootstrap** para construir una interfaz responsive utilizando:

* Layout
* Grid
* Spacing
* Botones
* Cards
* Formularios
* Utilidades de Bootstrap
* Diseño responsive

> **Entrega:** Deberán subir su código a un repositorio. No es necesario que todos compartan el enlace; solo un integrante del equipo debe realizar la entrega e incluir los nombres de todos los integrantes.

---

# 1. Situación

> Una biblioteca quiere una página web donde los usuarios puedan consultar los libros disponibles y solicitar un préstamo.

El equipo de desarrollo debe crear una primera versión del catálogo.

### La página debe tener:

1. Encabezado
2. Buscador
3. Categorías
4. Catálogo de libros
5. Formulario para solicitar un préstamo
6. Footer

---

# 2. Estructura de la página

Visualmente, la página debe seguir una estructura similar a:

```text
┌──────────────────────────────────────────────┐
│                  DevBooks                    │
│        Inicio | Libros | Categorías         │
└──────────────────────────────────────────────┘

        Encuentra tu próximo libro

┌──────────────────────────────────────────────┐
│ Buscar libro...                    [Buscar]  │
└──────────────────────────────────────────────┘

Categorías:

Todos | Java | JavaScript | Web | Bases de datos | DevOps


                    LIBROS

┌──────────┐  ┌──────────┐  ┌──────────┐
│  imagen  │  │  imagen  │  │  imagen  │
│          │  │          │  │          │
│  Libro 1 │  │  Libro 2 │  │  Libro 3 │
│  Autor   │  │  Autor   │  │  Autor   │
│  [Ver]   │  │  [Ver]   │  │  [Ver]   │
└──────────┘  └──────────┘  └──────────┘


             SOLICITAR PRÉSTAMO

Nombre
[________________________]

Correo
[________________________]

Libro
[________________________]

Fecha de devolución
[________________________]

              [Solicitar]
```

---

# 3. Reto 1 — Crear la estructura

Crear el archivo:

```text
index.html
```

La estructura inicial debe contener:

```html
<header>
</header>

<main>

    <section>
        <!-- buscador -->
    </section>

    <section>
        <!-- categorías -->
    </section>

    <section>
        <!-- libros -->
    </section>

    <section>
        <!-- formulario -->
    </section>

</main>

<footer>
</footer>
```

### Objetivo

En esta etapa **no buscamos que la página quede bonita todavía**.

La intención es recordar:

> **HTML = estructura**

---

# 4. Reto 2 — Incorporar Bootstrap

Agregar Bootstrap mediante CDN.

Después deberán comprobar que Bootstrap está funcionando utilizando, por ejemplo:

```html
<h1 class="text-primary">
    DevBooks
</h1>
```

Si el texto aparece estilizado con el color correspondiente, Bootstrap está funcionando correctamente.

---

# 5. Reto 3 — Crear el layout

Ahora deberán utilizar el sistema de grid de Bootstrap:

```text
container
    ↓
row
    ↓
col
```

Ejemplo:

```html
<div class="container">

    <div class="row">

        <div class="col">
            Contenido
        </div>

    </div>

</div>
```

### Conceptos a investigar

* `container`
* `row`
* `col`

---

# 6. Reto 4 — Catálogo responsive

Crear un catálogo con un mínimo de **6 libros**.

Cada libro debe representarse mediante una **Card de Bootstrap**.

### Libros

| Libro                        | Categoría    |
| ---------------------------- | ------------ |
| Clean Code                   | Programación |
| Java: The Complete Reference | Java         |
| Eloquent JavaScript          | JavaScript   |
| HTML & CSS                   | Web          |
| You Don't Know JS            | JavaScript   |
| Design Patterns              | Arquitectura |

Las seis tarjetas deben estar dentro de:

```html
<div class="row">
```

---

# 7. Reto 5 — Responsive

Realizar una pequeña investigación y experimentación con el sistema responsive de Bootstrap.

El catálogo debe adaptarse de acuerdo con el tamaño de pantalla.

### Celular

Debe mostrarse **un libro por fila**:

```text
┌───────────────┐
│    Libro      │
└───────────────┘

┌───────────────┐
│    Libro      │
└───────────────┘
```

### Tablet

Deben mostrarse **dos libros por fila**:

```text
┌─────────┐ ┌─────────┐
│  Libro  │ │  Libro  │
└─────────┘ └─────────┘
```

### Desktop

Deben mostrarse **tres libros por fila**:

```text
┌───────┐ ┌───────┐ ┌───────┐
│ Libro │ │ Libro │ │ Libro │
└───────┘ └───────┘ └───────┘
```

### Pista

Investigar las clases responsive de Bootstrap:

```text
col-12
col-md-6
col-lg-4
```

---

# 8. Reto 6 — Categorías

Crear botones para filtrar visualmente las categorías:

```text
Todos
Java
JavaScript
Web
Bases de Datos
DevOps
```

Por ahora **no es necesario implementar la funcionalidad de filtrado**.

Utilizar las herramientas de spacing de Bootstrap:

```text
m-*
p-*
gap-*
```

---

# 9. Reto 7 — Buscador

Crear un buscador con el siguiente diseño:

```text
┌──────────────────────────────────────────────┐
│ Buscar libro...                    [Buscar]  │
└──────────────────────────────────────────────┘
```

El buscador **no necesita funcionar**.

### Pista

Investigar el componente:

```text
input-group
```

También pueden utilizar:

```text
form-control
btn
```

---

# 10. Reto 8 — Formulario de préstamo

Crear un formulario que contenga:

```text
Nombre
Correo electrónico
Libro
Fecha de devolución

[Solicitar préstamo]
```

Utilizar los componentes de formulario de Bootstrap.

Algunos ejemplos:

```text
form-control
form-label
btn
```

---

# 11. Reto 9 — Aplicar utilidades

Ahora deberán mejorar visualmente la página **sin crear CSS nuevo**.

Utilizar al menos las siguientes clases de Bootstrap.

## Texto

```text
text-center
text-primary
text-muted
```

## Espaciado

```text
mt-*
mb-*
p-*
py-*
```

## Fondo

```text
bg-light
bg-dark
```

## Bordes

```text
border
rounded
```

## Flexbox

```text
d-flex
justify-content-center
justify-content-between
align-items-center
gap-*
```

---

# 12. Reto 10 — Regla importante

> **Durante este reto no pueden crear CSS para propiedades que Bootstrap ya pueda resolver.**

### Ejemplo

No crear:

```css
.titulo {
    text-align: center;
}
```

Cuando Bootstrap permite utilizar:

```html
<h1 class="text-center">
```

---

### Otro ejemplo

No crear:

```css
.card {
    margin-bottom: 20px;
}
```

Cuando Bootstrap permite:

```html
<div class="card mb-3">
```

---

### Otro ejemplo

No crear:

```css
.contenedor {
    display: flex;
}
```

Cuando Bootstrap permite:

```html
<div class="d-flex">
```

### Regla general

Antes de escribir CSS, pregúntate:

> **¿Bootstrap ya tiene una clase para hacer esto?**

Si la respuesta es sí, utiliza Bootstrap.

---

# 13. Reto final — Personalización

En esta etapa sí está permitido crear:

```text
style.css
```

Sin embargo, deberán utilizar **máximo 5 reglas CSS propias**.

Por ejemplo:

```css
body {
    font-family: Arial, sans-serif;
}

.logo {
    letter-spacing: 2px;
}
```

La idea es utilizar Bootstrap para la mayor parte de la interfaz y reservar el CSS propio para pequeñas personalizaciones.

---

# Estructura sugerida del proyecto

Al finalizar, el proyecto podría tener una estructura similar a:

```text
DevBooks/
│
├── index.html
├── styles.css
└── README.md
```

---

# Checklist de entrega

Antes de entregar el proyecto, comprueben que:

* [ ] Existe `index.html`
* [ ] Bootstrap está incorporado mediante CDN
* [ ] Existe un `<header>`
* [ ] Existe un buscador
* [ ] Existen categorías
* [ ] Existen mínimo 6 libros
* [ ] Los libros utilizan Cards de Bootstrap
* [ ] El catálogo utiliza `container`, `row` y `col`
* [ ] El catálogo es responsive
* [ ] En celular se muestra 1 libro por fila
* [ ] En tablet se muestran 2 libros por fila
* [ ] En desktop se muestran 3 libros por fila
* [ ] Existe un formulario de préstamo
* [ ] Existe un footer
* [ ] Se utilizan utilidades de Bootstrap
* [ ] No se creó CSS innecesario
* [ ] `style.css` contiene máximo 5 reglas propias
* [ ] El código fue subido a un repositorio
* [ ] El README incluye los nombres de los integrantes del equipo

---

# Integrantes del equipo


Angelica Amellali Mercado Aguilar<br>
Daniel Rosas Monroy

---

## Éxito con el reto

El objetivo principal no es solamente terminar la página, sino **experimentar con Bootstrap y comprender cómo sus clases permiten construir interfaces responsive sin depender de CSS personalizado**.
