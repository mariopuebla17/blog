---
layout: post
title: "Projetos utilizando Microcontrolador"
date: 2024-01-01 00:04:00 -0300
categories: sistemas-embarcados
author: Escrito por Prof. Mario Herrera
---

Olá! Hoje vamos falar sobre **Projetos utilizando Microcontrolador**

![](https://github.com/mariopuebla17/blog/blob/main/_images/202401/se4.jpg?raw=true)


### 1. Acendendo as Luzes:

Acender luzes é uma aplicação simples, mas fundamental em muitos projetos. Usando microcontroladores como Arduino, podemos facilmente controlar luzes LED.

**Exemplo prático:**

```cpp
#include <Arduino.h>

#define LED_PIN 13 // Pino onde está conectado o LED

void setup() {
  pinMode(LED_PIN, OUTPUT); // Configura o pino como saída
}

void loop() {
  digitalWrite(LED_PIN, HIGH); // Liga o LED
  delay(1000); // Espera 1 segundo
  digitalWrite(LED_PIN, LOW); // Desliga o LED
  delay(1000); // Espera 1 segundo
}
```

Neste exemplo, um LED conectado ao pino 13 é ligado e desligado alternadamente com intervalos de 1 segundo.

### 2. Efeitos com LEDs:

Além de acender e apagar LEDs, é possível criar efeitos interessantes, como piscar em sequências ou alterar cores.

**Exemplo prático:**

```cpp
#include <Arduino.h>

#define LED_PIN 13 // Pino onde está conectado o LED

void setup() {
  pinMode(LED_PIN, OUTPUT); // Configura o pino como saída
}

void loop() {
  for (int i = 0; i < 3; i++) {
    digitalWrite(LED_PIN, HIGH); // Liga o LED
    delay(500); // Espera 0,5 segundo
    digitalWrite(LED_PIN, LOW); // Desliga o LED
    delay(500); // Espera 0,5 segundo
  }
  delay(1000); // Espera 1 segundo antes de repetir
}
```

Neste exemplo, o LED pisca três vezes rapidamente e, em seguida, há uma pausa de 1 segundo antes de repetir o padrão.

### 3. Sonorizadores e Sensores Simples:

Utilizando sensores como os de luz, som ou movimento, e um buzzer, é possível criar projetos que reajam a estímulos do ambiente.

**Exemplo prático:**

```cpp
#include <Arduino.h>

#define SENSOR_PIN A0 // Pino onde está conectado o sensor de luz
#define BUZZER_PIN 9 // Pino onde está conectado o buzzer

void setup() {
  pinMode(SENSOR_PIN, INPUT); // Configura o pino do sensor como entrada
  pinMode(BUZZER_PIN, OUTPUT); // Configura o pino do buzzer como saída
}

void loop() {
  int valorSensor = analogRead(SENSOR_PIN); // Lê o valor do sensor de luz
  if (valorSensor > 500) { // Se for detectada luz forte
    tone(BUZZER_PIN, 1000); // Produz um som de 1000 Hz
    delay(500); // Espera 0,5 segundo
    noTone(BUZZER_PIN); // Para o som
    delay(500); // Espera 0,5 segundo
  }
}
```

Neste exemplo, um buzzer emite um som quando luz forte é detectada pelo sensor de luz.

Outras ideias:
- Controlando um motor CC
- Displays de LED
- Displays de cristal líquido
- Motores de passo e robôs
- Sensores		


Agradeço sua leitura até aqui, e estou à disposição para tirar qualquer dúvida através do meu email, localizado no rodapé!

Valeu!