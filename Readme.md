# Заметки по верстке и стилизации
* by Rob Kano

---
## Адаптивная верстка
~<meta name="viewport" content="width=device-width, initial-scale=1.0">~

### Адаптивные изображения
~~~~~~
img {
    max-width: 100%;
    height: auto;
  }
~~~~~~

### Центровка страницы
~~~
.page-container {
    max-width: 1200px;
    margin: 0 auto;
}
~~~

### Перевод фиксированных единиц в проценты (резина)
% = контейнер / фиксированную ширину элемента
* родительский элемент - flex
* ширина блоков в %
* высота - min-height

[Единицы измерения для адаптивных сайтов](https://toster.ru/q/332041#answer_840202)

---
### Стилизация svg встроенного object тегом
* встроить путь до стилевого файла css в файл svg *(перед тегом <svg>)*:
    ><?xml-stylesheet type="text/css" href="../path/to/your.css"?>
* добавить в элемент "svg" и "path" svg-файла, классы:
    ><svg class="logo-svg" ...>
    ><path class="logo-svg__path".../>
* стилизовать svg по классам в файле указаном выше

---

