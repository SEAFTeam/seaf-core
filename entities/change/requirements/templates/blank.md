# {{title}}
* ID: **{{id}}**
* Тип требования: **{{type}}**

## Описание
{{&description}}

## Обеспечивается
{{#functionality}}
* [{{title}}](/entities/aspects/blank?dh-aspect-id={{id}})
{{/functionality}}

## Контроль выполнения требований
| Критерий | Условие проверки  |
|----------|:------------------|
{{#verifications}}
| {{title}} | {{condition}} |
{{/verifications}}

