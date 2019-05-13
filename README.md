Task:
	Develop an independent Cloudformation tepmplate which takes State/Province as a paramter and exports the unix time for the given State/Province in Europe in the stack.
Findings:
	Used Cloudformation for designing the infrastructure.
	Used AWS lambda as a custom resource in Cloudformation.
	Used python for calculating Unixtime.
Challenges:
	1. I faced creating the appliccation for calculating unixtime
	2. I was not able to configure lambda functions for the task
How to implement:
	1. Pull the cloudformation template from the github and upload the zip file to your S3 bucket.
	2. Visit the AWS cloudformation link and and click on create new stack
	3. Import the pulled template
	4. Now it will ask you some details ex: Name of Stack,S3 bucket name,S3Key(Name of zip file) and an input State/Province
	5. In the rolse section either you can select role or you can check mark the IAM role.
	5. Now just go and launch the template
	6. Wait for sometime or you can see the progress of launching stack by clicking on the stack
	7. After launching successfully, click on the Output section, there you will be able to see "unix time" for the State/Province as the task is mentioned.
	