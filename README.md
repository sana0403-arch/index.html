# index.html<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AgroTech - A Transformação Digital no Campo</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #2c3e50;
            background-color: #f8fafc;
        }

        /* Header / Navegação */
        header {
            background-color: #1e3a27;
            color: #ffffff;
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #4ade80;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        nav a {
            color: #ffffff;
            text-decoration: none;
            margin-left: 20px;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #4ade80;
        }

        /* Seção Principal (Hero) */
        .hero {
            background: linear-gradient(rgba(30, 58, 39, 0.8), rgba(30, 58, 39, 0.9)), 
                        url('https://images.unsplash.com/photo-1592982537447-744077110b90?auto=format&fit=crop&q=80&w=1200') no-repeat center center/cover;
            color: #ffffff;
            padding: 100px 20px;
            text-align: center;
        }

        .hero h1 {
            font-size: 42px;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .hero p {
            font-size: 18px;
            max-width: 800px;
            margin: 0 auto 30px auto;
            color: #e2e8f0;
        }

        /* Container do Conteúdo */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* Seções de Texto */
        .intro-section {
            text-align: center;
            margin-bottom: 60px;
        }

        .intro-section h2 {
            font-size: 32px;
            color: #1e3a27;
            margin-bottom: 20px;
            position: relative;
            display: inline-block;
        }

        .intro-section h2::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: #4ade80;
            margin: 10px auto 0 auto;
            border-radius: 2px;
        }

        .intro-section p {
            font-size: 16px;
            color: #4a5568;
            max-width: 900px;
            margin: 0 auto;
        }

        /* Grid de Tecnologias (Cards) */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .feature-card {
            background-color: #ffffff;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0,0,0,0.1);
        }

        .feature-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .feature-content {
            padding: 25px;
        }

        .feature-content h3 {
            font-size: 20px;
            color: #1e3a27;
            margin-bottom: 12px;
        }

        .feature-content p {
            font-size: 14px;
            color: #718096;
            line-height: 1.5;
        }

        /* Bloco de Sustentabilidade */
        .benefits-section {
            background-color: #edf2f7;
            padding: 60px 20px;
            border-radius: 12px;
            margin-top: 40px;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 40px;
        }

        .benefits-text {
            flex: 1;
            min-width: 300px;
        }

        .benefits-text h2 {
            font-size: 28px;
            color: #1e3a27;
            margin-bottom: 20px;
        }

        .benefits-text ul {
            list-style: none;
        }

        .benefits-text li {
            margin-bottom: 12px;
            padding-left: 28px;
            position: relative;
            font-size: 15px;
            color: #2d3748;
        }

        .benefits-text li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #22c55e;
            font-weight: bold;
            font-size: 18px;
        }

        .benefits-image {
            flex: 1;
            min-width: 300px;
        }

        .benefits-image img {
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }

        /* Rodapé */
        footer {
            background-color: #1a202c;
            color: #a0aec0;
            text-align: center;
            padding: 30px 20px;
            margin-top: 60px;
            font-size: 14px;
        }

        footer strong {
            color: #ffffff;
        }

        /* Responsividade */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 15px;
            }
            .hero h1 {
                font-size: 32px;
            }
            .benefits-section {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">🌱 AgroTech</div>
        <nav>
            <a href="#tecnologias">Tecnologias</a>
            <a href="#sustentabilidade">Sustentabilidade</a>
        </nav>
    </header>

    <section class="hero">
        <h1>A Revolução Tecnológica no Agronegócio</h1>
        <p>Unindo inovação, precisão e respeito ao meio ambiente para alimentar o futuro com alta produtividade.</p>
    </section>

    <main class="container">
        
        <section class="intro-section">
            <h2>O Campo Conectado</h2>
            <p>
                A integração entre tecnologia e agricultura transformou radicalmente o setor. 
                O agronegócio moderno vai muito além do trabalho manual: hoje, o campo utiliza dados em tempo real, 
                automação e inteligência para garantir maior eficiência, atender à crescente demanda global por alimentos 
                e preservar as riquezas naturais de forma sustentável.
            </p>
        </section>

        <section id="tecnologias">
            <div class="intro-section" style="margin-bottom: 20px;">
                <h2 style="font-size: 24px;">Inovações Tecnológicas</h2>
            </div>
            
            <div class="features-grid">
                <div class="feature-card">
                    <img src="https://images.unsplash.com/photo-1508614589041-895b88991e3e?auto=format&fit=crop&q=80&w=600" alt="Drone monitorando plantação">
                    <div class="feature-content">
                        <h3>Drones e Monitoramento</h3>
                        <p>Sobrevoam as lavouras capturando imagens em tempo real para identificar pragas, falhas de plantio e áreas que necessitam de atenção imediata.</p>
                    </div>
                </div>

                <div class="feature-card">
                    <img src="https://images.unsplash.com/photo-1560493676-04071c5f467b?auto=format&fit=crop&q=80&w=600" alt="Inteligência artificial no campo">
                    <div class="feature-content">
                        <h3>Sensores e Inteligência Artificial</h3>
                        <p>Análise cirúrgica da umidade do solo e previsão climática precisa, auxiliando o produtor em tomadas de decisões inteligentes para evitar desperdícios.</p>
                    </div>
                </div>

                <div class="feature-card">
                    <img src="https://images.unsplash.com/photo-1530595467537-0b5996c41f2d?auto=format&fit=crop&q=80&w=600" alt="Maquinário automatizado com GPS">
                    <div class="feature-content">
                        <h3>Máquinas Automatizadas e GPS</h3>
                        <p>Tratores inteligentes e sistemas de irrigação automatizados que operam de forma autônoma para maximizar a colheita e economizar insumos.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="sustentabilidade" class="benefits-section">
            <div class="benefits-text">
                <h2>Eficiência e Sustentabilidade</h2>
                <p style="margin-bottom: 20px; color: #4a5568;">
                    A tecnologia é a maior aliada da preservação ambiental no ecossistema agrícola moderno. Produzir mais utilizando menos recursos já é uma realidade palpável.
                </p>
                <ul>
                    <li><strong>Redução de Desperdícios:</strong> Insumos aplicados com precisão milimétrica.</li>
                    <li><strong>Preservação de Recursos:</strong> Irrigação automatizada baseada na necessidade real da planta.</li>
                    <li><strong>Decisões Assertivas:</strong> Menor impacto ambiental com o aumento expressivo da produtividade.</li>
                    <li><strong>Progresso Consciente:</strong> Atendendo à demanda de alimentos com foco no amanhã.</li>
                </ul>
            </div>
            <div class="benefits-image">
                <img src="https://images.unsplash.com/photo-1625246333195-78d9c38ad451?auto=format&fit=crop&q=80&w=600" alt="Plantação verde e sustentável">
            </div>
        </section>

    </main>

    <footer>
        <p><strong>AgroTech</strong> - Inovação, Desenvolvimento e Progresso.</p>
        <p style="font-size: 12px; margin-top: 10px; color: #718096;">© Transformação Digital no Agronegócio. Criado para demonstrar o futuro do campo.</p>
    </footer>

</body>
</html>index.html
