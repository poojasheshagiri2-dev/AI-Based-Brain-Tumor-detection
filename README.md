# BrainTumor


BrainTumorAI, is an AI-powered healthcare platform for analyzing brain MRI scans. The system validates uploaded MRI images, preprocesses them, classifies tumors using a Hybrid 3D ResNet-50 and Vision Transformer model, explains predictions with Grad-CAM, segments tumors using U-NET, and calculates tumor measurements. It then generates a clinical analysis and a professional PDF report. The platform also includes secure authentication, a React-based dashboard, a RAG-powered medical chatbot, prediction history, and an admin dashboard. The goal is to build a scalable, production-ready decision-support system that assists clinicians with accurate and explainable brain tumor analysis.

**AI Pipeline**

      User Login
            │
            ▼
      Dashboard
            │
            ▼
      Patient Details
            │
            ▼
      Upload MRI
            │
            ▼
      FastAPI Backend
            │
            ▼
      ML Model
            │
            ├────────► Tumor Prediction
            │
            ├────────► Confidence Score
            │
            ├────────► Grad-CAM
            │
            └────────► AI Explanation
            │
            ▼
      React Dashboard
            │
            ▼
      Prediction History


Brain MRI Validator (Very Important)

Pipeline begins here.

            Upload MRI
            ↓
            CNN Validator
            ↓
            Brain MRI?
            _____|________
            ↓            ↓
            YES          NO
            ↓            ↓
            Continue     Reject

**Frontend**

- React + Vite
- Tailwind
- Material UI
- React Router
- Axios

**Backend**

- FastAPI
- PostgreSQL
- Alembic
- JWT
- bcryp

**Expected Outcome**

By the end of the project, the system will:

- Securely authenticate users.
  
- Accept Brain MRI scans.
  
- Validate the uploaded image.
  
- Detect and classify brain tumors.
  
- Highlight the tumor location.
  
- Measure tumor characteristics.
  
- Generate explainable AI visualizations.
  
- Produce a professional PDF report.
  
- Provide a medical AI assistant for domain-specific questions.
  
- Maintain prediction history and an admin dashboard.
