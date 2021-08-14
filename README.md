# Тестовое задание Junior

Здесь находится описание тестового задания на позицию Junior разработчика в компанию XXX.

## Задача

Создать одностраничное приложение файловый менеджер с поддержкой текстовых файлов и директорий с использованием фронтенд и бекенд фреймворков, БД с возможностью добавления/удаления/обновления файлов, директорий.

### Общие требования

- Дизайн на усмотрение разработчика.
- Вся информация должна сохраняться при перезагрузке страницы.
- Использовать любые frontend, backend фреймворки и СУБД, предпочтительно Angular, Symfony, PostgreSQL.

## Требования задачи

Всё, что не указано в требованиях, остаётся на усмотрение исполнителя задачи.

### Список с директориями и текстовыми файлами в текущей директории:

|Тип  |Название   |Удалить|Редактировать  |
|---  |---        |---    |---            |
|dir  |..         | -     | -             |
|dir  |Directory 1|delete |edit           |
|file |File 1     |delete |edit           |
|file |File 2     |delete |edit           |
| -   | new file  |new dir|trash          |

- Последняя строка представляет собой список действий: создание файла в текущей директории, создание директории в текущей директории, переход в корзину.
- При отображении всегда должна быть сортировка по типу, потом по названию: сначала директории отсортированные по названию, потом файлы названию.
- Нажатие на название директории открывает сожержимое директории.
- Нажатие на название файла открывает файл на редактирование.
- Файл содержит в себе название файла и текстовое содержимое.
- Нажатие на delete перемещает директорию/файл в корзину.
- Нажатие на new dir позволяет создать директорию в текущей директории.
- Нажатие на new file позволяет создать файл в текущей директории.
- Нажатие на .. открывает родительскую директорию текущей директори.
- Нажатие на trash открывает корзину удалённых файлов и директорий.

### Корзина 

|Тип  |Название   |Восстановить |Удалить        |
|---  |---        |---          |---            |
|dir  |..         | -           | -             |
|dir  |Directory 2|restore      |delete         |
|file |File 3     |restore      |delete         |

- Нажатие на restore восстанавливает директорию(и всё её содержимое)/файл.
- Нажатие на delete удаляет директорию(и всё её содержимое)/файл.
- При отображении всегда должна быть сортировка по типу, потом по названию: сначала директории отсортированные по названию, потом файлы названию.
- Если директория в которую происходит удаление файла/директории удалена, то восстанавливать в корень.

## Добавление/обновление файлов/директорий

- У файла должны быть редактируемое название и текстовое содержимое.
- У директории должно быть редактируемое название.

## Для Backend/Fullstack

- Ханить всю информацию в БД, можно использовать любую, предпочтительно PostgreSQL.

## Для Frontend/Fullstack

- В качесте хранилища использовать [Firebase](https://firebase.google.com/docs/database).
