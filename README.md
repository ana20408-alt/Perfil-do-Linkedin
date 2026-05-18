<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Perfil LinkedIn</title>

    <style>


        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
        }

        /* body */

        body{
            background:#f3f2ef;
            font-family: Arial, Helvetica, sans-serif;
            color:#000;
        }

        /* NAVBAR */

        .navbar{
            width:100%;
            height:60px;

            background:white;

            display:flex;
            align-items:center;
            justify-content:space-around;

            border-bottom:1px solid #ddd;

            position:sticky;
            top:0;

            z-index:1000;
        }
        
        .navbar input{
            width:280px;

            padding:10px;

            border:none;
            border-radius:6px;

            background:#eef3f8;

            outline:none;
        }

        .navbar nav{
            display:flex;
            gap:25px;
        }

        .navbar nav a{
            text-decoration:none;
            color:#666;

            font-size:14px;
            font-weight:bold;

            transition:0.3s;
        }

        .navbar nav a:hover{
            color:#000;
        }

        /* CONTAINER */

        .container{
            width:800px;
            margin:30px auto;
        }

        /* PERFIL */

        .perfil{
            background:white;

            border-radius:12px;

            overflow:hidden;

            position:relative;

            margin-bottom:20px;

            box-shadow:0 2px 10px rgba(0,0,0,0.05);
        }

        /* BANNER */

        .banner{
            height:220px;

            background-image:url('https://i.ibb.co/dsLzXf9c/20240716-142525.jpg"');

            background-size:cover;
            background-position:center;
        }

        /* FOTO */

        .foto{
            width:160px;
            height:160px;

            object-fit:cover;

            border-radius:50%;

            border:5px solid white;

            position:absolute;

            top:120px;
            left:35px;

            z-index:10;

            box-shadow:0 2px 10px rgba(0,0,0,0.2);
        }

        /* INFORMAÇÕES */

        .info{
            padding:100px 35px 35px 35px;
        }

        .info h1{
            font-size:30px;
            margin-bottom:8px;
        }

        .info h2{
            font-size:18px;
            color:#555;
            margin-bottom:10px;
            font-weight:normal;
        }

        .info p{
            color:#777;
            margin-bottom:15px;
        }

        /* BOTÕES */

        .botoes{
            display:flex;
            gap:10px;
        }

        .btn-azul{
            background:#0a66c2;
            color:white;

            border:none;

            padding:10px 18px;

            border-radius:30px;

            cursor:pointer;

            font-weight:bold;

            transition:0.3s;
        }

        .btn-azul:hover{
            background:#004182;
        }

        .btn-branco{
            background:white;
            color:#0a66c2;

            border:1px solid #0a66c2;

            padding:10px 18px;

            border-radius:30px;

            cursor:pointer;

            font-weight:bold;

            transition:0.3s;
        }

        .btn-branco:hover{
            background:#eef3f8;
        }

        /* CARDS */

        .card{
            background:white;

            border-radius:12px;

            padding:25px;

            margin-bottom:20px;

            box-shadow:0 2px 10px rgba(0,0,0,0.05);
        }

        .card h3{
            font-size:22px;
            margin-bottom:20px;
        }

        /* EXPERIÊNCIAS */

        .item{
            padding-bottom:20px;

            margin-bottom:20px;

            border-bottom:1px solid #eee;
        }

        .item:last-child{
            border:none;
        }

        .item h4{
            font-size:18px;
            margin-bottom:5px;
        }

        .item p{
            color:#555;
            margin-top:5px;
            line-height:1.5;
        }

        .item span{
            color:gray;
            font-size:14px;
        }

        /* RESPONSIVO */

        @media(max-width:900px){

            .container{
                width:95%;
            }

            .navbar{
                flex-direction:column;
                height:auto;

                padding:15px;
                gap:10px;
            }

            .navbar input{
                width:100%;
            }

            .navbar nav{
                flex-wrap:wrap;
                justify-content:center;
            }

            .foto{
                width:120px;
                height:120px;

                top:140px;
            }

            .info{
                padding-top:70px;
            }

        }

    </style>
</head>

<body>

    <!-- NAVBAR -->
    <header class="navbar">

    
        <input type="text" placeholder="Pesquisar">

        

    </header>

    <!-- CONTAINER -->

    <main class="container">

        <!-- PERFIL -->

        <section class="perfil">

            <div class="banner"></div>

            <img
                src="https://i.ibb.co/dsLzXf9c/20240716-142525.jpg"
                alt="Foto Perfil"
                class="foto"
            >

            <div class="info">

                <h1>Kaory Nakai</h1>

                <h2>Análise e Desenvolvimento de Sistemas</h2>

                <p>Ivaté - Paraná - Brasil</p>

                <div class="botoes">

                    <button class="btn-azul">
                        Conectar
                    </button>

                    <button class="btn-branco">
                        Mensagem
                    </button>

                </div>

            </div>

        </section>

        <!-- SOBRE -->

        <section class="card">

            <h3>Sobre</h3>

            <p>
                Cursando Análise e Desenvolvimento de Sistemas.
            </p>

        </section>

        <!-- EXPERIÊNCIAS -->

        <section class="card">

            <h3>Experiência</h3>

            <div class="item">

                <h4>Freelance Software Engineer - Contabilidade Digital </h4>

                <span>Remoto • 2021 - 2022</span>

                <p>
                    Atuação no desenvolvimento completo de uma solução mobile.
                </p>

            </div>

        
        </section>

        <!-- FORMAÇÃO -->

        <section class="card">

            <h3>Formação Acadêmica</h3>

            <div class="item">

                <h4>Colégio Estadual Rachel de Queiroz</h4>

                <span>Ensino médio - Conclusão - 2025</span>

                <p>
                    Com o novo ensino médio, visa conectar o ensino ao mercado de trabalho e ao projeto de vida do estudante.
                </p>

            </div>

        </section>

    </main>

</body>
</html>
