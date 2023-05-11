# Anotações de aulas Back-End

Usando como exemplo um exercicio onde deve-se calcular a media da matéria de Português onde as notas devem ser maior que 5.

## Function

```js
function verificarNota(notaAtiv, notaRedac) {
  let media = (notaAtiv + notaRedac) / 2;
  
 if(notaAtiv > 5 || notaRedac > 5){
        return("Todas as suas notas devem ser menor que 5!");
   }else{
        return("A média de português é: " + media);
  }
}
console.log(verificarNota(4, 8))
```

## Arrow Function:

```js
//Calculo da média + notas > 5
const verificarNota = (notaAtiv, notaRedac) => {
  let media = (notaAtiv + notaRedac) / 2;
  if (notaAtiv > 5 || notaRedac > 5){
        return("Ambas as notas devem ser maiores que 5!")
   }else{
        return("Sua média de português é: " + media);
  }
}

console.log(verificarNota(2, 8))
```

### Declarando a função das duas formas

```js
//Usando function
function dobro(num) {
  return num * 2;
}
console.log(dobro(6));
```

Neste caso a não utilização do () e {} funciona apenas para funções mais simples:
```js
//Usando Arrow function "=>"
const dobroArrow = num => num * 2;
console.log(dobroArrow(5));
```
### Operador Ternário:

Uma forma simplificada de utilisar o *if* e *else*
```js
//esfrututra: (conddição ? if : else)
console.log(1==2 ? "Verdade" : "Mentira")
```
Respondendo o exercício usando o **Operador Tenário**
```js
const verificarNota = (notaAtiv, notaRedac) => {
  let media = (notaAtiv + notaRedac) / 2;
  
  return(notaAtiv > 5 || notaRedac > 5 ? 
              "Sua nota deve não poder ser maior que 5" : "A média de português é: " + media )
}
console.log(verificarNota(4, 2))
```

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Diferença entre *return* e *console.log* :

* A declaração **return** finaliza a execução de uma função e especifica os valores que devem ser retonados para onde a função foi chamada.

* O **console.log** exibe uma mensagem no console (essa mensagem pode ser o resultado de uma função, variável ou algo estático)
