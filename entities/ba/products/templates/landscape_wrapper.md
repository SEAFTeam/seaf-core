{{#count}}
# Продуктовый ландшафт

![](@entity/seaf.ba.products/landscape_graph?domain={{domain}})
{{/count}}
{{^count}}
:warning: Продукты не опредены

---
Создайте минимальное определение хотя бы одного Продукта
```yaml
seaf.ba.products: # Раздел манифеста для объявления Продуктов
    product_id:
        title: Наименование Продукта
```
{{/count}}