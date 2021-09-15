# Build and deploy

Command to build the application. PLease remeber to change the project name and application name
```
gcloud builds submit --tag gcr.io/loan-status-predictor-rf-app/lsp-rf-app  --project=loan-status-predictor-rf-app
```

Command to deploy the application
```
gcloud run deploy --image gcr.io/loan-status-predictor-rf-app/lsp-rf-app --platform managed  --project=loan-status-predictor-rf-app --allow-unauthenticated