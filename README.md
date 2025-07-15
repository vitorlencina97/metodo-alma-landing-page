<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Método ALMA - Vitor Lencina | Desejo & Destino</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --indigo: #2E3A59;
            --gold: #D4AF37;
            --white: #FFFFFF;
            --light-gray: #F5F5F5;
            --dark-gray: #333333;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--light-gray);
            color: var(--dark-gray);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            background-color: var(--indigo);
            color: var(--white);
            padding: 40px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('images/banner_metodo_alma.png') no-repeat center center/cover;
            opacity: 0.3;
            z-index: 0;
        }

        header .content {
            position: relative;
            z-index: 1;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3.5em;
            margin-bottom: 10px;
            color: var(--gold);
        }

        header h2 {
            font-family: 'Playfair Display', serif;
            font-size: 1.8em;
            margin-top: 0;
            color: var(--white);
        }

        header p {
            font-size: 1.1em;
            max-width: 700px;
            margin: 20px auto;
        }

        .btn-primary {
            display: inline-block;
            background-color: var(--gold);
            color: var(--indigo);
            padding: 15px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s ease;
            margin-top: 20px;
        }

        .btn-primary:hover {
            background-color: #c09f2d;
        }

        section {
            padding: 60px 0;
            text-align: center;
        }

        section:nth-of-type(even) {
            background-color: var(--white);
        }

        h3 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5em;
            color: var(--indigo);
            margin-bottom: 40px;
        }

        .grid-4-phases {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .phase-item {
            background-color: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            text-align: left;
            transition: transform 0.3s ease;
        }

        .phase-item:hover {
            transform: translateY(-10px);
        }

        .phase-item img {
            max-width: 100px;
            margin-bottom: 20px;
        }

        .phase-item h4 {
            font-family: 'Playfair Display', serif;
            color: var(--gold);
            font-size: 1.8em;
            margin-top: 0;
        }

        .phase-item p {
            font-size: 1em;
            color: var(--dark-gray);
        }

        .about-vitor {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 40px;
            margin-top: 40px;
        }

        .about-vitor img {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid var(--gold);
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
        }

        .about-vitor .text-content {
            max-width: 800px;
            text-align: left;
        }

        .about-vitor .text-content p {
            font-size: 1.1em;
            margin-bottom: 15px;
        }

        .services-pricing .grid-services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .service-card {
            background-color: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .service-card h4 {
            font-family: 'Playfair Display', serif;
            color: var(--indigo);
            font-size: 2em;
            margin-top: 0;
            margin-bottom: 15px;
        }

        .service-card .price {
            font-family: 'Playfair Display', serif;
            font-size: 2.5em;
            color: var(--gold);
            margin-bottom: 10px;
        }

        .service-card ul {
            list-style: none;
            padding: 0;
            margin: 20px 0;
            text-align: left;
        }

        .service-card ul li {
            margin-bottom: 10px;
            font-size: 1.1em;
            position: relative;
            padding-left: 25px;
        }

        .service-card ul li::before {
            content: '✓';
            color: var(--gold);
            position: absolute;
            left: 0;
            top: 0;
        }

        .testimonials .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .testimonial-card {
            background-color: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            text-align: left;
        }

        .testimonial-card p {
            font-style: italic;
            margin-bottom: 15px;
        }

        .testimonial-card .author {
            font-weight: bold;
            color: var(--indigo);
        }

        .testimonial-card img {
            max-width: 100%;
            border-radius: 8px;
            margin-top: 15px;
        }

        .contact-section {
            background-color: var(--indigo);
            color: var(--white);
            padding: 60px 0;
        }

        .contact-section h3 {
            color: var(--gold);
        }

        .contact-info p {
            font-size: 1.1em;
            margin-bottom: 10px;
        }

        .social-links a {
            color: var(--white);
            font-size: 1.5em;
            margin: 0 15px;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--gold);
        }

        .faq-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .faq-item {
            background-color: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            text-align: left;
        }

        .faq-item h4 {
            font-family: 'Playfair Display', serif;
            color: var(--indigo);
            font-size: 1.5em;
            margin-top: 0;
            margin-bottom: 15px;
        }

        .faq-item p {
            font-size: 1em;
            color: var(--dark-gray);
            line-height: 1.6;
        }

        footer {
            background-color: var(--dark-gray);
            color: var(--white);
            text-align: center;
            padding: 20px 0;
            font-size: 0.9em;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5em;
            }

            header h2 {
                font-size: 1.5em;
            }

            h3 {
                font-size: 2em;
            }

            .grid-4-phases, .grid-services, .testimonial-grid, .faq-grid {
                grid-template-columns: 1fr;
            }

            .about-vitor {
                flex-direction: column;
            }

            .about-vitor img {
                width: 200px;
                height: 200px;
            }

            .faq-grid {
                grid-template-columns: 1fr;
            }

            .faq-item {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="content">
            <img src="images/logo_metodo_alma.jpg" alt="Logo Método ALMA" style="width: 150px; margin-bottom: 20px;">
            <h1>Método ALMA</h1>
            <h2>Análise • Liberação • Manifestação • Aperfeiçoamento</h2>
            <p>Sua jornada de cura profunda e autodescoberta guiada por Vitor Lencina | Desejo & Destino.</p>
            <a href="https://wa.me/5511963676104?text=Ol%C3%A1%2C%20gostaria%20de%20saber%20mais%20sobre%20o%20M%C3%A9todo%20ALMA!" class="btn-primary">Quero Transformar Minha Vida!</a>
        </div>
    </header>

    <section id="about">
        <div class="container">
            <h3>Quem é Vitor Lencina?</h3>
            <div class="about-vitor">
                <img src="images/vitor_lencina_2.jpg" alt="Vitor Lencina">
                <div class="text-content">
                    <p>Olá! Eu sou Vitor Lencina, seu guia na jornada de autodescoberta e transformação. Minha missão é unir a sabedoria ancestral, as práticas espirituais e as ferramentas terapêuticas modernas para te ajudar a desvendar a raiz dos seus desafios e florescer em seu potencial máximo.</p>
                    <p>Com anos de experiência em Tarot Terapêutico, Umbanda, Apometria, Magiterapia e Psicoterapia, atuo como um canal para que você encontre clareza, cura e direcionamento. Acredito que a verdadeira transformação acontece quando olhamos para dentro, liberamos o que não nos serve e manifestamos a vida que realmente desejamos.</p>
                    <p>Seja bem-vindo(a) ao seu novo caminho!</p>
                </div>
            </div>
        </div>
    </section>

    <section id="metodo-alma">
        <div class="container">
            <h3>O Que é o Método ALMA?</h3>
            <p>O Método ALMA é um caminho integrado e profundo, que cuida da sua história, do seu corpo, das suas crenças e da sua força interior. Uma jornada em 4 fases para uma transformação completa e duradoura:</p>
            <div class="grid-4-phases">
                <div class="phase-item">
                    <img src="images/infografico_4_fases.jpg" alt="Análise da Raiz" style="max-width: 80px;">
                    <h4>1. Análise da Raiz</h4>
                    <p>Identificamos a origem da dor e os padrões antigos que te impedem de avançar, através de psicoterapia profunda e tarot terapêutico.</p>
                </div>
                <div class="phase-item">
                    <img src="images/infografico_4_fases.jpg" alt="Liberação Corporal" style="max-width: 80px;">
                    <h4>2. Liberação Corporal</h4>
                    <p>Entendemos como o problema somatiza no seu corpo e dissolvemos essas tensões com radiestesia, apometria e cromoterapia.</p>
                </div>
                <div class="phase-item">
                    <img src="images/infografico_4_fases.jpg" alt="Manifestação de Crenças" style="max-width: 80px;">
                    <h4>3. Manifestação de Crenças</h4>
                    <p>Trazemos à tona crenças limitantes do futuro e ressignificamos padrões com tarot psicológico e constelação familiar.</p>
                </div>
                <div class="phase-item">
                    <img src="images/infografico_4_fases.jpg" alt="Aperfeiçoamento" style="max-width: 80px;">
                    <h4>4. Aperfeiçoamento</h4>
                    <p>Potencializamos seus recursos internos e poder pessoal com tarot transformacional, apometria intensiva e magia dos guias/Orixás.</p>
                </div>
            </div>
            <img src="images/infografico_4_fases.jpg" alt="Infográfico 4 Fases" style="max-width: 600px; margin-top: 50px;">
        </div>
    </section>

    <section id="services-pricing">
        <div class="container">
            <h3>Escolha Seu Caminho de Transformação</h3>
            <p>Ofereço flexibilidade para você iniciar sua jornada de cura. Escolha o que melhor se adapta às suas necessidades:</p>
            <div class="grid-services">
                <div class="service-card">
                    <h4>Método ALMA Completo</h4>
                    <p class="price">R$ 500</p>
                    <p>ou 4x de R$ 125 no crédito</p>
                    <ul>
                        <li>✓ Jornada completa em 4 fases</li>
                        <li>✓ 4 sessões individuais e personalizadas</li>
                        <li>✓ Leitura astrológica kármica & destino (bônus)</li>
                        <li>✓ Suporte exclusivo via WhatsApp</li>
                        <li>✓ Transformação profunda e duradoura</li>
                    </ul>
                    <a href="https://wa.me/5511963676104?text=Ol%C3%A1%2C%20gostaria%20de%20saber%20mais%20sobre%20o%20M%C3%A9todo%20ALMA%20Completo!" class="btn-primary">Quero o Método ALMA!</a>
                </div>
                <div class="service-card">
                    <h4>Sessões Individuais</h4>
                    <p class="price">R$ 150</p>
                    <p>por sessão</p>
                    <ul>
                        <li>✓ Contrate cada fase do ALMA separadamente</li>
                        <li>✓ Flexibilidade para focar em uma necessidade específica</li>
                        <li>✓ Ideal para quem busca um apoio pontual</li>
                        <li>✓ Possibilidade de experimentar o método passo a passo</li>
                    </ul>
                    <a href="https://wa.me/5511963676104?text=Ol%C3%A1%2C%20gostaria%20de%20saber%20mais%20sobre%20as%20Sess%C3%B5es%20Individuais%20do%20M%C3%A9todo%20ALMA!" class="btn-primary">Sessão Avulsa</a>
                </div>
                <div class="service-card">
                    <h4>Tarot Terapêutico (Leitura Simples)</h4>
                    <p class="price">Valor Justo</p>
                    <p>medido pelo oráculo</p>
                    <ul>
                        <li>✓ Leitura rápida para esclarecimento pontual</li>
                        <li>✓ Ideal para conhecer meus serviços</li>
                        <li>✓ Valor acessível e personalizado</li>
                        <li>✓ Respostas claras para suas dúvidas imediatas</li>
                    </ul>
                    <a href="https://wa.me/5511963676104?text=Ol%C3%A1%2C%20gostaria%20de%20uma%20Leitura%20Simples%20de%20Tarot%20Terap%C3%AAutico!" class="btn-primary">Quero uma Leitura!</a>
                </div>
            </div>
            <p style="margin-top: 40px; font-size: 1.1em;">Além disso, ofereço **Consultas Gratuitas com Guias em Giras a cada 15 dias**. Acompanhe minhas redes sociais para saber as datas!</p>
            <p style="font-size: 1.1em;">Para contratação de magias sem a terapia ALMA, o valor de troca também é medido pelo oráculo para que esteja dentro das condições de cada um e no valor justo. Entre em contato para mais informações.</p>
        </div>
    </section>

    <section id="testimonials">
        <div class="container">
            <h3>O Que Dizem Meus Clientes</h3>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <p>"Vitor, muito obrigada pelo seu atendimento. Eu já estava passando por um luto pós-término há uma semana e, após nossa conversa, consegui fazer um macarrão e comer. Você abriu alguns leques necessários e, além disso, aquela angústia que eu estava sentindo se acalmou por um tempo. Conversar com você fez toda a diferença. Você é um ser de luz!"</p>
                    <p class="author">- Paula (Depoimento real)</p>
                    <img src="images/depoimento_1.jpg" alt="Depoimento de Cliente">
                </div>
                <div class="testimonial-card">
                    <p>"O Método ALMA me ajudou a entender a raiz dos meus medos e a liberar pesos que eu nem sabia que carregava. A cada sessão, sinto uma leveza e um empoderamento que nunca imaginei. Recomendo a todos que buscam uma transformação verdadeira!"</p>
                    <p class="author">- Cliente Satisfeita</p>
                    <img src="images/tarot_ritual.jpg" alt="Tarot e Ritual">
                </div>
                <div class="testimonial-card">
                    <p>"A leitura de tarot com o Vitor foi um divisor de águas. Clareou muitas dúvidas e me deu o direcionamento que eu precisava para tomar decisões importantes. É incrível como ele conecta a espiritualidade com a nossa realidade de forma tão prática."</p>
                    <p class="author">- Higor</p>
                    <img src="images/vitor_lencina_3.jpg" alt="Vitor em entrevista">
                </div>
            </div>
        </div>
    </section>

    <section id="faq">
        <div class="container">
            <h3>Perguntas Frequentes</h3>
            <div class="faq-grid">
                <div class="faq-item">
                    <h4>Como funciona o processo de aprovação?</h4>
                    <p>Todos os serviços passam por uma pré-avaliação gratuita onde analiso sua saúde energética, emocional e espiritual. Através de orientações e acesso ao campo energético, meço o merecimento, resultados e energia a ser aplicada. Se aprovado, você pode agendar ou receber os serviços conforme o prazo estabelecido.</p>
                </div>
                <div class="faq-item">
                    <h4>Qual a diferença entre o Método ALMA completo e as sessões individuais?</h4>
                    <p>O Método ALMA completo oferece uma jornada estruturada em 4 fases para transformação profunda e duradoura. As sessões individuais permitem focar em necessidades específicas ou experimentar o método passo a passo. Ambas são eficazes, a escolha depende do seu momento e objetivos.</p>
                </div>
                <div class="faq-item">
                    <h4>Como é definido o valor da leitura simples de tarot?</h4>
                    <p>O valor da leitura simples é medido pelo próprio oráculo para garantir que esteja dentro das suas condições financeiras e seja justo para ambos. Isso garante acessibilidade e equilíbrio energético na troca.</p>
                </div>
                <div class="faq-item">
                    <h4>Quando acontecem as consultas gratuitas com guias?</h4>
                    <p>As consultas gratuitas com guias acontecem em giras a cada 15 dias. Acompanhe minhas redes sociais para saber as datas exatas e como participar. É uma oportunidade única de receber orientação espiritual sem custo.</p>
                </div>
                <div class="faq-item">
                    <h4>Posso fazer os atendimentos à distância?</h4>
                    <p>Sim! Atendo tanto à distância quanto presencialmente na região metropolitana de SP (Jaçanã). Os atendimentos à distância são tão eficazes quanto os presenciais, pois trabalho com energia e conexão espiritual que transcendem o espaço físico.</p>
                </div>
                <div class="faq-item">
                    <h4>O que está incluído no suporte via WhatsApp?</h4>
                    <p>No Método ALMA completo, você recebe suporte exclusivo via WhatsApp entre as sessões para tirar dúvidas, compartilhar insights e receber orientações pontuais. É um acompanhamento personalizado para potencializar sua transformação.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="contact-section">
        <div class="container">
            <h3>Fale Comigo!</h3>
            <p>Pronto(a) para iniciar sua jornada de transformação? Entre em contato e vamos conversar!</p>
            <div class="contact-info">
                <p><strong>WhatsApp:</strong> <a href="https://wa.me/5511963676104" style="color: var(--gold); text-decoration: none;">11 96367-6104</a></p>
                <p><strong>Instagram:</strong> <a href="https://www.instagram.com/vitorlencina.terapeuta" target="_blank" style="color: var(--gold); text-decoration: none;">@vitorlencina.terapeuta</a></p>
                <p><strong>TikTok:</strong> <a href="https://www.tiktok.com/@vitorlencina.c.s" target="_blank" style="color: var(--gold); text-decoration: none;">@vitorlencina.c.s</a></p>
                <p><strong>YouTube:</strong> <a href="https://www.youtube.com/@vitorlencina.terapeuta" target="_blank" style="color: var(--gold); text-decoration: none;">www.youtube.com/@vitorlencina.terapeuta</a></p>
            </div>
            <a href="https://wa.me/5511963676104?text=Ol%C3%A1%2C%20gostaria%20de%20saber%20mais%20sobre%20os%20servi%C3%A7os%20de%20Vitor%20de%20L%C3%BAcifer!" class="btn-primary">Enviar Mensagem no WhatsApp</a>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2025 Vitor de Lúcifer | Desejo & Destino. Todos os direitos reservados.</p>
        </div>
    </footer>
</body>
</html>

