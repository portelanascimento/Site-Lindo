<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portal de Notícias</title>
    <style>
        /* Estilos Globais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #f4f4f4;
            color: #333;
            transition: background-color 0.5s, color 0.5s;
        }

        body.dark-mode {
            background-color: #121212;
            color: #e0e0e0;
        }

        header {
            background-color: #007BFF;
            color: white;
            padding: 20px;
            text-align: center;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            margin: 20px auto;
            max-width: 1200px;
        }

        main {
            flex: 3;
            padding: 20px;
        }

        aside {
            flex: 1;
            padding: 20px;
            background-color: #f9f9f9;
            margin-left: 20px;
        }

        aside.dark-mode {
            background-color: #1e1e1e;
        }

        .article {
            background-color: white;
            margin-bottom: 20px;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .article.dark-mode {
            background-color: #1e1e1e;
        }

        .article img {
            max-width: 100%;
            border-radius: 8px;
        }

        .article h2 {
            margin-top: 10px;
        }

        .article p {
            margin-top: 10px;
            line-height: 1.6;
        }

        .btn {
            display: inline-block;
            padding: 10px 20px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }

        .btn-primary {
            background-color: #007BFF;
            color: white;
        }

        .btn-primary:hover {
            background-color: #0056b3;
        }

        .btn-dark-mode {
            background-color: #333;
            color: white;
        }

        .btn-dark-mode:hover {
            background-color: #555;
        }

        .sidebar-section {
            margin-bottom: 20px;
        }

        .sidebar-section h3 {
            margin-bottom: 10px;
        }

        .sidebar-section ul {
            list-style: none;
            padding-left: 0;
        }

        .sidebar-section ul li {
            margin-bottom: 10px;
        }

        .sidebar-section ul li a {
            color: #007BFF;
            text-decoration: none;
        }

        .sidebar-section ul li a:hover {
            text-decoration: underline;
        }

        .video-container {
            margin-bottom: 20px;
        }

        .video-container iframe {
            width: 100%;
            height: 315px;
            border-radius: 8px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Portal de Notícias</h1>
        <button class="btn btn-dark-mode" onclick="toggleDarkMode()">Alternar Modo Escuro</button>
    </header>

    <div class="container">
        <main>
            <!-- Notícias Esportivas -->
            <article class="article">
                <img src="https://upload.wikimedia.org/wikipedia/commons/a/a6/2002_FIFA_World_Cup_Trophy.jpg" alt="Brasil Campeão 2002">
                <h2>Brasil conquista o pentacampeonato na Copa do Mundo de 2002</h2>
                <p>Em 30 de junho de 2002, a seleção brasileira venceu a Alemanha por 2 a 0 na final da Copa do Mundo, realizada no estádio de Yokohama, Japão, tornando-se a única a conquistar cinco títulos mundiais. <a href="https://memoriaglobo.globo.com/jornalismo/jornalismo-e-telejornais/jornal-nacional/reportagens-e-entrevistas/noticia/copa-do-mundo-de-2002.ghtml">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>Copa do Mundo 2014: Brasil é eliminado pela Alemanha</h2>
                <p>Em 2014, o Brasil sofreu uma derrota histórica para a Alemanha por 7 a 1 na semifinal da Copa do Mundo, no Mineirão. A partida ficou marcada como uma das maiores humilhações na história das Copas. <a href="https://www.fifa.com/worldcup/news/semi-final-day-of-dreams-for-germany-2334676">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>O futebol feminino ganha destaque com a conquista da Copa do Mundo 2019</h2>
                <p>A seleção dos Estados Unidos se sagrou campeã da Copa do Mundo de Futebol Feminino em 2019, vencendo a Holanda na final. A competição ganhou visibilidade e mais apoio para as atletas mulheres. <a href="https://www.bbc.com/portuguese/geral-48775846">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>O revezamento do Brasil na Olimpíada de Tóquio 2020</h2>
                <p>Os Jogos Olímpicos de Tóquio 2020 foram realizados em 2021 devido à pandemia de COVID-19. O Brasil teve uma excelente participação, com destaque para o atletismo e o vôlei, conquistando várias medalhas. <a href="https://www.cbc.ca/sports/olympics/olympic-medals-2020-results-1.6065144">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>A estreia de Neymar no Paris Saint-Germain em 2017</h2>
                <p>Em 2017, Neymar fez sua estreia pelo Paris Saint-Germain, após ser transferido do Barcelona por uma quantia recorde de 222 milhões de euros, tornando-se o jogador mais caro da história. <a href="https://www.espn.com.br/futebol/artigo/_/id/3141477/o-que-nem-arrebenta-no-psg-e-segundo-a-espn">Leia mais...</a></p>
            </article>

            <!-- Notícias de Economia -->
            <article class="article">
                <h2>O impacto da pandemia no mercado de trabalho</h2>
                <p>A pandemia de COVID-19 teve um impacto devastador na economia mundial, levando a demissões em massa e alterando a dinâmica do mercado de trabalho. Muitos países adotaram medidas de auxílio para mitigar os efeitos. <a href="https://www.bbc.com/portuguese/internacional-55011539">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>O crescimento do mercado de criptomoedas</h2>
                <p>Nos últimos anos, o mercado de criptomoedas tem mostrado um crescimento expressivo, com destaque para o Bitcoin, Ethereum e outras moedas digitais que vêm ganhando cada vez mais investidores. <a href="https://www.nytimes.com/2021/02/19/technology/cryptocurrency.html">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>A recuperação da economia dos Estados Unidos pós-pandemia</h2>
                <p>Após a crise causada pela pandemia de COVID-19, a economia dos Estados Unidos começou a dar sinais de recuperação, com aumento do emprego e crescimento no mercado de ações. <a href="https://www.reuters.com/business/finance/us-economy-recovery-growth-2021-08-09">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>O aumento da inflação no Brasil em 2021</h2>
                <p>Em 2021, o Brasil enfrentou um aumento significativo na inflação, afetando o poder de compra da população e gerando desafios para a economia nacional. <a href="https://g1.globo.com/economia/noticia/2021/09/13/ipca-de-agosto-tem-maior-alta-em-12-anos.ghtml">Leia mais...</a></p>
            </article>

            <article class="article">
                <h2>O impacto da mudança do governo na economia brasileira</h2>
                <p>A troca de governo no Brasil em 2022 trouxe mudanças nas políticas econômicas, com um novo foco em programas de ajuda social e mudanças nas políticas fiscais. <a href="https://www.bbc.com/portuguese/brasil-58670294">Leia mais...</a></p>
            </article>

        </main>

        <aside>
            <div class="sidebar-section">
                <h3>Categorias</h3>
                <ul>
                    <li><a href="#">Política</a></li>
                    <li><a href="#">Economia</a></li>
                    <li><a href="#">Esportes</a></li>
                    <li><a href="#">Entretenimento</a></li>
                    <li><a href="#">Tecnologia</a></li>
                </ul>
            </div>

            <div class="sidebar-section">
                <h3>Vídeos</h3>
                <!-- Botões para redirecionar aos vídeos -->
                <button class="btn btn-primary" onclick="redirectToVideo1()">Assistir Vídeo 1</button>
                <button class="btn btn-primary" onclick="redirectToVideo2()">Assistir Vídeo 2</button>
                <button class="btn btn-primary" onclick="redirectToVideo3()">Assistir Vídeo 3</button>
            </div>
        </aside>
    </div>

    <script>
        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
            document.querySelectorAll('.article').forEach(article => {
                article.classList.toggle('dark-mode');
            });
            document.querySelector('aside').classList.toggle('dark-mode');
        }

        // Funções para redirecionar para os vídeos
        function redirectToVideo1() {
            window.location.href = 'https://youtu.be/ZbWIs6z3Thw?si=l80SeAIOV3x9f4sx';
        }

        function redirectToVideo2() {
            window.location.href = 'https://youtu.be/OFhMGhvW_5I?si=rnBApNQ6pzgO_WWl';
        }

        function redirectToVideo3() {
            window.location.href = 'https://youtu.be/8fnpxU-sQ9Y?si=gsmQ_CoiUysur2Ca';
        }
    </script>

</body>
</html>
