<h1>Clone do Mercado Livre</h1>

<h2>Visão Geral</h2>
<p>
	Este repositório contém uma página estática que replica a experiência visual do Mercado Livre para fins de estudo.
	A estrutura utiliza HTML semântico, CSS modularizado e JavaScript vanilla para renderizar dinamicamente uma vitrine
	de produtos e permitir buscas instantâneas.
</p>

<h2>Seções da Página</h2>
<ul>
	<li><strong>Header semântico (<code>header</code>, <code>nav</code>)</strong>: concentra logo, campo de busca e botão com ícone Font Awesome.</li>
	<li><strong>Hero (<code>section.hero</code>)</strong>: banner em tela cheia com chamada promocional e foco em campanhas sazonais.</li>
	<li><strong>Main (<code>main &gt; section</code>)</strong>: grade de cards com <code>article</code> representando cada produto, exibindo imagem, preço formatado e percentual de desconto.</li>
	<li><strong>Footer (<code>footer</code>)</strong>: assinatura simples reforçando que é um clone educacional.</li>
</ul>

<h2>Funcionalidades</h2>
<ol>
	<li>Renderização dinâmica: <code>script.js</code> percorre um array mockado e constrói o grid com template literals.</li>
	<li>Formatação monetária: a função <code>formatPrice</code> aplica locale <code>pt-BR</code> e moeda BRL.</li>
	<li>Busca unificada: tanto o clique no botão quanto a tecla Enter ativam <code>searchProducts</code>, que filtra títulos em minúsculas e re-renderiza o grid.</li>
	<li>Feedback visual: hover nos cards utiliza <code>transform</code> e <code>box-shadow</code> para reforçar interatividade.</li>
</ol>

<h2>Tecnologias Utilizadas</h2>
<ul>
	<li><strong>HTML5</strong> para marcação semântica e acessível.</li>
	<li><strong>CSS3</strong> com grid layout, variáveis de espaçamento e responsividade básica.</li>
	<li><strong>JavaScript ES6+</strong> para lógica de filtragem e manipulação do DOM.</li>
	<li><strong>Font Awesome CDN</strong> para o ícone de lupa sem arquivos locais.</li>
</ul>

<h2>Como Executar</h2>
<ol>
	<li>Clone este repositório ou faça o download do ZIP.</li>
	<li>Abra <code>index.html</code> direto no navegador ou sirva a pasta com um servidor estático simples.</li>
	<li>Digite no campo de busca e use Enter ou o botão de lupa para testar o filtro.</li>
</ol>

<h2>Estrutura dos Arquivos</h2>
<ul>
	<li><code>index.html</code>: organiza as seções, importa Font Awesome, <code>styles.css</code> e <code>script.js</code>.</li>
	<li><code>styles.css</code>: define reset, layout do header, hero, grade e interações.</li>
	<li><code>script.js</code>: lista de produtos mock, utilitários de formatação e lógica da busca.</li>
</ul>

<h2>Personalização Sugerida</h2>
<ul>
	<li>Substitua o array de <code>products</code> por dados reais de uma API REST.</li>
	<li>Ajuste cores e tipografia no CSS para simular outros temas.</li>
	<li>Inclua novos componentes semânticos (breadcrumbs, barra lateral de categorias, banners) mantendo o padrão de containers.</li>
	<li>Adicione breakpoints extras para telas menores que 768px.</li>
</ul>

<h2>Roadmap</h2>
<ol>
	<li>Implementar responsividade mobile avançada com off-canvas menu.</li>
	<li>Persistir o último termo buscado usando <code>localStorage</code>.</li>
	<li>Simular latência real com loading skeletons.</li>
	<li>Validar inputs e oferecer mensagens de “produto não encontrado”.</li>
</ol>
