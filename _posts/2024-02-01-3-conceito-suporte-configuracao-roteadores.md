---
layout: post
title: "Conceito de Suporte e Configuração de Roteadores"
date: 2024-02-01 00:03:00 -0300
categories: redes-comunicacao-dados-ii
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre **Conceito de Suporte e Configuração de Roteadores**

## Máscara de Sub-rede


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes.jpg?raw=true)

A máscara de sub-rede é um número que determina quais bits de um endereço IP representam a rede e quais representam o host. Ela é usada em conjunto com o endereço IP para dividir uma rede em sub-redes menores.

### Exemplo prático:

Se tivermos um endereço IP de 192.168.1.1 com uma máscara de sub-rede de 255.255.255.0, isso significa que os primeiros 24 bits (ou 3 octetos) do endereço IP são dedicados à rede e os últimos 8 bits (ou 1 octeto) são dedicados aos hosts na rede.

## Gateway e DNS


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes2.jpg?raw=true)

O gateway é o roteador que conecta uma rede local à Internet. Ele encaminha o tráfego entre a rede local e a Internet. O DNS (Domain Name System) é um sistema que traduz nomes de domínio em endereços IP.

### Exemplo prático:

Suponha que o endereço IP do gateway seja 192.168.1.1. O DNS pode ser configurado como 8.8.8.8 (servidor DNS público do Google) para traduzir nomes de domínio em endereços IP.

## Configurações Corretas de Rede


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes3.jpg?raw=true)

As configurações corretas de rede incluem o endereço IP, a máscara de sub-rede, o gateway padrão e as configurações de DNS. Essas configurações garantem que os dispositivos em uma rede possam se comunicar entre si e acessar a Internet.

### Exemplo prático:

Configurar um computador com endereço IP 192.168.1.100, máscara de sub-rede 255.255.255.0, gateway 192.168.1.1 e DNS 8.8.8.8.

## Configuração de Roteadores para Internet


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes4.jpg?raw=true)

A configuração de roteadores para a Internet envolve a configuração das interfaces WAN e LAN, endereços IP, configurações de NAT (Network Address Translation) e regras de firewall para permitir o tráfego da Internet.

### Exemplo prático:

Configurar a interface WAN do roteador com um endereço IP público fornecido pelo ISP e configurar a interface LAN com um intervalo de endereços IP privados, como 192.168.1.0/24.

## Internet Setup


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes5.jpg?raw=true)

A configuração de Internet (Internet Setup) em um roteador envolve a configuração da conexão com a Internet, como a configuração de IP público na interface WAN e a definição do tipo de conexão (IP fixo, IP dinâmico, PPPoE).

### Exemplo prático:

Configurar um roteador com uma conexão PPPoE, onde o ISP fornece um nome de usuário e senha para autenticação.

## IP Público - WAN; IP Fixo, IP Dinâmico e PPOE


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes.jpg?raw=true)

O IP público na interface WAN de um roteador é fornecido pelo ISP e pode ser fixo (estático) ou dinâmico. No caso de conexões PPPoE, o roteador usa um protocolo de autenticação para se conectar à Internet.

### Exemplo prático:

Se o ISP atribuir um IP fixo de 203.0.113.10 à interface WAN do roteador, é um IP fixo. Se o IP for atribuído automaticamente pelo ISP e pode mudar ocasionalmente, é um IP dinâmico.

## Network Setup


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes2.jpg?raw=true)

A configuração de rede (Network Setup) em um roteador envolve a definição das configurações da rede local (LAN), como o intervalo de endereços IP privados, DHCP e reserva de IP.

### Exemplo prático:

Configurar o roteador para atribuir automaticamente endereços IP aos dispositivos na rede local usando DHCP, com um intervalo de endereços IP de 192.168.1.100 a 192.168.1.200.

## IP Privativo - LAN; DHCP; Reserva de IP no DHCP


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes3.jpg?raw=true)

O IP privativo na interface LAN de um roteador é um intervalo de endereços IP reservados para uso em redes locais. O DHCP é um serviço que atribui automaticamente endereços IP aos dispositivos na rede. A reserva de IP no DHCP permite atribuir um endereço IP específico a um dispositivo com base no seu endereço MAC.

