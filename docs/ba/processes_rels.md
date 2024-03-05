###### :green_book: proсesses_rels.md

---

# Процессы

```yaml
seaf.ba.parties:                        

    party_a:
        title: Участник А                      

    party_a.deps.content_mng:
        title: Департамент управления контентом
        is_part_of: party_a
    
    party_a.deps.law:
        title:  Юридический департамент
        is_part_of: party_a

seaf.ba.products:                       

    party_a.content_access:
        title: Просмотр Контента
        owner: party_a.deps.content_mng               

seaf.ba.processes:                              # Процессы

    party_a.process_5_7:                        # Композитный процесс (содержит сценарий 5.7.1->5.7.2)
        title: Процесс 5.7
        owner: party_a

    party_a.process_5_7_1:
        title: Процесс 5.7.1
        is_part_of: party_a.process_5_7
        owner: party_a.deps.law
        next_processes:                         # Образует последовательность
            - party_a.process_5_7_2             # с Процессом 5.7.2

    party_a.process_5_7_2:
        title: Процесс 5.7.2
        is_part_of: party_a.process_5_7
        products:                               # Операционализирует  
            - party_a.content_access            # Продукт "Просмотр контента"
        owner: party_a.deps.content_mng               

```