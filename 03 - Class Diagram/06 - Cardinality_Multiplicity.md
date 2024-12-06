:::mermaid

classDiagram

%% 1 - Only 1
%% 0..1 Zero or One
%% 1.* One or more
%% * - Many
%% n - n
%% 0..n - zero to n
%% 1..n - one to n

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
    Mammal "0" o-- "*" Dog : aggregation
    Mammal "1" *-- "*" Dolphin : Composition
    Reptile "1" *-- "n" Platypus: Composition

    note "general note here"
    note for Mammal "general note here \n another line"