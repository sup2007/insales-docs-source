# ui-сompare-widget
  Компонент представляет собой ссылку на сравнение в виде иконки с колличеством товаров в сравнении. Возможно добавлять заголовок.

## Пример использования

````html
<ui-compares-widget
  color-sheme="transparent"
  title="{{ messages.compare_description }}"
>
</ui-compares-widget>
````

## Параметры

Данный компонент поддерживает следущие параметры

* `title` - Заголовок для сравнения.
* `vr-gutter` - Вертикальный отступ.
* `hr-gutter` - Горизонтальный отступ.


## Темизация
* `layout` - 
  - `count-bubble` - Колличество товара в круге прикрепленному к верхнему правому углу иконки сравнения.
* `color-sheme`
  - `count-background-main` - закрышивает фон колличества товара в основной цвет.
  - `count-background-sub` - закрышивает фон колличества товара в дополнительный цвет.