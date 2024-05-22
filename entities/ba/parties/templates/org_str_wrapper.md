{{#count}}
# Структура Участников

![](@entity/seaf.ba.parties/org_str_graph?domain={{domain}})
{{/count}}

{{^count}}
:warning: Участники не опредены

---
Создайте минимальное определение хотя бы одного Участника
```yaml
seaf.ba.parties: # Раздел манифеста для объявления Участников
    party_id:
        title: Наименование Участника
```
{{/count}}