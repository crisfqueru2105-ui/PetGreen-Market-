<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>PetOrganic - Alimentos Orgánicos para Mascotas</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
            font-family: Arial, Helvetica, sans-serif;
        }

        body{
            background:#f5f5f5;
        }

        header{
            background:#111;
            color:white;
            padding:20px;
            display:flex;
            justify-content:space-between;
            align-items:center;
        }

        header h1{
            font-size:22px;
        }

        nav a{
            color:white;
            text-decoration:none;
            margin-left:20px;
            font-size:14px;
        }

        .banner{
            background:linear-gradient(to right,#2ecc71,#27ae60);
            color:white;
            padding:60px 20px;
            text-align:center;
        }

        .banner h2{
            font-size:40px;
            margin-bottom:10px;
        }

        .productos{
            padding:40px 20px;
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
            gap:20px;
        }

        .card{
            background:white;
            border-radius:10px;
            overflow:hidden;
            box-shadow:0 5px 15px rgba(0,0,0,0.1);
            transition:0.3s;
        }

        .card:hover{
            transform:scale(1.05);
        }

        .card img{
            width:100%;
            height:200px;
            object-fit:cover;
        }

        .card-body{
            padding:15px;
        }

        .card-body h3{
            font-size:18px;
            margin-bottom:10px;
        }

        .precio{
            color:#27ae60;
            font-weight:bold;
            margin-bottom:10px;
        }

        .btn{
            display:block;
            background:#111;
            color:white;
            text-align:center;
            padding:10px;
            text-decoration:none;
            border-radius:5px;
            transition:0.3s;
        }

        .btn:hover{
            background:#27ae60;
        }

        footer{
            background:#111;
            color:white;
            text-align:center;
            padding:20px;
            margin-top:40px;
        }

        @media(max-width:600px){
            .banner h2{
                font-size:28px;
            }
        }
    </style>
</head>

<body>

<header>
    <h1>PetOrganic</h1>
    <nav>
        <a href="#">Inicio</a>
        <a href="#">Productos</a>
        <a href="#">Nosotros</a>
        <a href="#">Contacto</a>
    </nav>
</header>

<section class="banner">
    <h2>Alimentos Orgánicos Premium</h2>
    <p>Nutrición 100% natural para perros y gatos en Bogotá</p>
</section>

<section class="productos">

    <div class="card">
        <img src="https://images.unsplash.com/photo-1583337130417-3346a1be7dee" alt="Comida orgánica perro">
        <div class="card-body">
            <h3>Dog Natural Mix</h3>
            <p class="precio">$45.000</p>
            <a href="#" class="btn">Comprar</a>
        </div>
    </div>

    <div class="card">
        <img src="https://images.unsplash.com/photo-1598135753163-6167c1a1ad65" alt="Comida orgánica gato">
        <div class="card-body">
            <h3>Cat Organic Premium</h3>
            <p class="precio">$39.000</p>
            <a href="#" class="btn">Comprar</a>
        </div>
    </div>

    <div class="card">
        <img src="https://images.unsplash.com/photo-1601758125946-6ec2ef64daf8" alt="Snacks naturales">
        <div class="card-body">
            <h3>Snacks Naturales</h3>
            <p class="precio">$25.000</p>
            <a href="#" class="btn">Comprar</a>
        </div>
    </div>

</section>

<footer>
    <p>© 2026 PetOrganic - Bogotá, Colombia</p>
</footer>

</body>
</html>

