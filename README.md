### AWS Firehose Example

A lambda (Logger) writes event into streaming platform (DeliveryStream). Another lambda (ProcessLambdaFunction) does
data transformation and then the transformed data is sent to S3 

### Deployment

Make command prompt should be available. Following are the commands:

    $ make deployment_bucket  # This bucket will contain the artifacts
    $ make deploy

### Test
Test can be done manually after deployment. The event.json file has the sample event that can be sent as an event for
Logger lambda. At the end, we can check S3 bucket to see whether data ended up there or not.
