# Marzban Rules

Кастомные правила для Marzban (Clash, V2Ray, SingBox).

## Структура

```
marzban-rules/
├── README.md
├── clash/
│   └── custom.yml       # Clash конфигурация
├── v2ray/
│   └── custom.json      # V2Ray конфигурация
└── singbox/
    └── custom.json      # SingBox конфигурация
```

## Использование

Подключи репозиторий в Dockerfile через переменные:
- `RULES_REPO=https://github.com/kidsamort/marzban-rules`
- `RULES_BRANCH=main`

Все файлы скопируются в volume и будут доступны в Marzban.

## Правила

### Clash (`clash/custom.yml`)
- 🇷🇺 Российские сайты → DIRECT
- 👾 Discord → отдельная группа
- 🤖 AI (OpenAI, ChatGPT) → отдельная группа
- 🚀 Остальное → прокси

### V2Ray (`v2ray/custom.json`)
- routing rules для V2Ray

### SingBox (`singbox/custom.json`)
- route rules для SingBox
