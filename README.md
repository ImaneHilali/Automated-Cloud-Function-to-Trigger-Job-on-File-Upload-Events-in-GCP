# Automated Cloud Function to Trigger Job on File Upload Events in GCP
This Cloud Function listens for file upload events in a Google Cloud Storage bucket and triggers a specified job in a Cloud Run service. When a new file is uploaded to the translation-input bucket, this function captures the event details, packages them into a structured payload, and forwards it to a specified Cloud Run URL for processing.

The function:
 Extracts bucket and object name from the event data.
 Specifies an output bucket for the processed file, defaulting to translation-output.
 Encodes the payload in base64 and sends it as a POST request to the Cloud Run service.

This setup supports seamless automation in GCP, enabling various job triggers based on file upload events.
