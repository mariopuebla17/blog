---
layout: post
title: "Função PROCH"
date: 2023-06-06 00:00:00 -0300
categories: aplicativos-informatizados
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre a função **PROCH**

## O QUE É A FUNÇÃO PROCH?


A função **PROCH** é uma poderosa ferramenta do Microsoft Excel que permite buscar e recuperar informações em uma tabela, com base em um valor de referência. Ela é amplamente utilizada para realizar pesquisas e recuperar dados específicos, facilitando a análise e organização de grandes conjuntos de informações.

### Mas e aí, como fazer isso?

A sintaxe básica da função **PROCH** é a seguinte:

```
PROCH(valor_procurado, tabela, número_coluna, [intervalo_pesquisa])
```

**valor_procurado**: O valor que você deseja encontrar na tabela. Pode ser um número, texto, referência de célula ou fórmula  
**tabela**: A tabela ou intervalo de células onde a pesquisa será realizada. É importante que a coluna contendo o valor procurado esteja à esquerda da coluna de onde deseja-se recuperar o resultado  
**número_coluna**: O número da coluna da qual você deseja recuperar o resultado. Contando a partir da primeira coluna do intervalo de pesquisa  
**intervalo_pesquisa** (opcional): Define se a função realizará uma pesquisa aproximada ou exata. Use o valor "VERDADEIRO" para pesquisa aproximada (procura o valor mais próximo) ou "FALSO" para pesquisa exata.

**Exemplos práticos**

Suponha que você tenha uma tabela de funcionários com seus respectivos salários e precise recuperar o salário de um funcionário específico com base em seu nome. Utilize a função **PROCH** da seguinte maneira:

```
=PROCH("João", A2:B10, 2, FALSO)
```

Neste exemplo, a função **PROCH** buscará na coluna A o nome "João" e retornará o valor correspondente da coluna B, que é o salário de João.

Imagine que você esteja trabalhando em um projeto de controle de estoque e precise recuperar o preço de um produto com base em seu código. Use a função **PROCH** assim:

```
=PROCH(C2, A2:B100, 2, VERDADEIRO)
```

Neste caso, a função **PROCH** pesquisará o valor da célula C2 na coluna A e retornará o valor correspondente da coluna B. Como o último argumento é VERDADEIRO, a pesquisa será aproximada, buscando o valor mais próximo do código do produto.

Esses são apenas dois exemplos básicos de uso da função **PROCH** no Excel. Ela pode ser combinada com outras funções e recursos do Excel para realizar análises mais avançadas e complexas. Experimente explorar suas possibilidades e aprimorar suas habilidades com essa função poderosa!

**OBSERVAÇÃO**  
 Você sabia que **PROCV**, significa PROCURAR NA VERTICAL (PROC de Procurar, V de Vertical) e **PROCH** significa PROCURAR NA HORIZONTAL (PROC de Procurar, H horizontal)?
 Para saber mais, clique no vídeo abaixo:

[![PROCV e PROCH Passo a Passo](https://img.youtube.com/vi/t-xdWIF9j7c/0.jpg)](https://youtu.be/t-xdWIF9j7c)


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!