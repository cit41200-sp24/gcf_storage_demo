# Cloud Storage Triggered Cloud Function Demo

Sample that shows how to trigger a Cloud Function when a file is uploaded to Cloud Storage.

## Deploy Instructions
```
gcloud functions deploy storage_demo \
--runtime nodejs18 \
--entry-point fileData \
--trigger-event google.storage.object.finalize \
--trigger-resource sp24-41200-elliott-demo-bucket
```