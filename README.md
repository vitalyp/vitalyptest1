##Коллеги

>>после просмотра очередного эпизода Clean Code в воздухе витает идея организации Project Crash Test - мероприятия сходного со Startup Crash Test, но оценивается не идея проекта, а его код (стиль, архитектура, тесты, процедура установки и тд). Примерная процедура этого процесса следующая:
1. Желающие подают свои проекты для ревью
2. Все, кто хочет принять участие в оценке (абсолютно не важен опыт в технологиях проекта), получают доступ к конкретной версии кода проекта и к документации по установке (компилляция, запуск и тд).
3. Всем дается определенное время на ревью - неделя или две, например
4. После проведения ревью все собираемся и обсуждаем выбранный проект.
Понятное дело, весь код больших проектов мы вряд ли осилим, но основные моменты в архитектуре и стиле, а также наличия тестов и прочих бест практисес, можно будет уловить. Кстати, это также будет означать, что к проекту обязательно будет создано руководство по установке, чего у нас так не хватает для большинства проектов.

![Nitrous.IO](https://d1qb2nb5cznatu.cloudfront.net/startups/i/87273-d99f6a2e0583e0b32cdde5ef17c94876-medium_jpg.jpg?buster=1381989005 "Web IDE Nitrous.IO")


- Нажмите на эту кнопку
- [![Hack vitalyp/vitalyptest1 on Nitrous.IO](https://d3o0mnbgv6k92a.cloudfront.net/assets/hack-l-v1-4b6757c3247e3c50314390ece34cdb11.png)](https://www.nitrous.io/hack_button?source=embed&runtime=rails&repo=vitalyp%2Fvitalyptest1&file_to_open=README.md)
- зарегайтесь на сайте Через Github аккаунт
- (опционально: опять нажмите на кнопку если регистрация сбила контекст)
- Выберите эту опцию: 'or use one of these boxes: vitalyptest1'
- читайте инструкцию дальше, из под Nitrous.IO!


Инструкция Дальше:
==================

1. Directory tree -> /workspace/vitalypCrashTestV1 контекстное меню -> set as root
2. Console window in the bottom:

  
```bash
cd vitalypCrashTestV1

#! vitalypCrashTestV1     - my repo linked with Github (pull requests allowed)
#! workspace/vitalyptest1 - your copy of my project, not linked to Github (feel free with it)
```

```bash
bundle install
rake db:migrate
rails s
```

IDE Menu: Preview -> Port 3000 (no SSL)

##If ok:
  
  1.  `$ git checkout -b vitalyp_review1`   // _create new branch with master head_
  2.  Do code updates, Ctrl+S
  3.  `$ git add .`                         // _add to stage_
  4.  `$ git commit -m "review project structure."`
  5.  `$ git push origin vitalyp_review1`   // _push for pull request_
  6.   Navigate https://github.com/vitalyp/vitalyptest1/branches
  7.   At your brunch, click 'New pull request'
