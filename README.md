# Привет! 👋

## 🔧 Обо мне
- 🛠 **Системный администратор и DevOps Junior**, который умеет оживлять серверы и автоматизировать всё: от управления сервисами до обновлений через Git.
- 🐧 **Linux-мастер**, влюблённый в open-source решения и постоянное совершенствование инфраструктуры.
- 🤖 **Автоматизатор** с чувством юмора и любовью к bash-скриптам – от автоматической настройки мониторинга до регулярного обновления репозитория.

## 💻 Мои проекты и инструменты

### Автоматическая настройка сервера
- **auto-setup**: Скрипт для комплексной настройки сервера на Ubuntu 22.04.
  - **Что входит в проект:**
    - Установка и конфигурация **Grafana** (v11.6.0) с запуском на `127.0.0.1:3728`.
    - Развёртывание **Prometheus** и **Node Exporter** для мониторинга.
    - Настройка **Nginx** как reverse proxy для Grafana и Uptime Kuma.
    - Получение и обновление **SSL-сертификатов** через Certbot.
    - Перенастройка порта SSH и корректная настройка **UFW**.
    - Автоматический запуск **Uptime Kuma** с использованием docker-compose.
  - **Особенности:**
    - Интерактивное создание `.env` для первичной конфигурации.
    - Продуманное логирование с цветным выводом для наглядности.
    - Последовательное выполнение этапов с итоговым отчётом и прогресс-баром.

### Автоматическое обновление репозитория
- **auto_update.sh**: Скрипт для проверки обновлений закрытого репозитория по SSH.
  - **Что делает скрипт:**
    - Проверяет наличие или корректность git-репозитория в `/opt/auto-setup`.
    - Клонирует репозиторий, если его нет или он некорректный.
    - Сохраняет локальные изменения через `git stash` перед выполнением `git pull`.
    - Сравнивает локальные и удалённые коммиты для определения необходимости обновления.
    - Регистрирует задание в crontab для выполнения каждые 10 минут.
    - После обновления автоматически запускает основной скрипт `setup.sh`.
  - **Преимущества:**
    - Автоматизированное обновление инфраструктуры без лишних вопросов.
    - Регулярная проверка состояния репозитория с уведомлением о возможных конфликтах.

### Используемые технологии и инструменты
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Certbot](https://img.shields.io/badge/Certbot-4285F4?style=flat-square&logo=certbot&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F26A4B?style=flat-square&logo=grafana&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)

## 📁 Проекты на GitHub
- 🛠 **auto-setup** – Автоматическая настройка сервера с использованием bash-скриптов, docker-compose, Nginx, Certbot и системы мониторинга.
- 🔄 **auto_update.sh** – Скрипт для регулярного обновления репозитория и запуска основного скрипта установки.
- 💬 **TG Control Server** – [R00t4Xbot](https://github.com/R00t4X/R00t4Xbot): Бот для управления серверами через Telegram.
- 💻 **Flask Control Server** – [R00t4Xflask](https://github.com/R00t4X/R00t4Xflask): Веб-интерфейс на Flask для управления ботами.

## 📞 Контакты
- Telegram: [@R00t4X](https://t.me/R00t4X)

---

> 💪 Постоянно прокачиваюсь в мире DevOps и автоматизации. Открыт к новым идеям и сотрудничеству – всегда готов обсудить крутые проекты
