<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Biblioteca Digital - Ebooks Exclusivos</title>
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --text: #333;
            --shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f9f9f9;
            color: var(--text);
            line-height: 1.6;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Header */
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: var(--shadow);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
        }
        
        .logo span {
            color: var(--secondary);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--secondary);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(44, 62, 80, 0.8), rgba(44, 62, 80, 0.9)), url('https://images.unsplash.com/photo-1507842217343-583bb7270b66?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 5rem 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2980b9;
        }
        
        /* Features Section */
        .features {
            padding: 4rem 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            color: var(--primary);
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .feature-card {
            background-color: var(--light);
            padding: 2rem;
            border-radius: 8px;
            text-align: center;
            box-shadow: var(--shadow);
            transition: transform 0.3s;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
        }
        
        .feature-icon {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 1rem;
        }
        
        /* Ebooks Section */
        .ebooks {
            padding: 4rem 0;
            background-color: #f5f5f5;
        }
        
        .ebooks-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .ebook-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: transform 0.3s;
        }
        
        .ebook-card:hover {
            transform: translateY(-5px);
        }
        
        .ebook-image {
            height: 200px;
            background-color: #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            color: var(--primary);
        }
        
        .ebook-info {
            padding: 1.5rem;
        }
        
        .ebook-title {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }
        
        .ebook-author {
            color: #666;
            margin-bottom: 1rem;
        }
        
        .ebook-price {
            font-weight: bold;
            color: var(--accent);
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }
        
        /* CTA Section */
        .cta {
            background-color: var(--primary);
            color: white;
            padding: 4rem 0;
            text-align: center;
        }
        
        .cta h2 {
            margin-bottom: 1.5rem;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .social-links {
            margin: 1rem 0;
        }
        
        .social-links a {
            color: white;
            margin: 0 0.5rem;
            font-size: 1.5rem;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
            }
            
            nav ul {
                margin-top: 1rem;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">Minha<span>Biblioteca</span></div>
                <nav>
                    <ul>
                        <li><a href="#inicio">Início</a></li>
                        <li><a href="#ebooks">Ebooks</a></li>
                        <li><a href="#sobre">Sobre</a></li>
                        <li><a href="#contato">Contato</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="inicio">
        <div class="container">
            <h1>Descubra um Mundo de Conhecimento</h1>
            <p>Minha biblioteca digital oferece ebooks exclusivos para todos os gostos. Aprenda, explore e transforme sua vida através da leitura.</p>
            <a href="#ebooks" class="btn">Explorar Ebooks</a>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features">
        <div class="container">
            <h2 class="section-title">Por que escolher minha biblioteca?</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">📚</div>
                    <h3>Conteúdo Exclusivo</h3>
                    <p>Ebooks únicos que você não encontra em outros lugares, criados com expertise e cuidado.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">📱</div>
                    <h3>Acesso Imediato</h3>
                    <p>Download instantâneo após a compra. Leia em qualquer dispositivo, a qualquer hora.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">💰</div>
                    <h3>Preços Justos</h3>
                    <p>Conteúdo de alta qualidade a preços acessíveis que cabem no seu orçamento.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Ebooks Section -->
    <section class="ebooks" id="ebooks">
        <div class="container">
            <h2 class="section-title">Meus Ebooks em Destaque</h2>
            <div class="ebooks-grid">
                <!-- Ebook 1 - Substitua com seus ebooks -->
                <div class="ebook-card">
                    <div class="ebook-image">📖</div>
                    <div class="ebook-info">
                        <h3 class="ebook-title">Título do Seu Ebook 1</h3>
                        <p class="ebook-author">Seu Nome</p>
                        <p class="ebook-price">R$ 24,90</p>
                        <a href="#" class="btn">Comprar Agora</a>
                    </div>
                </div>
                
                <!-- Ebook 2 -->
                <div class="ebook-card">
                    <div class="ebook-image">📖</div>
                    <div class="ebook-info">
                        <h3 class="ebook-title">Título do Seu Ebook 2</h3>
                        <p class="ebook-author">Seu Nome</p>
                        <p class="ebook-price">R$ 29,90</p>
                        <a href="#" class="btn">Comprar Agora</a>
                    </div>
                </div>
                
                <!-- Ebook 3 -->
                <div class="ebook-card">
                    <div class="ebook-image">📖</div>
                    <div class="ebook-info">
                        <h3 class="ebook-title">Título do Seu Ebook 3</h3>
                        <p class="ebook-author">Seu Nome</p>
                        <p class="ebook-price">R$ 19,90</p>
                        <a href="#" class="btn">Comprar Agora</a>
                    </div>
                </div>
                
                <!-- Ebook 4 -->
                <div class="ebook-card">
                    <div class="ebook-image">📖</div>
                    <div class="ebook-info">
                        <h3 class="ebook-title">Título do Seu Ebook 4</h3>
                        <p class="ebook-author">Seu Nome</p>
                        <p class="ebook-price">R$ 27,90</p>
                        <a href="#" class="btn">Comprar Agora</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="container">
            <h2>Comece sua jornada de leitura hoje!</h2>
            <p>Adquira meus ebooks exclusivos e transforme seu conhecimento.</p>
            <a href="#ebooks" class="btn" style="background-color: var(--accent);">Ver Todos os Ebooks</a>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contato">
        <div class="container">
            <div class="footer-content">
                <div class="logo">Minha<span>Biblioteca</span></div>
                <p>Sua fonte de conhecimento digital exclusivo</p>
                <div class="social-links">
                    <a href="#">📘</a>
                    <a href="#">📷</a>
                    <a href="#">🐦</a>
                </div>
                <p>Entre em contato: seuemail@exemplo.com</p>
                <p>&copy; 2023 Minha Biblioteca. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>
</body>
</html>
