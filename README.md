# Sentinel_IoT

Um sistema integrado de hardware e software para monitoramento de umidade em tempo real, focado na prevenção de danos a equipamentos eletrônicos sensíveis. Mas facilmente adaptavel a outras finalidades.

![Status](https://img.shields.io/badge/Status-Concluído-success)
![Flutter](https://img.shields.io/badge/Flutter-Mobile-blue?logo=flutter)
![ESP32](https://img.shields.io/badge/Hardware-ESP32-black?logo=espressif)
![Firebase](https://img.shields.io/badge/Database-Firebase-orange?logo=firebase)

# Projeto desenvolvido em colaboração por:
- Gabriel Rezende Pires (</strong><a href="https://github.com/boosa515"><strong>GitHub</strong></a>)
- Artur Morais Brasileiro (</strong><a href="https://github.com/Artur-Brasileiro"><strong>GitHub</strong></a>)

## Sobre o Projeto
O sistema utiliza um microcontrolador ESP32 para ler dados do sensor e sincronizá-los em milissegundos com um aplicativo mobile em qualquer rede, emitindo alertas críticos mesmo quando o celular do usuário está com a tela bloqueada.

## Funcionalidades
* **Monitoramento em Tempo Real:** Sincronização via WebSockets (Firebase Realtime Database) com latência quase nula.
* **Interface Reativa:** O design do app altera dinamicamente com base em limiares de segurança (30% - 50% de umidade).
* **Notificações Push Nativas:** Integração com a REST API do OneSignal para acordar o dispositivo do usuário em caso de anomalias climáticas.

## Arquitetura e Tecnologias

### Hardware (Edge)
* **Microcontrolador:** ESP32-WROOM-32U
* **Sensor:** DHT11 (Temperatura e Umidade)
* **Linguagem:** C/C++ (Framework Arduino)

### Software (Nuvem & Mobile)
* **Front-end:** Flutter (Dart) - *Suporte nativo a Android e iOS*
* **Banco de Dados:** Firebase Realtime Database (NoSQL)
* **Mensageria Push:** OneSignal

*Desenvolvido como projeto prático de integração de sistemas.*
