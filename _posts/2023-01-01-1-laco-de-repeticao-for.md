---
layout: post
title: "Laço de Repetição: FOR"
date: 2023-01-01 00:01:00 -0300
categories: desenvolvimento-de-sistemas-1
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre o laço de repetição **FOR**

## O QUE É LAÇO DE REPETIÇÃO FOR?


![](https://github.com/mariopuebla17/blog/blob/main/_images/202301/pw1.jpeg?raw=true)

O laço de repetição **FOR** é uma estrutura de controle em programação que permite a execução repetida de um bloco de código por um número conhecido de vezes. Ele é especialmente útil quando **se deseja iterar sobre uma sequência de elementos, como uma lista, tupla ou string**, executando uma ação para cada item. A sintaxe básica do **FOR** consiste em uma variável que assume o valor de cada elemento da sequência em cada iteração, seguida por dois pontos e o bloco de código a ser executado. Ao final de cada iteração, a variável é atualizada para o próximo elemento da sequência até que todos os elementos tenham sido processados.

```
for (comandos de inicialização;condição de teste;incremento/decremento) 
{ 
    // comandos a serem repetidos 
    // comandos a serem repetidos 
}
```

### Mas e aí, como fazer isso?

O funcionamento é o seguinte: 

1\. Executa os comandos de inicialização;
2\. Testa a condição;
3\. Se a condição for falsa então executa o comando que está logo após o bloco subordinado ao **FOR**
4\. Se condição for verdadeira então executa os comandos que estão subordinados ao **FOR**
5\. Executa os comandos de incremento/decremento
6\. Volta ao passo 2


O comando **FOR** deve ser usado sempre que: 

. soubermos exatamente quantas vezes o laço deve ser repetido;  
. o teste deva ser feito antes da execução de um bloco de comandos;  
. houver casos em que o laço não deva ser repetido nenhuma vez. 

### Exemplos

```c++
int contador; 

for (contador = 0; contador < 10; contador = contador+1) 
{ 
    printf(contador); 
} 

printf("FIM LAÇO");
```  


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!