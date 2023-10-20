# DIO_Santander_Java_APi_RESTful_Java
Santander Bootcamp 2023 - Backend | Java RESTful API criada para a Santander Java Week.

# Nota Importante: Este Projeto é Estritamente Educacional

Caros visitantes,
Gostaríamos de enfatizar que este projeto tem exclusivamente fins educacionais. Sua concepção e implementação destinam-se à aprendizagem e desenvolvimento de habilidades técnicas.
Agradeço pela compreensão e respeito à natureza educacional deste projeto.

Atenciosamente, Douglas Moro.

## Diagrama de classes
```mermaid
classDiagram
  class User {
    -name: String
    -account: Account
    -features: Feature[]
    -card: Card
    -news: News[]
  }

  class Account {
    -number: String
    -agency: String
    -balance: Number
    -limit: Number
  }

  class Feature {
    -icon: String
    -description: String
  }

  class Card {
    -number: String
    -limit: Number
  }

  class News {
    -icon: String
    -description: String
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News
```
