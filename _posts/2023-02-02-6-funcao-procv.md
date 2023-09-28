---
layout: post
title: "Função PROCV"
date: 2023-02-02 00:06:00 -0300
categories: aplicativos-informatizados
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre a função **PROCV**

## O QUE É A FUNÇÃO PROCV?


![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/excel1.jpg?raw=true)

A função **PROCV** (procura vertical) é uma função de pesquisa e referência no Microsoft Excel, projetada para localizar um valor específico em uma tabela e retornar um valor correspondente em uma coluna adjacente. Ela é frequentemente utilizada para buscar dados em grandes conjuntos de dados ou tabelas, agilizando o processo de pesquisa e análise.

### Mas e aí, como fazer isso?

A sintaxe básica da função **PROCV** é a seguinte:

```
PROCV(valor_procurado;tabela_procurada;coluna_retorno;[procurar_intervalo])
```

**valor_procurado:** é o valor que você deseja procurar na tabela  
**tabela_procurada:** é a tabela ou intervalo de células em que você deseja realizar a pesquisa  
**coluna_retorno:** é o número da coluna da tabela_procurada a partir da qual você deseja retornar um valor correspondente  
**procurar_intervalo:** é um valor opcional que indica se você deseja que o Excel encontre uma correspondência exata ou uma correspondência aproximada. Se omitido, a correspondência exata é utilizada.

**Exemplos práticos**

1\. Suponha que você tenha uma lista de produtos em uma tabela e queira encontrar o preço correspondente a um determinado produto. Utilizando a função **PROCV**, você pode fazer o seguinte:

```
=PROCV("A";A1:B10;2;0)
```

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/excel16.jpg?raw=true)  

Neste exemplo, "Produto A" é o valor procurado, A1:B10 é o intervalo em que a pesquisa será realizada, 2 é o número da coluna que contém os preços e 0 indica uma correspondência exata. O Excel irá encontrar o valor correspondente ao "Produto A" na segunda coluna da tabela e retorná-lo.

2\. Suponha que você tenha uma tabela de funcionários com seus respectivos salários e queira encontrar o salário de um funcionário específico, cujo nome está em outra célula. Você pode usar a função **PROCV** da seguinte forma:

```
=PROCV(A2;A1:B10;2;0)
```

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/excel17.jpg?raw=true)  

Neste exemplo, A2 contém o nome do funcionário que você deseja pesquisar, A1:B10 é o intervalo de células onde a pesquisa será realizada, 2 é o número da coluna que contém os salários e 0 indica uma correspondência exata. O Excel encontrará o salário correspondente ao funcionário e o retornará.

Esses são apenas exemplos básicos de uso da função **PROCV**. É possível combinar a função **PROCV** com outras funções do Excel para obter resultados mais avançados e complexos, dependendo das necessidades do seu trabalho ou análise de dados.

**OBSERVAÇÃO**  
 Você sabia que **PROCV**, significa PROCURAR NA VERTICAL (PROC de Procurar, V de Vertical) e **PROCH** significa PROCURAR NA HORIZONTAL (PROC de Procurar, H horizontal)?
 Para saber mais, clique no vídeo abaixo:

[![PROCV e PROCH Passo a Passo](https://img.youtube.com/vi/t-xdWIF9j7c/0.jpg)](https://youtu.be/t-xdWIF9j7c)  


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!
