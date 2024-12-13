AWS Control Tower Controls Template
This repository contains a CloudFormation template for enabling AWS Control Tower controls on specified Organizational Units (OUs).

Usage
Navigate to the templates/ folder to find the CloudFormation templates:
2-controls.yaml: Contains 2 example controls.
4-controls.yaml: Contains 4 example controls.
Use these templates to enable specific controls, such as:
Encryption
CloudTrail detection
Root user restrictions
Parameters
Parameter	Description
ouId	Organizational Unit ID (OU) from AWS Control Tower. Example: ou-abcd-12345678
orgId	Organization ID from AWS Organizations. Example: o-abcdefghij
Deployment Instructions
Upload the CloudFormation template:

Open the AWS Management Console.
Navigate to the CloudFormation service.
Select Create Stack and upload the desired YAML template from this repository.
Enter the required parameters:

Provide valid values for ouId and orgId.
Example inputs:
ouId: ou-abcd-12345678
orgId: o-abcdefghij
Deploy and validate:

Launch the stack by clicking Submit.
Monitor the stack status. If errors occur, review the input parameters and resolve issues.
Troubleshooting:

Check the AWS CloudFormation Events tab for detailed error messages.
Ensure the provided ouId and orgId match the values in your AWS account.
