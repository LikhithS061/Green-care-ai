## Class Relationships

### Association

- User **1** --- **\*** SoilProfile (One user has many soil profiles)
- User **1** --- **\*** Recommendation (One user receives many recommendations)
- User **1** --- **\*** DiagnosisReport (One user has many diagnosis reports)

### Dependency

- Recommendation depends on SoilProfile (uses soil data)
- DiagnosisReport depends on Disease (references diseases)

### Aggregation

- DiagnosisReport **◇** --- **\*** Disease (Report contains diseases)

### Association

- Recommendation **\*** --- **\*** Plant (Many-to-many through confidence scores)