### Exemplo prático:

Configurar o roteador com um intervalo de endereços IP privados de 192.168.1.0/24 para a LAN. Configurar o DHCP para atribuir endereços IP da faixa de 192.168.1.100 a 192.168.1.200 e reservar o endereço IP 192.168.1.50 para um determinado dispositivo.

## Critérios para Endereçamento IP


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes4.jpg?raw=true)

Os critérios para o endereçamento IP incluem a divisão da rede em sub-redes menores, a atribuição de endereços IP a dispositivos individuais e a garantia de que todos os dispositivos na rede possam se comunicar entre si.

### Exemplo prático:

Ao dividir uma rede em sub-redes menores, como uma rede de escritório em várias sub-redes para diferentes departamentos, é necessário garantir que cada sub-rede tenha um intervalo de endereços IP exclusivo e que as rotas estejam configuradas corretamente para permitir a comunicação entre as sub-redes.

## Utilização da Máscara de Sub-rede IP


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes5.jpg?raw=true)

A máscara de sub-rede é usada para determinar quais partes de um endereço IP pertencem à parte da rede e quais pertencem à parte do host. Ela é essencial para dividir uma rede em sub-redes menores.

### Exemplo prático:

Ao configurar uma sub-rede com a máscara de sub-rede 255.255.255.0, você está dividindo a rede em várias sub-redes menores, onde os primeiros 24 bits são dedicados à identificação da rede e os últimos 8 bits são dedicados à identificação do host.

## Funções de Switch/Gateway


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes.jpg?raw=true)

Um switch é um dispositivo de rede que encaminha quadros de dados dentro de uma rede local. Um gateway é um dispositivo de rede que conecta diferentes redes e encaminha o tráfego entre elas.

### Exemplo prático:

Um switch conecta dispositivos em uma rede local, enquanto um gateway conecta a rede local à Internet ou a outra rede externa.

## Redes Seguras com VPN


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes2.jpg?raw=true)

Uma VPN (Virtual Private Network) cria uma conexão segura entre dois dispositivos ou redes através da Internet. Ela protege os dados transmitidos através da criptografia e autenticação.

### Exemplo prático:

Configurar uma VPN entre dois roteadores para permitir que os funcionários acessem a rede corporativa de forma segura enquanto estão fora do escritório.

## Túneis VPN entre Roteadores


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes3.jpg?raw=true)

Um túnel VPN é uma conexão segura estabelecida entre dois roteadores através da Internet. Ele permite que o tráfego de dados seja criptografado e transmitido com segurança entre as redes conectadas.

### Exemplo prático:
Configurar um túnel VPN entre dois roteadores para estabelecer uma conexão segura entre duas redes corporativas.

## Função VPN-Passthrough


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes4.jpg?raw=true)

O VPN-Passthrough é uma função em roteadores que permite que o tráfego VPN passe pelo roteador sem interferência. Ele é usado quando um roteador atua como intermediário para conexões VPN estabelecidas entre dispositivos externos.

### Exemplo prático:

Ativar a função VPN-Passthrough em um roteador para permitir que o tráfego VPN passe pelo roteador sem restrições.

## Configuração de Túnel VPN Dentro de Roteador de Alta Segurança


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes5.jpg?raw=true)

Configurar um túnel VPN dentro de um roteador de alta segurança envolve a configuração de políticas de segurança, autenticação, criptografia e definição de rotas para o tráfego VPN.

### Exemplo prático:

Configurar um túnel VPN IPSec dentro de um roteador de alta segurança com autenticação por certificado e criptografia AES-256.

## Uso e Limitações da DMZ - Zona Desmilitarizada


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes.jpg?raw=true)

A DMZ é uma zona de rede separada e desprotegida que fica entre a rede interna e a Internet. Ela é usada para hospedar serviços que precisam ser acessíveis a partir da Internet, como servidores web ou de e-mail.

### Exemplo prático:
Configurar um servidor web na DMZ do roteador para que ele possa ser acessado da Internet, enquanto a rede interna permanece protegida por um firewall.


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!