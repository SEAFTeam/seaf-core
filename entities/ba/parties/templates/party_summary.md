###### :id: {{id}}

---
# {{body.title}} 

{{body.description}}

#### Контрагенты:
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


#### Вышестоящая структура:
{{#managedBy}}
* ["{{title}}" :id: {{domain}}](/entities/seaf.ba.parties/party_summary?domain={{domain}}) {{#description}}-- {{.}}{{/description}}
{{/managedBy}}

#### Внутренняя структура:
{{#members}}
* ["{{title}}" :id: {{domain}}](/entities/seaf.ba.parties/party_summary?domain={{domain}}) {{#description}}-- {{.}}{{/description}}
{{/members}}

