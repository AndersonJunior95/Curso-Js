## Curso JavaScript

## Tópicos: 
### 1-Introdução
### 2-Manipulando a DOM
### 3-App de Todos
### 4-Js assíncrono

## Aula 01
#### Variáveis e dados 
```
    var nome = "Anderson";
    var idade = 14;
    var peso = 45;
    var humano = true;

    var alunos = ["Anderson", "Jefersson", "Kayk"];

    var aluno = {
    nome: "Anderson",
    peso: 45,
    humano: true
    };
```
    console.log(peso);

## Aula 02
#### Operações matemáticas
```
     var x = 10, y = 5;
```

###### Também posso fazer
```
     x += 3; 

     var x = 10, y = 5; 
```

###### Também posso fazer 

``` 
    x += 3; 

     x *= y; 
```

###### Posso multiplicar também por outras variáveis 


``` 
    x = x + 3;

    console.log(x); 
```
###### Como incrementar o valor de X com o número 3
```
     x *= y;
```
###### Posso multiplicar também por outras variáveis
```
     x = x + 3; 

    console.log(x);
```
###### Como incrementar o valor de X com o número 3


###### Operação matemática 
```
      var x = 10, y = 5;

      var resultado = x + y;

     console.log(resultado); 
```
##### Não podemos somar uma string com um número 

##### Se eu fizer isso ele irá cocatenar minha string fazendo o valor se tornar 105 ao invés de somar 

##### Consigo fazer Multiplicação, Divisão, Soma, Substração e consigo fazer a operação de módulo que retorna o resto de uma divisão 

#####  Não podemos somar uma string com um número

#####  Se eu fizer isso ele irá cocatenar minha string fazendo o valor se tornar 105 ao invés de somar

#####  Consigo fazer Multiplicação, Divisão, Soma, Substração e consigo fazer a operação de módulo que retorna o resto de uma divisão

##### Como criar funções

## Aula 03

```
function soma(numero1, numero2){
    var resultado = numero1 + numero2;

    return resultado;
    }

    var resultado = soma(1, 2);
    
    console.log(resultado);
```

## Aula 04

##### Se tiver dois '==' ele verifica se os valores são iguais 
### Exemplo de verificação: 
##### Se eu colocar só o "==" ele vai me retornar true por que o valor é igual por que o valor contido nas duas váriaveis são iguais, porem o tipo delas é diferente a partir do momento que eu coloco "===" além dele verificar o valor das variáveis ele vai verificar também se o tipo das variáveis é igual e dai nesse caso vai me retornar false
```
 if (1 == "1") {

 }
```
##### No exemplo abaixo eu consigo concatenar o IF O ELSE IF e o ELSE como a valvula de escape caso nenhuma das outras opções em baixo tiver entrado
```
    function retornaSexo(sexo){
        // M, F
        // Masculino, Feminino

                
    if (sexo === 'M'){
        return "Masculino";
            } else if (sexo === 'F') {
                return 'Feminino';
                } else{
                    return 'Outro';
                }
            }
```

#### Abaixo: Outra opção que a gente consegue trabalhar quando estamos usando muitos IF em cima da mesma variável só verificando igualdade é trabalhar com o switch case a sintaxe do switch no JavaScript ela é muito parecida com a sintaxe das outras linguagens

```
    function retornaSexo(sexo){
        switch (sexo) {
            case 'M':
                return 'Masculino';
            case 'F':
                return 'Feminino';
            default: 
                return: 'Outro';
                }
            }

            var resultado = retornaSexo("M");
    
            console.log(resultado);
```

#### Acima: Então basicamente o que eu aprendi nessa aula foi fazer uma estrutura um condicional simples ultilizando o IF o ELSEIF e também o ELSE e ultilizar o switch case quando a gente precisa verificar a igualdade de valores de uma mesma variavel multiplas vezes

## Aula 05

```
    // AND, OR, NOT

        var sexo = 'F';


        if (sexo !== 'M') {
            console.log('OK');
            }
```

#### Acima: Basicamente esses são os três operadores lógicos que eu mais irei ultilizar nas condições do Javascript 

#### Abaixo: Veja que eu armazenei o valor da condição dentro do IF ou seja se ele for masculino é TRUE e se for feminino é FALSE

```
// AND, OR, NOT

    var sexo = 'F';


        if (sexo !== 'M') {
            console.log('OK');
        }
```

#### Abaixo: O que eu posso fazer para deixar isso menor ainda
```
    // AND, OR, NOT

        var sexo = 'M';

            var masculino = sexo === 'M';

            console.log(masculino)
```

#### Acima: Se eu colocar o F no lugar do M vai dar False e eu deixar o M vai dar true então dentro do Javascript dentro do IF ela sempre retorna um TRUE ou um FALSE e como aqui eu estou realizando apenas uma condição não preciso nem dos parentes essa foi a aula de operadores lógicos e também sobre armazenamento dessas variáveis aqui dessas condições dentro dessas variáveis 