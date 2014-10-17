
![Nitrous.IO](https://d1qb2nb5cznatu.cloudfront.net/startups/i/87273-d99f6a2e0583e0b32cdde5ef17c94876-medium_jpg.jpg?buster=1381989005 "Web IDE Nitrous.IO")


- Нажмите на эту кнопку
- [![Hack vitalyp/vitalyptest1 on Nitrous.IO](https://d3o0mnbgv6k92a.cloudfront.net/assets/hack-l-v1-4b6757c3247e3c50314390ece34cdb11.png)](https://www.nitrous.io/hack_button?source=embed&runtime=rails&repo=vitalyp%2Fvitalyptest1&file_to_open=README.md)
- зарегайтесь на сайте Через Github аккаунт
- Далее -> Ок -> Согласинг
- Открывайте проект из под веб-ide
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

