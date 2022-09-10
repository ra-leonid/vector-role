Vector-role
=========

Устанавливает и настраивает [Vector](https://vector.dev/).

Requirements
------------

Поддерживаемые системы:
* CentOS 7
* Ubuntu

Role Variables
--------------
|Переменная|Значение по умолчанию|Назначение|
|---|---|---|
|vector_version|0.24.0|Определяет устанавливаемую версию|
|clickhouse_user|logger|Пользователь для подключения к ClickHouse|
|clickhouse_password|logger|Пароль пользователя ClickHouse|


Dependencies
------------

Эта роль - результат выполнения домашнего задания. Для использования в продуктиве - не предназначена ;-).

Чтобы её использовать, необходимо:

1. Добавить в файл `requirements.yml` текст:
``` yaml
- name: vector-role
  src: git@github.com:ra-leonid/vector-role.git
  scm: git
  version: <last tag>
```
`<last tag>` заменить на значение последнего тэга.

2. Выполнить команду копирования роли:
``` bash
ansible-galaxy install -r requirements.yml -p roles -f
```

Example Playbook
----------------

``` yaml
- name: Install Vector
  hosts: <vector host>
  roles:
    - vector-role
```

License
-------

MIT

Author Information
------------------

Расторгуев Леонид.
