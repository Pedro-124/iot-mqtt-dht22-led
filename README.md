🟦 Projeto IoT – Sensor DHT22 + LED + MQTT
Objetos Inteligentes Conectados – Trabalho Final

<img width="739" height="493" alt="image" src="https://github.com/user-attachments/assets/3d62445d-ec7a-442e-824b-965dbe73d698" />

Este repositório apresenta o desenvolvimento de um protótipo IoT baseado em um sensor DHT22 e um LED como atuador, utilizando comunicação via protocolo MQTT.
O projeto foi simulado no Tinkercad e demonstra a funcionalidade de monitoramento ambiental aplicada à ODS 3 – Saúde e Bem-Estar.

📌 1. Objetivo do Projeto

O objetivo deste trabalho é demonstrar um sistema IoT simples capaz de:

Medir temperatura e umidade com o sensor DHT22

Publicar valores no MQTT (projeto/sensor)

Receber comandos via MQTT (projeto/led)

Acionar um LED conforme instruções remotas

Representar graficamente o funcionamento por meio de diagramas, esquema eletrônico e fluxograma

Documentar todo o projeto em um repositório público no GitHub

⚙️ 2. Tecnologias Utilizadas

Arduino Uno (simulado no Tinkercad)

Sensor DHT22

LED + resistor

Protocolo MQTT

Cliente MQTT (MQTT.fx / EMQX / HiveMQ Web Client)

GitHub para armazenamento e documentação

Diagramas gerados em estilo Fritzing / fluxograma ilustrado

🏗️ 3. Arquitetura Geral do Sistema

O sistema segue o padrão de um projeto IoT básico:

✔ Coleta de Dados

O sensor DHT22 mede temperatura e umidade.

✔ Processamento

O Arduino (simulado) organiza os dados e executa comandos.

✔ Comunicação MQTT

O sistema publica dados ambientais no tópico:

projeto/sensor


O sistema recebe comandos no tópico:

projeto/led

✔ Ação

led_on → LED acende

led_off → LED apaga

📡 4. Tópicos MQTT Utilizados
Função	Tópico	Exemplo de Mensagem
Publicação do sensor	projeto/sensor	{"temperatura": 32, "umidade": 65}
Controle do atuador	projeto/led	led_on / led_off
🔧 5. Código-Fonte

O código utilizado no Arduino está disponível em:

/src/codigo.ino


O programa inclui:

Leitura do DHT22

Conversão dos dados em JSON

Lógica de acionamento do LED

Interface serial para simulação no Tinkercad

🖼️ 6. Diagramas e Fluxograma

Todos os diagramas estão armazenados em:

/docs/diagramas


E o fluxograma completo do funcionamento em:

/docs/fluxograma

🖼️ 7. Prints de Funcionamento

Imagens da simulação do Tinkercad e da comunicação MQTT estão em:

/docs/prints


Inclui:

LED funcionando

Publicação de dados

Comandos via MQTT

Conexão ao broker

Tópicos assinados

🎥 8. Vídeo de Demonstração

O vídeo explicando e demonstrando o funcionamento completo está disponível em:

👉 INSIRA AQUI O LINK DO YOUTUBE

📄 9. Artigo Final

A versão final do artigo em PDF está na raiz deste repositório:



👤 Autor

Pedro Gabriel Fernandes de Almeida
Trabalho Final — Objetos Inteligentes Conectados
Faculdade Presbiteriana Mackenzie
