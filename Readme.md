**To run the project, execute the following command:**

```
  uvicorn app:app --reload
```

**To test the project**

* either execute the following command::

```
  curl -X POST "http://127.0.0.1:8000/predict" -H "Content-Type: application/json" -d "{\"tenure\": 72, \"InternetService\": \"Fiber optic\", \"OnlineSecurity\": \"Yes\", \"TechSupport\": \"Yes\", \"Contract\": \"Two year\", \"PaymentMethod\": \"Credit card (automatic)\"}"
```

* or make a POST request using an HTTP client(POSTMAN, INSOMNIA) to the address: *http://localhost:8000/predict* passing the following object: 
```
  {
    "tenure": 72,
    "InternetService": "Fiber optic",
    "OnlineSecurity": "Yes",
    "TechSupport": "Yes",
    "Contract": "Two year",
    "PaymentMethod": "Credit card (automatic)"
  }

```