:::mermaid

---
title: Animal Relationship
---

classDiagram

    direction LR

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

    Animal <|-- Mammal : Inheritance
    Animal <|-- Reptile: Inheritance
    Mammal o-- Dog : aggregation
    Mammal *-- Dolphin : Composition
    Reptile *-- Platypus: Composition

    note "general note here"
    note for Mammal "general note here \n another line"