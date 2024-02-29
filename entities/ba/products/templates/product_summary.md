###### Сводная информация по Продукту :id: {{id}}

---
# {{body.title}} 

{{body.description}}

{{#wrappers_num}}###### Потребляется как часть продуктов:{{/wrappers_num}}
{{#wrappers}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.products/product_summary?id={{id}}) {{#body.description}}-- {{.}}{{/body.description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.products/product_summary?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{alias_id}}
{{/alias_body}}
{{/alias}}
{{/wrappers}}

{{#processes_num}}###### Поддерживается процессами:{{/processes_num}}
{{#processes}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.processes/process_summary?id={{id}}) {{#body.description}}-- {{.}}{{/body.description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.processes/process_summary?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{alias_id}}
{{/alias_body}}
{{/alias}}
{{/processes}}

{{#wraps_num}}###### Имеет в составе выделенные подпродукты:{{/wraps_num}}
{{#wraps}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.products/product_summary?id={{id}}) {{#body.description}}-- {{.}}{{/body.description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.products/product_summary?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{alias_id}}
{{/alias_body}}
{{/alias}}
{{/wraps}}

### Владелец
{{#owner}}
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

{{#consumers_num}}#### Потребители:{{/consumers_num}}
{{#consumers}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.parties/party_summary?domain={{id}}) {{#body.description}}-- {{.}}{{/body.description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.parties/party_summary?domain={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{alias_id}}
{{/alias_body}}
{{/alias}}
{{/consumers}}

