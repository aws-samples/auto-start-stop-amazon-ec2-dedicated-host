# auto-start-stop-dedicated-host
Dedicated host can help you bring your own licences for operating systems and applications, they can help in customising the underlying hardware infrastructure to meet your specific requirements,etc. Generally to save cost we tend to stop the instances running during off hours, but stopping instances in a dedicated host wont help us save because you are billed at host level.This solution helps in automating the allocation and de-allocation of dedicated host between running hours(work hours) to save cost. While the host is de-allocated, the instances that were previously on the host is not terminated, rather they remain in stop state and they can be re-launched in a new dedicated host based on wake up schedule.
Automation is achieved using AWS Lambda, SDK for Python (Boto3), and Amazon EventBridge. 


## To Launch the Cloudformation Template via AWS Management Console 

    1. Sign in  to the AWS Management Console
        Make sure you are signed in to your AWS account

    2. Navigate to AWS Cloudformation service Page

    3. Create a New Stack
        In the cloudformation dasboard click on the "create Stack" button 

    4. Specify the Template
        In the wizard, choose "Template is ready" and select "Upload the Teamplate.yaml" file from your local

    5.  Configure Stack Details
        Provide a stack name for the cloudformation stack.
        Configure additional Parameters like az, instance id's, hostname and cron 

    6. Review and Create the stack by acknowledging

## Pre-requisite

    1. An AWS account in which the solution can be deployed
    2. EC2 instances that needed to auto stopped and started
    Note: if this is the first time you are trying, make sure the instance is in stop state and launch the stack

## How it works 
    
![SolutionArchDiagram.png ]  

    
