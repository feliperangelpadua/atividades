# Exercicio 1
## Tags
```html
<head>Cabeçalho</head>
<title>Título</title>
<style>EStilo</style>
<body>Corpo</body>
	Atributos
	align -> alinhamento
	title -> Hint
	onclick -> Função ao clicar
	onmousehover -> Função ao parar em cima
	onmouseout -> Função ao sair de cima
	style -> estilo
	class -> Classe
	id -> ID
<h1>Heading -> Título para o corpo</h1>
	Atributos
	align -> alinhamento
	title -> Hint
	onclick -> Função ao clicar
	onmousehover -> Função ao parar em cima
	onmouseout -> Função ao sair de cima
	style -> estilo
	class -> Classe
	id -> ID
<p>parágrafo</p>
	Atributos
	align -> alinhamento
	title -> Hint
	onclick -> Função ao clicar
	onmousehover -> Função ao parar em cima
	onmouseout -> Função ao sair de cima
	style -> estilo
	class -> Classe
	id -> ID
<div>Seção</div>
	Atributos
	align -> alinhamento
	title -> Hint
	onclick -> Função ao clicar
	onmousehover -> Função ao parar em cima
	onmouseout -> Função ao sair de cima
	style -> estilo
	class -> Classe
	id -> ID
<img> <- Imagem
	Atributos
	src -> Endereço da imagem
	alt -> Texto quando para em cima (Hint)
	border -> Borda
	title -> Hint
	onclick -> Função ao clicar
	onmousehover -> Função ao parar em cima
	onmouseout -> Função ao sair de cima
	style -> estilo
	class -> Classe
	id -> ID
<input> <- Entrada
	Atributos
	align -> alinhamento
	title -> Hint
	onclick -> Função ao clicar
	onmousehover -> Função ao parar em cima
	onmouseout -> Função ao sair de cima
	style -> estilo
	class -> Classe
	id -> ID
	value -> Valor
	placeholder -> texto que fica lá até alguem digitar
<hr> <- desenha um linha
<br> <- saltar linha
<!--comentário-->
```

## CSS
```css
.classe
{
	/*tipo de letra*/
	font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

	/*tamanho da letra*/
	font-size: 20px;

	/*negrito*/
	font-weight: bold;

	/*italico*/
	font-style: italic;

	/*cor da letra*/
	color: #fff;

	/*cor do fundo*/
	background-color: #f80;

	/*imagem de fundo*/
	background-image: url('pasta/nome_img.jpg');

	/*tamanho da img de fundo (largura/altura)*/
	background-size: 50px 50px;

	/*posicao da img de fundo (left,top,bottom,right ou 5px 10px (5px da esquerda e 10px do topo))*/
	background-position: center;

	/*repetição da img do fundo*/
	background-repeat: no-repeat;

	/*largura*/
	width: 800px;

	/*altura*/
	height: 600px;

	/*altura da linha (alinha verticalmente)*/
	line-height: 60px;

	/*alinhamento do texto*/
	text-align: center;

	/*ponteiro do mouse*/
	cursor: pointer;

	/*sombra da caixa (x,y,esfumaçamento,cor)*/
	box-shadow: 0px 0px 20px #aa00ff44;

	/*sombra do texto (x,y,esfumaçamento,cor)*/
	text-shadow: 0px -2px 0px #6600bb;

	/*margem*/
	margin: 20px;

	/*borda(largura,tipo,cor)*/
	border: 1px solid red;

	/*arredondamento de borda*/
	border-radius: 50px;

	/*espaçamento interno*/
	padding: 20px;
}

/*:hover -> ao parar com mouse em cima*/
#idObjeto:hover
{
	...
}
```