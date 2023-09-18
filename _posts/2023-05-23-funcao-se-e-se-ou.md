---
layout: post
title: "Funções SE E e SE OU"
date: 2023-05-23 00:00:00 -0300
categories: aplicativos-informatizados
author: Escrito por Mario Herrera
---
 
Olá! Hoje vamos falar sobre as Funções **SE E** e **SE OU**

## O QUE É A FUNÇÃO SE E?


A função SE E (AND) é usada para verificar se todas as condições especificadas são verdadeiras. Ela retorna VERDADEIRO se todas as condições forem verdadeiras e FALSO se pelo menos uma das condições for falsa.

### Mas e aí, como fazer isso?

```
=SE(E(condição1;condição2;...);valor_se_verdadeiro;valor_se_falso)
```

**Exemplo**  
Suponha que você deseje verificar se um aluno obteve notas acima de 70 em todas as disciplinas. Se todas as notas forem maiores que 70, você quer exibir "Aprovado", caso contrário, exibir "Reprovado". A fórmula seria:

```
=SE(E(A2>70;B2>70;C2>70);"Aprovado";"Reprovado")
```

![](https://github.com/mariopuebla17/blog/blob/main/_images/20230523/Screenshot_1.jpg?raw=true)

Neste exemplo, as células A2, B2 e C2 contêm as notas nas três disciplinas.

## O QUE É A FUNÇÃO SE OU?


A função SE OU (OR) é usada para verificar se pelo menos uma das condições especificadas é verdadeira. Ela retorna VERDADEIRO se pelo menos uma das condições for verdadeira e FALSO se todas as condições forem falsas.

### Mas e aí, como fazer isso?

```
=SE(OU(condição1;condição2;...);valor_se_verdadeiro;valor_se_falso)
```

**Exemplo**  
Digamos que você queira verificar se um funcionário está qualificado para receber um bônus com base em seu desempenho. Se ele atingir a meta de vendas ou exceder a meta de satisfação do cliente, você deseja conceder o bônus. A fórmula seria:

```
=SE(OU(B6>=1000;B7>90%);"Bônus concedido";"Sem bônus")
```

![](https://github.com/mariopuebla17/blog/blob/main/_images/20230523/Screenshot_2.jpg?raw=true)

Neste exemplo, A2 representa as vendas do funcionário e B2 representa a porcentagem de satisfação do cliente.

Esses exemplos mostram como as funções **SE E** e **SE OU** podem ser usadas para realizar testes lógicos com várias condições no Excel.  


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!