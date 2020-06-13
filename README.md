## Curso JavaScript

## Tópicos: 
### 1-Introdução
### 2-Manipulando a DOM
### 3-App de Todos
### 4-Js assíncrono

# Aula 01
## Variáveis e dados 
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

# Aula 02
## Operações matemáticas
```
     var x = 10, y = 5;
```

#### Também posso fazer
```
     x += 3; 

     var x = 10, y = 5; 
```

#### Também posso fazer 

``` 
    x += 3; 

     x *= y; 
```

#### Posso multiplicar também por outras variáveis 


``` 
    x = x + 3;

    console.log(x); 
```
#### Como incrementar o valor de X com o número 3
```
     x *= y;
```
#### Posso multiplicar também por outras variáveis
```
     x = x + 3; 

    console.log(x);
```
#### Como incrementar o valor de X com o número 3


#### Operação matemática 
```
      var x = 10, y = 5;

      var resultado = x + y;

     console.log(resultado); 
```
### Não podemos somar uma string com um número 

### Se eu fizer isso ele irá cocatenar minha string fazendo o valor se tornar 105 ao invés de somar 

### Consigo fazer Multiplicação, Divisão, Soma, Substração e consigo fazer a operação de módulo que retorna o resto de uma divisão 

### Não podemos somar uma string com um número

###  Se eu fizer isso ele irá cocatenar minha string fazendo o valor se tornar 105 ao invés de somar

### Como criar funções

# Aula 03
##  Operações matemáticas

```
function soma(numero1, numero2){
    var resultado = numero1 + numero2;

    return resultado;
    }

    var resultado = soma(1, 2);
    
    console.log(resultado);
```

# Aula 04
## Condicionais

### Se tiver dois '==' ele verifica se os valores são iguais 
### Exemplo de verificação: 
##### Se eu colocar só o "==" ele vai me retornar true por que o valor é igual por que o valor contido nas duas váriaveis são iguais, porem o tipo delas é diferente a partir do momento que eu coloco "===" além dele verificar o valor das variáveis ele vai verificar também se o tipo das variáveis é igual e dai nesse caso vai me retornar false
```
 if (1 == "1") {

 }
```
### No exemplo abaixo eu consigo concatenar o IF O ELSE IF e o ELSE como a valvula de escape caso nenhuma das outras opções em baixo tiver entrado
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

### Abaixo: Outra opção que a gente consegue trabalhar quando estamos usando muitos IF em cima da mesma variável só verificando igualdade é trabalhar com o switch case a sintaxe do switch no JavaScript ela é muito parecida com a sintaxe das outras linguagens

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

### Acima: Então basicamente o que eu aprendi nessa aula foi fazer uma estrutura um condicional simples ultilizando o IF o ELSEIF e também o ELSE e ultilizar o switch case quando a gente precisa verificar a igualdade de valores de uma mesma variavel multiplas vezes

# Aula 05
## Operadores lógicos

```
    // AND, OR, NOT

        var sexo = 'F';


        if (sexo !== 'M') {
            console.log('OK');
            }
```

### Acima: Basicamente esses são os três operadores lógicos que eu mais irei ultilizar nas condições do Javascript 

### Abaixo: Veja que eu armazenei o valor da condição dentro do IF ou seja se ele for masculino é TRUE e se for feminino é FALSE

```
// AND, OR, NOT

    var sexo = 'F';


        if (sexo !== 'M') {
            console.log('OK');
        }
```

### Abaixo: O que eu posso fazer para deixar isso menor ainda
```
    // AND, OR, NOT

        var sexo = 'M';

            var masculino = sexo === 'M';

            console.log(masculino)
```

### Acima: Se eu colocar o F no lugar do M vai dar False e eu deixar o M vai dar true então dentro do Javascript dentro do IF ela sempre retorna um TRUE ou um FALSE e como aqui eu estou realizando apenas uma condição não preciso nem dos parentes essa foi a aula de operadores lógicos e também sobre armazenamento dessas variáveis aqui dessas condições dentro dessas variáveis 

# Aula 06

## Condição ternária

```
    var sexo = 'M';


        var retorno = (sexo === 'M') ? 'Masculino' : 'Feminino'
            console.log(retorno);
```

### Acima: Isso é uma condição ternária quando a gente na mesma linha ultilizando o sinal de "?" e ":" a gente faz uma condição simples para verificar se uma variavel entra em uma condição simples se não a gente coloca outro valor 

# Aula 07

## Estruturas de repetição

```
    // for, while

        for (var i = 0; i <= 100; i++){
            console.log(i);
        } //Intervalo

        var j = 0;

            while (j <= 100) {
                console.log(j);

                j++;
            }
```

## Aula 08

#### Intervalo e timeout

```
    function exibeAlgo(){
        console.log("Hello World")
        }

    setTimeout(exibeAlgo, 5000);
```

# DESAFIO
## 1º Exercício


### Crie uma função que dado o objeto a seguir:

var endereco = {
 rua: "Rua dos pinheiros",
 numero: 1293,
 bairro: "Centro",
 cidade: "São Paulo",
 uf: "SP"
};

## Retorne o seguinte conteúdo: 
#### O usuário mora em São Paulo / SP, no bairro Centro, na rua "Rua dos Pinheiros" com nº 1293.


