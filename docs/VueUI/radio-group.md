# Компонент радио-кнопки `ui-radio-group`

Используется когда нужно выбрать одно значение из нескольких. Как правило используется в формах. При создании по-умолчанию выбран первый пункт.

### Пример использования

```
<ui-radio-group
  name="content"
  :options="[{ label: 'chose', value: '1' }, { label: 'wat', value: '2' }, { label: 'nom', value: 'wooop' }]"
/>
```

### Параметры компонента
 - `name` - уникальное системное имя для компонента
 - `options` - массив обьектов с параметрами радио-кнопок. Принимают `label` и `value`.