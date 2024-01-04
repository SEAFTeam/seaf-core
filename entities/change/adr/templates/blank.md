# {{title}}
id: **{{id}}**

# Проблема
{{issue}}

# Решение
{{decision}}.

# Предпосылки
{{#context}}
___
* Область: **{{area}}**
* Эффект: **{{vector}}**

{{content}} 
{{/context}}

# Какие требования учтены
{{#requirements}}
* [{{title}}]({{link}})
{{/requirements}}

# Ожидаемые последствия от решения
{{#consequences}}
___
* Область: **{{area}}**
* Эффект: **{{vector}}**

{{content}}
{{/consequences}}

# От какого решения зависит
{{#dependencies}}
* [{{title}}]({{link}})
{{/dependencies}}

# Какие решения зависят от этого
{{#blocked}}
* [{{title}}]({{link}})
{{/blocked}}

# Кто принимал решение
{{#deciders}}
* {{.}}
{{/deciders}}

