## SRS Overall Description

### 2.1 Product Perspective

Greencare AI is a standalone web application with a modular microservice
architecture consisting of:

- **Frontend**: React.js responsive web interface
- **Backend**: Flask-based REST API gateway
- **AI Layer**: Transformer model for recommendations, YOLOv8 for disease detection
- **Database**: MongoDB for user and plant data storage
- **Storage**: AWS S3 for image uploads

### 2.2 User Characteristics

Target users are non-technical home gardeners with:

- Basic smartphone/web literacy
- Interest in gardening and plant care
- Desire for personalized, data-driven advice

### 2.3 Constraints

| Constraint | Description                                                 |
| ---------- | ----------------------------------------------------------- |
| Technical  | Must run on standard web browsers (Chrome, Firefox, Safari) |
| Resource   | Image upload limit: 5MB maximum                             |
| Network    | Requires active internet connection for AI inference        |
| Platform   | Web-first approach; mobile via PWA                          |
