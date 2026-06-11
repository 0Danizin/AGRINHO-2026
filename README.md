<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro Forte, Futuro Sustentável</title>
    <style>
        /* Reset básico e fontes */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f4f7f5;
            color: #333;
            line-height: 1.6;
        }

        /* Cabeçalho e Navegação */
        header {
            background-color: #1b4332;
            color: #ffffff;
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #52b788;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            color: #ffffff;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: #52b788;
        }

        /* Banner Principal (Hero) */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&q=80&w=1470') no-repeat center center/cover;
            height: 70vh;
            color: #ffffff;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 1rem;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            max-width: 800px;
        }

        .hero p {
            font-size: 1.25rem;
            max-width: 600px;
            margin-bottom: 2rem;
        }

        .btn {
            background-color: #52b788;
            color: #1b4332;
            padding: 0.75rem 2rem;
            border: none;
            border-radius: 5px;
            font-weight: bold;
            text-decoration: none;
            transition: background-color 0.3s, transform 0.2s;
        }

        .btn:hover {
            background-color: #74c69d;
            transform: translateY(-2px);
        }

        /* Seções Gerais */
        section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            color: #1b4332;
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: #52b788;
            margin: 10px auto 0;
            border-radius: 2px;
        }

        /* Sobre / O Equilíbrio */
        .sobre-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .sobre-img img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        /* Pilares / Destaques */
        .pilares {
            background-color: #e9f5ed;
            max-width: 100%;
        }

        .grid-pilares {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .pilar-card {
            background: #ffffff;
            padding: 2.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: center;
            transition: transform 0.3s;
        }

        .pilar-card:hover {
            transform: translateY(-5px);
        }

        .pilar-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .pilar-card h3 {
            color: #2d6a4f;
            margin-bottom: 1rem;
        }

        /* Contato */
        .contato-form {
            max-width: 600px;
            margin: 0 auto;
            background: #ffffff;
            padding: 2.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: #1b4332;
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 1rem;
        }

        .form-group input:focus, .form-group textarea:focus {
            outline: none;
            border-color: #52b788;
        }

        /* Rodapé */
        footer {
            background-color: #1b4332;
            color: #ffffff;
            text-align: center;
            padding: 2rem;
            font-size: 0.9rem;
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 1rem;
            }
            nav ul li {
                margin: 0 1rem;
            }
            .hero h1 {
                font-size: 2rem;
            }
            .sobre-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo">AgroForte 🌱</div>
            <nav>
                <ul>
                    <li><a href="#home">Início</a></li>
                    <li><a href="#sobre">O Equilíbrio</a></li>
                    <li><a href="#pilares">Pilares</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home" class="hero" style="max-width:100%; padding:0;">
        <h1>Agro Forte, Futuro Sustentável</h1>
        <p>Alimentando o mundo hoje, preservando a terra para as próximas gerações através do equilíbrio e da tecnologia.</p>
        <a href="#sobre" class="btn">Saiba Mais</a>
    </section>

    <section id="sobre">
        <h2 class="section-title">O Equilíbrio Necessário</h2>
        <div class="sobre-container">
            <div class="sobre-texto">
                <p>O grande desafio do século XXI é aumentar a produção de alimentos para uma população global em crescimento, enquanto reduzimos drasticamente o impacto ambiental. O <strong>Agro Forte</strong> não caminha separado da preservação; ele depende dela.</p>
                <br>
                <p>Através de práticas modernas, manejo consciente do solo e respeito à biodiversidade, mostramos que é possível ter uma produção recorde que caminha lado a lado com a conservação das nossas florestas e recursos hídricos.</p>
            </div>
            <div class="sobre-img">
                <img src="https://images.unsplash.com/photo-1625246333195-78d9c38ad451?auto=format&fit=crop&q=80&w=600" alt="Plantação jovem com tecnologia de irrigação moderna">
            </div>
        </div>
    </section>

    <section id="pilares" class="pilares">
        <h2 class="section-title">Nossos Pilares</h2>
        <div class="grid-pilares">
            <div class="pilar-card">
                <div class="pilar-icon">🚜</div>
                <h3>Tecnologia Verde</h3>
                <p>Uso de agricultura de precisão, drones e sensores para otimizar insumos, evitando desperdícios e protegendo o solo.</p>
            </div>
            <div class="pilar-card">
                <div class="pilar-icon">💧</div>
                <h3>Manejo Hídrico</h3>
                <p>Sistemas inteligentes de irrigação e captação de água da chuva que garantem a produção sem esgotar as fontes naturais.</p>
            </div>
            <div class="pilar-card">
                <div class="pilar-icon">🌳</div>
                <h3>Reflorestamento</h3>
                <p>Integração Lavoura-Pecuária-Floresta (ILPF) para recuperar áreas degradadas e sequestrar carbono da atmosfera.</p>
            </div>
        </div>
    </section>

    <section id="contato">
        <h2 class="section-title">Fale Conosco</h2>
        <div class="contato-form">
            <form action="#" method="POST" onsubmit="event.preventDefault(); alert('Mensagem enviada com sucesso! (Simulação)');">
                <div class="form-group">
                    <label for="nome">Nome:</label>
                    <input type="text" id="nome" required placeholder="Seu nome completo">
                </div>
                <div class="form-group">
                    <label for="email">E-mail:</label>
                    <input type="email" id="email" required placeholder="seu.email@exemplo.com">
                </div>
                <div class="form-group">
                    <label for="mensagem">Mensagem:</label>
                    <textarea id="mensagem" rows="5" required placeholder="Como podemos construir um futuro mais sustentável juntos?"></textarea>
                </div>
                <button type="submit" class="btn" style="width: 100%; cursor: pointer;">Enviar Mensagem</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 AgroForte Sustentável. Todos os direitos reservados.</p>
        <p>Desenvolvido focado no futuro do nosso planeta.</p>
    </footer>

</body>
</html>
