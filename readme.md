 1. Create GCP Project. Note ID
 2. Enable Identity Platform
 3. Users > Setup Details > Copy the Code in main.js
 4. main.js > Update backendHostUrl with PROJECT_ID 
 5. backend/app.yaml > Paste project ID to FIREBASE_PROJECT_ID 
 6. Add Identity Platform provider
 7. Identity Platform > Settings > Authorized Domain > Add [PROJECT_ID].appspot.com
 8. cd backend > pip install -t lib -r requirements.txt
 9. For local: dev_appserver.py frontend/app.yaml backend/app.yaml
 10. For GCP: gcloud app deploy backend/index.yaml frontend/app.yaml backend/app.yaml
