Установка Docker и nginx на чистый сервер (Ubuntu 22.04)
=========

Роль для настройки веб-сервера
------------

Устанавливает docker, docker-compose и nginx(вместе с конфигурацией)


Переменные
--------------

*group_vars*: ansible_host, ansible_user, ansible_password, ansible_sudo_pass
*vars(main.yml)*: В этом файле описаны все пакеты для установки, также пароль для ansible пользователя и имя проекта(исп. в конфигурации nginx)

        
*   Проверить соединение можно командой:

        sudo ansible ИМЯ_ХОСТА -i hosts -m ping -b

Пример использования роли
----------------

*   Для использования роли достаточно запустить команду:

        sudo ansible-playbook -i hosts StartSetup.yml

