Vector-role
=========

Устанавливает и настраивает [Vector](https://vector.dev/).
Поддерживаемые системы:
* CentOS 7
* Ubuntu

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
|clickhouse_host_name|clickhouse-01|В inventory.yml имя хоста ClickHouse|


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

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

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
