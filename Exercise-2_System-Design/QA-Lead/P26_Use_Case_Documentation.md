## Use Case Documentation

### UC-05: View Disease Diagnosis

**Use Case ID:** UC-05  
**Use Case Name:** View Disease Diagnosis  
**Actor:** Gardener

**Preconditions:**

1. User is logged in
2. Image has been uploaded successfully
3. Image format is valid (JPG/PNG, <5MB)

**Main Flow:**

1. System receives uploaded image
2. System sends image to API Gateway
3. API Gateway forwards to YOLO Model
4. YOLO Model processes image
5. YOLO Model returns disease name and confidence score
6. System displays diagnosis result to user

**Alternative Flows:**

- **AF-1:** Image unclear
  - System requests user to re-upload clearer image

- **AF-2:** No disease detected
  - System displays "Plant appears healthy" message

**Postconditions:**

- Diagnosis result displayed to user
- Report saved in database
