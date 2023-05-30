---
layout: post
title: "Função SOMASE"
date: 2023-05-30 00:00:00 -0300
categories: aplicativos-informatizados
author: Escrito por Mario Herrera
---
 
Olá! Hoje vamos falar sobre a função **SOMASE** do Excel

## O QUE É A FUNÇÃO SOMASE?


A função SOMASE no Excel é uma função de planilha que permite somar os valores de um intervalo específico com base em um ou mais critérios. Ela é extremamente útil quando você precisa realizar cálculos condicionais, onde apenas as células que atendem a certas condições são incluídas na soma total.

### Mas e aí, como fazer isso?

A sintaxe básica da função SOMASE é a seguinte:

```
=SOMASE(intervalo, critérios, [intervalo_soma])
```

**intervalo**: o intervalo de células no qual os critérios serão verificados  
**critérios**: a condição ou condições que devem ser atendidas pelas células correspondentes. Isso pode ser um valor único, uma referência de célula ou uma expressão  
**intervalo_soma (opcional)**: o intervalo de células cujos valores serão somados. Se omitido, o intervalo especificado na primeira etapa será usado como intervalo_soma  

**Exemplos**:

Vamos supor que você tenha uma lista de vendas mensais e deseja somar apenas as vendas que excedem $1.000. A fórmula seria:

```
=SOMASE(B2:B10, ">1000")
```

Neste exemplo, o intervalo é B2:B10 (a coluna onde as vendas estão registradas) e o critério é ">1000" (apenas vendas acima de $1.000 serão incluídas na soma).

Digamos que você tenha uma planilha de despesas com diferentes categorias, e você deseja somar apenas as despesas relacionadas à categoria "Transporte". A fórmula seria:

```
=SOMASE(C2:C10, "Transporte", D2:D10)
```

Neste caso, o intervalo é C2:C10 (a coluna onde as categorias estão listadas), o critério é "Transporte" (apenas despesas da categoria "Transporte" serão incluídas) e o intervalo_soma é D2:D10 (a coluna com os valores das despesas).

Esses são apenas exemplos básicos de uso da função SOMASE. Ela pode ser combinada com outros recursos do Excel, como intervalos dinâmicos e múltiplos critérios, para atender a diferentes necessidades de análise de dados.


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!