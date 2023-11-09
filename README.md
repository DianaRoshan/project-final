## [REST API](http://localhost:8080/doc)

## Концепция:

- Spring Modulith
    - [Spring Modulith: достигли ли мы зрелости модульности](https://habr.com/ru/post/701984/)
    - [Introducing Spring Modulith](https://spring.io/blog/2022/10/21/introducing-spring-modulith)
    - [Spring Modulith - Reference documentation](https://docs.spring.io/spring-modulith/docs/current-SNAPSHOT/reference/html/)

```
  url: jdbc:postgresql://localhost:5432/jira
  username: jira
  password: JiraRush
```

- Есть 2 общие таблицы, на которых не fk
    - _Reference_ - справочник. Связь делаем по _code_ (по id нельзя, тк id привязано к окружению-конкретной базе)
    - _UserBelong_ - привязка юзеров с типом (owner, lead, ...) к объекту (таска, проект, спринт, ...). FK вручную будем
      проверять

## Аналоги

- https://java-source.net/open-source/issue-trackers

## Тестирование

- https://habr.com/ru/articles/259055/

- Список выполненных задач:
- 1-Разобраться со структурой проекта (onboarding).
- 2-Удалить социальные сети: vk, yandex.
- ![image](https://github.com/DianaRoshan/project-final/assets/77641186/4a4d7897-4b6b-4eb8-bd48-127c1d905f55)
- ![image](https://github.com/DianaRoshan/project-final/assets/77641186/11d25100-384c-4f6f-8e40-642587026c2b)
- ![image](https://github.com/DianaRoshan/project-final/assets/77641186/73a9704e-e8a5-4961-a291-4960e6ffa685)
- 6-Сделать рефакторинг метода com.javarush.jira.bugtracking.attachment.FileUtil#upload чтоб он использовал современный подход для работы с файловой системмой ( Использовала Path, Paths, Files).
- ![image](https://github.com/DianaRoshan/project-final/assets/77641186/4298f49d-8e8a-4d23-af51-bf1917df6197)
- Вынести чувствительную информацию в отдельный проперти файл
- Добавить локализацию минимум на двух языках для шаблонов писем (mails) и стартовой страницы index.html.
- ![image](https://github.com/DianaRoshan/project-final/assets/77641186/04f16510-04dc-4bc9-8cb2-b7a256f79fa4)


