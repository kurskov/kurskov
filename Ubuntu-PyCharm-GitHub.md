# Настройка PyCharm + GitHub под Ubuntu

Краткая инструкция по настройке работы PyCharm с репозиторием GitHub в системе Ubuntu.

## Установка Git в Ubuntu

Обновляем списки пакетов из репозиториев:    
```
$ sudo apt update
```

Загружаем и устанавливаем программу:    
```
$ sudo apt install git
```

Проверяем версию:    `
```
$ git --version
```

## Настройка Git

Инициация пользователя:
```
$ git config --global user.name "Your Name"
$ git config --global user.email "youremail@domain.com"
```
Проверка установленных параметров:
```
$ git config --list
```

## Источники

[Установка Git в Ubuntu](https://losst.ru/ustanovka-git-ubuntu-16-04)
