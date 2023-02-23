#Images Convertor

Разработать сервис обработки фото, который принимает ряд параметров
**Возможные параметры**
- таргет формат
- качество?
- один свой параметр?
И имеет ряд ограничений
**Ограничения**
- Для каждого клиента, сервер одновременно может обрабатываться не более чем 1 документ
- Всего может обрабатываться не более трех документов за раз
- Максимальный размер 1-го документа не более 50mb

##START

1) Create .env, add PORT=5000
2) npm install
3) npm run start 

##Queries

POST (convert image):
URL: http://localhost:5000/images/upload
PARAMS: {format: String; image: File}
format: 'webp' || 'jpeg' || 'png'

GET (status):
URL: http://localhost:5000/images/status:{id}

GET (download image):
URL: http://localhost:5000/images/download:{id}
