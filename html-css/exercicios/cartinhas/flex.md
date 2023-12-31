# Flex
### HTML
```html
<div class='dv cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>
```
### CSS
```css
.dv div
{
	flex: 1;
}
.cover
{
	background-color: #264653;
}
.cover div
{
	color: #000;
	text-align: center;
}
.cover div:nth-child(1)
{
	background-color: #2a9d8f;
}
.cover div:nth-child(2)
{
	background-color: #e9c46a;
}
.cover div:nth-child(3)
{
	background-color: #f4a261;
}
.cover div:nth-child(4)
{
	background-color: #e76f51;
}
```


## Flex Horizontal `(row)`
```css
.dv
{
	display: flex;

	/* Horizontal */
	flex-direction: row;
}
```
<style>
.dv1b
{
	display: flex;
	flex-direction: row;
}
.cover div
{
	flex: 1;
}
.cover
{
	background-color: #264653;
}
.cover div
{
	color: #000;
	text-align: center;
}
.cover div:nth-child(1)
{
	background-color: #2a9d8f;
}
.cover div:nth-child(2)
{
	background-color: #e9c46a;
}
.cover div:nth-child(3)
{
	background-color: #f4a261;
}
.cover div:nth-child(4)
{
	background-color: #e76f51;
}
</style>
<div class='dv1b cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>


## Flex Horizontal invertido `(row-reverse)`
```css
.dv
{
	display: flex;

	/* Horizontal invertido */
	flex-direction: row-reverse;
}
```
<style>
.dv1c
{
	display: flex;
	flex-direction: row-reverse;
}
</style>
<div class='dv1c cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>




<br /><br />

## Flex Vertical `(column)`

```css
.dv
{
	display: flex;

	/* vertical */
	flex-direction: column;
}
```
<style>
.dv2
{
	display: flex;
	flex-direction: column;
}
</style>
<div class='dv2 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>




<br /><br />

## Flex Vertical invertido `(column-reverse)`

```css
.dv
{
	display: flex;

	/* vertical invertido */
	flex-direction: column-reverse;
}
```
<style>
.dv2b
{
	display: flex;
	flex-direction: column-reverse;
}
</style>
<div class='dv2b cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>






<br /><br />

## Espaçamento interno `(padding)`
```css
.dv
{
	display: flex;
	flex-direction: row;

	/*espaçamento interno*/
	padding: 20px;
}
```
<style>
.dv3
{
	display: flex;
	flex-direction:row;
	padding: 20px;
}
</style>
<div class='dv3 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>





<br /><br />

## Espaço entre os objetos `(gap)`
```css
.dv
{
	display: flex;
	flex-direction: row;
	padding: 20px;

	/* espaço entre os objetos */
	gap: 20px;
}
```
<style>
.dv4
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
}
</style>
<div class='dv4 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>




<br /><br />

