 1. Create GCP Project. Note ID
 2. Enable Identity Platform
 3. Users > Setup Details > Copy the Code in main.js
 4. backend/app.yaml > Paste project ID to FIREBASE_PROJECT_ID 
 5. Add Identity Platform provider
 6. Identity Platform > Settings > Authorized Domain > Add [PROJECT_ID].appspot.com
 7. cd backend > pip install -t lib -r requirements.txt
 8. For local: dev_appserver.py frontend/app.yaml backend/app.yaml
 9. For GCP: gcloud app deploy backend/index.yaml frontend/app.yaml backend/app.yaml
