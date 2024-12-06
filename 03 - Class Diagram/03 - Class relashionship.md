:::mermaid

%% + public
%% - private
%% # protected
%% ~ internal
%% * static

%% <|-- Inheritance
%% *-- Composition
%% o-- Aggregation
%% --> Association
%% -- Link
%% ..> Dependency
%% ..|> Realization
%% .. Link ( Dashed )

classDiagram
    class BankAccount{
        -String ouner,
        -BigDecimal balance,
        +withdrawl(amount) bool,
        -deposit(amount) int

        method1()*
        method2() String$
    }
    class Person
        Person: -String name
        Person: -Integer age
        Person: #List~string~ siblings
        Person: +walk(Integer distance)
        Person: +talk() List~string~

    BankAccount --|> Person