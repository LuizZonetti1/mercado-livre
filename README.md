<!DOCTYPE html>
<html lang="pt-BR">

<head>
	<meta charset="UTF-8" />
	<title>README · Clone do Mercado Livre</title>
</head>

<body>
	<header>
		<h1>Clone do Mercado Livre</h1>
		<p>
			Interface front-end inspirada na home do Mercado Livre, desenvolvida para estudos de HTML, CSS e JavaScript
			vanilla.
			O projeto replica a estrutura visual de busca, vitrines e destaque promocional, permitindo experimentos com
			filtragem de produtos e componentes reutilizáveis.
		</p>
		<nav aria-label="Sumário">
			<ul>
				<li><a href="#sobre">Sobre</a></li>
				<li><a href="#recursos">Recursos</a></li>
				<li><a href="#tecnologias">Tecnologias</a></li>
				<li><a href="#execucao">Como Executar</a></li>
				<li><a href="#estrutura">Estrutura</a></li>
				<li><a href="#personalizacao">Personalização</a></li>
				<li><a href="#roadmap">Roadmap</a></li>
			</ul>
		</nav>
	</header>

	<main>
		<section id="sobre">
			<h2>Sobre o Projeto</h2>
			<p>
				A aplicação carrega uma lista mockada de produtos, renderiza cards dinamicamente e disponibiliza um campo
				de busca com suporte tanto ao clique no botão quanto ao uso da tecla Enter. O layout prioriza o visual
				característico do Mercado Livre, com hero em tela cheia, identidade amarela predominante e destaque para
				valores promocionais.
			</p>
		</section>

		<section id="recursos">
			<h2>Recursos Principais</h2>
			<ul>
				<li>Filtro de produtos instantâneo reutilizando a mesma lógica para botão e tecla Enter.</li>
				<li>Grade responsiva de cards com imagens, preço formatado em Real e destaque de desconto.</li>
				<li>Seção hero com imagem de campanha e chamada para ação.</li>
				<li>Microinterações em hover, tipografia consistente e espaçamentos alinhados ao branding original.</li>
			</ul>
		</section>

		<section id="tecnologias">
			<h2>Tecnologias Utilizadas</h2>
			<dl>
				<dt>HTML5</dt>
				<dd>Estrutura semântica da página, containers reutilizáveis e integração com CDN de ícones.</dd>
				<dt>CSS3</dt>
				<dd>Layout responsivo em grid, estilização do header, hero e cartas, além de micro animações.</dd>
				<dt>JavaScript (ES6+)</dt>
				<dd>Renderização dos produtos, formatação monetária e lógica de busca.</dd>
				<dt>Font Awesome CDN</dt>
				<dd>Ícone do botão de busca, dispensando assets locais.</dd>
			</dl>
		</section>

		<section id="execucao">
			<h2>Como Executar Localmente</h2>
			<ol>
				<li>Clone este repositório ou faça download do pacote ZIP.</li>
				<li>Abra <code>index.html</code> diretamente no navegador ou sirva a pasta usando qualquer servidor estático (ex.: <code>npx serve</code>).</li>
				<li>Utilize o campo de busca para filtrar os produtos e pressione Enter ou clique na lupa para disparar o filtro.</li>
			</ol>
		</section>

		<section id="estrutura">
			<h2>Estrutura do Projeto</h2>
			<pre>
<code>index.html   <!-- Estrutura da página e importação de assets -->
styles.css   <!-- Estilos globais, cabeçalho, hero, grid e rodapé -->
script.js    <!-- Mock de produtos, formatação e lógica de busca -->
</code>
			</pre>
			<article aria-label="Fluxo da busca">
				<h3>Fluxo da funcionalidade de busca</h3>
				<p>
					O listener de <code>DOMContentLoaded</code> renderiza todos os produtos inicialmente, associa o clique do botão <code>#searchBtn</code> à função
					<code>searchProducts</code> e adiciona um <code>keydown</code> ao campo <code>#searchInput</code> para ouvir Enter. A filtragem compara o valor digitado
					com títulos em caixa baixa e re-renderiza o grid com o resultado.
				</p>
			</article>
		</section>

		<section id="personalizacao">
			<h2>Personalização</h2>
			<ul>
				<li>Troque a lista de objetos em <code>script.js</code> por dados de uma API real ou arquivo JSON.</li>
				<li>Ajuste cores, espaçamentos e tipografia em <code>styles.css</code> para testar variações de branding.</li>
				<li>Inclua novas seções (categorias, banners, depoimentos) reutilizando a classe <code>.container</code>.</li>
				<li>Adicione breakpoints extras para otimizar a experiência mobile.</li>
			</ul>
		</section>

		<section id="roadmap">
			<h2>Roadmap e Próximos Passos</h2>
			<ol>
				<li>Tornar o layout completamente responsivo abaixo de 768&nbsp;px.</li>
				<li>Persistir o termo pesquisado usando <code>localStorage</code>.</li>
				<li>Exibir skeleton loading enquanto simula requisições assíncronas.</li>
				<li>Integrar com uma API pública para substituir o mock local.</li>
			</ol>
		</section>
	</main>

	<footer>
		<p>Projeto educacional mantido por LuizZonetti1 · Atualizado em 2025.</p>
	</footer>
</body>

</html>
