:::mermaid

---
title: Animal Relationship
---

classDiagram
    Animal <|-- Mammal
    Animal <|-- Reptile
    Mammal o-- Dog
    Mammal *-- Dolphin
    Reptile *-- Platypus

    class Animal {
        - age: int
        + makesound()
    }

    class Mammal {
        # furColor: string
        - giveBirth() void
    }

    class Reptile {
        # scaleType: string
        + layEggs() void
    }

    class Dog {
        # breed: string
        + bark() void
    }

    class Dolphin {
        + swim() void
    }

    class Platypus {
        # poisonous: boolean,
        swim() void
    }
    