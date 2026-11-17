# 4. Детальное описание функции покупки товара

В данном разделе описано, как технически реализуется функция отметки товара как «купленного» (пункт 5 задания).
## UML Диаграмма классов (структура данных)

```mermaid
classDiagram
    class ShoppingList {
        +UUID id
        +String title
        +Date created_at
    }
    class Item {
        +UUID id
        +UUID list_id
        +String name
        +Boolean is_bought
        +Date updated_at
    }
    ShoppingList "1" *-- "many" Item
```
