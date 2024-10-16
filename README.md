# 🔧 Projeto Arduino: Pisca-Pisca com LED Interno

Nesta primeira etapa, fiz o LED interno do Arduino (conectado ao pino 13) piscar com um intervalo de meio segundo. 

## 🎯 Objetivo

Fazer o LED interno do Arduino piscar automaticamente com intervalos.

## 🛠️ Materiais Utilizados

- Arduino Uno
- Cabo USB para conexão
- Computador com software Arduino IDE instalado

## 🔧 Montagem

Não é necessária nenhuma montagem externa, pois utilizei o LED interno do Arduino. Esse LED está conectado ao pino digital 13 da placa. 

## 📜 Código

Aqui está o código que usei para fazer o LED piscar:

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
## 📽️ Demonstração em Vídeo
[Assista ao vídeo da demonstração no YouTube](https://youtube.com/shorts/GTIZzNoFm28?feature=share)
<br><br>
## 🚀 Próximos Passos
Agora que fiz o LED interno piscar, o próximo passo será conectar LEDs externos e criar padrões de pisca-pisca mais avançados.