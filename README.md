# Budgy-Your-Budget-Buddy-Major-Project
Budgy, Budgeting App; Desktop &amp; Mobile.


## Class Diagram

```mermaid
classDiagram
    class Transaction
    class Budget
    class AlertSystem
    class BudgetManager
    class FileStorage

    BudgetManager "1" *-- "0..*" Transaction : manages
    BudgetManager "1" *-- "0..*" Budget : tracks
    BudgetManager "1" *-- "1" AlertSystem : uses
    BudgetManager ..> FileStorage : saves and loads
    AlertSystem ..> Budget : checks spending limits
```
