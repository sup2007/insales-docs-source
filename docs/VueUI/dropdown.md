# ui-dropdown

Данный компонент представляет собой выпадающий блок с кнопкой и произвольным контентом.

## Пример использования

````html
<ui-dropdown
  class="some_class"
  caption="Открывалко"
  position="top"
  open-on-hover
  toggle-icon="fa fa-angle-down"
>
  Привет!! я какой-то контент, который виден при открытии
  <div>
    можно вставлять произвольный контент
  </div>
</ui-dropdown>
````

## Параметры

Данный компонент поддерживает следущие параметры

* `caption` - подпись на кнопке открывашке
* `toggle-icon` - иконка, указывающая, что это выпадашка
* `position` - положение выпадашки относительно кнопки. Возможные значения: * `top`, `right`, `bottom`, `left`. По-умолчанию `bottom`.
* `open-on-hover` - если указан, выпадающий список показывает при наведении на кнопку.

## Классы компонента

В ходе работы компонента к его различным элементам присваиваются следующие классы.

### Переключатель

`.dropdown__toggle` - опорный класс переключателя
`.dropdown__toggle.is-focused` - кнопка в фокусе, эквивалент `:focus`
`.dropdown__toggle.is-hovered` - кнопка, под курсором, эквивалент `:hover`
`.dropdown__toggle.is-opened` - дроп открыт
`.dropdown__toggle.is-closed` - дроп закрыт

### выпадашка

`dropdown__popup` - контейнер пвыпадающего списка
`dropdown__popup_opened` - контейнер показан
`dropdown__popup_closed` - контейнер спрятаня

## Особенности
