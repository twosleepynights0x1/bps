# BPS (Bypassing Blocks) 🚀

**Автоматически обновляемый сервис для обхода блокировок**

[![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/your-username/bps/releases)
[![Version](https://img.shields.io/badge/version-1.0.0-blue?style=for-the-badge)](https://github.com/your-username/bps)
[![Auto Update](https://img.shields.io/badge/auto_update-✓-success?style=for-the-badge)](https://github.com/your-username/bps)
[![Background](https://img.shields.io/badge/background_mode-✓-success?style=for-the-badge)](https://github.com/your-username/bps)
[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)

## 📖 О проекте

BPS — это интеллектуальный сервис для обхода интернет-блокировок, работающий в фоновом режиме на Windows. Сервис автоматически обновляется и обеспечивает беспрепятственный доступ к заблокированным ресурсам.

## ✨ Особенности

- 🔄 **Автоматическое обновление** — всегда актуальная версия сервиса
- 🌐 **Автономная работа** — работает в системном трее без окон
- 📡 **Динамические домен-листы** — автоматическая загрузка обновленных списков блокировок
- ⚡ **Интеграция с WinWS** — использование самописных инструментов для обхода

## 🛠️ Как это работает

### Архитектура системы

```mermaid
flowchart TD
    A[🚀 Запуск bps.exe] --> B[🔄 Проверка сервера обновлений]
    B --> C[📦 Загрузка актуальной версии]
    C --> D[⚡ Запуск основного сервиса]
    
    subgraph MainService [Основной сервис]
        D --> E[🌐 Загрузка блоклиста]
        D --> F[🛠️ Загрузка инструментов WinWS]
        E --> G[⚙️ Настройка окружения]
        F --> G
        G --> H[▶️ Запуск в фоновом режиме]
    end
    
    H --> I[📌 Системный трей]
    H --> J[🛡️ Обход блокировок]
    H --> K[🔍 Мониторинг работы]
    
    K -->|Новая версия| B
    
    style A fill:#0078D6,color:white
    style C fill:#107C10,color:white
    style H fill:#FFB900,color:black
    style J fill:#E81123,color:white
