## Workflow Documentation

### Plant Recommendation Workflow

| Phase    | Activity        | Actor  | System Response    |
| -------- | --------------- | ------ | ------------------ |
| Auth     | Check Login     | System | Redirect if needed |
| Input    | Enter Soil Data | User   | Show form          |
| Validate | Check Ranges    | System | Error or proceed   |
| Process  | Run AI Model    | System | Generate scores    |
| Output   | Display Results | System | Show top 3 plants  |

### Data Validation Rules

| Field          | Valid Range | Unit  |
| -------------- | ----------- | ----- |
| Nitrogen (N)   | 0 - 140     | mg/kg |
| Phosphorus (P) | 5 - 145     | mg/kg |
| Potassium (K)  | 5 - 205     | mg/kg |
| pH             | 3.5 - 9.5   | -     |
| Temperature    | 10 - 45     | °C    |
