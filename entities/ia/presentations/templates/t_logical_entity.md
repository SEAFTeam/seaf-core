# Логическая сущность
## Системное имя: {{id}}

[//]: # (отображаем агрегаты как ссылки только для описанных в `$$.seaf.ia.aggregat`, для неописанных - текст)
[//]: # (отображаем Мастер-систему как ссылку только для АС, описанных в `$$.components`, для неописанных - текст)

Мета атрибуты               | Значения
:------------               | :------------
Код                         | {{code}}
Наименование                | {{title}}
Агрегат                     | {{#aggregat_link}}[{{aggregat_name}}]({{aggregat_link}}){{/aggregat_link}}{{^aggregat_link}}{{aggregat_name}}{{/aggregat_link}}
Описание                    | {{description}}
Категория                   | {{category}}
Наличие персональных данных | {{pdn_flag}}
Наличие критических данных  | {{cde_flag}}
Мастер-система              | {{#master_system_link}}[{{master_system}}]({{master_system_link}}){{/master_system_link}}{{^master_system_link}}{{master_system}}{{/master_system_link}}
Комментарии                 | {{comments}}

## Логические атрибуты
![Логические аттрибуты](@entity/seaf.ia.logical_attributes/registry_by_data_objects?id={{id}})

## Логические связи
![Связи](@entity/seaf.ia.logical_links/registry_by_data_objects?id={{id}})

## Связанные бизнес-термины
![Бизнес-термины](@entity/seaf.ia.business_objects/registry_by_data_objects?id={{id}})

## Физические таблицы
![Входящие связи](@entity/seaf.ia.physical_tables/registry_by_data_objects?id={{id}})
