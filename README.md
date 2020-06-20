# vk-courier

cd ./curier-back
docker-compose -f "docker-compose.yml" up -d --build
Установить ngrok
./ngrok http http://localhost:9000 -host-header="localhost:9000" 
Скопировать/записать/запомнить адрес, который будет выведен после запуска в формате https://XXXXXXXXXX.ngrok.io
cd ./vk-courier/vk-courier-front/src/modules
В файле backRequests.js изменить константу back_url на адрес от ngrok
Вернуться в ./vk-courier, зарпустить фронт 
nmp start
Запустить ngrok 
ngrok http https://localhost:10888 -host-header="localhost:10888"
Скопировать/записать/запомнить адрес, который будет выведен после запуска в формате https://XXXXXXXXXX.ngrok.io
Указать его в настройках приложения в ВК


