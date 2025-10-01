# CodeTech-Internship-Task-3

# CODTECH — Multi-Cloud Demo (AWS + GCP)

## Overview
This demo demonstrates interoperability between GCP (GKE + Cloud Storage + Pub/Sub) and AWS (EKS + S3 + Kinesis). The goal is to show a request originating in GCP triggering processing in AWS with secure networking and observability.

## What to show
1. Create a user via GCP endpoint → file saved to GCS.
2. Event published to Pub/Sub → forwarded to AWS.
3. AWS service consumes event → writes audit entry to S3.
4. Tracing shows a distributed trace across both clouds.

## Commands (examples)
- `gsutil mb gs://codtech-multicloud-gcs`
- `aws s3 cp sample.txt s3://codtech-multicloud-s3/`

(Full step-by-step script in DOCUMENTATION.md)
