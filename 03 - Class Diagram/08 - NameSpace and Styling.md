:::mermaid
classDiagram
    Animal <|-- Dog
    Animal <|-- Bird

    Dog <|-- GermanShepherd
    Dog <|-- Poodle

    Bird <|-- Parrot
    Bird <|-- Sparrow

    class Animal {
        <<abstract>> +name: string
        +makeSound() void
    }

    namespace DogFamily {

        class Dog{
            +breed: string
            +bark() void
        }

        class GermanShepherd{
            +loyaltylevel number
            +guard() void
        }

        class Poodle {
            +groomingNeeds string
            +fetch() void
        }
    }

    namespace BirdFamily{
        class Bird {
            +species string
            +fly() void
        }

        class Parrot{
            +color string
            +talk() void
        }

        class Sparrow{
            +nwstBuildingSkill string
            +chirp() void
        }

    }
