# Инструкция для Маркдаун

## Что такое Markdown?

 Markdown — это облегченный язык разметки с синтаксисом форматирования обычного текста.

## Полужирное и курсивное начертания

 Чтобы задать для текста полужирное начертание, заключите его в двойные звездочки:
  **bold**.

 Чтобы задать для текста курсивное начертание, заключите его в одинарные звездочки:
 *italic*.

Чтобы задать для текста полужирное и курсивное начертание, заключите его в тройные звездочки:
***bold and italic***.

## Заголовки

 Заголовки обозначаются знаком #.
 Подзаголовок обозначается двойным знаком ##.
 Возможно использование подзаголовков более низкого уровня до шести знаков ######.

## Изображения

 Для изображений по умолчанию поддерживаются следующие типы файлов: .jpg, .png
 Чтобы было возможно использовать другие типы изображений, например .gif, их необходимо добавить в качестве ресурсов в docfx.json:
 "resource": 
  
    "files" : [
      "**/*.png",
      "**/*.jpg,
      "**/*.gif"
    ]

Базовый синтаксис Markdown для внедрения изображения:

 Example:
 [ < alt text> ] ( < folderPath > )
 В примере написано с пробелами, в синтаксисе пробелов быть не должно!

 Где < alt text > — краткое описание изображения, а < folder path > — относительный путь к нему. Заменяющий текст необходим для средств чтения с экрана для слабовидящих. Он также удобен при возникновении ошибок на сайте, из-за которых не удается воспроизвести изображение.

## Списки (нумерованные, маркированные, контрольные)

 ### Нумерованный список
 Чтобы создать нумерованный список, можно использовать все единицы. При публикации числа отображаются в возрастающем порядке в виде последовательного списка. Например:
  1. это раз
  2. это два
  3. это три

 ### Маркированный список
 Для создания маркированного списка используйте - или *, за которым следует пробел в начале каждой строки/ Пример:
 * это раз
 * это два
 * это три

 ## Контрольный список
 Контрольные списки доступны для использования в Microsoft Learn через пользовательское расширение Markdown. Пример:
 > * List item 1
 > * List item 2
 > * List item 3

## Таблицы
Использование вертикальных линий и строк является самым простым способом создания таблиц в Markdown. Чтобы создать стандартную таблицу с заголовком, вставьте пунктирную линию после первой строки.
Пример:
|This is   |a simple   |table header|
|----------|-----------|------------|
|table     |data       |here        |
|it doesn't|actually   |have to line up nicely!|
