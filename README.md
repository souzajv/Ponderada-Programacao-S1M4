# 🔧 Projeto Arduino: Pisca-Pisca com LED Interno e Externo

Nesta primeira etapa, fiz o LED interno do Arduino (conectado ao pino 13) piscar com um intervalo de meio segundo. Já na segunda etapa, fiz com que dois LEDs externos (conectados aos pinos 11 e 12) piscassem um após o outro com um intervalo de 3 milissegundos.

## 🎯 Objetivo

Fazer os LEDs interno e externo do Arduino piscar automaticamente com intervalos. 

## 🛠️ Materiais Utilizados

#### Primeira parte:
- Arduino Uno
- Cabo USB para conexão
- Computador com software Arduino IDE instalado

#### Segunda parte:
- Ambiente Tinkercad

&emsp;&emsp;[Link do Tinkercad](https://www.tinkercad.com/things/eardg6gO9r4-fantastic-gaaris-leelo/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits&sharecode=_3IJK8Sriac9FYLNAMMB-Gnetl0rCxx1Wsz-chByW38)


## 🔧 Montagem

#### Primeira parte:
Não é necessária nenhuma montagem externa, pois utilizei o LED interno do Arduino. Esse LED está conectado ao pino digital 13 da placa. 

#### Segunda parte:
Para montar o circuito com o Arduino, utilizei dois LEDs e dois resistores de 220 ohms:

LED 1: Conectei o anodo (perna longa) ao pino 12 do Arduino e o catodo (perna curta) a um resistor de 220 ohms, que foi ligado ao GND.

LED 2: Fiz o mesmo com o segundo LED, conectando o anodo ao pino 11 e o catodo ao resistor, também ligado ao GND. Os resistores servem para limitar a corrente, protegendo os LEDs.

## 📜 Código

Aqui está o código que usei para fazer o LED interno piscar:

```cpp
void setup()
{
  pinMode(13, OUTPUT); // Define o pino 13 como saída (LED interno)
}

void loop()
{
  digitalWrite(13, HIGH); // Liga o LED
  delay(500);             // Aguarda 500 ms
  digitalWrite(13, LOW);  // Desliga o LED
  delay(500);             // Aguarda mais 500 ms
}
```
Código que utilizei para fazer os LEDs externos piscarem:
```cpp
void setup()
{
  pinMode(12, OUTPUT);
  pinMode(11, OUTPUT);
}

void loop()
{
  digitalWrite(12, HIGH);
  delay(100);
  digitalWrite(12, LOW);
  delay(100);
  digitalWrite(11, HIGH);
  delay(100);
  digitalWrite(11, LOW);
  delay(100);
}
```

## 📽️ Demonstração em Vídeo
[Parte 1](https://youtube.com/shorts/GTIZzNoFm28?feature=share)

[Parte 2](https://youtu.be/fy0MJN0I7AI)
<hr>