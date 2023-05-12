---
layout: post
title: "Laço de Repetição: WHILE"
date: 2022-05-04 00:00:00 -0300
categories: desenvolvimento-de-sistemas-1
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre o laço de repetição **WHILE**

## O QUE É LAÇO DE REPETIÇÃO WHILE?

O laço de repetição while é uma estrutura de controle utilizada em programação que permite executar repetidamente um bloco de código enquanto uma determinada condição for verdadeira. Ou seja, enquanto a expressão booleana que é avaliada no início do laço for verdadeira, o bloco de código dentro do laço é executado repetidamente. Quando a condição se tornar falsa, a execução do laço é interrompida e o controle é passado para o próximo comando após o bloco while. Isso torna o while útil para executar ações repetidamente até que uma determinada condição seja atendida.

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

```c++
#include<conio.h> 
#include<stdio.h> 
 
int main() 
{ 
    int i = 0; 
    while(i < 10) 
    { 
        i = i + 1; // ou i++ 
        printf ("%d\n", i); 
    }     
return 0; 
}
```

```c++
#include<conio.h> 
#include<stdio.h> 

int main() 
{ 
    int total, num; 
    total = 0; 
    while(total < 20) 
    { 
        cout << "Total = " << total << endl; 
        cout << "Entre com um numero: ";  
        cin >> num; 
        total = total + num; 
    } 
cout << "Final total = " << total << endl; 
return 0;
} 
```

Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!