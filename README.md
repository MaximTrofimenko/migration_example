Минимальная возможная конфигурация для работы с liquibase в связке с spring boot

1. зависимость liquibase-core https://mvnrepository.com/artifact/org.liquibase/liquibase-core
2. настройки в application.yaml описывающие путь к changelog файлу и наименование схемы в базе данных
3. пустой changelog.xml файл куда в дальнейшем будут добавляться описания миграций
