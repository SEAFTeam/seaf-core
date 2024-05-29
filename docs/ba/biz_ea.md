###### :green_book: biz_ea.md

---

# Отношения с другими слоями корпоративной архитектуры (в объеме SEAF-CORE)

###### Процесс поддерживается прикладными сервисами (`components`)

```yaml
seaf.ba.processes:                        

    party_a.process_5_7_1:
        title: Процесс 5.7.1   
        supported:
            - party_a.some_it_component          

    components:
        party_a.some_it_component:
            title: ИТ компонент
            type: service
```

###### Процесс использует бизнес-объекты (`seaf.ia.business_objects`)

```yaml
seaf.ba.processes:                        

    party_a.process_5_7_1:
        title: Процесс 5.7.1                       

    seaf.ba.business_objects:
        party_a.some_biz_obj:
            title: Бизнес-объект(данных)
            processes:
                - party_a.process_5_7_1
```

###### Процесс предъявляет требования (`seaf.change.requirements`)

```yaml
seaf.ba.processes:                        

    party_a.process_5_7_1:
        title: Процесс 5.7.1    
        requirements:
            - party_a.req_9_43                   

    seaf.change.requirements:
        party_a.req_9_43:
            title: Требование 9ю43
```
