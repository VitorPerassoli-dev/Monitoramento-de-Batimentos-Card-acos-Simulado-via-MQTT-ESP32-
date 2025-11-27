❤️ Sistema de Monitoramento de Batimentos Cardíacos (IoT + MQTT)

Este projeto apresenta um protótipo de monitoramento de batimentos cardíacos (BPM) utilizando ESP32 e comunicação MQTT. O valor do BPM é simulado por um potenciômetro e enviado em tempo real para um painel via MQTTX. Quando o BPM ultrapassa um limite de segurança, um LED de alerta é acionado.

🔧 Hardware (Simulado)

• Microcontrolador: ESP32 (DevKit V1)

• Sensor: Potenciômetro (no pino D34) — simula o sensor de batimento cardíaco

• Atuador: LED vermelho (no pino D25) — alerta de BPM alto

• Resistor: 220Ω (em série com o LED)

🚀 Como testar (Simulação)
1. Wokwi

Abra o projeto no Wokwi:

https://wokwi.com/projects/447801207838347265

2. MQTTX

No APLICATIVO MQTTX (tem que ser no app pois la tem a opção de mqtt, no web não tem) configure assim:

Host: broker.hivemq.com

Porta: 1883

Client ID: esp32_vitu

Username / Password: (deixe em branco)

SSL/TLS: Desativado

Depois, vá em Subscribe e adicione o tópico:

vitu/projeto/bpm


Agora, ao girar o potenciômetro, os BPMs irão aparecer em tempo real. 
