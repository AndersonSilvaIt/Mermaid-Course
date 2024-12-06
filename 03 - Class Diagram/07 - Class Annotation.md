:::mermaid

classDiagram

    Animal <|-- Mammal 
    Animal <|-- Reptile
    Mammal <|-- Dog
    Mammal <|-- Cat

    class Animal {
        + name: string
        + age: int
        + makeSound()
    }

    class Mammal {
        <<Abstract>>
        - furColor: string
        + giveBirth() void
    }

    class Reptile {
    <<interface>>
        - scaleType: string
        + layEggs() void
    }

    class Reptile
        Reptile: -scaleColor string
        Reptile: +layEggs() void

    class Dog {
        + breed: string
        + bark() void
    }

    class Cat {
        + eyeColor: string
        + meow() void
    }

