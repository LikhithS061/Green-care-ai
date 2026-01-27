# Class Diagram

## Greencare AI

### Classes Identified

1. **User** - System user/gardener
2. **SoilProfile** - Environmental data
3. **Plant** - Plant information
4. **Disease** - Disease information
5. **Recommendation** - Plant suggestions
6. **DiagnosisReport** - Disease detection results

---

## Class Diagram

```mermaid
classDiagram
    class User {
        -String userId
        -String name
        -String email
        -String password
        +register()
        +login()
        +updateProfile()
    }

    class SoilProfile {
        -String profileId
        -Float nitrogen
        -Float phosphorus
        -Float potassium
        -Float pH
        -Float temperature
        +updateData()
        +validate()
    }

    class Plant {
        -String plantId
        -String plantName
        -String scientificName
        -String careInstructions
        -String imageUrl
        +getDetails()
        +getCarePlan()
    }

    class Disease {
        -String diseaseId
        -String diseaseName
        -String symptoms
        -String remedy
        +getRemedy()
    }

    class Recommendation {
        -String recommendationId
        -Date generatedAt
        -Float confidenceScore
        +generateRecommendation()
        +getTopPlants()
    }

    class DiagnosisReport {
        -String reportId
        -String imageUrl
        -Date diagnosedAt
        -Float confidence
        +generateReport()
        +getRemedySuggestions()
    }

    User "1" --> "*" SoilProfile : has
    User "1" --> "*" Recommendation : receives
    User "1" --> "*" DiagnosisReport : receives
    SoilProfile "1" --> "1" Recommendation : generates
    Recommendation "*" --> "*" Plant : suggests
    DiagnosisReport "*" o-- "*" Disease : contains
```

---

## Class Relationships

| Relationship                 | Description                                         |
| ---------------------------- | --------------------------------------------------- |
| User → SoilProfile           | One user can have multiple soil profiles (1:\*)     |
| User → Recommendation        | One user receives multiple recommendations (1:\*)   |
| SoilProfile → Recommendation | Soil profile generates recommendations (dependency) |
| Recommendation → Plant       | Recommendation suggests multiple plants (_:_)       |
| DiagnosisReport ◇ Disease    | Diagnosis report aggregates diseases (aggregation)  |
