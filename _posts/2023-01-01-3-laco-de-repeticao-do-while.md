---
layout: post
title: "Laço de Repetição: DO WHILE"
date: 2023-01-01 00:03:00 -0300
categories: desenvolvimento-de-sistemas-1
author: Escrito por Prof. Mario Herrera
---

Olá! Hoje vamos falar sobre o laço de repetição **DO WHILE**

## O QUE É LAÇO DE REPETIÇÃO DO WHILE?


![](https://github.com/mariopuebla17/blog/blob/main/_images/202301/pw1.jpeg?raw=true)

O laço de repetição **DO WHILE** é uma estrutura de controle de fluxo em programação que permite a execução repetida de um bloco de código enquanto uma condição é verdadeira. A diferença entre este laço e outros como o **WHILE** é que o **DO WHILE** executa o bloco de código pelo menos uma vez, independentemente da condição ser verdadeira ou falsa.

### Mas e aí, como fazer isso?

A sintaxe básica do **DO WHILE** é a seguinte:

```
do {
   // código a ser executado
} while (condição);
```

No exemplo acima, o bloco de código dentro das chaves é executado pelo menos uma vez antes de verificar a condição especificada no final do laço. Se a condição for verdadeira, o bloco de código é executado novamente e o processo continua até que a condição seja falsa.

### Exemplos

**Exemplo 1:** Imprimir os números de 1 a 10 usando um laço **DO WHILE**
```c#
int i = 1;
do 
{
   System.out.println(i);
   i++;
} while (i <= 10);
System.out.println(i);
```

**Exemplo 2:** Calcular a soma dos números de 1 a 100 usando um laço **DO WHILE**
```c#
int i = 1;
int soma = 0;
do {
   soma += i;
   i++;
} while (i <= 100);
System.out.println("A soma dos números de 1 a 100 é: " + soma);
```

**Exemplo 3:** Ler uma sequência de números do usuário até que ele digite um número negativo usando um laço **DO WHILE**
```c#
Scanner scanner = new Scanner(System.in);
int numero;
do {
   System.out.print("Digite um número: ");
   numero = scanner.nextInt();
} while (numero >= 0);
System.out.println("Você digitou um número negativo. Encerrando o programa.");
```  


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu! 