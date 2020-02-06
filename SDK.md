# Вопросы
## SDK
1. Explain data model concepts – scene graph, properties, appearance, layers, etc.
2. Part representations: restrictions of number of each type and why? How to convert between them?
3. What is LOD? Why do we need them? How to find medium LOD? How to create a new LOD?
4. Appearances: Which objects in data model can bear appearances? Priority of appearances attached to
various objects?
5. Write code to find unique parts for a given model.
6. General architecture of import workflow. Key classes and their roles. For a given format (e.g. JT, Parasolid,
ACIS, etc.) explain workflow.
7. Validation properties. What are these? Why? Which are supported by CAD Exchanger?
8. Interoperability with OCC (geometry, topology, XDE). How to convert to/from CAD Exchanger?
9. Which debugging techniques are available (asserts, logging, DRAW, etc.)? Where each could be helpful? Give
examples of usage. What would you add/extend and why?
10. Explain test library usage. Explain creation of a new test / extension of existing – show examples of your
created test cases and explain why you did that way.
11. SDK public API. How is it separated from private API? Which classes are part of it.
12. Are there direct mappings between formats (e.g. STEP to Para)? Why yes or why not?

## SDK
1. Объясните понятия модели данных-граф сцены, свойства, внешний вид, слои и т. д.
2. Представления частей: ограничения числа каждого типа и почему? Как конвертировать между ними?
3. Что такое Лод? Зачем они нам нужны? Как найти среднего Лода? Как создать новый Лод?
4. Внешние виды: какие объекты в модели данных могут иметь внешние виды? Приоритет внешних проявлений, прилагаемых к
различные предметы?
5. Напишите код для поиска уникальных деталей для данной модели.
6. Общая архитектура процесса импорта. Ключевые классы и их роли. Для данного формата (например, JT, Parasolid,
ACIS и др.) объясните рабочий процесс.
7. Свойства проверки. Что это такое? Почему? Какие поддерживаются CAD-обменником?
8. Взаимодействие с OCC (геометрия, топология, XDE). Как конвертировать в / из CAD-обменника?
9. Какие методы отладки доступны (asserts, logging, DRAW и т. д.)? Где каждый из них может быть полезен? Дай
пример использования. Что бы вы добавили / расширили и почему?
10. Объясните использование библиотеки тестов. Объясните создание нового теста / расширение существующего-покажите примеры вашего
создавал тестовые случаи и объяснял, почему вы так поступили.
11. SDK public API. Как он отделен от private API? Какие классы являются его частью.
12. Существуют ли прямые сопоставления между форматами (например, шаг к пункту)? Почему да или почему нет?

# Ответы

## 1
https://cadexchanger.com/download/sdk/doc/dev/html/sdk_data_model_product_structure.html

## 2
   1. Brep 0/1
   2. Polygonal 0/1+
   3. https://cadexchanger.com/download/sdk/doc/dev/html/sdk_data_model_representations.html

## 3
* https://cadexchanger.com/download/sdk/doc/dev/html/sdk_data_model_representations.html
* https://cadexchanger.com/download/sdk/doc/dev/html/sdk_usage_meshing.html

## 4
https://cadexchanger.com/download/sdk/doc/dev/html/sdk_data_model_styles.html

## 5
   1. Sener
   2. ...

## 6
   1. doxygen

## 7
   1. STEP
   2. Para
   3. X3D
   4. OBJ
   5. и т.д.

## 8 
   1. BRep rep
   2. Triangulation
   3. PMI
   4. Texture
   5. Materials
Примеры:
   1. STEP может хранить Бреп и ПМИ
   2. JT BRep Tri PMI...
   3. https://cadexchanger.com/download/sdk/doc/dev/html/sdk_supported_formats.html