---
layout: post
title: "Fundamentos de Roteamento"
date: 2024-02-01 00:02:00 -0300
categories: redes-comunicacao-dados-ii
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre **Fundamentos de Roteamento - protocolos e configurações**

## Conceitos de Roteamento


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes.jpg?raw=true)

O roteamento é o processo de encaminhamento de pacotes de dados de uma rede para outra. Um roteador é um dispositivo de rede que encaminha dados com base no endereço IP de destino dos pacotes. Ele utiliza tabelas de roteamento para determinar a melhor rota para os pacotes viajarem da origem ao destino.

### Exemplo prático:

Imagine uma empresa com várias filiais conectadas por meio de uma rede WAN (Wide Area Network). Cada filial possui um roteador que encaminha o tráfego de dados para a filial correta com base no endereço IP de destino dos pacotes.

## Protocolos de Roteamento e Roteáveis


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes2.jpg?raw=true)

Existem diversos protocolos de roteamento utilizados para trocar informações sobre rotas entre roteadores em uma rede. Alguns dos protocolos mais comuns incluem o Protocolo de Roteamento por Vetor de Distância (RIPv2), o Protocolo de Informações de Roteamento (RIPng), o Protocolo de Gateway de Borda (BGP) e o Protocolo de Roteamento de Estado de Enlace (OSPF). Esses protocolos determinam as rotas mais eficientes para encaminhar o tráfego com base em diferentes métricas, como distância, largura de banda ou número de saltos.

### Exemplo prático:

Suponha que uma empresa esteja configurando roteamento entre suas filiais usando o OSPF (Protocolo de Roteamento de Estado de Enlace). Os roteadores em cada filial trocam informações sobre a topologia da rede e calculam as melhores rotas com base na largura de banda disponível. Isso permite que o tráfego seja encaminhado de forma eficiente entre as filiais, garantindo uma comunicação rápida e confiável.

## Endereços IP no Roteamento e Interconexão de Redes


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes3.jpg?raw=true)

Os endereços IP são fundamentais para o roteamento e a interconexão de redes, pois permitem que os roteadores determinem o destino dos pacotes de dados. Cada dispositivo em uma rede possui um endereço IP único que identifica sua localização na rede. Os roteadores usam esses endereços para encaminhar os pacotes de dados para o destino correto.

### Exemplo prático:

Ao configurar uma conexão entre duas redes, os roteadores são configurados com endereços IP em cada interface que faz fronteira com outra rede. Por exemplo, se duas redes estiverem sendo interconectadas, o roteador que faz a conexão terá um endereço IP em cada uma dessas redes. Quando um pacote de dados chega ao roteador, ele consulta sua tabela de roteamento e encaminha o pacote para a interface apropriada com base no endereço IP de destino.


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!