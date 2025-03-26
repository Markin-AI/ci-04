# Домашнее задание к занятию "`Jenkins`" - `Маркин Алексей`

## Подготовка к выполнению

1. Создать два VM: для jenkins-master и jenkins-agent.
2. Установить Jenkins при помощи playbook.
3. Запустить и проверить работоспособность.
4. Сделать первоначальную настройку.

## Основная часть

1. Сделать Freestyle Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.

![1](https://github.com/Markin-AI/ci-04/blob/main/img/1.png)

2. Сделать Declarative Pipeline Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.

![2](https://github.com/Markin-AI/ci-04/blob/main/img/2.png)

3. Перенести Declarative Pipeline в репозиторий в файл [`Jenkinsfile`](https://github.com/Markin-AI/ci-04/blob/main/Jenkinsfile).

![3](https://github.com/Markin-AI/ci-04/blob/main/img/3.png)

4. Создать Multibranch Pipeline на запуск `Jenkinsfile` из репозитория.

![4](https://github.com/Markin-AI/ci-04/blob/main/img/4.png)

5. Создать Scripted Pipeline, наполнить его скриптом из [pipeline](./pipeline).

![5](https://github.com/Markin-AI/ci-04/blob/main/img/5.png)

![6](https://github.com/Markin-AI/ci-04/blob/main/img/6.png)

6. Внести необходимые изменения, чтобы Pipeline запускал `ansible-playbook` без флагов `--check --diff`, если не установлен параметр при запуске джобы (prod_run = True). По умолчанию параметр имеет значение False и запускает прогон с флагами `--check --diff`.
7. Проверить работоспособность, исправить ошибки, исправленный Pipeline вложить в репозиторий в файл `ScriptedJenkinsfile`.
8. Отправить ссылку на [репозиторий с ролью](https://github.com/Markin-AI/vector-role) и [Declarative Pipeline](https://github.com/Markin-AI/ci-04/blob/main/Jenkinsfile) и [Scripted Pipeline](https://github.com/Markin-AI/ci-04/blob/main/ScriptedJenkinsfile).
9. Сопроводите процесс настройки скриншотами для каждого пункта задания!!

---