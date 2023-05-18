---
layout: post
title: "Função CONT.SE"
date: 2023-06-06 00:00:00 -0300
categories: aplicativos-informatizados
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre a função **CONT.SE** do Excel

## O QUE É A FUNÇÃO CONT.SE?


No mundo dos negócios e da análise de dados, muitas vezes precisamos contar valores em uma planilha do Excel que atendam a determinadas condições. É aí que entra a função CONT.SE, uma poderosa ferramenta que permite contar células com base em critérios específicos. Neste artigo, exploraremos em detalhes a função CONT.SE e forneceremos exemplos práticos para ajudá-lo a entender seu funcionamento.

### Mas e aí, como fazer isso?

A função CONT.SE é usada para contar o número de células em um intervalo que satisfazem uma condição específica. Ela tem a seguinte sintaxe:
```
CONT.SE(intervalo, critérios)
```

**Intervalo**: é o intervalo de células no qual você deseja contar os valores  
**Critérios**: é a condição que você deseja aplicar aos valores do intervalo  

**Exemplos práticos**  
Agora, vamos explorar alguns exemplos para entender como a função CONT.SE pode ser aplicada.

1\. Suponha que você tenha uma planilha com informações sobre vendas mensais de produtos. A coluna A contém os nomes dos produtos e a coluna B contém a quantidade vendida. Se você deseja contar quantas vezes o produto "Maçã" foi vendido, pode usar a função CONT.SE da seguinte forma:

```
=CONT.SE(A1:A10, "Maçã")
```

Neste exemplo, o intervalo A1:A10 define o intervalo de células em que queremos contar as ocorrências da palavra "Maçã".

2\. Agora, suponha que você queira contar quantas vendas ultrapassaram um determinado valor. Se você tiver a lista de vendas na coluna B e o valor de referência na célula E1, pode usar a função CONT.SE da seguinte maneira:

```
=CONT.SE(B1:B10, ">"&E1)
```

Neste exemplo, o intervalo B1:B10 define o intervalo de células que contém os valores de vendas, enquanto ">"&E1 define a condição, onde ">" indica que queremos contar as vendas maiores que o valor em E1.

**Conclusão**  
A função CONT.SE é uma ferramenta valiosa para contar células que atendem a determinadas condições em uma planilha do Excel. Ela pode ser usada para diversas finalidades, desde contar ocorrências de palavras específicas até contar valores que excedem um limite. Esperamos que os exemplos práticos fornecidos neste artigo tenham ajudado você a entender melhor como utilizar a função CONT.SE em suas análises de dados. Experimente-a em suas planilhas e aproveite todos os benefícios que ela pode oferecer.


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!