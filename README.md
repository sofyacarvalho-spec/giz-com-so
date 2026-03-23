<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brinquedaria Express - Loja Online de Brinquedos</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- HEADER -->
    <header class="header">
        <div class="container">
            <div class="logo">
                <h1>🎮 Brinquedaria Express</h1>
            </div>
            <nav class="menu">
                <ul>
                    <li><a href="#home">Início</a></li>
                    <li><a href="#produtos">Produtos</a></li>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
            <div class="cart-icon">
                <button id="cart-btn">🛒 Carrinho (<span id="cart-count">0</span>)</button>
            </div>
        </div>
    </header>

    <!-- BANNER PRINCIPAL -->
    <section class="banner" id="home">
        <div class="banner-content">
            <h2>Bem-vindo à Brinquedaria Express!</h2>
            <p>Os melhores brinquedos com os melhores preços</p>
            <button class="btn-banner" onclick="document.getElementById('produtos').scrollIntoView({behavior: 'smooth'})">
                Ver Produtos
            </button>
        </div>
    </section>

    <!-- PRODUTOS -->
    <section class="produtos" id="produtos">
        <div class="container">
            <h2>Nossos Produtos</h2>
            <div class="produtos-grid" id="produtos-grid">
                <!-- Produtos serão inseridos aqui pelo JavaScript -->
            </div>
        </div>
    </section>

    <!-- SOBRE -->
    <section class="sobre" id="sobre">
        <div class="container">
            <h2>Sobre a Brinquedaria Express</h2>
            <p>Somos uma loja online especializada em brinquedos de qualidade para crianças de todas as idades. 
            Com mais de 10 anos de experiência, oferecemos os melhores produtos com entrega rápida e segura.</p>
        </div>
    </section>

    <!-- CONTATO -->
    <section class="contato" id="contato">
        <div class="container">
            <h2>Entre em Contato</h2>
            <div class="contato-info">
                <div class="info-item">
                    <h3>📱 Telefone</h3>
                    <p>(11) 98765-4321</p>
                </div>
                <div class="info-item">
                    <h3>📧 Email</h3>
                    <p>contato@brinquedaria.com.br</p>
                </div>
                <div class="info-item">
                    <h3>📍 Endereço</h3>
                    <p>Rua dos Brinquedos, 123 - São Paulo, SP</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2026 Brinquedaria Express. Todos os direitos reservados.</p>
        </div>
    </footer>

    <!-- MODAL DO CARRINHO -->
    <div id="cart-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2>Seu Carrinho</h2>
            <div id="cart-items">
                <p>Seu carrinho está vazio</p>
            </div>
            <div class="cart-total">
                <h3>Total: R$ <span id="cart-total">0.00</span></h3>
            </div>
            <button class="btn-checkout" onclick="alert('Finalize sua compra com segurança!')">
                Finalizar Compra
            </button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