# Resposta:
# 1º Exercicio
```
    var rua = "Rua dos pinheiros"
    var numero = 1293
    var bairro = "Centro,"
    var cidade = "São Paulo"
    var uf = "SP,"

        console.log("O usuario mora em", cidade, "/", uf, "no bairro", bairro, "na rua", rua, "com nº", numero)
```

# 2º Exercicio:
### Crie uma função que dado um intervalo (entre x e y) exiba todos número pares:

```
function pares(x, y) {
 // código aqui
}

pares(32, 321);
```

# Resposta:

```
    function pares(x, y) {
        var par = x % 2 == 0;

            return par;

        }
        var resultado = pares(22, 32, 321);

        console.log(resultado)
```
# 3º Exercicio:

### Escreva uma função que verifique se o vetor de habilidades passado possui a habilidade "Javascript" e retorna um booleano true/false caso exista ou não.

## Exemplo:
function temHabilidade(skills) {
 // código aqui
}
var skills = ["Javascript", "ReactJS", "React Native"];
temHabilidade(skills); // true ou false

# Resposta:
```
    function temHabilidades(skills) {
        var skill;
            if (skills.indexOf('Javascript')) {
                return false;
            } else {
                return true;
            }
        }
        var skills = ['Javascript'];
        console.log(temHabilidades(skills));
```
# 4º Exercicio:

### Escreva uma função que dado um total de anos de estudo retorna o quão experiente o usuário é:

## Exemplo:

```
    function experiencia(anos) {
        // código aqui
    }
var anosEstudo = 7;
experiencia(anosEstudo);

// De 0-1 ano: Iniciante
// De 1-3 anos: Intermediário
// De 3-6 anos: Avançado
// De 7 acima: Jedi Master
```

# Resposta: 

```
    function experiencia(anos) {
        if (anos < 0) return 'Impossivel';        
           switch (anos) {
                case 0:
                case 1:
                   return 'Iniciante';
                case 2:
                case 3:
                   return 'Intermediário'
                case 4:
                case 5:
                case 6: 
                    return 'Avançado'
                case 7:
                    return 'Jedi Master'
           }
        }
        var anosEstudo = 7;
        console.log(experiencia(anosEstudo));

// De 0-1 ano: Iniciante
// De 1-3 anos: Intermediário
// De 3-6 anos: Avançado
// De 7 acima: Jedi Master
```

# 5º Exercicio:

### Dado o seguinte vetor de objetos:

## Exemplo:

```
var usuarios = [
    {
        nome: "Diego",
        habilidades: ["Javascript", "ReactJS", "Redux"]
 },
 {
    nome: "Gabriel",
    habilidades: ["VueJS", "Ruby on Rails", "Elixir"]
 }
];
```
### Escreva uma função que produza o seguinte resultado:

## Exemplo: 
```
O Diego possui as habilidades: Javascript, ReactJS, Redux
O Gabriel possui as habilidades: VueJS, Ruby on Rails, Elixir
```

# Resposta:
```
    var usuarios = [
        {
            nome: 'Diego',
            habilidades: ['Javascript', 'ReactJS', 'Redux']
        },
        {
            nome: 'Gabriel',
            habilidades: ['VueJS', 'Ruby on Rails', 'Elixir']
        }
    ]

        for (let usuario of usuarios) {
            console.log('O ' + usuario.nome + ' possui as habilidades: ' + usuario.habilidades.join(", "));
    }
```

# ===================================

# Manipulando a DOM

# AULA 01

## Eventos inline

### DOM é a árvore de elementos do nosso HTML a DOM é composta por todos os elementos visualmente dispostos em tela então basicamente é isso que o Javascript vai poder controlar vamos poder por exemplo manipular quando um elemento é clicado quando alguma informação é passado o mouse por cima e assim por diante a gente consegue fazer várias coisas manipulando esses elementos da DOM como descobrir quando um úsuario clickou ou não um botão ou quando passou o mouse por cima isso não vale só para botão esses eventos que a gente vai aplicar no Mobal em sí eles podem ser ultilizados em qualquer outro elemento da DOM qualquer outro elemento HTML

```
    <div id="app">
        <input onkeypress="mostraAlerta()" />
    </div>

    <script>
        function mostraAlerta() {
            alert('Botão foi clicado');
        }
    </script>
```

## Trabalhando com a DOM

# AULA 02

### Como buscar um função na nossa árvore de elementos atraves do nosso script

```
    <div id="app">
        <input type="text" name="nome" />
        <button class="botao">Adicionar</button>
    </div>

    <script>
       var inputElement = document.querySelector('input[name=nome]')

       var btnElement = document.querySelector('button.botao');


        btnElement.onclick = function () {
            var text = inputElement.value;

            alert(text);
        }
    </script>
```

## Lidando com elementos

# Aula 03

## Além da gente poder referênciar elementos da nossa DOM atráves do Javascript a gente pode criar novos elementos atráves do Javascript

```
    <div id="app">
        <input id='nome' />
    </div>

    <script>
        var linkElement = document.createElement('a')

        linkElement.setAttribute('href', 'http://rocketseat.com.br');

        linkElement.setAttribute('title', 'Site da Rocketseat');


        var textElement = document.createTextNode('Acessar site da Rocketseat');

        linkElement.appendChild(textElement);

        var containerElement = document.querySelector('#app')

        containerElement.appendChild(linkElement);

        var inputElement = document.querySelector('#nome')

        containerElement.removeChild(inputElement)
    </script>
```

