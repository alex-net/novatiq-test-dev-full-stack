# Тестовое задание для вёстки WebApps для Telegram.

#### Задача:
Есть [дизайн в Figma](https://www.figma.com/file/oCE7kXXlzmN3ARegcDt1Of/%D0%A5%D0%BE%D0%B7%D1%8F%D0%B8%D0%BD-%D0%B3%D0%BE%D1%80%D0%B1%D1%83%D1%88%D0%BA%D0%B8?type=design&node-id=815-5715&mode=design&t=HU5YPL5ZnVZBmovS-0). По ссылке одна страница которую нужно сверстать, все иконки и фотографии товаров есть в самой Figma Вам нужно их от туда экспортировать сомостоятельно. Страница предоставленная по ссылке, это мобильная версия которая должна быть адаптивна под любой размер экрана.

### Какие требования есть к вёрстке?
Придерживайтесь строго к дизайну который создал дизайнер.

### Как предоставить готовое выполнения задания?
Используйте во время верстки git, по окончанию пришлите в чат который вас добавили ссылку на свой репозиторий.

### Какой фремворк заюзать для верстки?
Решать вам.

### Где взять иконки?
В Figma, экспортируйте их от туда.


## Реализация ..

Результат выполнения находится в файлике *index.html* в корне репозитория.
Для сборки стилей из scss ... нужно выполнить следующие шаги:
* запуск контаенера при помощи команды
``` docker run --rm -u 1000:1000 --name sassc -d -v ./scss:/input -v ./css:/output gerrit91/scss-watcher ```
* выполнить команду  ``` docker exec -ti sassc sassc ./input/style.scss output/style.css ```
* после успешного выполнения можно потушить контейнер командой ```docker stop sassc ```
