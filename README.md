Добавлен плагин для удобной работы с liquibase

1. добавлен liquibase-maven-plugin в pom.xml
2. свойства для плагина вынесены в файл liquibase.properties
3. добавлена миграция с удалением колонки из таблицы

Самые полезные команды:

1. mvn liquibase:update - развертывает любые изменения, которые находятся в файле журнала изменений и которые еще не были развернуты в вашей базе данных
2. mvn liquibase:dropAll - удаляет все объекты базы данных
3. mvn liquibase:dbDoc - генерирует в папку target/docs информацию о базе данных в удобном формате
4. mvn liquibase:tag -Dliquibase.tag=my_tag - добавляет тэг к последней миграции
5. mvn liquibase:rollback -Dliquibase.rollbackTag=my_ta - откатить все изменения до этого тэга
6. mvn liquibase:rollback -Dliquibase.rollbackCount=2 - откатить последние миграции указав их количество

https://docs.liquibase.com/tools-integrations/maven/commands/home.html
