---
layout: post
title: "Introdução ao Microcontrolador"
date: 2024-01-01 00:03:00 -0300
categories: sistemas-embarcados
author: Escrito por Prof. Mario Herrera
---

Olá! Hoje vamos falar sobre Microcontrolador

## O que é um Microcontrolador?


![](https://github.com/mariopuebla17/blog/blob/main/_images/202401/se.jpg?raw=true)

Um microcontrolador é um pequeno computador embutido em um único chip, projetado para controlar funções específicas em sistemas incorporados. Ele contém um processador, memória, periféricos de entrada/saída e, às vezes, até mesmo um sistema operacional em um único dispositivo. Os microcontroladores são amplamente utilizados em aplicações que exigem controle em tempo real, como automação industrial, sistemas embarcados, dispositivos médicos, entre outros.

### Instalação do IDE do Microcontrolador e Sua Configuração

A instalação do Ambiente de Desenvolvimento Integrado (IDE) para o microcontrolador é uma etapa crucial para iniciar o desenvolvimento de projetos. O IDE permite escrever, compilar, depurar e carregar o código para o microcontrolador.

### Exemplo prático:

**IDE Arduino (Exemplo para Arduino Uno):**

1\. Instalação:
- Baixe e instale o Arduino IDE no site oficial: Arduino Software.

2\. Configuração:
- Conecte a placa Arduino Uno ao computador via cabo USB.
- Abra o Arduino IDE.
- Selecione o tipo de placa em Ferramentas > Placa (Arduino Uno, neste caso).
- Selecione a porta serial em Ferramentas > Porta (a porta onde o Arduino está conectado).

3\. Exemplo de Programa:

```cpp
void setup() {
  // Inicialização: configura o pino 13 como saída
  pinMode(13, OUTPUT);
}

void loop() {
  // Loop: acende e apaga o LED conectado ao pino 13
  digitalWrite(13, HIGH);   // Liga o LED
  delay(1000);               // Espera 1 segundo
  digitalWrite(13, LOW);    // Desliga o LED
  delay(1000);               // Espera 1 segundo
}
```

Este exemplo pisca um LED conectado ao pino 13 do Arduino Uno.

**IDE PlatformIO (Exemplo para ESP32):**

1\. Instalação:
- Baixe e instale o PlatformIO IDE no Visual Studio Code: PlatformIO.

2\. Configuração:
- Conecte a placa ESP32 ao computador via cabo USB.
- Abra o Visual Studio Code.
- Crie um novo projeto PlatformIO.
- Selecione a placa ESP32 no arquivo platformio.ini.

3\. Exemplo de Programa:
``` cpp
#include <Arduino.h>

#define LED_PIN 2 // Define o pino do LED como 2

void setup() {
  // Inicialização: configura o pino 2 como saída
  pinMode(LED_PIN, OUTPUT);
}

void loop() {
  // Loop: acende e apaga o LED conectado ao pino 2
  digitalWrite(LED_PIN, HIGH);   // Liga o LED
  delay(1000);                    // Espera 1 segundo
  digitalWrite(LED_PIN, LOW);     // Desliga o LED
  delay(1000);                    // Espera 1 segundo
}
```

Este exemplo pisca um LED conectado ao pino 2 do ESP32.

Agora você está pronto para começar a desenvolver projetos com microcontroladores!


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!