# black_bucks_ASS-5
# AI-Powered Code Generation & Deployment
## PART 1: AI for Code Generation (CRUD App with Flask)

### Objective:
Use AI tools (ChatGPT/GitHub Copilot) to generate a simple backend application with CRUD functionality.

### What was done:
- Prompted ChatGPT to generate a Flask-based CRUD backend for user data.
- Implemented `Create`, `Read`, `Update`, `Delete` endpoints.
- Used SQLite as the backend database.
- API tested with `curl` and Postman.
### Project Structure:
```
crud_app/
├── app.py
├── database.db
└── requirements.txt
```

### Sample Endpoint:
```bash
curl -X POST http://127.0.0.1:5000/users -H "Content-Type: application/json" -d '{"name":"John", "email":"john@example.com"}'
```
---

## PART 2: Deploying a Simple AI Model (Iris Classifier)

### Objective:
Train a machine learning model and deploy it using a web API endpoint.

### What was done:
- Trained a Decision Tree Classifier on the Iris dataset.
- Saved the model using `joblib`.
- Built a Flask API with a `/predict` endpoint.
- Accepts flower features as input and returns predicted species.

### Project Structure:
```
ml_app/
├── model.py            # for training the model
├── app.py              # Flask app for prediction API
└── iris_model.pkl      # saved ML model
```

### Sample Prediction Request:
```bash
curl -X POST http://127.0.0.1:5000/predict -H "Content-Type: application/json" -d "{\"features\": [5.1, 3.5, 1.4, 0.2]}"
```

### Sample Response:
```json
{
  "prediction": "Setosa"
}
```

---
### Conclusion
This project showcases how AI can accelerate both software development and machine learning workflows. Using AI tools like ChatGPT allowed me to generate clean, functional code for both backend services and ML model deployment efficiently.

```

---

Let me know your repo name or structure if you'd like it tailored even more specifically!
