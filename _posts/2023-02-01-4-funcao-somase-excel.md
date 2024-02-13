---
layout: post
title: "Função SOMASE no Microsoft Excel"
date: 2023-02-01 00:04:00 -0300
categories: aplicativos-informatizados
author: Escrito por Prof. Mario Herrera
---
 
Olá! Hoje vamos falar sobre a função **SOMASE** do Excel

## O QUE É A FUNÇÃO SOMASE?


![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/excel1.jpg?raw=true)

A função **SOMASE** no Excel é uma função de planilha que permite somar os valores de um intervalo específico com base em um ou mais critérios. Ela é extremamente útil quando você precisa realizar cálculos condicionais, onde apenas as células que atendem a certas condições são incluídas na soma total.

### Mas e aí, como fazer isso?

A sintaxe básica da função **SOMASE** é a seguinte:

```
=SOMASE(intervalo, critérios, [intervalo_soma])
```

**intervalo**: o intervalo de células no qual os critérios serão verificados  
**critérios**: a condição ou condições que devem ser atendidas pelas células correspondentes. Isso pode ser um valor único, uma referência de célula ou uma expressão  
**intervalo_soma (opcional)**: o intervalo de células cujos valores serão somados. Se omitido, o intervalo especificado na primeira etapa será usado como intervalo_soma  

**Exemplos**:

Vamos supor que você tenha uma lista de vendas mensais e deseja somar apenas as vendas que excedem R$1.000. A fórmula seria:

```
=SOMASE(B1:B10;">=1000")
```

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/excel12.jpg?raw=true)  

Neste exemplo, o intervalo é *B1:B10* (a coluna onde as vendas estão registradas) e o critério é ">1000" (apenas vendas acima de R$1.000 serão incluídas na soma).

Digamos que você tenha uma planilha de despesas com diferentes categorias, e você deseja somar apenas as despesas relacionadas à categoria "Transporte". A fórmula seria:

```
=SOMASE(C1:C10;"Transporte";D1:D10)
```

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/excel13.jpg?raw=true)  

Neste caso, o intervalo é *C1:C10* (a coluna onde as categorias estão listadas), o critério é "Transporte" (apenas despesas da categoria "Transporte" serão incluídas) e o intervalo_soma é *D1:D10* (a coluna com os valores das despesas).

Esses são apenas exemplos básicos de uso da função **SOMASE**. Ela pode ser combinada com outros recursos do Excel, como intervalos dinâmicos e múltiplos critérios, para atender a diferentes necessidades de análise de dados.  


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!