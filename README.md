# Simulador de Loteria

Este projeto é um simulador da *megasenna*,onde o usuário digita seis números
e sorteamos aleatoriamente outros seis números e comparamos para verificar
quantos números você acertou.

**Não é para jogos oficiais**

## Tecnologias utilizadas
1. **HTML**: HTML é uma linguagem de marcação utilizada na construção da estrutura de páginas na Web.
2. **CSS**: Cascading Style Sheets (CSS) é um mecanismo para adicionar estilo (cores, fontes, espaçamento, etc.) a um documento web.
3. **JS**: JavaScript (frequentemente abreviado como JS) é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica fraca e multiparadigma (protótipos, orientado a objeto, imperativo e, funcional).
4. ~~**Jquery**~~: não foi utilizado.


## Funções Principais
Aqui será apresentado as duas funções principais do site


### Sorteio de numeros
Nessa função os números são sorteados aleatoriamente
```
function sortearNumeros() {
  numSort = [];
  let sort;
  for (var i = 0; i < 6; i++) {
    do{
      sort = Math.ceil(Math.random() * 60);
      sort = (sort == 0) ? 1 : sort;
      }while (numSort.includes(sort));
      numSort.push(sort);
  }
}  




```


### Lendo os números digitados
Lê as entradas de numero digitadas pelo usuário
```
function addToList(num, pos) {
  if(num.lenght == 2){
  if (numEsco.includes(num)) {
    alert("Numero Escolhido Anteriormente.Digite outro numero")
    }else if(parseInt(num) > 60){
      alert("O numero digitado não pode ser maior que 60")
      }else {
        numEsco[pos-1] = num;
  }
 }
}
```

## Como Rodar o código
> Simplesmente baixe o codigo e abra o arquivo
**_index.html_** no seu navegador

## Imagens da tela
tela 1: tela de abertura
![tela 1](/imagens/tela1.png)

#### referências
* HTML: [wikipedia](https://pt.wikipedia.org/wiki/HTML)
* CSS: [w3school](https://www.w3schools.com/css/)
* JavaScript: [wikipedia](https://pt.wikipedia.org/wiki/JavaScript)
