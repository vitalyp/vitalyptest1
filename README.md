##Коллеги

после просмотра очередного эпизода Clean Code в воздухе витает идея организации Project Crash Test - мероприятия сходного со Startup Crash Test, но оценивается не идея проекта, а его код (стиль, архитектура, тесты, процедура установки и тд). Примерная процедура этого процесса следующая:
1. Желающие подают свои проекты для ревью
2. Все, кто хочет принять участие в оценке (абсолютно не важен опыт в технологиях проекта), получают доступ к конкретной версии кода проекта и к документации по установке (компилляция, запуск и тд).
3. Всем дается определенное время на ревью - неделя или две, например
4. После проведения ревью все собираемся и обсуждаем выбранный проект.

Понятное дело, весь код больших проектов мы вряд ли осилим, но основные моменты в архитектуре и стиле, а также наличия тестов и прочих бест практисес, можно будет уловить. Кстати, это также будет означать, что к проекту обязательно будет создано руководство по установке, чего у нас так не хватает для большинства проектов.


## 1 Directory tree -> /workspace/vitalypCrashTestV1 контекстное меню -> set as root
## 2 Console window in the bottom:
      $ cd vitalypCrashTestV1        //  vitalypCrashTestV1     - my repo linked with Github (pull requests allowed)
                                     //  workspace/vitalyptest1 - your copy of my project, not linked to Github (feel free with it)
      $ bundle install
      $ rake db:migrate
      $ rails s
## 3 IDE Menu: Preview -> Port 3000 (no SSL)

If ok:
  1.
      $ git checkout -b vitalyp_review1  // create new branch with master head
  2.
      Do code updates, Ctrl+S
  3.
      $ git add .                                  // add to stage
      $ git commit -m "review project structure."
      $ git push origin vitalyp_review1            // push for pull request
  4.
      Navigate https://github.com/vitalyp/vitalyptest1/branches
      At your brunch, click 'New pull request'
