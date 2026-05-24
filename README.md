# 🛰️ DeepCore OS v1.0

> **Status do Projeto:** 🚀 Concluído e Operacional

O **DeepCore OS** é uma solução integrada de IoT e Automação Industrial desenvolvida para monitorar e resfriar dinamicamente infraestruturas críticas de processamento, como servidores de Data Centers voltados para Inteligência Artificial.

---

## 🛠️ Arquitetura do Sistema

O projeto opera de forma **non-blocking** (não-bloqueante) usando `millis()` na IDE do Arduino para garantir a automação local mesmo se a rede oscilar.

┌─────────────────┐             ┌─────────────────┐             ┌─────────────────┐
│   BANCADA FISICA│             │   NUVEM (BROKER)│             │   PAINEL WEB    │
│  ESP32 + OLED   │ ──(MQTT)──> │    EMQX Cloud   │ ──(WSS)───> │  GitHub Pages   │
└─────────────────┘             └─────────────────┘             └─────────────────┘

### 🔌 Componentes Utilizados
* **Microcontrolador:** ESP32 NodeMCU
* **Display:** OLED 0.96" I2C (SSD1306)
* **Sensor de Temperatura:** DS18B20
* **Atuador:** Módulo Relé de 5V

---

## 🧑‍💻 Desenvolvedor
* **Nome:** Kleydesson
* **Formação:** Graduando em Análise e Desenvolvimento de Sistemas (ADS)