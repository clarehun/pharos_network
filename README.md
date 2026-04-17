# Pharos Atlantic Testnet Bot

---

## Описание
Этот бот автоматизирует типовые действия в тестовой сети Pharos Atlantic. Он реализует:
- Ежедневный чек-ин (Daily check-in)
- Получение токенов из Faucet
- Swaps (обмен токенов)
- Добавление/изъятие ликвидности (Liquidity)
- Делегирование и стейкинг (Stake)
- Торговлю фьючерсами/CFD Trading
- Переводы токенов друзьям (Send Token To Friends)
- Реферальную систему (Refferals)
- Сбор NFT (Collect NFTs)
- Социальные задания: твиттер, дискорд

Все сценарии реализованы по аналогии и согласно заданиям на https://testnet.pharosnetwork.xyz/

---

## Требования:
- **Python:** 3.10+
- **ОС:** Linux/MacOS/Windows
- **Зависимости:** указаны в requirements.txt

---

## Быстрый старт
```sh
git clone https://github.com/clarehun/pharos_network.git
cd pharos_network
python -m venv venv
source venv/bin/activate  # или venv\Scripts\activate для Windows
pip install -r requirements.txt
cp .env.example .env
# Заполнить .env своими данными
python main.py
```

---

## Настройка переменных окружения (.env)
(значения берите с https://testnet.pharosnetwork.xyz/ или своих аккаунтов)
```
PHAROS_RPC_URL=https://rpc.atlantic.pharosnetwork.xyz/
PHAROS_CHAIN_ID=5463
PHAROS_FAUCET_URL=https://testnet.pharosnetwork.xyz/faucet/
WALLET_PRIVATE_KEY=ВАШ_ПРИВАТНЫЙ_КЛЮЧ
DISCORD_TOKEN=необязательно
TWITTER_TOKEN=необязательно
PROXY_URL=необязательно
```

---

## Как использовать и цель
- Все действия аналогичны инструкциям на https://testnet.pharosnetwork.xyz/
- Для каждой операции есть отдельные Python-функции, параметры настраиваются в settings.yaml или .env
- Для соц. задач добавьте токены Discord/Twitter и настройте соответствующие файлы в /files/
- Для работы с NFT/Referral функции используйте приведённые в проекте структуры данных.

---

## Ссылки Pharos:
- Документация: https://testnet.pharosnetwork.xyz/
- Фаусет: https://testnet.pharosnetwork.xyz/faucet/
- Эксплорер: https://explorer.testnet.pharosnetwork.xyz/
- RPC: https://rpc.atlantic.pharosnetwork.xyz/
- WebSocket: ws://ws.atlantic.pharosnetwork.xyz:8546

---

## Лицензия
Проект распространяется под лицензией MIT. Условия в файле LICENSE.