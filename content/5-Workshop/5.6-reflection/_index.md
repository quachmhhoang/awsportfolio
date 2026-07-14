---
title: "Reflection"
date: 2026-07-10
weight: 6
chapter: false
pre: " <b> 5.6. </b> "
---

### Challenges
- IAM roles must be configured with the correct permissions for each service.
- API Gateway and Cognito must match the JWT authorizer configuration.
- SES sandbox requires both sender and recipient emails to be verified.
- SQS FIFO and DLQ must be configured with the correct redrive policy.

### Solutions
- Check CloudWatch logs when Lambda or API errors occur.
- Recheck Lambda environment variables.
- Verify SES identity before testing email sending.
- Monitor SQS and DLQ to check the notification flow.

### Future Development
- Integrate Amazon Bedrock or Comprehend to classify tickets automatically.
- Add live chat using API Gateway WebSocket.
- Build a reporting dashboard using Athena or QuickSight.