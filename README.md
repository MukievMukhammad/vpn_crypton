# VPN сервер WireGuard

## Настройка сервера

Развернуть VPN сервер на основе WireGuard используя готовый скрипт созданный разработчиками из команды [Crypton](https://www.youtube.com/c/CryptonAcademy/featured).

Команда для выполнения скрипта по развертыванию VPN сервера

```bash
«wget -q -O vpn_crypton.sh https://raw.githubusercontent.com/MukievMukhammad/vpn_crypton/main/vpn_crypton.sh && chmod +x vpn_crypton.sh && sudo /bin/bash vpn_crypton.sh»
```

После завершения настройки на экране должны появится 10 наборов данных, состоящих из двух абзацев: [Interface] и [Peer] и QR-кода, в который «зашиты» эти же данные. **Сохранить эти данные себе!**

> Можно так же установить используя Docker, будет GUI для управления доступом, что возможно удобней. [https://hub.docker.com/r/linuxserver/wireguard](https://hub.docker.com/r/linuxserver/wireguard)

## Подключение к серверу

### Телефон

1. Установить приложение WireGuard
2. Нажать +, сканировать сохраненный ранее QR код

### ПК

1. Установить приложение WireGuard
2. Скопируйте любой из созданных наборов данных из терминала командной строки в любой текстовый редактор и сохраните файл с расширением «.conf».
3. Откройте клиент программы WireGuard на компьютере и нажмите «Импорт туннелей из файла»
