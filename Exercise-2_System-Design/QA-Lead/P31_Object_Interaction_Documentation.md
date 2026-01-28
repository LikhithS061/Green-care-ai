## Object Interaction Documentation

### Key Object Interactions

| Sender      | Message          | Receiver    | Response              |
| ----------- | ---------------- | ----------- | --------------------- |
| User        | uploadImage()    | Frontend    | Success/Error         |
| Frontend    | validateFormat() | Self        | Boolean               |
| Frontend    | POST /diagnose   | API Gateway | JSON                  |
| API Gateway | predict()        | YOLO Model  | {disease, confidence} |
| API Gateway | saveReport()     | Database    | Confirmation          |
| Database    | getRemedy()      | API Gateway | Remedy details        |

### Interaction Notes

1. All API calls are asynchronous
2. Frontend shows loading state during processing
3. Error handling at each interaction point
