<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PetGreen</title>

<style>
body{
    margin:0;
    font-family:Arial, sans-serif;
    background:#f4f4f4;
}

header{
    background:#14532d;
    color:white;
    text-align:center;
    padding:20px;
}

.banner{
    background:#16a34a;
    color:white;
    text-align:center;
    padding:40px 20px;
}

.seccion{
    padding:40px 20px;
    background:white;
    margin:20px;
    border-radius:10px;
}

.productos{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(160px,1fr));
    gap:15px;
    padding:20px;
}

.card{
    background:white;
    border-radius:8px;
    padding:10px;
    box-shadow:0 3px 8px rgba(0,0,0,0.1);
    text-align:center;
}

.card img{
    width:100%;
    height:100px;
    object-fit:cover;
    border-radius:6px;
}

.card h4{
    font-size:14px;
    margin:8px 0;
}

.card p{
    font-size:12px;
    color:#555;
}

.precio{
    color:#16a34a;
    font-weight:bold;
}

button{
    background:#14532d;
    color:white;
    border:none;
    padding:6px;
    width:100%;
    border-radius:5px;
    cursor:pointer;
    font-size:12px;
}

button:hover{
    background:#16a34a;
}

.carrito{
    position:fixed;
    right:15px;
    top:100px;
    background:white;
    width:200px;
    padding:15px;
    border-radius:8px;
    box-shadow:0 4px 10px rgba(0,0,0,0.2);
    font-size:13px;
}

footer{
    background:#14532d;
    color:white;
    text-align:center;
    padding:15px;
    margin-top:30px;
}
</style>
</head>

<body>

<header>
<h1>PetGreen</h1>
<p>Alimentos Orgánicos para Mascotas</p>
</header>

<section class="banner">
<h2>Nutrición Natural y Sostenible en Bogotá</h2>
</section>

<section class="productos">

<div class="card">
<img src="https://images.unsplash.com/photo-1601758228041-f3b2795255f1">
<h4>Concentrado Orgánico</h4>
<p>Pollo natural y vegetales ecológicos.</p>
<div class="precio">$48.000</div>
<button onclick="agregar('Concentrado Orgánico',48000)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1583512603805-3cc6b41f3edb">
<h4>Alimento Deshidratado</h4>
<p>Carne natural sin conservantes.</p>
<div class="precio">$42.000</div>
<button onclick="agregar('Alimento Deshidratado',42000)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1568640347023-a616a30bc3bd">
<h4>Snacks Ecológicos</h4>
<p>Premios saludables para perros y gatos.</p>
<div class="precio">$26.000</div>
<button onclick="agregar('Snacks Ecológicos',26000)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1548767797-d8c844163c4c">
<h4>Línea Premium Bio</h4>
<p>Receta gourmet con empaque biodegradable.</p>
<div class="precio">$65.000</div>
<button onclick="agregar('Línea Premium Bio',65000)">Agregar</button>
</div>

</section>

<section class="seccion">
<h2>Misión</h2>
<p>Somos una empresa dedicada a la comercialización de alimentos saludables y ecológicos para mascotas, ofreciendo productos naturales de alta calidad que contribuyen al bienestar animal y al cuidado del medio ambiente.</p>

<h2>Visión</h2>
<p>Para el año 2030, ser reconocidos en Bogotá como líderes en la comercialización de alimentos sostenibles para mascotas, destacándonos por nuestra innovación y compromiso ambiental.</p>

<h2>Objetivos</h2>
<ul>
<li>Implementar empaques biodegradables en la mayoría de nuestros productos.</li>
<li>Trabajar con proveedores responsables y sostenibles.</li>
<li>Desarrollar productos innovadores basados en economía circular.</li>
<li>Promover el consumo responsable en Bogotá y Colombia.</li>
</ul>
</section>

<div class="carrito">
<h3>🛒 Carrito</h3>
<ul id="lista"></ul>
<p><strong>Total: $<span id="total">0</span></strong></p>
</div>

<footer>
© 2026 PetGreen - Bogotá, Colombia
</footer>

<script>
let total = 0;

function agregar(nombre, precio){
    let lista = document.getElementById("lista");
    let item = document.createElement("li");
    item.textContent = nombre + " - $" + precio;
    lista.appendChild(item);
    total += precio;
    document.getElementById("total").textContent = total;
}
</script>

</body>
</html>


