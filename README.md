# ATHLEX

<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ATHLEX | Ropa Deportiva</title>

<style>
:root {
    --negro: #101010;
    --naranja: #ff6b18;
    --blanco: #ffffff;
    --gris: #f3f3f3;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
    scroll-behavior: smooth;
}

body {
    background: var(--blanco);
    color: var(--negro);
}

/* NAVEGACIÓN */

header {
    background: var(--negro);
    color: white;
    padding: 18px 7%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: sticky;
    top: 0;
    z-index: 100;
}

.logo {
    font-size: 30px;
    font-weight: 900;
    letter-spacing: 3px;
}

.logo span {
    color: var(--naranja);
}

nav {
    display: flex;
    gap: 25px;
    align-items: center;
}

nav a {
    text-decoration: none;
    color: white;
    font-size: 14px;
    transition: .3s;
}

nav a:hover {
    color: var(--naranja);
}

.carrito-btn {
    background: var(--naranja);
    color: white;
    border: none;
    padding: 11px 18px;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
}

/* PORTADA */

.hero {
    min-height: 570px;
    background:
    linear-gradient(90deg, rgba(0,0,0,.90), rgba(0,0,0,.30)),
    url("https://images.unsplash.com/photo-1534438327276-14e5300c3a48?auto=format&fit=crop&w=1800&q=85");
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    padding: 70px 9%;
    color: white;
}

.hero-content {
    max-width: 600px;
}

.hero h1 {
    font-size: clamp(48px, 7vw, 78px);
    font-weight: 900;
    line-height: 1;
    margin-bottom: 22px;
}

.hero h1 span {
    color: var(--naranja);
}

.hero p {
    font-size: 18px;
    line-height: 1.7;
    margin-bottom: 30px;
}

.btn {
    display: inline-block;
    padding: 15px 30px;
    background: var(--naranja);
    color: white;
    border: none;
    border-radius: 4px;
    text-decoration: none;
    font-weight: bold;
    cursor: pointer;
    transition: .3s;
}

.btn:hover {
    background: #e65300;
    transform: translateY(-3px);
}

/* SECCIONES */

section {
    padding: 75px 7%;
}

.titulo {
    text-align: center;
    margin-bottom: 40px;
}

.titulo h2 {
    font-size: 35px;
    font-weight: 900;
    text-transform: uppercase;
}

.titulo span {
    color: var(--naranja);
}

.titulo p {
    color: #777;
    margin-top: 10px;
}

/* CATEGORÍAS */

.categorias {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 25px;
}

.categoria {
    height: 300px;
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: end;
    padding: 30px;
    color: white;
    border-radius: 8px;
    overflow: hidden;
    transition: .3s;
}

.categoria:hover {
    transform: scale(1.02);
}

.categoria h3 {
    font-size: 30px;
    text-transform: uppercase;
}

.hombres {
    background-image: linear-gradient(0deg, #000b, transparent),
    url("https://images.unsplash.com/photo-1517836357463-d25dfeac3438?auto=format&fit=crop&w=900&q=80");
}

.mujeres {
    background-image: linear-gradient(0deg, #000b, transparent),
    url("https://images.unsplash.com/photo-1518310383802-640c2de311b2?auto=format&fit=crop&w=900&q=80");
}

/* PRODUCTOS */

.productos {
    background: var(--gris);
}

.filtros {
    display: flex;
    justify-content: center;
    gap: 12px;
    flex-wrap: wrap;
    margin-bottom: 30px;
}

.filtro {
    padding: 10px 20px;
    border: 1px solid #ddd;
    background: white;
    cursor: pointer;
    border-radius: 25px;
}

.filtro.activo,
.filtro:hover {
    background: var(--naranja);
    color: white;
    border-color: var(--naranja);
}

.productos-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 22px;
}

.producto {
    background: white;
    border-radius: 8px;
    overflow: hidden;
    transition: .3s;
}

.producto:hover {
    transform: translateY(-7px);
    box-shadow: 0 8px 20px #0002;
}

.producto img {
    width: 100%;
    height: 260px;
    object-fit: cover;
}

.producto-info {
    padding: 18px;
}

.producto-info small {
    color: var(--naranja);
    font-weight: bold;
}

.producto-info h3 {
    margin: 9px 0;
    font-size: 17px;
}

.precio {
    font-size: 21px;
    font-weight: 900;
    margin: 12px 0;
}

.agregar {
    width: 100%;
    padding: 12px;
    border: none;
    background: var(--negro);
    color: white;
    cursor: pointer;
    border-radius: 4px;
}

.agregar:hover {
    background: var(--naranja);
}

/* PROMOCIÓN */

.promocion {
    background: var(--negro);
    color: white;
    text-align: center;
}

.promocion h2 {
    font-size: 38px;
    margin-bottom: 15px;
}

.promocion span {
    color: var(--naranja);
}

/* NOSOTROS */

.nosotros {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 45px;
    align-items: center;
}

.nosotros img {
    width: 100%;
    border-radius: 8px;
}

.nosotros h2 {
    font-size: 35px;
    margin-bottom: 20px;
}

.nosotros h2 span {
    color: var(--naranja);
}

.nosotros p {
    line-height: 1.8;
    color: #666;
    margin-bottom: 15px;
}

/* CONTACTO */

.contacto {
    background: var(--gris);
    text-align: center;
}

.contacto p {
    margin: 12px;
    color: #555;
}

.contacto a {
    color: var(--naranja);
    text-decoration: none;
    font-weight: bold;
}

/* CARRITO */

.carrito {
    position: fixed;
    top: 0;
    right: -450px;
    width: min(400px, 100%);
    height: 100vh;
    background: white;
    z-index: 300;
    padding: 25px;
    box-shadow: -5px 0 20px #0003;
    transition: .3s;
    overflow-y: auto;
}

.carrito.abierto {
    right: 0;
}

.carrito-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 25px;
}

