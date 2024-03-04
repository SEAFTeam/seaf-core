###### Сводная информация по Процессу :id: {{id}}

---
# Процесс: "{{body.title}}" 

{{body.description}}

{{#owner_num}}
{{#owner}}
### Владелец
["{{body.title}}" :id: {{id}}](/entities/seaf.ba.parties/party_summary?domain={{id}}) {{#body.description}}-- {{.}}{{/body.description}}
{{#alias}}
{{#alias_body}}
* ["{{alias.body.title}}" :id: {{alias.id}}](/entities/seaf.ba.parties/party_summary?domain={{alias.id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
* :warning: Справочное значение отсутствует :id: {{id}}
{{/alias_body}}
{{/alias}}
{{/owner}}
{{/owner_num}}
{{^owner_num}}
:warning: Владелец не указан
{{/owner_num}}


{{#products_num}}#### Поддерживает Продукты:{{/products_num}}
{{#products}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.products/product_summary?id={{id}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.products/product_summary?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/alias_body}}
{{/alias}}
{{/products}}

{{#requirements_num}}#### Требования:{{/requirements_num}}
{{#requirements}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.change.requirements/blank?seaf-req-id={{id}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.change.requirements/blank?seaf-req-id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/alias_body}}
{{/alias}}
{{/requirements}}


{{#biz_obj_num}}###### Бизнес-объекты{{/biz_obj_num}}
{{#biz_obj}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ia.business_objects/card?id={{id}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ia.business_objects/card?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/alias_body}}
{{/alias}}
{{/biz_obj}}


{{#systems_num}}#### Автоматизация:{{/systems_num}}
{{#systems}}
* ["{{title}}" :id: {{domain}}](/entities/component/summary?component={{id}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#body_com}}
    * ["{{body_com.title}}" :id: {{id}}](/entities/component/summary?component={{id}}) {{#body_com.description}}-- {{.}}{{/body_com.description}}
{{/body_com}} 
{{^body_com}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/body_com}}
{{/alias}}
{{/systems}}


