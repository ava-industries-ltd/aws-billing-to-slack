
 Install 

    ```

    AWS_SDK_LOAD_CONFIG=true AWS_PROFILE="ava" AWS_REGION="ca-central-1" serverless deploy --stage="ava" --param="slack_url=https://hooks.slack.com/services/xxx/yyy/zzzz" --param="aws_account=AVA-Master"
    
    AWS_SDK_LOAD_CONFIG=true AWS_PROFILE="ava-development" AWS_REGION="ca-central-1" serverless deploy --stage="ava-development" --param="slack_url=https://hooks.slack.com/services/xxx/yyy/zzzz" --param="aws_account=AVA-Development"
    
    AWS_SDK_LOAD_CONFIG=true AWS_PROFILE="ava-testing" AWS_REGION="ca-central-1" serverless deploy --stage="ava-testing" --param="slack_url=https://hooks.slack.com/services/xxx/yyy/zzzz" --param="aws_account=AVA-Testing"
    
    AWS_SDK_LOAD_CONFIG=true AWS_PROFILE="ava-demo" AWS_REGION="ca-central-1" serverless deploy --stage="ava-demo" --param="slack_url=https://hooks.slack.com/services/xxx/yyy/zzzz" --param="aws_account=AVA-Demo"

    ```


1. Manual Run for a single account
   
    ```
    AWS_SDK_LOAD_CONFIG=true AWS_PROFILE="ava" AWS_REGION="ca-central-1" serverless invoke --function report_cost --stage="ava" --param="slack_url=https://hooks.slack.com/services/xxx/yyy/zzzz" 
    
    AWS_SDK_LOAD_CONFIG=true AWS_PROFILE="ava-development" AWS_REGION="ca-central-1" serverless invoke --function report_cost --stage="ava-development" --param="slack_url=https://hooks.slack.com/services/xxx/yyy/zzzz" 

    AWS_SDK_LOAD_CONFIG=true AWS_PROFILE="ava-testing" AWS_REGION="ca-central-1" serverless invoke --function report_cost --stage="ava-testing" --param="slack_url=https://hooks.slack.com/services/xxx/yyy/zzzz" 

    ```