.cerrar {
    border: none;
    background: none;
    font-size: 28px;
    cursor: pointer;
}

.item-carrito {
    display: flex;
    justify-content: space-between;
    gap: 10px;
    padding: 15px 0;
    border-bottom: 1px solid #ddd;
}

.item-carrito button {
    border: none;
    color: red;
    background: none;
    cursor: pointer;
}

.total {
    font-size: 22px;
    font-weight: bold;
    margin: 25px 0;
}

.whatsapp {
    width: 100%;
    background: #20b85a;
    color: white;
    padding: 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
}

.overlay {
    display: none;
    position: fixed;
    inset: 0;
    background: #0008;
    z-index: 200;
}

.overlay.visible {
    display: block;
}

/* PIE DE PÁGINA */

footer {
    background: var(--negro);
    color: white;
    text-align: center;
    padding: 30px 15px;
}

footer span {
    color: var(--naranja);
}

footer p {
    margin: 8px;
    color: #aaa;
}

/* RESPONSIVE */

@media(max-width: 900px) {
    .productos-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    nav {
        gap: 12px;
    }
}

@media(max-width: 600px) {
    header {
        flex-wrap: wrap;
        gap: 15px;
    }

    nav {
        width: 100%;
        justify-content: center;
        flex-wrap: wrap;
    }

    .hero {
        min-height: 480px;
        padding: 40px 7%;
    }

    .categorias,
    .nosotros {
        grid-template-columns: 1fr;
    }

    .productos-grid {
        grid-template-columns: 1fr 1fr;
        gap: 12px;
    }

    .producto img {
        height: 180px;
    }

    .producto-info {
        padding: 12px;
    }

    .titulo h2 {
        font-size: 27px;
    }
}

