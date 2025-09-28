[deepseek_html_20250928_dcd316 (1).html](https://github.com/user-attachments/files/22582612/deepseek_html_20250928_dcd316.1.html)
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Metside Smartphones - Reparação de Telemóveis</title>
    <style>
        /* Reset e estilos gerais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary: #1a5276;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --success: #2ecc71;
        }
        
        body {
            line-height: 1.6;
            color: #333;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        section {
            padding: 60px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .section-title h2 {
            font-size: 2.2rem;
            color: var(--primary);
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            width: 70px;
            height: 3px;
            background: var(--secondary);
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background: var(--secondary);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: 600;
            transition: all 0.3s ease;
            text-decoration: none;
        }
        
        .btn:hover {
            background: #2980b9;
            transform: translateY(-2px);
        }
        
        .btn-accent {
            background: var(--accent);
        }
        
        .btn-accent:hover {
            background: #c0392b;
        }
        
        /* Header */
        header {
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
            display: flex;
            align-items: center;
        }
        
        .logo-placeholder {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, #1a5276, #3498db);
            color: white;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border-radius: 8px;
            margin-right: 12px;
            font-weight: bold;
            text-align: center;
            line-height: 1;
            padding: 5px;
            font-size: 0.7rem;
        }
        
        .logo-placeholder .top {
            font-size: 0.6rem;
            font-weight: 800;
        }
        
        .logo-placeholder .bottom {
            font-size: 0.5rem;
        }
        
        .logo-text {
            display: flex;
            flex-direction: column;
            line-height: 1;
        }
        
        .logo-text .main {
            font-size: 1.5rem;
            font-weight: 800;
        }
        
        .logo-text .sub {
            font-size: 0.9rem;
            font-weight: 600;
            color: var(--secondary);
            margin-top: -2px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--secondary);
        }
        
        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(26, 82, 118, 0.8), rgba(26, 82, 118, 0.8)), url('https://images.unsplash.com/photo-1556656793-08538906a9f8?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 150px 0 100px;
            margin-top: 70px;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        /* Serviços */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
        }
        
        .service-icon {
            background: var(--secondary);
            height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.5rem;
            color: white;
        }
        
        .service-content {
            padding: 25px;
        }
        
        .service-content h3 {
            margin-bottom: 15px;
            color: var(--primary);
        }
        
        /* Sobre */
        .about {
            background: #f9f9f9;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-image {
            flex: 1;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Porquê nós */
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .feature {
            text-align: center;
            padding: 30px 20px;
        }
        
        .feature-icon {
            font-size: 3rem;
            color: var(--secondary);
            margin-bottom: 20px;
        }
        
        /* Preços */
        .pricing-table {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }
        
        .pricing-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }
        
        .pricing-card:hover {
            transform: translateY(-5px);
        }
        
        .pricing-header {
            background: var(--primary);
            color: white;
            padding: 20px;
        }
        
        .pricing-header h3 {
            font-size: 1.5rem;
        }
        
        .price {
            font-size: 2.5rem;
            font-weight: 700;
            margin: 15px 0;
        }
        
        .pricing-features {
            padding: 20px;
            list-style: none;
        }
        
        .pricing-features li {
            padding: 10px 0;
            border-bottom: 1px solid #eee;
        }
        
        .pricing-features li:last-child {
            border-bottom: none;
        }
        
        .pricing-footer {
            padding: 20px;
        }
        
        /* Contactos */
        .contact {
            background: #f9f9f9;
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }
        
        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: flex-start;
            gap: 15px;
        }
        
        .contact-icon {
            font-size: 1.5rem;
            color: var(--secondary);
        }
        
        .contact-form {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }
        
        /* Footer */
        footer {
            background: var(--primary);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-column h3::after {
            content: '';
            position: absolute;
            width: 50px;
            height: 2px;
            background: var(--secondary);
            bottom: 0;
            left: 0;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: var(--secondary);
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            color: white;
            text-decoration: none;
            transition: all 0.3s;
        }
        
        .social-links a:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 0.9rem;
            color: #ddd;
        }
        
        /* Responsividade */
        @media (max-width: 992px) {
            .about-content {
                flex-direction: column;
            }
            
            .about-image {
                order: -1;
            }
        }
        
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .logo-text .main {
                font-size: 1.2rem;
            }
            
            .logo-text .sub {
                font-size: 0.8rem;
            }
            
            nav ul {
                display: none;
                position: absolute;
                top: 70px;
                left: 0;
                width: 100%;
                background: white;
                flex-direction: column;
                padding: 20px 0;
                box-shadow: 0 5px 10px rgba(0,0,0,0.1);
            }
            
            nav ul.active {
                display: flex;
            }
            
            nav ul li {
                margin: 0;
                text-align: center;
            }
            
            nav ul li a {
                display: block;
                padding: 10px 0;
            }
            
            .mobile-menu {
                display: block;
            }
        }

        @media (max-width: 480px) {
            .logo {
                font-size: 1.4rem;
            }
            
            .logo-placeholder {
                width: 40px;
                height: 40px;
                font-size: 0.6rem;
            }
            
            .logo-text .main {
                font-size: 1rem;
            }
            
            .logo-text .sub {
                font-size: 0.7rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">
                <div class="logo-placeholder">
                    <div class="top">METSIDE</div>
                    <div>PHONES</div>
                    <div class="bottom">SMART</div>
                </div>
                <div class="logo-text">
                    <div class="main">Metside</div>
                    <div class="sub">Smartphones</div>
                </div>
            </a>
            <div class="mobile-menu">☰</div>
            <nav>
                <ul>
                    <li><a href="#home">Início</a></li>
                    <li><a href="#servicos">Serviços</a></li>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#precos">Preços</a></li>
                    <li><a href="#contactos">Contactos</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Reparação Profissional de Telemóveis</h1>
            <p>Na Metside Smartphones, recuperamos o seu dispositivo com a máxima qualidade, garantia e aos melhores preços. Especialistas em todas as marcas e modelos.</p>
            <a href="#contactos" class="btn">Contacte-nos Agora</a>
            <a href="#servicos" class="btn btn-accent">Nossos Serviços</a>
        </div>
    </section>

    <!-- Serviços -->
    <section id="servicos">
        <div class="container">
            <div class="section-title">
                <h2>Nossos Serviços</h2>
                <p>Oferecemos uma gama completa de serviços de reparação para o seu telemóvel</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">📱</div>
                    <div class="service-content">
                        <h3>Troca de Tela</h3>
                        <p>Reparamos telas partidas de todas as marcas com componentes originais ou de alta qualidade.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔋</div>
                    <div class="service-content">
                        <h3>Troca de Bateria</h3>
                        <p>Se a sua bateria não dura o dia, temos a solução. Troca rápida com garantia.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔧</div>
                    <div class="service-content">
                        <h3>Reparações Gerais</h3>
                        <p>Problemas de software, conectividade, câmara, altifalante e muito mais.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔄</div>
                    <div class="service-content">
                        <h3>Venda de Acessórios</h3>
                        <p>Temos uma variedade de capas, películas, carregadores e outros acessórios.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">💻</div>
                    <div class="service-content">
                        <h3>Atualização de Software</h3>
                        <p>Resolvemos problemas de sistema operacional e aplicações.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">📞</div>
                    <div class="service-content">
                        <h3>Diagnóstico Gratuito</h3>
                        <p>Faça um diagnóstico gratuito do seu dispositivo sem compromisso.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sobre -->
    <section class="about" id="sobre">
        <div class="container">
            <div class="section-title">
                <h2>Sobre a Metside Smartphones</h2>
                <p>Conheça a nossa história e valores</p>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3>Especialistas em Reparação de Telemóveis desde 2021</h3>
                    <p>A Metside Smartphones nasceu da paixão pela tecnologia e do desejo de oferecer um serviço de excelência na reparação de dispositivos móveis. Ao longo dos anos, tornámo-nos referência na região pela nossa competência, transparência e compromisso com o cliente.</p>
                    <p>Contamos com uma equipa de técnicos certificados e em constante formação para lidar com as mais recentes tecnologias. Utilizamos apenas componentes de qualidade e oferecemos garantia em todos os nossos serviços.</p>
                    <p>O nosso objetivo é devolver-lhe o seu dispositivo em perfeitas condições, no menor tempo possível e a um preço justo.</p>
                    <a href="#contactos" class="btn">Visite-nos</a>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1563013541-666ab0851fbd?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Técnico a reparar telemóvel">
                </div>
            </div>
        </div>
    </section>

    <!-- Porquê nós -->
    <section>
        <div class="container">
            <div class="section-title">
                <h2>Porquê Escolher a Metside Smartphones?</h2>
                <p>As vantagens de confiar no seu dispositivo aos nossos cuidados</p>
            </div>
            <div class="features">
                <div class="feature">
                    <div class="feature-icon">⏱️</div>
                    <h3>Reparação Rápida</h3>
                    <p>Muitas reparações são concluídas no mesmo dia, para que não fique sem o seu dispositivo.</p>
                </div>
                <div class="feature">
                    <div class="feature-icon">✅</div>
                    <h3>Garantia nos Serviços</h3>
                    <p>Oferecemos garantia em todas as reparações para sua total tranquilidade.</p>
                </div>
                <div class="feature">
                    <div class="feature-icon">💎</div>
                    <h3>Componentes de Qualidade</h3>
                    <p>Utilizamos apenas componentes originais ou de alta qualidade compatíveis.</p>
                </div>
                <div class="feature">
                    <div class="feature-icon">💰</div>
                    <h3>Preços Competitivos</h3>
                    <p>Oferecemos os melhores preços do mercado sem comprometer a qualidade.</p>
                </div>
                <div class="feature">
                    <div class="feature-icon">👨‍🔧</div>
                    <h3>Técnicos Certificados</h3>
                    <p>A nossa equipa é composta por técnicos especializados e em constante formação.</p>
                </div>
                <div class="feature">
                    <div class="feature-icon">📞</div>
                    <h3>Atendimento Personalizado</h3>
                    <p>Valorizamos cada cliente e oferecemos um atendimento próximo e transparente.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Preços -->
    <section class="pricing" id="precos">
        <div class="container">
            <div class="section-title">
                <h2>Preços de Referência</h2>
                <p>Consulte os nossos preços para reparações mais comuns</p>
            </div>
            <div class="pricing-table">
                <div class="pricing-card">
                    <div class="pricing-header">
                        <h3>Troca de Tela</h3>
                        <div class="price">a partir de 1200 MZN</div>
                    </div>
                    <ul class="pricing-features">
                        <li>Para a maioria dos modelos</li>
                        <li>Componentes de alta qualidade</li>
                        <li>Garantia de 12 meses</li>
                        <li>Reparação em até 2 horas</li>
                    </ul>
                    <div class="pricing-footer">
                        <a href="#contactos" class="btn">Solicitar Orçamento</a>
                    </div>
                </div>
                <div class="pricing-card">
                    <div class="pricing-header">
                        <h3>Troca de Bateria</h3>
                        <div class="price">a partir de 500 MZN</div>
                    </div>
                    <ul class="pricing-features">
                        <li>Baterias de alta capacidade</li>
                        <li>Garantia de 12 meses</li>
                        <li>Reparação em 1 hora</li>
                        <li>Diagnóstico gratuito</li>
                    </ul>
                    <div class="pricing-footer">
                        <a href="#contactos" class="btn">Solicitar Orçamento</a>
                    </div>
                </div>
                <div class="pricing-card">
                    <div class="pricing-header">
                        <h3>Reparação por Água</h3>
                        <div class="price">a partir de 1800 MZN</div>
                    </div>
                    <ul class="pricing-features">
                        <li>Limpeza especializada</li>
                        <li>Diagnóstico detalhado</li>
                        <li>Taxa só se reparação for possível</li>
                        <li>Orçamento gratuito</li>
                    </ul>
                    <div class="pricing-footer">
                        <a href="#contactos" class="btn">Solicitar Orçamento</a>
                    </div>
                </div>
            </div>
            <div style="text-align: center; margin-top: 30px;">
                <p><strong>Nota:</strong> Os preços podem variar consoante o modelo e a extensão dos danos. Contacte-nos para um orçamento personalizado.</p>
            </div>
        </div>
    </section>

    <!-- Contactos -->
    <section class="contact" id="contactos">
        <div class="container">
            <div class="section-title">
                <h2>Contactos</h2>
                <p>Estamos aqui para ajudar. Visite-nos ou entre em contacto</p>
            </div>
            <div class="contact-container">
                <div class="contact-info">
                    <div class="contact-item">
                        <div class="contact-icon">📍</div>
                        <div>
                            <h3>Morada</h3>
                            <p>Terminal de Autocarros Bedene, Matola, Maputo 1112</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">📞</div>
                        <div>
                            <h3>Telefone</h3>
                            <p>+258 865930583</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">✉️</div>
                        <div>
                            <h3>Email</h3>
                            <p>metsideservicos@gmail.com</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">🕒</div>
                        <div>
                            <h3>Horário de Funcionamento</h3>
                            <p>Segunda a Sexta: 8h00 - 18h00<br>Sábado: 9h00 - 15h00</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">💬</div>
                        <div>
                            <h3>Redes Sociais</h3>
                            <div class="social-links">
                                <a href="https://facebook.com/MetsideSmartphones" target="_blank">FB</a>
                            </div>
                            <p style="margin-top: 10px;">Facebook: Metside Smartphones</p>
                        </div>
                    </div>
                </div>
                <div class="contact-form">
                    <h3>Envie-nos uma mensagem</h3>
                    <form id="contactForm">
                        <div class="form-group">
                            <label for="name">Nome</label>
                            <input type="text" id="name" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="phone">Telemóvel</label>
                            <input type="tel" id="phone" class="form-control">
                        </div>
                        <div class="form-group">
                            <label for="message">Mensagem</label>
                            <textarea id="message" class="form-control" required></textarea>
                        </div>
                        <button type="submit" class="btn">Enviar Mensagem</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Metside Smartphones</h3>
                    <p>Especialistas em reparação de telemóveis com qualidade, garantia e os melhores preços do mercado.</p>
                    <div class="social-links">
                        <a href="https://facebook.com/MetsideSmartphones" target="_blank">FB</a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Links Rápidos</h3>
                    <ul class="footer-links">
                        <li><a href="#home">Início</a></li>
                        <li><a href="#servicos">Serviços</a></li>
                        <li><a href="#sobre">Sobre Nós</a></li>
                        <li><a href="#precos">Preços</a></li>
                        <li><a href="#contactos">Contactos</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Serviços</h3>
                    <ul class="footer-links">
                        <li><a href="#">Troca de Tela</a></li>
                        <li><a href="#">Troca de Bateria</a></li>
                        <li><a href="#">Reparações Gerais</a></li>
                        <li><a href="#">Venda de Acessórios</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contactos</h3>
                    <ul class="footer-links">
                        <li>📍 Terminal de Autocarros Bedene, Matola</li>
                        <li>📞 +258 865930583</li>
                        <li>✉️ metsideservicos@gmail.com</li>
                        <li>🕒 Seg-Sex: 8h-18h | Sáb: 9h-15h</li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Metside Smartphones - Reparação de Telemóveis. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        // Menu mobile
        document.querySelector('.mobile-menu').addEventListener('click', function() {
            document.querySelector('nav ul').classList.toggle('active');
        });
        
        // Fechar menu ao clicar num link
        document.querySelectorAll('nav ul li a').forEach(link => {
            link.addEventListener('click', () => {
                document.querySelector('nav ul').classList.remove('active');
            });
        });
        
        // Form submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Obrigado pela sua mensagem! Entraremos em contacto brevemente.');
            this.reset();
        });
        
        // Smooth scrolling para âncoras
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 70,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
