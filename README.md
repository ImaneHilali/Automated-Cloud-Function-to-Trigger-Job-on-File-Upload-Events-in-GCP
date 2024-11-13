# Automated-Cloud-Function-to-Trigger-Job-on-File-Upload-Events-in-GCP
This Cloud Function listens for file upload events in a GCP Storage bucket. Upon receiving an event, it extracts the bucket and object details, encodes them in a payload, and forwards the request to a Cloud Run service. The function automates job triggers, allowing for seamless processing of uploaded files.
