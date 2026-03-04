<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Café Aroma</title>

    <style>
        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Corpo */
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background: linear-gradient(135deg, #f5f0e6, #e6d5c3);
            color: #333;
        }

        /* Header */
        header {
            background: linear-gradient(to right, #6b3e26, #4b2e1f);
            color: white;
            text-align: center;
            padding: 50px 20px;
        }

        header h1 {
            font-size: 3rem;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.2rem;
            opacity: 0.9;
        }

        /* Navegação */
        nav {
            background-color: #3b2418;
            display: flex;
            justify-content: center;
            padding: 15px;
            gap: 30px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            position: relative;
            transition: 0.3s;
        }

        nav a::after {
            content: "";
            position: absolute;
            width: 0%;
            height: 2px;
            background: #ffd9b3;
            left: 0;
            bottom: -5px;
            transition: 0.3s;
        }

        nav a:hover::after {
            width: 100%;
        }

        /* Conteúdo */
        .conteudo {
            text-align: center;
            padding: 80px 20px;
        }

        .conteudo h2 {
            font-size: 2.2rem;
            margin-bottom: 20px;
            color: #6b3e26;
        }

        .conteudo p {
            max-width: 600px;
            margin: 0 auto 40px;
            line-height: 1.6;
            font-size: 1.1rem;
        }

        /* Botão */
        .botao {
            display: inline-block;
            background: #6b3e26;
            color: white;
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .botao:hover {
            background: #4b2e1f;
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.3);
        }

        /* Responsividade */
        @media (max-width: 600px) {
            nav {
                flex-direction: column;
                gap: 15px;
            }

            header h1 {
                font-size: 2.2rem;
            }
        }
    </style>

</head>
<body>

    <header>
        <h1>Café Aroma</h1>
        <p>O melhor café da cidade ☕</p>
    </header>

    <nav>
        <a href="#">Início</a>
        <a href="#">Sobre</a>
        <a href="cardapio.html">Cardápio</a>
        <a href="#">Contato</a>
    </nav>

    <section class="conteudo">
        <h2>Bem-vindo!</h2>
        <p>
            No Café Aroma você encontra cafés especiais, salgados fresquinhos 
            e um ambiente aconchegante para relaxar ou trabalhar.
        </p>

        <a href="cardapio.html" class="botao">Ver Cardápio</a>
    </section>

</body>
</html>
