---
layout: post
title: "Laço de Repetição: SWITCH"
date: 2023-06-01 00:00:00 -0300
categories: dsenvolvimento-de-sistemas-1
author: Escrito por Mario Herrera
---
 
Olá! Hoje vamos falar sobre o laço de repetição **SWITCH**

## O QUE É LAÇO DE REPETIÇÃO SWITCH?


O laço de repetição **switch** é uma estrutura de controle em linguagens de programação que permite a seleção entre várias opções de execução com base em uma expressão ou valor. Ele oferece uma alternativa concisa e legível para estruturas de controle condicional, como o **if-else** encadeado, especialmente quando existem múltiplas condições a serem verificadas.

### Mas e aí, como fazer isso?

1\. Verificação de dia da semana:

```c++
#include <iostream>
using namespace std;

int main() {
    int dia;
    cout << "Digite o número do dia da semana (1-7): ";
    cin >> dia;

    switch (dia) {
        case 1:
            cout << "Domingo" << endl;
            break;
        case 2:
            cout << "Segunda-feira" << endl;
            break;
        case 3:
            cout << "Terça-feira" << endl;
            break;
        case 4:
            cout << "Quarta-feira" << endl;
            break;
        case 5:
            cout << "Quinta-feira" << endl;
            break;
        case 6:
            cout << "Sexta-feira" << endl;
            break;
        case 7:
            cout << "Sábado" << endl;
            break;
        default:
            cout << "Dia inválido" << endl;
            break;
    }

    return 0;
}
```

2\. Verificação de mês do ano:

```c++
#include <iostream>
using namespace std;

int main() {
    int mes;
    cout << "Digite o número do mês (1-12): ";
    cin >> mes;

    switch (mes) {
        case 1:
            cout << "Janeiro" << endl;
            break;
        case 2:
            cout << "Fevereiro" << endl;
            break;
        case 3:
            cout << "Março" << endl;
            break;
        case 4:
            cout << "Abril" << endl;
            break;
        case 5:
            cout << "Maio" << endl;
            break;
        case 6:
            cout << "Junho" << endl;
            break;
        case 7:
            cout << "Julho" << endl;
            break;
        case 8:
            cout << "Agosto" << endl;
            break;
        case 9:
            cout << "Setembro" << endl;
            break;
        case 10:
            cout << "Outubro" << endl;
            break;
        case 11:
            cout << "Novembro" << endl;
            break;
        case 12:
            cout << "Dezembro" << endl;
            break;
        default:
            cout << "Mês inválido" << endl;
            break;
    }

    return 0;
}
```

Esses exemplos demonstram como utilizar o laço de repetição switch para selecionar diferentes opções de acordo com o valor da variável. É importante notar o uso do comando **break** após cada caso para evitar que a execução continue nos casos subsequentes. O bloco **default** é acionado quando nenhum dos casos correspondentes é encontrado, fornecendo uma resposta para entradas inválidas.  


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!