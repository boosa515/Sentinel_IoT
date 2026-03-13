# Sentinel_IoT
<br/>
<br/>
<p align="center">
  <img src="https://img.shields.io/badge/C++-20232A?style=for-the-badge&logo=C++&logoColor=61DAFB" alt="C++"/>
  <img src="https://img.shields.io/badge/arduino-646CFF?style=for-the-badge&logo=arduino&logoColor=white" alt="Arduino"/>
  <img src="https://img.shields.io/badge/firebase-8E75B2?style=for-the-badge&logo=firebase&logoColor=white" alt="Firebase"/>
  <img src="https://img.shields.io/badge/flutter-646CFF?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter"/>
</p>
<br/>

<br/>
<br/>

Um sistema integrado de hardware e software para monitoramento de umidade em tempo real, focado na prevenção de danos a equipamentos eletrônicos sensíveis. Mas facilmente adaptavel a outras finalidades.

<br/>

## Sobre o Projeto
O sistema utiliza um microcontrolador ESP32 para ler dados do sensor e sincronizá-los em milissegundos com um aplicativo mobile em qualquer rede, emitindo alertas críticos mesmo quando o celular do usuário está com a tela bloqueada.

<br/>

## Funcionalidades
* **Monitoramento em Tempo Real:** Sincronização via WebSockets (Firebase) com latência quase nula.
* **Interface Reativa:** O design do app altera dinamicamente com base em limiares de segurança (30% - 50% de umidade).

<br/>

## Arquitetura e Tecnologias

### Hardware (Edge)
* **Microcontrolador:** ESP32-WROOM-32U
* **Sensor:** DHT11 (Temperatura e Umidade)

### Software (Nuvem & Mobile)
* **Front-end:** Flutter (Dart) - *Suporte nativo a Android e iOS*
* **Banco de Dados:** Firebase Realtime Database (NoSQL)
* * **Linguagem:** C/C++ (Framework Arduino)
