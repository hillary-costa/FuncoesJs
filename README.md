# Criação de funções em JavaScript

# Declaration 

- Declaration:
  A function declaration ou declaração de função é uma forma de declarar uma função em JavaScript. Uma função é um bloco
  de código que pode ser chamado e executado em qualquer parte do progama. Para declarar uma função em JavaScript utilizando
  a Function Declaration, basta utilizar a palavra-chave function, seguida pelo nome da função e os parênteses que podem
  conter os parâmetros da função.
- Vantagens:
  Uma das vantagens é que as funções declaradas dessa forma são hoisted, ou seja, são movidas para o topo do escopo em que
  foram declaradas. Isso significa que é possível chamar uma função antes mesmo de sua declaração no código. As funções
  declaradas com Function Declaration são mais fáceis de serem identificadas e debugadas.
- Desvantagens:
  O hoisting pode causar confusão para desenvolvedores iniciantes que podem não entender por que a função funciona antes
  de ser declarada. As declarações de função não podem ser usadas diretamente como valores ou passadas como argumentos
  para outras funções.
- Exemplos;
  1. function square(numero) {
       return numero * numero;
     }
  2. function somar(a,b) {
       return a + b;
     }
  3. function dividir (h,f) {
       return h/f;
     }


# Expression

- Expression:
  Uma função JavaScript também pode ser definida usando uma expressão. Uma expressão de função pode ser armazenada
  em uma variável:
  
  1. const x = function (a,b) {return a * b}:
     
  Depois que uma expressão de função é armazenada em uma variável, a variável pode ser usada como uma função:
  
  2. const x = function (a,b) {return a * b};
     let z = x (4,3):

  A função acima é na verdade uma função anônima (uma função sem nome). Funções aramazenadas em variáveis não
  precisam de nomes. Elas são sempre invocadas (chamadas) usando o nome da variável.

- Vantagens:
  Permitem criar funções anônimas, evitando a poluição do escopo global e faciitando a criação de estruturas de
  código mais lmpas e organizadas. Além disso, são mais flexíveis.
- Desvantagens:
  Dificulta na depuração de funções anônimas, possível redução de legibilidade do código e a não possibilidade
  de uso de hoisting.

  3. let saudacao = function (nome) {
       return "Olá, " +nome+ "!";
     }

# Arrow

- Arrow:
  Uma expressão arrow function possui uma sintaxe mais curta quando comparada a uma expressão de função (function expression)
  e não tem seu própio this, argument, super ou new.target. Estas expressões de funções são melhor aplicadas para funções
  que não sejam métodos, e elas não podem ser usadas como construtores (construtors).
- Vantagens:
  Maior concisão, facilidade de leitura e de escrita, e retorno implícito para funções de uma única linha. Além disso, tem menos propensas e erros.
- Desvantagens:
  Corre o risco de sobrescrever alguma propiedade do objeto window, por que as arrow functions não tem seu tis própio.
- Exemplos:
  1. const soma = (a,b) => a + b:
  2. const quadrado = x => x * x;
  3. const numeros = [1,2,3,4,5]:
     const quadrados = numeros.map(numero => numero * numero):;
     const pares = numeros.filter(numero => numero % 2 == 0);
  



  
  
