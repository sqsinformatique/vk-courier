# vk-courier

Запуск бэка:
1) Перейти в ./curier-back
2) Установить docker-compose, docker
3) Запустить бэк командой
   docker-compose -f "docker-compose.yml" up -d --build
4) Установить ngrok
5) Запустить ngrok
   ngrok http http://localhost:9000 -host-header="localhost:9000" 
6) Скопировать/записать/запомнить адрес, который будет выведен после запуска в формате https://XXXXXXXXXX.ngrok.io
7) Перейти в ./vk-courier/vk-courier-front/src/modules
8) В файле backRequests.js изменить константу back_url на адрес полученный от ngrok на шаге 6
Если нужно сменить порт для бэка, то:
1) Перейти в ./curier-back
2) В файле variables.env в строке с параметром PUBLICHTTP_LISTEN изменить порт 9000 на произвольный

Запуск фронта
1) Вернуться в ./vk-courier, запустить фронт 
   nmp start
2) Запустить ngrok 
   ngrok http https://localhost:10888 -host-header="localhost:10888"
3) Скопировать/записать/запомнить адрес, который будет выведен после запуска в формате https://XXXXXXXXXX.ngrok.io
4) Указать адрес с шага 3 в настройках приложения в ВК

Контакты:
телеграм @SoldatovSergey


