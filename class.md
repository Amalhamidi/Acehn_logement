classDiagram
    Logement <|-- Social
    Logement <|-- Privé
    Logement <|-- HLM
    Logement : +String Type
    Logement : +int Disponibilité
    Logement : +String Qualité
    Logement : +String Surface
    Logement : +String Coût
    Logement : +String ConditionsAccès
    Logement : +String Demande
  
    class Social {
        +Type: "social"
        +Disponibilité: 2
        +Qualité: "neuf"
        +Surface: "20m²"
        +Coût: "500£"
        +ConditionsAccès: "aides"
        +Demande: "excès"
    }

    class Privé {
        +Type: "privé"
        +Disponibilité: 5
        +Qualité: "ancien"
        +Surface: "50m²"
        +Coût: "1100£"
        +ConditionsAccès: "revenus"
        +Demande: "équilibré"
    }

    class HLM {
        +Type: "HLM"
        +Disponibilité: 1
        +Qualité: "rénové"
        +Surface: "35m²"
        +Coût: "850£"
        +ConditionsAccès: "social ou HLM"
        +Demande: "excès"
    }
