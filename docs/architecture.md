# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 | Encrypted permit storage for each organization |
| Textract | Text and tables read from scanned permits |
| Bedrock | Conditions, dates and required documents extracted |
| Lambda and DynamoDB | Permit records, reminders and the review log |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
