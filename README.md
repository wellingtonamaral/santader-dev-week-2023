# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Wek

##  Diagrama de Classes

```mermaid
classDiagram
    class User {
        -name: String
        -account: Account
        -features: List<Feature>
        -card: Card
        -news: List<News>
    }

    class Account {
        -accountNumber: String
        -accountAgency: String
        -accountBalance: Double
        -accountLimit: Double
    }

    class Feature {
        -icon: String
        -description: String
    }

    class Card {
        -cardNumber: String
        -cardLimit: Double
    }

    class News {
        -icon: String
        -description: String
    }

    User "1" *--> "1" Account
    User "1 " *--> "N" Feature
    User "1" *--> "1" Card
    User "1" *--> "N" News
```
