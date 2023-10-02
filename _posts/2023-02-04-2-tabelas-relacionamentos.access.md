---
layout: post
title: "Tabelas e Relacionamentos no Microsoft Access"
date: 2023-02-04 00:02:00 -0300
categories: aplicativos-informatizados
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre **Tabelas e Relacionamentos no Microsoft Access**

## Tabelas e Relacionamentos no Microsoft Access: Estruturando Seu Banco de Dados


![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/access.jpg?raw=true)

Nesta aula vamos mergulhar fundo na criação de tabelas e estabelecimento de relacionamentos. As tabelas servem como a base fundamental do seu banco de dados, onde você organiza e armazena seus dados de maneira estruturada. Os relacionamentos, por sua vez, permitem conectar informações de diferentes tabelas, tornando seu banco de dados mais eficiente e flexível.

### Exemplos Práticos:

1\. **Criando uma Tabela de Clientes:** Imagine que você está gerenciando um banco de dados de uma loja e deseja armazenar informações sobre seus clientes. Você pode criar uma tabela chamada "Clientes". Os campos dessa tabela podem incluir: ID do Cliente (chave primária), Nome, Sobrenome, Endereço e Número de Telefone. Cada campo representa um atributo específico dos clientes.

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/access3.jpg?raw=true)  

2\. **Chave Primária:** A chave primária (ID do Cliente, neste caso) é um campo especial que identifica exclusivamente cada registro em uma tabela. Isso garante que não haja duplicatas e permite a referência fácil de cada registro em outras tabelas.

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/access5.jpg?raw=true)  

3\. **Criando uma Tabela de Pedidos:** Agora, imagine que você também deseja rastrear os pedidos de seus clientes. Você pode criar uma segunda tabela chamada "Pedidos". Esta tabela pode incluir campos como ID do Pedido (chave primária), Data do Pedido, Produto, Quantidade e ID do Cliente. Observe como o campo "ID do Cliente" em "Pedidos" cria um vínculo com a tabela "Clientes".

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/access7.jpg?raw=true)  

4\. **Estabelecendo Relacionamentos:** Para criar um relacionamento entre as tabelas "Clientes" e "Pedidos", você pode usar o campo "ID do Cliente" como chave estrangeira em "Pedidos". Isso permite que você associe cada pedido a um cliente específico. Quando você precisa consultar os pedidos de um cliente específico, os relacionamentos facilitam a busca dos dados relevantes em ambas as tabelas.

![](https://github.com/mariopuebla17/blog/blob/main/_images/202302/access6.jpg?raw=true)  

**Conclusão:** Nesta aula, você aprenderá a criar tabelas com campos significativos e a estabelecer relacionamentos sólidos entre elas. Isso é fundamental para construir um banco de dados eficaz que possa crescer e se adaptar às necessidades do seu negócio. Acompanhe nossas próximas aulas para aprender a criar consultas, formulários e relatórios que aproveitem ao máximo a estrutura de seu banco de dados no Microsoft Access.

Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!