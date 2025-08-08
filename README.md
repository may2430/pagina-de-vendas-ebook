#     .container {
        max-width: 960px;
        margin: auto;
        padding: 0 20px;
        position: relative;
        z-index: 2; /* Garante que o texto fique acima da imagem e do overlay */
    }

    /* Hero Section (Topo da página) */
    .hero {
        position: relative; /* Container pai para posicionamento */
        color: #a020f0; /* Roxo para destaque */
        text-align: center;
        padding: 80px 20px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        min-height: 400px; /* Altura mínima para o hero */
        display: flex;
        align-items: center;
        justify-content: center;
    }
    
    .hero-image {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
        z-index: 0; /* Garante que a imagem fique atrás do texto */
    }
    
    /* Camada transparente para o texto */
    .hero::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.3); /* Camada semi-transparente */
        z-index: 1; /* Garante que a camada fique entre a imagem e o texto */
    }

    .hero h1 {
        /* Aplicação da fonte 'Montserrat' para o título */
        font-family: 'Montserrat', sans-serif;
        font-size: 2.5em;
        margin-bottom: 10px;
        font-weight: bold; /* Ativa o negrito como solicitado */
    }

    .hero p {
        font-size: 1.2em;
        color: #ffffff; /* Texto branco para o subtítulo */
        opacity: 0.9;
    }

    /* Seção do Ebook */
    .ebook-section {
        padding: 60px 0;
        background-color: #000000; /* Fundo preto */
        color: #ffffff;
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;
        overflow: hidden;
    }

    /* Mockup Container */
    .mockup-container {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 20px;
        margin-bottom: 30px;
    }

    /* Mockup de Tablet */
    .tablet-mockup {
        width: 400px;
        height: 500px;
        background-color: #1a1a1a;
        border: 10px solid #2d2d2d;
        border-radius: 20px;
        box-shadow: 0 10px 20px rgba(160, 32, 240, 0.3); /* Sombra roxa */
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
        position: relative;
    }

    /* Mockup de Celular */
    .phone-mockup {
        width: 250px;
        height: 450px;
        background-color: #1a1a1a;
        border: 10px solid #2d2d2d;
        border-radius: 40px;
        box-shadow: 0 10px 20px rgba(160, 32, 240, 0.3); /* Sombra roxa */
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
        position: relative;
    }

    /* Imagem da capa dentro dos mockups */
    .mockup-image {
        width: 100%;
        height: 100%;
        object-fit: cover; /* A imagem irá cobrir o espaço do mockup */
    }

    .ebook-section h2 {
        font-size: 2em;
        color: #a020f0; /* Roxo */
    }

    .ebook-section p {
        max-width: 700px;
        font-size: 1.1em;
        margin-top: 20px;
        margin-bottom: 40px;
    }

    /* Botão de Chamada para Ação (CTA) */
    .cta-button {
        display: inline-block;
        background-color: #a020f0; /* Roxo */
        color: #ffffff;
        padding: 12px 30px;
        text-decoration: none;
        font-size: 1.2em;
        font-weight: bold;
        border-radius: 8px; /* Mais quadradinho */
        box-shadow: 0 4px 8px rgba(160, 32, 240, 0.2); /* Sombra mais sutil */
        transition: all 0.3s ease;
        margin-top: 20px;
    }

    .cta-button:hover {
        background-color: #8a2be2; /* Roxo um pouco mais escuro */
        transform: translateY(-2px); /* Efeito de elevação sutil */
        box-shadow: 0 6px 12px rgba(160, 32, 240, 0.3);
    }
    
    .cta-button.secondary {
         background-color: #000000;
         border: 2px solid #a020f0;
         color: #a020f0;
    }
    
     .cta-button.secondary:hover {
        background-color: #1a1a1a;
    }


    /* Seção de Conteúdo */
    .content-section {
        padding: 60px 0;
        background-color: #1a1a1a; /* Cinza escuro para a seção de conteúdo */
        text-align: center;
    }
    
    .content-section .cta-bottom {
         margin-top: 40px;
    }

    .content-section h3 {
        font-size: 1.8em;
        color: #a020f0; /* Roxo */
        margin-bottom: 40px;
    }

    .content-section .content-item {
        display: flex;
        align-items: center;
        justify-content: center;
        margin-bottom: 40px;
        text-align: left;
        background-color: #000000; /* Fundo preto para os itens */
        color: #ffffff;
        padding: 25px;
        border-radius: 10px;
        border: 1px solid #a020f0; /* Borda em roxo */
        box-shadow: 0 2px 8px rgba(160, 32, 240, 0.2);
    }

    .content-section .content-item .icon {
        font-size: 2em;
        color: #a020f0;
        margin-right: 20px;
    }

    .content-section .content-item h4 {
        font-size: 1.3em;
        margin: 0;
        color: #a020f0;
    }

    .content-section .content-item p {
        margin: 5px 0 0 0;
        font-size: 1em;
    }
    
    .content-section .content-item:nth-child(even) {
         flex-direction: row-reverse;
         text-align: right;
    }
    
    .content-section .content-item:nth-child(even) .icon {
         margin-left: 20px;
         margin-right: 0;
    }

    /* Seção de Benefícios (design mais visual) */
    .benefits-section {
        padding: 60px 0;
        background-color: #000000; /* Fundo preto */
        color: #ffffff;
        text-align: center;
    }
    
    .benefits-section h3 {
         color: #a020f0; /* Roxo */
         font-size: 2em;
         margin-bottom: 40px;
    }
    
    .benefits-section ul {
        list-style: none;
        padding: 0;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 20px;
        justify-content: center;
    }

    .benefits-section li {
        background-color: #1a1a1a;
        padding: 30px;
        border-radius: 15px;
        border: 1px solid #a020f0;
        box-shadow: 0 4px 12px rgba(160, 32, 240, 0.3);
        font-size: 1.1em;
        text-align: center;
        position: relative;
        color: #ffffff;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    .benefits-section .icon-benefit {
        font-size: 3em;
        color: #a020f0;
        margin-bottom: 15px;
    }


    /* Seção do Autor -> Atualizada para focar no Ebook */
    .author-section {
        padding: 60px 0;
        background-color: #1a1a1a; /* Cinza escuro para a seção do autor */
        text-align: center;
        color: #ffffff;
    }
    
    .author-section .cta-bottom {
         margin-top: 40px;
    }

    .author-section h3 {
        font-size: 1.8em;
        color: #a020f0; /* Roxo */
    }

    .author-section p {
        max-width: 700px;
        margin: 20px auto;
        font-size: 1.1em;
    }

    /* Rodapé */
    footer {
        background-color: #000000;
        color: #666666;
        text-align: center;
        padding: 30px 20px;
        margin-top: 40px;
    }

    /* Responsividade para telas menores */
    @media (max-width: 768px) {
        .hero h1 {
            font-size: 2em;
        }
        .ebook-section .mockup-container {
            flex-direction: column;
            gap: 50px; /* Aumenta o espaço entre os mockups quando eles empilham */
        }
         .content-section .content-item {
            flex-direction: column;
            text-align: center;
        }

        .content-section .content-item:nth-child(even) {
            flex-direction: column;
        }
        
        .content-section .content-item .icon {
            margin: 0 0 10px 0;
        }

         .content-section .content-item:nth-child(even) .icon {
            margin: 0 0 10px 0;
        }

        .benefits-section li {
             padding: 20px;
             font-size: 1em;
        }
    }
