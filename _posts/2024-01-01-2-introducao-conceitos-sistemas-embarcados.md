---
layout: post
title: "Introdução aos Conceitos de Sistemas Embarcados"
date: 2024-01-01 00:02:00 -0300
categories: sistemas-embarcados
author: Escrito por Prof. Mario Herrera
---

Olá! Hoje vamos falar sobre **Conceitos de Sistemas Embarcados**

## Funções de Inicialização e Laços de Repetição Global


![](https://github.com/mariopuebla17/blog/blob/main/_images/202401/se.jpg?raw=true)

Em sistemas embarcados, as funções de inicialização são cruciais para configurar o ambiente e os periféricos do sistema após a inicialização. Geralmente, essas funções são chamadas logo no início do programa. Os laços de repetição global, por sua vez, são usados para manter o sistema em execução contínua, realizando tarefas essenciais.

### Exemplo prático:

```c++
#include <iostream>

// Função de inicialização
void init_system() {
    // Configuração de periféricos
    // Inicialização de variáveis globais
    // Outras configurações necessárias
    std::cout << "Sistema inicializado!\n";
}

// Laço de repetição global
void main_loop() {
    while(true) {
        // Tarefas principais do sistema
        // Controle de sensores, processamento de dados, etc.
        std::cout << "Executando tarefa principal...\n";
    }
}

int main() {
    // Chamada da função de inicialização
    init_system();
    
    // Laço de repetição principal
    main_loop();
    
    return 0;
}
```

Neste exemplo em C++, a função `init_system()` é chamada no início do programa para realizar as configurações iniciais do sistema. O laço `while(true)` no `main_loop()` garante que o sistema execute suas tarefas principais de forma contínua.

## Constantes Pré-definidas de I/O


![](https://github.com/mariopuebla17/blog/blob/main/_images/202401/se4.jpg?raw=true)

Constantes pré-definidas de I/O são utilizadas para representar endereços de registradores de dispositivos de entrada e saída (I/O) em sistemas embarcados. Elas simplificam o acesso e a manipulação dos periféricos conectados ao microcontrolador ou microprocessador.

### Exemplo prático:

```c++
#include <iostream>

// Define constantes pré-definidas para I/O
#define LED_PIN 13 // Pino do LED

void setup() {
    // Configura o pino do LED como saída
    pinMode(LED_PIN, OUTPUT);
}

void loop() {
    // Acende o LED
    digitalWrite(LED_PIN, HIGH);
    delay(1000); // Espera 1 segundo

    // Apaga o LED
    digitalWrite(LED_PIN, LOW);
    delay(1000); // Espera 1 segundo
}

int main() {
    // Configuração inicial
    setup();

    // Laço de repetição principal
    while (true) {
        loop();
    }

    return 0;
}
```

Neste exemplo, em Arduino C++, a constante `LED_PIN` é usada para representar o pino onde o LED está conectado. Isso simplifica a leitura e a escrita no pino do LED durante a execução do programa.


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!