@media(max-width: 380px) {
    .productos-grid {
        grid-template-columns: 1fr;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">ATH<span>LEX</span></div>

    <nav>
        <a href="#inicio">Inicio</a>
        <a href="#categorias">Categorías</a>
        <a href="#productos">Productos</a>
        <a href="#nosotros">Nosotros</a>
        <a href="#contacto">Contacto</a>
        <button class="carrito-btn" onclick="abrirCarrito()">
            🛒 Carrito (<span id="cantidad">0</span>)
        </button>
    </nav>
</header>

<main>

<section class="hero" id="inicio">
    <div class="hero-content">
        <h1>SUPERA TUS <span>LÍMITES.</span></h1>
        <p>
            No se trata solamente de entrenar, se trata de
            demostrar de qué estás hecho. Descubre nuestra
            colección de ropa deportiva y lleva tu rendimiento
            al siguiente nivel.
        </p>
        <a href="#productos" class="btn">EXPLORAR COLECCIÓN</a>
    </div>
</section>

<section id="categorias">
    <div class="titulo">
        <h2>ELIGE TU <span>ESTILO</span></h2>
        <p>Encuentra tu outfit deportivo ideal.</p>
    </div>

    <div class="categorias">
        <a href="#productos" class="categoria hombres">
            <h3>Hombres</h3>
        </a>

        <a href="#productos" class="categoria mujeres">
            <h3>Mujeres</h3>
        </a>
    </div>
</section>

<section class="productos" id="productos">
    <div class="titulo">
        <h2>NUESTROS <span>PRODUCTOS</span></h2>
        <p>Calidad, comodidad y estilo en cada movimiento.</p>
    </div>

    <div class="filtros">
        <button class="filtro activo" onclick="filtrar('todos',this)">Todos</button>
        <button class="filtro" onclick="filtrar('hombres',this)">Hombres</button>
        <button class="filtro" onclick="filtrar('mujeres',this)">Mujeres</button>
        <button class="filtro" onclick="filtrar('accesorios',this)">Accesorios</button>
    </div>

    <div class="productos-grid" id="lista-productos"></div>
</section>

<section class="promocion">
    <h2>ENTRENA CON <span>ACTITUD.</span></h2>
    <p>Tu esfuerzo merece un estilo que esté a tu altura.</p>
    <br>
    <a href="#productos" class="btn">VER PRODUCTOS</a>
</section>

<section class="nosotros" id="nosotros">
    <div>
        <img src="https://images.unsplash.com/photo-1517836357463-d25dfeac3438?auto=format&fit=crop&w=1000&q=85"
        alt="Entrenamiento deportivo">
    </div>

    <div>
        <h2>SOMOS <span>ATHLEX</span></h2>

        <p>
            ATHLEX nace con la idea de ofrecer ropa deportiva
            que combine comodidad, diseño y funcionalidad.
        </p>

        <p>
            Buscamos acompañar a cada persona en sus actividades
            físicas y en su día a día, brindando prendas que
            representen energía, disciplina y superación.
        </p>

        <p>
            Nuestra filosofía es simple: superar tus límites
            comienza con creer en ti mismo.
        </p>
    </div>
</section>

<section class="contacto" id="contacto">
    <div class="titulo">
        <h2>CONTÁCTANOS</h2>
        <p>Estamos listos para atenderte.</p>
    </div>

    <p><strong>Marca:</strong> ATHLEX</p>
    <p><strong>Ubicación:</strong> Quetzaltenango, Guatemala</p>
    <p><strong>WhatsApp:</strong> <a id="contacto-whatsapp"
    href="#" target="_blank">Configurar número</a></p>
    <p><strong>Redes sociales:</strong> ATHLEX</p>
</section>

</main>

<footer>
    <div class="logo">ATH<span>LEX</span></div>
    <p>SUPERA TUS LÍMITES.</p>
    <p>© 2026 ATHLEX. Todos los derechos reservados.</p>
</footer>

<!-- CARRITO -->

<div class="overlay" id="overlay" onclick="cerrarCarrito()"></div>

<aside class="carrito" id="carrito">
    <div class="carrito-header">
        <h2>Tu carrito</h2>
        <button class="cerrar" onclick="cerrarCarrito()">×</button>
    </div>

    <div id="contenido-carrito">
        <p>Tu carrito está vacío.</p>
    </div>

    <div class="total">
        Total: Q<span id="total">0.00</span>
    </div>

    <button class="whatsapp" onclick="comprarWhatsApp()">
        REALIZAR PEDIDO POR WHATSAPP
    </button>
</aside>

<script>

// CONFIGURACIÓN DE LA TIENDA

// Reemplaza este número por tu WhatsApp.
// Formato: código de país + número, sin espacios.
const NUMERO_WHATSAPP = "50200000000";

// PRODUCTOS DE EJEMPLO

const productos = [
    {
        id: 1,
        nombre: "Camiseta deportiva ATHLEX",
        precio: 125,
        categoria: "hombres",
        imagen: "https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?auto=format&fit=crop&w=700&q=80"
    },
    {
        id: 2,
        nombre: "Conjunto deportivo",
        precio: 225,
        categoria: "mujeres",
        imagen: "https://images.unsplash.com/photo-1518310383802-640c2de311b2?auto=format&fit=crop&w=700&q=80"
    },
    {
        id: 3,
        nombre: "Sudadera deportiva",
        precio: 250,
        categoria: "hombres",
        imagen: "https://images.unsplash.com/photo-1556821840-3a63f95609a7?auto=format&fit=crop&w=700&q=80"
    },
    {
        id: 4,
        nombre: "Leggings deportivos",
        precio: 175,
        categoria: "mujeres",
        imagen: "https://images.unsplash.com/photo-1506629905607-d9c297d7e5d5?auto=format&fit=crop&w=700&q=80"
    },
    {
        id: 5,
        nombre: "Short deportivo",
        precio: 110,
        categoria: "hombres",
        imagen: "https://images.unsplash.com/photo-1591195853828-11db59a44f6b?auto=format&fit=crop&w=700&q=80"
    },
    {
        id: 6,
        nombre: "Top deportivo",
        precio: 135,
        categoria: "mujeres",
        imagen: "https://images.unsplash.com/photo-1503342217505-b0a15ec3261c?auto=format&fit=crop&w=700&q=80"
    },
    {
        id: 7,
        nombre: "Gorra deportiva",
        precio: 85,
        categoria: "accesorios",
        imagen: "https://images.unsplash.com/photo-1588850561407-ed78c282e89b?auto=format&fit=crop&w=700&q=80"
    },
    {
        id: 8,
        nombre: "Bolso deportivo",
        precio: 195,
        categoria: "accesorios",
        imagen: "https://images.unsplash.com/photo-1553062407-98eeb64c6a62?auto=format&fit=crop&w=700&q=80"
    }
];

let carrito = [];

// MOSTRAR PRODUCTOS

function mostrarProductos(categoria = "todos") {
    const lista = document.getElementById("lista-productos");

    const filtrados = categoria === "todos"
        ? productos
        : productos.filter(p => p.categoria === categoria);

    lista.innerHTML = filtrados.map(p => `
        <article class="producto">
            <img src="${p.imagen}" alt="${p.nombre}"
            loading="lazy">
            <div class="producto-info">
                <small>ATHLEX COLLECTION</small>
                <h3>${p.nombre}</h3>
                <div class="precio">Q${p.precio.toFixed(2)}</div>
                <button class="agregar"
                onclick="agregarCarrito(${p.id})">
                    AGREGAR AL CARRITO
                </button>
            </div>
        </article>
    `).join("");
}

// FILTRAR PRODUCTOS

function filtrar(categoria, boton) {
    document.querySelectorAll(".filtro").forEach(b => {
        b.classList.remove("activo");
    });

    boton.classList.add("activo");
    mostrarProductos(categoria);
}

// AGREGAR PRODUCTOS

function agregarCarrito(id) {
    const producto = productos.find(p => p.id === id);
    const existente = carrito.find(p => p.id === id);

    if (existente) {
        existente.cantidad++;
    } else {
        carrito.push({...producto, cantidad: 1});
    }

    actualizarCarrito();
    abrirCarrito();
}

// ACTUALIZAR CARRITO

function actualizarCarrito() {
    const contenido = document.getElementById("contenido-carrito");

    let total = 0;
    let cantidad = 0;

    if (carrito.length === 0) {
        contenido.innerHTML = "<p>Tu carrito está vacío.</p>";
    } else {
        contenido.innerHTML = carrito.map(p => {
            total += p.precio * p.cantidad;
            cantidad += p.cantidad;

            return `
                <div class="item-carrito">
                    <div>
                        <strong>${p.nombre}</strong>
                        <p>Q${p.precio.toFixed(2)} x ${p.cantidad}</p>
                    </div>
                    <button onclick="eliminarProducto(${p.id})">
                        Eliminar
                    </button>
                </div>
            `;
        }).join("");
    }

    document.getElementById("total").textContent = total.toFixed(2);
    document.getElementById("cantidad").textContent = cantidad;
}

// ELIMINAR PRODUCTOS

function eliminarProducto(id) {
    const producto = carrito.find(p => p.id === id);

    if (producto.cantidad > 1) {
        producto.cantidad--;
    } else {
        carrito = carrito.filter(p => p.id !== id);
    }

    actualizarCarrito();
}

// ABRIR Y CERRAR CARRITO

function abrirCarrito() {
    document.getElementById("carrito").classList.add("abierto");
    document.getElementById("overlay").classList.add("visible");
}

function cerrarCarrito() {
    document.getElementById("carrito").classList.remove("abierto");
    document.getElementById("overlay").classList.remove("visible");
}

// PEDIDO POR WHATSAPP

function comprarWhatsApp() {
    if (carrito.length === 0) {
        alert("Agrega productos antes de realizar tu pedido.");
        return;
    }

    const numero = NUMERO_WHATSAPP;

    if (!/^\d{10,15}$/.test(numero) || /^0+$/.test(numero)) {
        alert("Configura primero el número de WhatsApp de ATHLEX en el código.");
        return;
    }

    let mensaje = "¡Hola! Quiero realizar un pedido en ATHLEX:\n\n";

    let total = 0;

    carrito.forEach(p => {
        mensaje += `${p.nombre} - Cantidad: ${p.cantidad} - Q${(p.precio * p.cantidad).toFixed(2)}\n`;
        total += p.precio * p.cantidad;
    });

    mensaje += `\nTOTAL: Q${total.toFixed(2)}`;
    mensaje += "\n\nQuisiera información sobre disponibilidad y entrega.";

    const url = "https://wa.me/" + numero + "?text=" +
        encodeURIComponent(mensaje);

    window.open(url, "_blank");
}

// INICIALIZAR PÁGINA

mostrarProductos();
actualizarCarrito();

document.getElementById("contacto-whatsapp").href =
    "https://wa.me/" + NUMERO_WHATSAPP;

</script>

</body>
</html>
