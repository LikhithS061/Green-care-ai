# Project Charter: Greencare AI

## 1. Project Selection & Team Formation

**Project Title:** Greencare AI: Personalized Plant Recommendation and Gardening Assistant

**Team Members:**
| Name | Roll Number |
|------|-------------|
| Bathini Indra Sena Reddy | 2023BCSE07AED076 |
| Dharshan G | 2023BCSE07AED071 |
| Likhith S | 2023BCSE07AED061 |
| Bindela Sai Vamshidar Reddy | 2023BCSE07AED049 |

---

## 2. Team Agreement

| Aspect              | Agreement                                                    |
| ------------------- | ------------------------------------------------------------ |
| **Meeting Norms**   | Weekly sync on Fridays at 4 PM                               |
| **Decision Making** | Majority vote; Mentor has final say on technical disputes    |
| **Communication**   | WhatsApp for urgent updates; GitHub Issues for task tracking |
| **Version Control** | Feature branch workflow; no direct commits to main           |

---

## 3. Problem Statement

**Problem:** Novice gardeners often fail because they choose plants ill-suited to their environment (soil/climate) and cannot identify plant diseases in time.

**Solution:** An AI-powered application providing personalized plant recommendations based on environmental parameters (NPK, pH, location) and real-time disease diagnosis via image recognition.

**Target Users:** Home gardeners, hobbyists, and urban farmers.

**Value Proposition:** Reduces plant mortality rates and simplifies the gardening learning curve.

---

## 4. Stakeholder Analysis

### Primary Stakeholders

- **Home Gardeners (Users)** - End users seeking plant advice
- **Development Team** - Project executors
- **Project Mentor** - Academic supervisor

### Secondary Stakeholders

- **Alliance University** - Academic institution
- **API Providers** - OpenWeatherMap
- **Hosting Provider** - AWS/Render

---

## 5. Stakeholder Interests

| Stakeholder | Interest                                    | Influence Level  |
| ----------- | ------------------------------------------- | ---------------- |
| Users       | Want accurate, easy-to-understand advice    | High (Adoption)  |
| Mentor      | Wants technical depth and timely completion | High (Grading)   |
| Developers  | Want to learn MLOps and React/Flask         | High (Execution) |

---

## 6. Scope Definition

### In-Scope

- User Profiling (Soil type, location inputs)
- Plant Recommendation Engine (Transformer-based)
- Plant Disease Diagnosis (YOLOv8-based)
- Web Interface (React.js) and Backend API (Flask)
- Basic Explainable AI (SHAP analysis)

### Out-of-Scope

- E-commerce integration (selling plants/fertilizers)
- IoT Hardware sensor integration (manual input only for now)
- Large-scale commercial crop management

### Scope Boundaries

- The system operates on user-provided data; it does not automatically sense soil moisture
- The system requires an active internet connection for AI inference