</style>
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Como a IA pode multiplicar a sua produtividade na criação de conteúdo para redes sociais</title>
    <!-- Importação das fontes 'Slabo 27px' e 'Montserrat' do Google Fonts para a página -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Slabo+27px&display=swap" rel="stylesheet">
    <style>
        /* Reset e Configurações globais */
        body {
            font-family: 'Slabo 27px', serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #000000; /* Fundo preto */
            color: #ffffff; /* Texto branco */
        }

        .container {
            max-width: 960px;
            margin: auto;
            padding: 0 20px;
            position: relative;
            z-index: 2; /* Garante que o texto fique acima da imagem e do overlay */
        }

        /* Hero Section (Topo da página) */
        .hero {
            position: relative; /* Container pai para posicionamento */
            color: #a020f0; /* Roxo para destaque */
            text-align: center;
            padding: 80px 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            min-height: 400px; /* Altura mínima para o hero */
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .hero-image {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 0; /* Garante que a imagem fique atrás do texto */
        }
        
        /* Camada transparente para o texto */
        .hero::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.3); /* Camada semi-transparente */
            z-index: 1; /* Garante que a camada fique entre a imagem e o texto */
        }

        .hero h1 {
            /* Aplicação da fonte 'Montserrat' para o título */
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5em;
            margin-bottom: 10px;
            font-weight: bold; /* Ativa o negrito como solicitado */
        }

        .hero p {
            font-size: 1.2em;
            color: #ffffff; /* Texto branco para o subtítulo */
            opacity: 0.9;
        }

        /* Seção do Ebook */
        .ebook-section {
            padding: 60px 0;
            background-color: #000000; /* Fundo preto */
            color: #ffffff;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            overflow: hidden;
        }

        /* Mockup Container */
        .mockup-container {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
        }

        /* Mockup de Tablet */
        .tablet-mockup {
            width: 400px;
            height: 500px;
            background-color: #1a1a1a;
            border: 10px solid #2d2d2d;
            border-radius: 20px;
            box-shadow: 0 10px 20px rgba(160, 32, 240, 0.3); /* Sombra roxa */
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
        }

        /* Mockup de Celular */
        .phone-mockup {
            width: 250px;
            height: 450px;
            background-color: #1a1a1a;
            border: 10px solid #2d2d2d;
            border-radius: 40px;
            box-shadow: 0 10px 20px rgba(160, 32, 240, 0.3); /* Sombra roxa */
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
        }

        /* Imagem da capa dentro dos mockups */
        .mockup-image {
            width: 100%;
            height: 100%;
            object-fit: cover; /* A imagem irá cobrir o espaço do mockup */
        }

        .ebook-section h2 {
            font-size: 2em;
            color: #a020f0; /* Roxo */
        }

        .ebook-section p {
            max-width: 700px;
            font-size: 1.1em;
            margin-top: 20px;
            margin-bottom: 40px;
        }

        /* Botão de Chamada para Ação (CTA) */
        .cta-button {
            display: inline-block;
            background-color: #a020f0; /* Roxo */
            color: #ffffff;
            padding: 12px 30px;
            text-decoration: none;
            font-size: 1.2em;
            font-weight: bold;
            border-radius: 8px; /* Mais quadradinho */
            box-shadow: 0 4px 8px rgba(160, 32, 240, 0.2); /* Sombra mais sutil */
            transition: all 0.3s ease;
            margin-top: 20px;
        }

        .cta-button:hover {
            background-color: #8a2be2; /* Roxo um pouco mais escuro */
            transform: translateY(-2px); /* Efeito de elevação sutil */
            box-shadow: 0 6px 12px rgba(160, 32, 240, 0.3);
        }
        
        .cta-button.secondary {
             background-color: #000000;
             border: 2px solid #a020f0;
             color: #a020f0;
        }
        
         .cta-button.secondary:hover {
            background-color: #1a1a1a;
        }


        /* Seção de Conteúdo */
        .content-section {
            padding: 60px 0;
            background-color: #1a1a1a; /* Cinza escuro para a seção de conteúdo */
            text-align: center;
        }
        
        .content-section .cta-bottom {
             margin-top: 40px;
        }

        .content-section h3 {
            font-size: 1.8em;
            color: #a020f0; /* Roxo */
            margin-bottom: 40px;
        }

        .content-section .content-item {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 40px;
            text-align: left;
            background-color: #000000; /* Fundo preto para os itens */
            color: #ffffff;
            padding: 25px;
            border-radius: 10px;
            border: 1px solid #a020f0; /* Borda em roxo */
            box-shadow: 0 2px 8px rgba(160, 32, 240, 0.2);
        }

        .content-section .content-item .icon {
            font-size: 2em;
            color: #a020f0;
            margin-right: 20px;
        }

        .content-section .content-item h4 {
            font-size: 1.3em;
            margin: 0;
            color: #a020f0;
        }

        .content-section .content-item p {
            margin: 5px 0 0 0;
            font-size: 1em;
        }
        
        .content-section .content-item:nth-child(even) {
             flex-direction: row-reverse;
             text-align: right;
        }
        
        .content-section .content-item:nth-child(even) .icon {
             margin-left: 20px;
             margin-right: 0;
        }

        /* Seção de Benefícios (design mais visual) */
        .benefits-section {
            padding: 60px 0;
            background-color: #000000; /* Fundo preto */
            color: #ffffff;
            text-align: center;
        }
        
        .benefits-section h3 {
             color: #a020f0; /* Roxo */
             font-size: 2em;
             margin-bottom: 40px;
        }
        
        .benefits-section ul {
            list-style: none;
            padding: 0;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            justify-content: center;
        }

        .benefits-section li {
            background-color: #1a1a1a;
            padding: 30px;
            border-radius: 15px;
            border: 1px solid #a020f0;
            box-shadow: 0 4px 12px rgba(160, 32, 240, 0.3);
            font-size: 1.1em;
            text-align: center;
            position: relative;
            color: #ffffff;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .benefits-section .icon-benefit {
            font-size: 3em;
            color: #a020f0;
            margin-bottom: 15px;
        }


        /* Seção do Autor -> Atualizada para focar no Ebook */
        .author-section {
            padding: 60px 0;
            background-color: #1a1a1a; /* Cinza escuro para a seção do autor */
            text-align: center;
            color: #ffffff;
        }
        
        .author-section .cta-bottom {
             margin-top: 40px;
        }

        .author-section h3 {
            font-size: 1.8em;
            color: #a020f0; /* Roxo */
        }

        .author-section p {
            max-width: 700px;
            margin: 20px auto;
            font-size: 1.1em;
        }

        /* Rodapé */
        footer {
            background-color: #000000;
            color: #666666;
            text-align: center;
            padding: 30px 20px;
            margin-top: 40px;
        }

        /* Responsividade para telas menores */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2em;
            }
            .ebook-section .mockup-container {
                flex-direction: column;
                gap: 50px; /* Aumenta o espaço entre os mockups quando eles empilham */
            }
             .content-section .content-item {
                flex-direction: column;
                text-align: center;
            }

            .content-section .content-item:nth-child(even) {
                flex-direction: column;
            }
            
            .content-section .content-item .icon {
                margin: 0 0 10px 0;
            }

             .content-section .content-item:nth-child(even) .icon {
                margin: 0 0 10px 0;
            }

            .benefits-section li {
                 padding: 20px;
                 font-size: 1em;
            }
        }
    </style>
