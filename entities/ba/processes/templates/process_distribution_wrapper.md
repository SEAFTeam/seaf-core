{{#count}}
# Распределение Процессов по продуктам

![](@entity/seaf.ba.processes/process_distribution_graph?domain={{domain}})
{{/count}}
{{^count}}
:warning: Процессы не опредены

---
Создайте минимальное определение хотя бы одного Процесса
```yaml
seaf.ba.processes: # Раздел манифеста для объявления Процессов
    process_id:
        title: Наименование Процесса
```
{{/count}}