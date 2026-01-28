## Alternative Flows

### UC-05 Alternative Flows

**AF-1: Invalid Image Format**

1. User uploads non-JPG/PNG file
2. System displays error "Invalid format. Please upload JPG or PNG"
3. User re-uploads correct format
4. Continue from main flow step 2

**AF-2: Image Too Large**

1. User uploads image > 5MB
2. System displays error "Image too large. Maximum 5MB"
3. User uploads smaller image
4. Continue from main flow step 2

**AF-3: No Disease Detected**

1. YOLO returns confidence < 50%
2. System displays "Plant appears healthy!"
3. Use case ends

**AF-4: Network Error**

1. API call times out
2. System displays "Connection error. Please retry"
3. User clicks retry button
4. Continue from main flow step 3
