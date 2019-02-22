# ui-button
Компонент кнопок.
## Параметры

Компонент кнопок принимать следующие параметры:
 - href: Ссылка
 - theme: Тема кнопки. Используется как название класса
 - type: Тип кнопки `button, submit`
 - variant: Вариант стилевого оформления `primary, secondary`. По-умолчанию `primary`
 - size: Размер (фактический) кнопки. Значения `xs | s | m | l | xl`. По-умолчанию `m`
 - icon: Иконка для кнопки из списка иконок (список иконок находится в файле темы `icons.js`)
 ## Темизация
 * ### `layout`
 * `default` - значение по-умолачанию
 * `collapse-reverse` - Изменяет направление `flex` внутреннего контейнера.
 * ### `color-sheme`
 * `default` - Фон кнопки цвета ссылки, текст контрастный от цвета ссылки.
 * `is-text` - Фон кнопки прозрачный, текст цвета текста.
 * `transparent` - Фон кнопки прозрачный, текст цвета ссылки.
 * ### `themes`
 * `bold` - Жирный шрифт внутри кнопки.
 * `border` - Граница вокруг кнопки.
 * `fluid` - `min-height`, `min-widht` равны `100%`.
 * `no-padding` - Убирает отступы у кнопки.
 * `padding` - Отступ сверху и снизу `1rem`.
 * `size_s`, `size_m`, `size_l`, `size_xl` - Устанавливает ширину и высоту кнопки отступами заданными переменными `var(--button-size-s)`, `var(--button-size-m)`, `var(--button-size-l)`, `var(--button-size-xl)`.
 * `text-left` - Текст кнопки слева.
 * `uppercase` - Преобразует текст кнопки в верхний регистр.

 ### Ниже представлен вариант исполнения кнопки:
```
  <ui-button
    type="submit"
    icon="filter.section.submit"
    :theme="secondary"
    :href="window.location"
    :icon="currentIcon"
    >
    <slot></slot>
  </ui-button>

```
    <ui-form-item
      name="author"
      label="Фамилия"
      value="">
    </ui-form-item>

    <ui-form-item
      name="author"
      label="Имя"
      value="">
```
После отправки придет письмо с `Фамилия Имя: Иванов Иван`
Массивы значений будут перечисляться через запятую.
Соответственно все поля в поле `content` тоже будут обьединяться, но каждое поле будет начинаться с новой строки.

Пройдемся по свойствам формы:
 - `send-method`- назначение формы. Может быть 3 варианта: `message`,`review`,`comment`. По-умолчанию `message`.
 - `product-id` - *(опционально)* указывается при отправке отзыва к товару. Если не добавлен, ищет id товара на странице которого находимся.
 - `from`  - *(обязательно)* указывается при отправке обратного сообщения. Email отправителя.
 - `show-recaptcha` - показ рекапчи для проверки.
 - `submit-caption` - надпись для отправления кнопки. По-умолчанию "Отправить"

Свойства полей формы:
 - `type` - тип поля. По-умолчанию это однострочное поле. Может принимать значения `input`,`textarea`,`select`,`checkbox`,`checkbox-group`,`rating`.
 -  `label` - "метка" поля. Лейбл он и в Африке.
 -  `name` - имя поля. Обязательно
 -  `:rules` - правила заполнения поля. Принимает в себя обьект пока с одним полем `required`со значением `true\false`
 -  `value`- значение по-умолчанию

### Свойства для конкретных полей
 - `:options` - массив значений для `radio-group`, `checkbox-group`, `select`. Пример: ``` :options="[{ label: 'chose', value: '1' }, { label: 'wat', value: '2' }, { label: 'nom', value: 'wooop' }]" ```