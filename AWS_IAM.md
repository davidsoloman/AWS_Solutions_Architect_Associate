## AWS: Identity Access Management
<img src="https://clouda-assets.s3.amazonaws.com/upload/54d0e3c7d287c266042be5dc.png?1422975944" width="600">

**What is IAM?**
- AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources for your users. You use IAM to control who can use your AWS resources (authentication) and what resources they can use and in what ways (authorization).
- IAM is a feature of your AWS account offered at no additional charge. You will be charged only for use of other AWS services by your users.

**What does IAM provide?**
- Centralized control of AWS account
- Shared Access of AWS account
- Granular permissions for individual user or service
- Identity Federation (including active directory, facebook, linkedin, google linking)
- Allow multi-factor authentication
- Provide temporary access to devices , services
- Allow to set up password rotation policy
- Support PCI-DSS compliance

**Important terms in IAM?**
Users - End users
Groups - Groups or departments in office
Roles - Roles can be created and then assigned to AWS resources. Eg. A role can be defined for EC2 instance to process data and load to S3
Policies - Policiy documents define the rules and permissions. 

**Setting up IAM**
Security
- IAM is a global feature, it is not bound to a region
- IAM users sign in link consist of the AWS account number of parent account 
e.g. https://552619384927.signin.aws.amazon.com/console
This login link can be set to customized link => https://dhananjay-test-28.signin.aws.amazon.com/console
- Set up multifactor authentication for root user
 
Following are the steps for setting up the IAM:

<img src="./Images/IAM/IAM1.png" width="600">

**Step 1:** IAM in the AWS Dashboard
 
<img src="./Images/IAM/IAM2.png" width="600">

**Step 2:** IAM Dashboard 
 
<img src="./Images/IAM/IAM3.png" width="600">

**Step 3:** Activate Multifactor Authentication on the root
  
<img src="./Images/IAM/IAM4.png" width="600">

**Step 4:** Add new IAM Users

<img src="./Images/IAM/IAM5.png" width="600">

**Step 5:** Set type of access for each user.

<img src="./Images/IAM/IAM6.png" width="600">

**Step 6:** Add users to groups
 
<img src="./Images/IAM/IAM7.png" width="600">

**Step 7:** Assign different privileges to user groups
 
<img src="./Images/IAM/IAM8.png" width="600">

**Step 8:** Review permissions for group

<img src="./Images/IAM/IAM9.png" width="600">

**Step 9:** Users are added successfully with access assigned to users.

<img src="./Images/IAM/IAM10.png" width="600">

**Step 10:** Users can be added to more than one groups and granted additional permissions.

<img src="./Images/IAM/IAM11.png" width="600">

**Step 11:** Access can be revoked for a user or can be made inactive

<img src="./Images/IAM/IAM12.png" width="600">

**Step 12:** Admin can set up a password policy for the users

<img src="./Images/IAM/IAM13.png" width="600">

**Step 13:** After all the 5 fields are green IAM is good.
 
 
 
 