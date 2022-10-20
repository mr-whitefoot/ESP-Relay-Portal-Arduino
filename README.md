# ESP-Relay-Portal-Arduino

WiFi реле на ESP-01/ESP-01s.

### Возможности: 
- Управление через web портал;
- Управление через MQTT;
- Интеграция с [HomeAssistant](https://www.home-assistant.io) через MQTT;
- Обновление прошивки через web портал;
- Поддержка управления реле как по высокому, так и по низкому уровню сигнала;
- Сохранение состояния реле при потере питания;
- Переход в режим точки доступа, при недоступности Wi-Fi указанного в настройках;
- Переход в режим клиента Wi-Fi при доступности WiFi указанного в настройках.


### Интерфейс web портала:
Главный экран<br>
<img width="389" alt="main" src="https://user-images.githubusercontent.com/16363451/197064457-455fc27a-cce4-4100-985f-9d602ddb5188.png">

Выбор настроек<br>
<img src="https://user-images.githubusercontent.com/16363451/197059246-f744cb51-43c3-43cf-b79c-b898cdecf48b.png" width="400">

Настройки реле<br>
<img width="386" alt="preferences" src="https://user-images.githubusercontent.com/16363451/197064615-bbcfbd92-4fc6-41d3-a8e4-4dd3bb9980e8.png">

Обновление прошивки по Wi-Fi<br>
<img src="https://user-images.githubusercontent.com/16363451/197058992-d8bc1296-aa61-4ff9-ba36-1ad8a007244e.png" width="400">


### Первоначальная настройка:
- Подключиться к точке доступа relayAP;
- Откроется портал, если не откроется, перейти по адресу 192.168.4.1;
- Нажать кнопку Configuration;
- Нажать WiFi configuration;
- Указать данные вашего Wi-Fi: SSID, пароль;
- Нажать кнопку Save and reboot.

После перезагрузки устройства в браузере перейти по адресу relay.local, либо посмотреть IP адрес на роутере.


### Обновление прошивки через портал:
- Скачать [последнюю версию прошивки](https://github.com/mr-whitefoot/ESP-Relay-Portal-Arduino/releases/latest);
- Перейти на портале устройства Configuration -> Firmware upgrade;
- Нажать кнопку OTA firmware;
- Выбрать скачанный bin файл;
- Дождаться обновления страницы с сообщением Update Success! Rebooting...;
- Подождать не менее 15 секунд и нажать кнопку Home, для перехода на главную страницу;
- Проверить версию устройства в блоке Information.