</head>
<body>

    <header class="hero">
        <img src="download.jpg-8bedc29f-00d4-4ac8-9182-1882d9ff8237" alt="Imagem de cabeçalho com inteligência artificial" class="hero-image">
        <div class="container">
            <h1>Como a IA pode multiplicar a sua produtividade na criação de conteúdo para redes sociais</h1>
            <p>Chega de posts sem engajamento! Aprenda a usar o Chat GPT para criar legendas que realmente conectam.</p>
        </div>
    </header>

    <main>
        <section class="ebook-section">
            <div class="container">
                <div class="mockup-container">
                    <!-- Mockup do Tablet -->
                    <div class="tablet-mockup">
                        <img src="download (1).jpg-42e41769-0de2-465f-a4e7-3e8095253f2b" alt="Capa do Ebook no tablet" class="mockup-image">
                    </div>
                    <!-- Mockup do Celular -->
                    <div class="phone-mockup">
                         <img src="download (1).jpg-42e41769-0de2-465f-a4e7-3e8095253f2b" alt="Capa do Ebook no celular" class="mockup-image">
                    </div>
                </div>

                <h2>Descubra o segredo que grandes criadores de conteúdo usam para economizar tempo e aumentar resultados.</h2>
                <p>
                    Aproveite o poder da inteligência artificial para ir além da inspiração. Este e-book é o seu atalho para gerar ideias, criar legendas que vendem, e roteirizar vídeos que capturam a atenção, tudo com a voz autêntica da sua marca. Pare de apenas postar e comece a impactar.
                </p>
                <a href="#" class="cta-button secondary">Compre para transformar sua estratégia de conteúdo.</a>
            </div>
        </section>

        <section class="benefits-section">
            <div class="container">
                <h3>Com este ebook, você vai:</h3>
                <ul>
                    <li>
                         <span class="icon-benefit">💡</span>
                         Aprender a adaptar o Chat GPT ao seu estilo e voz de marca.
                    </li>
                    <li>
                         <span class="icon-benefit">✍️</span>
                         Criar conteúdos que geram conexão, valor e engajamento com seu público.
                    </li>
                    <li>
                         <span class="icon-benefit">⏱️</span>
                         Aumentar sua produtividade e reduzir o tempo de produção de conteúdo.
                    </li>
                    <li>
                         <span class="icon-benefit">📈</span>
                         Desenvolver uma estratégia consistente e alinhada aos objetivos do seu negócio.
                    </li>
                    <li>
                         <span class="icon-benefit">📱</span>
                         Dominar as técnicas de criação de legendas para Instagram, TikTok e LinkedIn.
                    </li>
                    <li>
                         <span class="icon-benefit">🎥</span>
                         Gerar ideias infinitas de conteúdo e roteiros para vídeos curtos.
                    </li>
                </ul>
            </div>
        </section>
        
        <section class="content-section">
            <div class="container">
                <h3>O que você vai encontrar neste Ebook?</h3>
                <div class="content-item">
                    <span class="icon">💡</span>
                    <div>
                        <h4>Capítulo 1: Introdução ao ChatGPT e Legendas</h4>
                        <p>Descubra a importância de uma legenda estratégica, como o Chat GPT funciona e suas vantagens. Aprenda a configurar a ferramenta e a criar prompts de sucesso para gerar textos que prendem a atenção.</p>
                    </div>
                </div>
                <div class="content-item">
                     <span class="icon">🎯</span>
                    <div>
                        <h4>Capítulo 2: Preparação para Criação de Conteúdo</h4>
                        <p>Domine os pilares da estratégia de conteúdo. Entenda as características de cada rede social, o comportamento do seu público e como planejar um calendário editorial consistente, tudo com o apoio da IA.</p>
                    </div>
                </div>
                <div class="content-item">
                    <span class="icon">✍️</span>
                    <div>
                        <h4>Capítulo 3: Estilos de Legenda e Modelos Prontos</h4>
                        <p>Aprenda as estruturas de legendas de storytelling, diretas ao ponto e educativas. O e-book oferece exemplos práticos e dicas de prompts para você aplicar a técnica que mais se encaixa na sua marca.</p>
                    </div>
                </div>
                 <div class="content-item">
                    <span class="icon">🧠</span>
                    <div>
                        <h4>Bônus: Como Manter a Autenticidade com IA</h4>
                        <p>Descubra as melhores práticas para usar a IA de forma estratégica sem perder a voz e a personalidade da sua marca. A tecnologia é uma aliada, não uma substituta para sua criatividade.</p>
                    </div>
                </div>
                <a href="#" class="cta-button cta-bottom">Quero destravar minha criatividade e ter ideias infinitas de conteúdo.</a>
            </div>
        </section>

        <section class="author-section">
            <div class="container">
                <h3>O Futuro do seu Conteúdo Começa Agora</h3>
                <p>
                    A inteligência artificial não é uma ameaça, mas um convite para você se tornar um estrategista de conteúdo ainda mais eficiente. Este e-book é o seu guia prático para dominar as ferramentas de IA, adaptar a voz da sua marca e evoluir junto com o futuro da comunicação digital.
                </p>
                <a href="#" class="cta-button cta-bottom">Quero destravar minha criatividade e ter ideias infinitas de conteúdo.</a>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2025 Seu Nome. Todos os direitos reservados.</p>
        </div>
    </footer>

</body>
</html>
