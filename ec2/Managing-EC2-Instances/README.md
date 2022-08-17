# Staring and Stopping EC2 Instances mornings and nights

## Notes

### Lambda Function

Be sure to set the Lambda function timeout high enough (i.e. 1 minute) so that it can iterate through every instance in every region.

### EventBridge Rules

Cron expression: `0 6 ? * MON-FRI *`
Cron expression: `0 16 ? * MON-FRI *`
