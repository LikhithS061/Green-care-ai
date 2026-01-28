## Class Attributes and Methods

### User Class

**Attributes:**

- userId: String
- name: String
- email: String
- password: String (hashed)

**Methods:**

- register()
- login()
- updateProfile()

### SoilProfile Class

**Attributes:**

- profileId: String
- nitrogen: Float
- phosphorus: Float
- potassium: Float
- pH: Float
- temperature: Float

**Methods:**

- updateData()
- validate()

### Plant Class

**Attributes:**

- plantId: String
- plantName: String
- scientificName: String
- careInstructions: String
- imageUrl: String

**Methods:**

- getDetails()
- getCarePlan()
