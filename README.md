# BHT theme für PlantUML

UML-Diagramme in den Farben der 
[Berliner Hochschule für Technik (BHT)](https://www.bht-berlin.de/) können 
in [PlantUML](https://plantuml.com/de/) mit diesem Theme erstellt werden. 
Es ist eine Abwandlung des Themes [Cerulean](https://github.com/bschwarz/puml-themes). Ich verwende es, um ansprechende Diagramme für meine 
Masterarbeit zu erzeugen, welche zu den Templates der BHT passen.
Disclaimer: Ich kann nicht garantieren, dass alle Diagrammtypen und PlantUML-Features unterstützt werden. 

## Beispiel

Das Beispiel kann mit dem [PlantUML Web Server](https://www.plantuml.com/plantuml/uml/FO_1IWCn48RlUOhnrXxQtDk3hOWej2XO7o3T_RU9RYRBP89GyTtTpLBd49ZyCz_7xB8wqH9xSwSU4NJsIfsaI5vro1jhnNslBq5zEPSCQH8hMDTDYhRhamJ7ZF8LfF5W-_1yMWszumcugZmhwBBrS6ssqGMsnfYgDCFu10s9wHYKtgQjZ-E1VWoD5JfQx9bQ28tC-oMf1zFYqorhl9ac0zFaUt9o1c_hFoS5zUYqTbETwb6l0vZUKv46z1yLLWWTNqwhGxY2hpK0jvKoQ_QS1y5qMWjw3EuYBaRCBlGPj604Njw6MmZohDpUQA4ploPh6inkx4hi_m00) ausprobiert werden. Das Diagramm wird durch den unten stehenden Code generiert, das Theme wird in der ersten Zeile über eine URL geladen.

![](beispiel.png)

```
!theme bht from https://raw.githubusercontent.com/florianneukirchen/BHT-plantuml-theme/refs/heads/main/
@startuml

start
partition Mit PlantUML {
    if (An der BHT?) then (ja)
    :UML in BHT-Farben;
    note left
        Theme Open Source 
        unter MIT-Lizenz
    end note
    :Ansprechende Diagramme;
    else (nein)
    :Anderes Theme;
    endif
}
stop

@enduml
```

