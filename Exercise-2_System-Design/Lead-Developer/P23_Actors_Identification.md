## Actors Identification

### Primary Actors

| Actor       | Description                   | Goals                                  |
| ----------- | ----------------------------- | -------------------------------------- |
| 🧑‍🌾 Gardener | End-user seeking plant advice | Get recommendations, diagnose diseases |
| 👨‍💼 Admin    | System administrator          | Manage plant database, monitor system  |

### Secondary Actors

| Actor          | Description                | Interaction                           |
| -------------- | -------------------------- | ------------------------------------- |
| 🤖 AI Engine   | Internal system processing | Process recommendations and diagnosis |
| 🌐 Weather API | External service           | Provide climate data                  |

### Actor Relationships

- Gardener is the primary actor for all user-facing use cases
- Admin manages backend configuration
- AI Engine is triggered by user actions
