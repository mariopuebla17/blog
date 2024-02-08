---
layout: post
title: "Fundamentos de Switches"
date: 2024-02-01 00:01:00 -0300
categories: redes-comunicacao-dados-ii
author: Escrito por Mario Herrera
---

Olá! Hoje vamos falar sobre **Fundamentos de Switches - estrutura e configurações**

## Funcionamento de um Switch


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes.jpg?raw=true)

Os switches desempenham um papel crucial na infraestrutura de redes de comunicação de dados. Eles são dispositivos inteligentes que operam na camada de enlace do modelo OSI, e sua função principal é encaminhar quadros de dados dentro de uma rede local. Quando um quadro chega a um switch, ele examina o endereço MAC de destino e o encaminha apenas para a porta relevante, onde o dispositivo de destino está conectado. Isso aumenta a eficiência e a segurança da rede, reduzindo o tráfego desnecessário. Os switches aprendem automaticamente os endereços MAC dos dispositivos conectados às suas portas, criando uma tabela de comutação que é usada para encaminhar o tráfego. Este é apenas o básico do funcionamento de um switch, e há muito mais a explorar sobre suas capacidades e funcionalidades avançadas.

### Exemplo prático:

Imagine uma pequena empresa com vários computadores conectados a um switch. Quando um computador (A) deseja enviar dados para outro computador (B) na mesma rede local, ele envia um pacote de dados. O switch verifica a tabela de endereços MAC para determinar em qual porta o computador de destino (B) está conectado e encaminha o pacote apenas para essa porta, reduzindo o tráfego desnecessário na rede.

## Configuração de Senhas no Switch


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes2.jpg?raw=true)

A segurança é uma preocupação fundamental em qualquer rede de comunicação de dados, e os switches não são exceção. A configuração de senhas no switch é essencial para proteger o acesso não autorizado e garantir a integridade da rede. Existem várias senhas que podem ser configuradas em um switch, incluindo senhas de console, que controlam o acesso ao dispositivo através da porta de console, e senhas de usuário privilegiado (enable password), que controlam o acesso a comandos privilegiados. Além disso, é importante garantir que as senhas sejam complexas e alteradas regularmente para aumentar a segurança. Ao configurar senhas adequadas, os administradores de rede podem garantir que apenas usuários autorizados tenham acesso aos recursos do switch.

### Exemplo prático:

Suponha que você esteja configurando um switch Cisco e deseja definir uma senha de console para restringir o acesso à sua interface de console. Você pode usar o seguinte comando:

``` arduino
Switch(config)# line console 0
Switch(config-line)# password minha_senha
Switch(config-line)# login
```

Isso configura uma senha de console chamada "minha_senha" e requer que os usuários façam login com essa senha ao acessar o switch pela porta de console.

## Armazenamento e Backup da Configuração do Switch


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes3.jpg?raw=true)

A configuração de um switch é composta por uma série de comandos que definem seu comportamento e funcionalidades. É crucial armazenar e fazer backup dessa configuração para evitar perda de dados em caso de falha do dispositivo ou necessidade de reconfiguração. Existem várias maneiras de fazer isso, incluindo o uso de armazenamento local, TFTP (Trivial File Transfer Protocol) ou FTP (File Transfer Protocol) para fazer o backup da configuração. Fazer backup regularmente da configuração do switch é uma prática recomendada pelos administradores de rede para garantir a continuidade operacional e simplificar processos de recuperação em caso de falha.

### Exemplo prático:

Para fazer backup da configuração de um switch Cisco usando TFTP, você pode usar os seguintes comandos:

``` arduino
Switch# copy running-config tftp:
Address or name of remote host []? 192.168.1.10
Destination filename [switch-config]? backup.cfg
```

Isso copia a configuração atual do switch para um servidor TFTP com o endereço IP 192.168.1.10 e salva o arquivo como "backup.cfg".

## Redes Locais Virtuais (VLANs): Conceitos e Configurações


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes4.jpg?raw=true)

As Redes Locais Virtuais (VLANs) são uma forma de segmentar uma rede física em redes lógicas separadas, proporcionando benefícios em termos de desempenho, segurança e gerenciamento. As VLANs permitem que dispositivos em diferentes partes da rede comuniquem-se entre si como se estivessem na mesma rede física, mesmo que estejam fisicamente separados. Isso é alcançado atribuindo portas do switch a VLANs específicas e configurando o tráfego entre VLANs (trunking). As VLANs são uma ferramenta poderosa para organizar e gerenciar redes de comunicação de dados, e entender seus conceitos e configurações é fundamental para administradores de rede.

### Exemplo prático:

Imagine que você deseja segmentar sua rede em duas VLANs: VLAN 10 para o departamento de vendas e VLAN 20 para o departamento de marketing. Você pode configurar isso da seguinte maneira em um switch Cisco:

``` scss
Switch(config)# vlan 10
Switch(config-vlan)# name vendas

Switch(config)# vlan 20
Switch(config-vlan)# name marketing

Switch(config)# interface range gigabitEthernet0/1-10
Switch(config-if-range)# switchport mode access
Switch(config-if-range)# switchport access vlan 10

Switch(config)# interface range gigabitEthernet0/11-20
Switch(config-if-range)# switchport mode access
Switch(config-if-range)# switchport access vlan 20
```

Isso cria duas VLANs (VLAN 10 e VLAN 20) e atribui portas específicas a cada VLAN.

## Backup e Atualização do Sistema Operacional (IOS) de um Switch


![](https://github.com/mariopuebla17/blog/blob/main/_images/202402/redes5.jpg?raw=true)

Assim como qualquer outro sistema computacional, os switches também precisam de atualizações periódicas de seu sistema operacional (IOS) para corrigir falhas de segurança, melhorar o desempenho e adicionar novos recursos. Além disso, fazer backup do IOS é importante para garantir a capacidade de restaurar o switch em caso de falha durante uma atualização. Existem diferentes métodos para fazer backup e atualizar o IOS de um switch, incluindo o uso de protocolos de transferência de arquivos como TFTP ou FTP. É importante seguir as práticas recomendadas ao realizar essas operações para evitar interrupções na rede e garantir a integridade do switch.

### Exemplo prático:

Para fazer backup do IOS de um switch Cisco usando TFTP, você pode usar os seguintes comandos:

``` less
Switch# copy flash tftp:
Source filename [switch-ios]? current-ios.bin
Address or name of remote host []? 192.168.1.10
Destination filename [current-ios.bin]? backup-ios.bin
```

Isso copia o sistema operacional atual do switch para um servidor TFTP com o endereço IP *192.168.1.10* e salva o arquivo como "backup-ios.bin".

Para atualizar o IOS de um switch, você pode fazer o download da versão mais recente do IOS da Cisco, transferi-la para o switch e, em seguida, usar o comando copy para substituir o IOS existente pelo novo.

Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!