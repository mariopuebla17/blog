---
layout: post
title: "Laço de Repetição: WHILE"
date: 2023-05-04 00:00:00 -0300
categories: desenvolvimento-de-sistemas-1
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre o laço de repetição **WHILE**

## O QUE É LAÇO DE REPETIÇÃO WHILE?

O laço de repetição **while** é uma estrutura de controle utilizada em programação que permite executar repetidamente um bloco de código enquanto uma determinada condição for verdadeira. Ou seja, enquanto a expressão booleana que é avaliada no início do laço for verdadeira, o bloco de código dentro do laço é executado repetidamente. Quando a condição se tornar falsa, a execução do laço é interrompida e o controle é passado para o próximo comando após o bloco **while**. Isso torna o **while** útil para executar ações repetidamente até que uma determinada condição seja atendida.

### Mas e aí, como fazer isso?

Necessariamente ele testa a condição e se caso for verdadeiro executa o bloco abaixo, caso seja falso ele vai para a próxima instrução fora do laço. 

```
While (Condição) 
{ 
  Comandos; 
} 
```

**Condição:** Pode ser qualquer expressão válida ou até quando a verdadeira.  
**Comando:** pode ser um bloco de comando vazio ou de repetição definido por um término.

### Exemplos

**Exemplo 1:** Imprimir os números de 1 a 10 usando um laço **WHILE**
```java
int i = 1;
while (i <= 10) 
{
   System.out.println(i);
   i++;
}
```

**Exemplo 2:** Calcular a soma dos números de 1 a 100 usando um laço **WHILE**
```java
int i = 1;
int soma = 0;
while (i <= 100) 
{
   soma += i;
   i++;
   System.out.println("A soma dos números de 1 a 100 é: " + soma);
}
```

**Exemplo 3:** Ler uma sequência de números do usuário até que ele digite um número negativo usando um laço **WHILE**
```java
Scanner scanner = new Scanner(System.in);
int numero = 0;
while (numero >= 0) 
{
   System.out.print("Digite um número: ");
   numero = scanner.nextInt();
}
System.out.println("Você digitou um número negativo. Encerrando o programa.");
```

Lembrando que, em relação ao exemplo 1, é necessário garantir que a variável utilizada para controle do laço seja inicializada antes do início do **WHILE**. Caso contrário, o bloco de código não será executado nenhuma vez.  


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!