# AWS-IAM-least-privilege-mfa-lab
AWS IAM least privilege and MFA security hardening lab


![IAM Dashboard](https://github.com/Amir-Fadelelsaid/AWS-IAM-least-privilege-mfa-lab/blob/50026977d3ca4965dc841f876dd3699c30d3b169/AWS%20IAM%20Dashboard%20Overview.png)
### IAM Dashboard – Secure Account Baseline

The AWS IAM dashboard confirms the account security posture after configuration. 
Root user MFA is enabled, no active root access keys exist, and IAM resources are 
properly segmented. This establishes a secure identity baseline before applying 
least-privilege controls to IAM users.

![Least Privilege Permissions](https://github.com/Amir-Fadelelsaid/AWS-IAM-least-privilege-mfa-lab/blob/c817e38738fe7fd62fea5c04aea2d64ac3d25394/AWS%20IAM%20User%20Least%20Privilege%20Permissions.png)
### IAM User – Least Privilege Permissions Applied

The cloud-security-user IAM account is restricted using least-privilege access. 
Only ReadOnlyAccess and password self-management policies are attached, preventing 
administrative actions while allowing safe visibility into AWS resources. This 
demonstrates controlled identity permissions aligned with security best practices.
