# ui-notice
  Представляет собой уведомление

## Пример использования
```html
<ui-notice>
  Текст уведомления
</ui-notice>
```

## Параметры

* `variant` - Вариант уведомления, влияет на окрас уведомления. Доступные значения: `info`, `succes`, `warning`, `error`. Можно указать своё значение. Класс для кастомизации `notice_your-class`. Значение по-умолчанию `info`.
* `fadeTime` - Время исчезновения уведомления. Значение по-умолчанию `2000`.
* `isFixed` - Сделать уведомление фиксированым.
* `vertical` - Вертикальная позиция уведомления при `isFixed`.  Доступные значение `bottom`, `top`. Значение по-умолчанию `bottom`.
* `horizontal` - Горизонтальная позиция уведомления при `isFixed`.  Доступные значение `right`, `left` Значение по-умолчанию `right`.
* `hideIcon` - Скрыть иконку уведомления.

## Слоты
  У компонента есть слот используемы по умолчанию, в нем может быть указан текст увдомления.