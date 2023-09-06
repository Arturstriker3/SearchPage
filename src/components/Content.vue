<template>
	<a class="mainhyper" href="#">
		<div class="comp-box">
			<div class="card-tag">
				<img id="dateimg" src="@/assets/hostico.webp" alt="dateimg">
				<span>01/04/2023</span>
			</div>
			<div class="main-content">
				<img id="main-img" src="db/image1.webp" alt="dateimg">
				<p>GPT, tradução automática e o quão bons eles são: uma avaliação abrangente</p>
				<span>Artigo Publicado por Priscila Soares</span>
			</div>
			<div class="content-tags">
				<div id="tag">
					<div id="fig1"></div>
					<span>Ciências da Computação</span>
				</div>
				<div id="tag">
					<div id="fig2"></div>
					<span>IA</span>
				</div>
			</div>
		</div>
	</a>
</template>

<script setup>

</script>

<style scoped>

	/* Estilização da Box */

	.comp-box{
		width: 270px;
		height: 278px;
		background-color: var(--Bcolor);
		flex: none;
		align-items: center;
		overflow: hidden; /* Evitar vazamento de conteúdo */
		border-radius: 10px; /* Cantos arredondados */
	}

	/* Estilização do Hyperlink */
	.mainhyper a{
		width: 100%; /* Ocupar 100% da largura da comp-box */
		height: 100%; /* Ocupar 100% da altura da comp-box */
		display: block; /* Garantir que ocupe toda a largura disponível */
		text-decoration: none; /* Remover sublinhado padrão */
		will-change: filter;
        transition: filter 300ms;
	}

	.mainhyper:hover{
		filter: drop-shadow(0 0 0.5em var(--black));
        background-color: transparent;
        opacity: 0.85;
	}

	/* Estilização Data */

	.card-tag{
	padding: 5px 10px;
	color: var(--black);
	border-radius: 2px;
	display: flex;
	align-items: center;
	gap: 10px;
	}

	.card-tag span{
	font-size: 15px;
	}

	#dateimg{
		width: 15px;
		height: 15px;
	}

	/* Estilização Conteúdo Central */

	.main-content {
	display: flex; /* Tornar a div um container flexível */
	flex-direction: column; /* Alinhar os elementos verticalmente */
	align-items: center; /* Centralizar horizontalmente */
	text-align: center; /* Centralizar o texto horizontalmente */
	}
	
	.main-content p{
		font-size: 14px; /* Tamanho da fonte do parágrafo */
  		margin: 1px 0; /* Margem superior e inferior para separar o texto */
		font-weight: bold; /* Define o texto como negrito */
  		color: var(--black); /* Define a cor do texto (por exemplo, vermelho) */
	}

	.main-content span{
		font-size: 14px; /* Tamanho da fonte da assinatura */
		color: var(--black);
		font-size: 12px;
		margin: 2px 0;
	}

	#main-img{
		width: 90px;
		height: 90px;
		border-radius: 10px; /* Cantos arredondados */
	}

	/* Estilização Tags */

	.content-tags{
		margin: 3px 0;
		display: flex;
		align-items: center;
		flex-direction: column; /* Colocar os elementos em coluna */
	}

	.content-tags span{
		font-size: 15px;
		font-weight: bold;
		color: var(--black);
	}

	#tag {
	display: flex; /* Usar flexbox para alinhar os elementos lado a lado */
	align-items: center; /* Centralizar verticalmente os elementos */
	margin-top: 10px;
	}

	#fig1{
		width: 25px;
		height: 8px;
		background-color: var(--color1);
		border-radius: 25px; /* Define o raio dos cantos para criar um retângulo arredondado */
		margin-right: 5px; /* margem direita */
	}

	#fig2{
		width: 25px;
		height: 8px;
		background-color: var(--color3);
		border-radius: 25px; /* Define o raio dos cantos para criar um retângulo arredondado */
		margin-right: 5px; /* margem direita */
	}



</style>