# HW1 - Подготовка к курсу и инфраструктура ПО 
 ## Описание/Пошаговая инструкция выполнения домашнего задания:
   ### 1. Docker
   
    - Установить Docker себе на локальную машину
    - Описать инфраструктуру в Docker-compose, которая включает в себя
    - nginx (обрабатывает статику, пробрасывает выполнение скриптов в fpm)
    - php-fpm (соединяется с nginx через unix-сокет)
    - redis (соединяется с php по порту)
    - memcached (соединяется с php по порту)
    - БД подключать как отдельную VM (можно на базе Homestead), либо как контейнер (но тогда не забудьте про директории с данными)
    - Не забудьте про Composer
  
 ### 2*. Виртуальные машины.
   
    - Развернуть Homestead VM при помощи Vagrant и VirtualBox
    - Сайт должен отвечать на доменное имя application.local
    - Должна быть поддержка проброса директорий

    
#### Критерии оценки:
    
    Каждый RUN в Dockerfile будет создавать промежуточный образ при сборке. Помните об этом. Желательно снизить их использование до минимума.
    Docker - основная задача