## Tamanhos diversos `(flex: 1...)`
```css
.dv div:nth-child(1)
{
	flex: 1;
}
.dv div:nth-child(2)
{
	flex: 2;
}
.dv div:nth-child(3)
{
	flex: 3;
}
.dv div:nth-child(4)
{
	flex: 4;
}
```
<style>
.dv5
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
}
.dv5 div:nth-child(1)
{
	flex: 1;
}
.dv5 div:nth-child(2)
{
	flex: 2;
}
.dv5 div:nth-child(3)
{
	flex: 3;
}
.dv5 div:nth-child(4)
{
	flex: 4;
}
</style>
<div class='dv5 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Saltar de linha `(flex-wrap)`
## Desconsiderar tamanho padrão `(flex: none)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;

	/*
	Saltar linha

	nowrap -> Não saltar -> Default
	wrap -> Saltar
	wrap-reverse -> Quebrar pra cima
	*/
	flex-wrap: wrap;
}
.dv div:nth-child(1)
{
	/* desconsiderar tamanho padrão */
	flex: none;

	/* novo tamanho em porcentagem descontando o espaço do GAP */
	width: calc(25% - 20px);
}
.dv div:nth-child(2)
{
	flex: none;
	width: calc(75% - 20px);
}
.dv div:nth-child(3)
{
	flex: none;
	width: calc(50% - 20px);
}
.dv div:nth-child(4)
{
	flex: none;
	width: calc(50% - 20px);
}
```
<style>
.dv6
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
}
.dv6 div:nth-child(1)
{
	flex: none;
	width: calc(25% - 20px);
}
.dv6 div:nth-child(2)
{
	flex: none;
	width: calc(75% - 20px);
}
.dv6 div:nth-child(3)
{
	flex: none;
	width: calc(50% - 20px);
}
.dv6 div:nth-child(4)
{
	flex: none;
	width: calc(50% - 20px);
}
</style>
<div class='dv6 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Considerando os novos tamanhos
## Alinhando os objetos no topo `(flex-start)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;

	/* altura */
	height: 100px;

	/* Alinhando os objetos no topo */
	align-items: flex-start;
}
.dv div:nth-child(1)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv div:nth-child(2)
{
	flex: none;
	width: 50px;
	height: 50px;
}
.dv div:nth-child(3)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv div:nth-child(4)
{
	flex: none;
	width: 50px;
	height: 80px;
}
```
<style>
.dv7
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: flex-start;
}
.dv7 div:nth-child(1)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv7 div:nth-child(2)
{
	flex: none;
	width: 50px;
	height: 50px;
}
.dv7 div:nth-child(3)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv7 div:nth-child(4)
{
	flex: none;
	width: 50px;
	height: 80px;
}
</style>
<div class='dv7 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos ao centro verticalmente `(center)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;

	/* Alinhando os objetos ao centro verticalmente */
	align-items: center;
}
```
<style>
.dv8
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;
}
.dv8 div:nth-child(1)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv8 div:nth-child(2)
{
	flex: none;
	width: 50px;
	height: 50px;
}
.dv8 div:nth-child(3)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv8 div:nth-child(4)
{
	flex: none;
	width: 50px;
	height: 80px;
}
</style>
<div class='dv8 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos em baixo `(flex-end)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;

	/* Alinhando os objetos em baixo */
	align-items: flex-end;
}
```
<style>
.dv9
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: flex-end;
}
.dv9 div:nth-child(1)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv9 div:nth-child(2)
{
	flex: none;
	width: 50px;
	height: 50px;
}
.dv9 div:nth-child(3)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv9 div:nth-child(4)
{
	flex: none;
	width: 50px;
	height: 80px;
}
</style>
<div class='dv9 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos esticando `(stretch)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;

	/* Alinhando os objetos esticando */
	align-items: stretch;
}
.dv div:nth-child(1)
{
	flex: none;
	width: 50px;
	height: unset;
}
.dv div:nth-child(2)
{
	flex: none;
	width: 50px;
	height: unset;
}
.dv div:nth-child(3)
{
	flex: none;
	width: 50px;
	height: unset;
}
.dv div:nth-child(4)
{
	flex: none;
	width: 50px;
	height: unset;
}
```
<style>
.dv10
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: stretch;
}
.dv10 div:nth-child(1)
{
	flex: none;
	width: 50px;
}
.dv10 div:nth-child(2)
{
	flex: none;
	width: 50px;
}
.dv10 div:nth-child(3)
{
	flex: none;
	width: 50px;
}
.dv10 div:nth-child(4)
{
	flex: none;
	width: 50px;
}
</style>
<div class='dv10 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos na base `(baseline)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;

	/* Alinhando os objetos na base */
	align-items: baseline;
}
```
<style>
.dv11
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: baseline;
}
.dv11 div:nth-child(1)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv11 div:nth-child(2)
{
	flex: none;
	width: 50px;
	height: 50px;
}
.dv11 div:nth-child(3)
{
	flex: none;
	width: 50px;
	height: 30px;
}
.dv11 div:nth-child(4)
{
	flex: none;
	width: 50px;
	height: 80px;
}
</style>
<div class='dv11 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos à esquerda `(flex-start)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;

	/* Alinhando os objetos à esquerda */
	justify-content: flex-start;
}
```
<style>
.dv12
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;
	justify-content: flex-start;
}
.dv12 div:nth-child(1)
{
	flex: none;
	width: 50px;
}
.dv12 div:nth-child(2)
{
	flex: none;
	width: 50px;
}
.dv12 div:nth-child(3)
{
	flex: none;
	width: 50px;
}
.dv12 div:nth-child(4)
{
	flex: none;
	width: 50px;
}
</style>
<div class='dv12 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos à direita `(flex-end)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 400px;
	align-items: center;

	/* Alinhando os objetos à direita */
	justify-content: flex-end;
}
```
<style>
.dv13
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;
	justify-content: flex-end;
}
.dv13 div:nth-child(1)
{
	flex: none;
	width: 50px;
}
.dv13 div:nth-child(2)
{
	flex: none;
	width: 50px;
}
.dv13 div:nth-child(3)
{
	flex: none;
	width: 50px;
}
.dv13 div:nth-child(4)
{
	flex: none;
	width: 50px;
}
</style>
<div class='dv13 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos ao centro `(center)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 400px;
	align-items: center;

	/* Alinhando os objetos ao centro */
	justify-content: flex-end;
}
```
<style>
.dv14
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;
	justify-content: center;
}
.dv14 div:nth-child(1)
{
	flex: none;
	width: 50px;
}
.dv14 div:nth-child(2)
{
	flex: none;
	width: 50px;
}
.dv14 div:nth-child(3)
{
	flex: none;
	width: 50px;
}
.dv14 div:nth-child(4)
{
	flex: none;
	width: 50px;
}
</style>
<div class='dv14 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos `(space-between)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 400px;
	align-items: center;

	/* Alinhando os objetos space-between */
	justify-content: space-between;
}
```
<style>
.dv15
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;
	justify-content: space-between;
}
.dv15 div:nth-child(1)
{
	flex: none;
	width: 50px;
}
.dv15 div:nth-child(2)
{
	flex: none;
	width: 50px;
}
.dv15 div:nth-child(3)
{
	flex: none;
	width: 50px;
}
.dv15 div:nth-child(4)
{
	flex: none;
	width: 50px;
}
</style>
<div class='dv15 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos `(space-around)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 400px;
	align-items: center;

	/* Alinhando os objetos space-around */
	justify-content: space-around;
}
```
<style>
.dv16
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;
	justify-content: space-around;
}
.dv16 div:nth-child(1)
{
	flex: none;
	width: 50px;
}
.dv16 div:nth-child(2)
{
	flex: none;
	width: 50px;
}
.dv16 div:nth-child(3)
{
	flex: none;
	width: 50px;
}
.dv16 div:nth-child(4)
{
	flex: none;
	width: 50px;
}
</style>
<div class='dv16 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>



<br /><br />

## Alinhando os objetos `(space-evenly)`
```css
.dv
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 400px;
	align-items: center;

	/* Alinhando os objetos space-evenly */
	justify-content: space-evenly;
}
```
<style>
.dv17
{
	display: flex;
	flex-direction:row;
	padding: 20px;
	gap: 20px;
	flex-wrap: wrap;
	height: 100px;
	align-items: center;
	justify-content: space-evenly;
}
.dv17 div:nth-child(1)
{
	flex: none;
	width: 50px;
}
.dv17 div:nth-child(2)
{
	flex: none;
	width: 50px;
}
.dv17 div:nth-child(3)
{
	flex: none;
	width: 50px;
}
.dv17 div:nth-child(4)
{
	flex: none;
	width: 50px;
}
</style>
<div class='dv17 cover'>
	<div>Dv1</div>
	<div>Dv2</div>
	<div>Dv3</div>
	<div>Dv4</div>
</div>