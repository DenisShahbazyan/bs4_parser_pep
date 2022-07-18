# Парсер документации PEP

## Описание:
Парсер документации PEP. Парсит статьи по нововведениям в Python, статусы последних версий со ссылками на документацию, формирование таблицы с количеством PEP в каждом статусе, а так же скачивает документации по последней версии Python.

### Опции:
1. ```--output pretty``` - вывод в табличном представлении в консоль.
2. ```--output file``` - вывод таблицы с результатами в файл csv.
3. ```-c``` - очистка кеша перед следующими запросами парсера.

## Развертывание:
- Склонируйте проект на Ваш компьютер 
```sh 
git clone https://github.com/DenisShahbazyan/bs4_parser_pep.git
``` 
- Перейдите в папку с проектом 
```sh 
cd bs4_parser_pep
``` 
- Создайте и активируйте виртуальное окружение 
```sh 
python -m venv venv 
source venv/Scripts/activate 
``` 
- Обновите менеджер пакетов (pip) 
```sh 
pip install --upgrade pip 
``` 
- Установите необходимые зависимости 
```sh 
pip install -r requirements.txt
``` 

### Режимы работы парсера:
1. ```python main.py whats-new``` - Парсер статей по нововведениям в Python.
2. ```python main.py latest-versions``` - Статусы последних версий со ссылками на документацию.
3. ```python main.py download``` - Скачивание документации по последней версии Python.
4. ```python main.py pep``` - Формирование таблицы с количеством PEP в разрезе по статусам.

### Запуск парсера:
```
main.py [-h] [-c] [-o {pretty,file}] {whats-new,latest-versions,download,pep}
Парсер документации Python

positional arguments:
  {whats-new,latest-versions,download,pep}
                        Режимы работы парсера

optional arguments:
  -h, --help            show this help message and exit
  -c, --clear-cache     Очистка кеша
  -o {pretty,file}, --output {pretty,file}
                        Дополнительные способы вывода данных
```

## Системные требования:
- [Python](https://www.python.org/) 3.10.4

## Планы по доработке:
>Проект сделан в учебных целях, доработка не планируется.

## Используемые технологии:
-   [BeautifulSoup](https://pypi.org/project/beautifulsoup4/) 4.11.1
-   [lxml](https://pypi.org/project/lxml/) 4.9.1
-   [PrettyTable](https://pypi.org/project/prettytable/) 3.3.0
-   [requests-cache](https://pypi.org/project/requests-cache/) 0.9.5
-   [tqdm](https://pypi.org/project/tqdm/) 4.64.0

## Авторы:
- [Denis Shahbazyan](https://github.com/DenisShahbazyan)

## Лицензия:
- MIT
