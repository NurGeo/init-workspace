# Настройка SSH

Этот скрипт автоматизирует настройку SSH ключей для вашего пользователя.

## Шаги для настройки SSH ключей

1. **Склонируйте репозиторий**:

    ```sh
    git clone https://github.com/nurgeo/init-workspace.git
    ```

2. **Перейдите в директорию с репозиторием**:

    ```sh
    cd init-workspace
    ```

3. **Дайте права на выполнение скрипта**:

    ```sh
    chmod +x setup-ssh.sh
    ```

4. **Запустите скрипт**:

    ```sh
    sudo ./setup-ssh.sh
    ```

5. **Следуйте инструкциям на экране для ввода данных о приватном и публичном ключах, а также для настройки SSH конфигурации**.

6. **Проверьте, что ключи успешно добавлены в SSH агент**:

    ```sh
    ssh-add -l
    ```

7. **Проверьте подключение к серверу или GitHub, используя команду**:

    ```sh
    ssh -T git@github.com
    ```

Эти шаги помогут вам настроить SSH ключи для вашего пользователя автоматически.