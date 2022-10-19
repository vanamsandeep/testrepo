
$ sudo apt install default-jre
testing plant uml
 testing only

```plantuml
@startuml
skinparam linetype ortho

rectangle ESP #lightblue
rectangle Roxie #lightblue {
    rectangle "Custom ECL" as ECL #CornflowerBlue {
        rectangle "KEL Generated Code" #AliceBlue
    }
}
rectangle {
    rectangle worker as worker1 #lightblue {
        database index as index1 #CornflowerBlue
    } 
    rectangle worker as worker2 #lightblue{
        database index as index2 #CornflowerBlue
    } 
    rectangle worker as worker3 #lightblue{
        database index as index3 #CornflowerBlue
    }     
}

ESP <--> Roxie
ECL -down-> worker1
ECL -down-> worker2
ECL -down-> worker3
@enduml
```
test


@startuml
class Car

Driver - Car : drives >
Car *- Wheel : have 4 >
Car -- Person : < owns

@enduml

