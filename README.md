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
    background:#f4f6f5;
}

header{
    background:#14532d;
    color:white;
    text-align:center;
    padding:20px;
}

.seccion{
    background:white;
    margin:20px;
    padding:25px;
    border-radius:12px;
    box-shadow:0 2px 8px rgba(0,0,0,0.05);
}

.productos{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(160px,1fr));
    gap:15px;
    padding:20px;
}

.card{
    background:white;
    border-radius:10px;
    padding:8px;
    box-shadow:0 2px 6px rgba(0,0,0,0.1);
    text-align:center;
    font-size:12px;
}

.card img{
    width:100%;
    height:65px;
    object-fit:cover;
    border-radius:6px;
}

.card h4{
    font-size:13px;
    margin:5px 0;
}

.card p{
    font-size:11px;
    color:#555;
}

.card select{
    width:100%;
    padding:4px;
    margin:5px 0;
    font-size:11px;
}

button{
    background:#14532d;
    color:white;
    border:none;
    padding:5px;
    width:100%;
    border-radius:5px;
    cursor:pointer;
    font-size:11px;
}

button:hover{
    background:#16a34a;
}

.carrito{
    position:fixed;
    right:15px;
    top:120px;
    background:white;
    width:220px;
    padding:15px;
    border-radius:10px;
    box-shadow:0 4px 10px rgba(0,0,0,0.2);
    font-size:12px;
}

footer{
    background:#14532d;
    color:white;
    text-align:center;
    padding:15px;
    margin-top:20px;
}
</style>
</head>

<body>

<header>
<h1>PetGreen</h1>
<p>Alimentos Orgánicos para Mascotas</p>
</header>

<!-- INFORMACIÓN DE LA EMPRESA PRIMERO -->

<section class="seccion">
<h2>¿De qué trata nuestra empresa?</h2>
<p>PetGreen es una empresa dedicada a la comercialización de alimentos orgánicos para mascotas en Bogotá. Ofrecemos productos naturales, saludables y sostenibles que mejoran la calidad de vida de perros y gatos mientras cuidamos el medio ambiente.</p>

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

<!-- PRODUCTOS -->

<section class="productos">

<div class="card">
<img src="https://images.unsplash.com/photo-1601758228041-f3b2795255f1">
<h4>Concentrado Orgánico</h4>
<p>Pollo natural, arroz integral y vegetales ecológicos.</p>
<select>
<option value="20000">1kg - $20.000</option>
<option value="38000">3kg - $38.000</option>
<option value="55000">5kg - $55.000</option>
<option value="75000">10kg - $75.000</option>
<option value="80000">Bulto 20kg - $80.000</option>
</select>
<button onclick="agregar(this)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1583512603805-3cc6b41f3edb">
<h4>Alimento Deshidratado</h4>
<p>Carne natural sin conservantes artificiales.</p>
<select>
<option value="22000">1kg - $22.000</option>
<option value="40000">3kg - $40.000</option>
<option value="60000">5kg - $60.000</option>
<option value="78000">10kg - $78.000</option>
<option value="80000">Bulto 20kg - $80.000</option>
</select>
<button onclick="agregar(this)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1568640347023-a616a30bc3bd">
<h4>Snacks Ecológicos</h4>
<p>Premios naturales con proteína vegetal orgánica.</p>
<select>
<option value="10000">250g - $10.000</option>
<option value="18000">500g - $18.000</option>
<option value="32000">1kg - $32.000</option>
<option value="70000">5kg - $70.000</option>
</select>
<button onclick="agregar(this)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1548767797-d8c844163c4c">
<h4>Línea Premium Bio</h4>
<p>Receta gourmet con empaques biodegradables.</p>
<select>
<option value="25000">1kg - $25.000</option>
<option value="45000">3kg - $45.000</option>
<option value="65000">5kg - $65.000</option>
<option value="80000">Bulto 20kg - $80.000</option>
</select>
<button onclick="agregar(this)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1600804340584-c7db2eacf0bf">
<h4>Mix Natural Canino</h4>
<p>Res orgánica, quinoa y zanahoria natural.</p>
<select>
<option value="21000">1kg - $21.000</option>
<option value="39000">3kg - $39.000</option>
<option value="58000">5kg - $58.000</option>
<option value="76000">10kg - $76.000</option>
</select>
<button onclick="agregar(this)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1598137262014-8c5c9d6b5b9f">
<h4>Fórmula Verde Felina</h4>
<p>Pescado natural y espinaca ecológica.</p>
<select>
<option value="23000">1kg - $23.000</option>
<option value="42000">3kg - $42.000</option>
<option value="63000">5kg - $63.000</option>
<option value="80000">Bulto 20kg - $80.000</option>
</select>
<button onclick="agregar(this)">Agregar</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1589927986089-35812388d1b4">
<h4>EcoBalance Senior</h4>
<p>Receta orgánica especial para mascotas mayores.</p>
<select>
<option value="24000">1kg - $24.000</option>
<option value="45000">3kg - $45.000</option>
<option value="67000">5kg - $67.000</option>
<option value="80000">10kg - $80.000</option>
</select>
<button onclick="agregar(this)">Agregar</button>
</div>

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

function agregar(boton){
    let card = boton.parentElement;
    let nombre = card.querySelector("h4").textContent;
    let precio = parseInt(card.querySelector("select").value);
    let texto = card.querySelector("select").selectedOptions[0].text;

    let lista = document.getElementById("lista");
    let item = document.createElement("li");
    item.textContent = nombre + " (" + texto + ")";
    lista.appendChild(item);

    total += precio;
    document.getElementById("total").textContent = total;
}
</script>

</body>
</html>
