###### Сводная информация по Участнику :id: {{id}}

---
# {{body.title}} 

{{body.description}}

{{#products_num}}#### Продукты{{/products_num}}
{{#owner_num}}###### предоставляемые{{/owner_num}}
{{#owner}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.products/product_summary?id={{id}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.products/product_summary?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/alias_body}}
{{/alias}}
{{/owner}}

{{#processes_owned_num}}#### Владение процессами{{/processes_owned_num}}
{{#processes_owned}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.processes/process_summary?id={{id}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.processes/process_summary?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/alias_body}}
{{/alias}}
{{/processes_owned}}


{{#consumes_num}}###### потребляемые{{/consumes_num}}
{{#consumes}}
* ["{{body.title}}" :id: {{id}}](/entities/seaf.ba.products/product_summary?id={{id}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#alias_body}}
    * ["{{alias_body.title}}" :id: {{alias_id}}](/entities/seaf.ba.products/product_summary?id={{alias_id}}) {{#alias_body.description}}-- {{.}}{{/alias_body.description}}
{{/alias_body}} 
{{^alias_body}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/alias_body}}
{{/alias}}
{{/consumes}}


{{#counterparts_num}}#### Контрагенты:{{/counterparts_num}}
{{#counterparts}}
* ["{{title}}" :id: {{domain}}](/entities/seaf.ba.parties/party_summary?domain={{domain}}) {{#description}}-- {{.}}{{/description}}
{{#alias}}
{{#body_com}}
    * ["{{body_com.title}}" :id: {{id}}](/entities/seaf.ba.parties/party_summary?domain={{id}}) {{#body_com.description}}-- {{.}}{{/body_com.description}}
{{/body_com}} 
{{^body_com}}
    * :warning: Справочное значение отсутствует :id: {{id}}
{{/body_com}}
{{/alias}}
{{/counterparts}}


{{#managedBy_num}}#### Вышестоящая структура:{{/managedBy_num}}
{{#managedBy}}
* ["{{title}}" :id: {{domain}}](/entities/seaf.ba.parties/party_summary?domain={{domain}}) {{#description}}-- {{.}}{{/description}}
{{/managedBy}}

{{#members_num}}#### Внутренняя структура:{{/members_num}}
{{#members}}
* ["{{title}}" :id: {{domain}}](/entities/seaf.ba.parties/party_summary?domain={{domain}}) {{#description}}-- {{.}}{{/description}}
{{/members}}

