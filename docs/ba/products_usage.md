###### :green_book: products.md

---

# Продукты

Продукт -- это механизм, с помощью которого Участники могут осуществить обмен Ресурсами.

```yaml
seaf.ba.parties:                        

    party_a:
        title: Участник А                       # Участник А
        has_interest:
            - party_a.party_b.channel           # является пользователем канала

    party_a.deps.sales:
        title: Департамент продаж
        is_part_of: party_a

    party_a.clients:                             # Клиенты Участника А
        title: Клиенты
        has_interest:                            # могут воспользоваться продуктами:   
            - party_a.subscribtion                  # "Оформить подписку"
            - party_a.content_access                # и "Просмотреть контент"
           
    party_a.party_b:
        title: party_b                 

seaf.ba.products:                       

    party_a.content_access:
        title: Просмотр Контента
        owner: party_a                  
        used_in: 
            - party_a.party_b.channel             # через
    
    party_a.subscribtion:
        title: Оформление подписки на ФП
        owner: party_a.deps.sales               
        used_in: 
            - party_a.party_b.channel
    
    party_a.party_b.channel:                       # Канал,      
        title: Канал
        owner: party_a.party_b                     # предоставляемый Участником В

```