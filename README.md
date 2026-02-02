# AWS IAM Least Privilege & MFA Security Hardening Lab

## Overview
This lab demonstrates the implementation of AWS Identity and Access Management (IAM) security best practices using the principle of least privilege and multi-factor authentication (MFA).

The project simulates a real-world cloud security scenario where an IAM user is created with restricted permissions, tested for enforcement, and hardened with MFA.

---

## Objectives
- Create an IAM user with least privilege permissions
- Assign access using group-based IAM policies
- Validate permission enforcement through access denial testing
- Secure IAM user access using multi-factor authentication (MFA)
- Demonstrate AWS IAM security best practices

---

## Architecture Summary
- AWS IAM User
- IAM Group with ReadOnlyAccess
- Permission enforcement testing
- MFA-enabled console access

---

## Security Principles Applied
- Least Privilege
- Zero Trust Identity
- Defense in Depth
- Secure Authentication

---

## Screenshots Walkthrough


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

![Blocked Permissions](https://github.com/Amir-Fadelelsaid/AWS-IAM-least-privilege-mfa-lab/blob/b64a484716e8275baae0030796d218a506d5f29c/AWS%20IAM%20Least%20Privilege%20Blocked.png)
### Least Privilege Enforcement – Action Blocked

An attempt to escalate permissions was denied by AWS IAM. The cloud-security-user 
was prevented from attaching additional policies due to restricted privileges. 
This confirms that least-privilege controls are actively enforced and administrative 
actions are blocked.

![ReadOnly Group](https://github.com/Amir-Fadelelsaid/AWS-IAM-least-privilege-mfa-lab/blob/9d1f72b7b992ad95f1144427c97a3c0de4ee4f09/AWS-IAM-User-Creation-ReadOnly.png)
### IAM User Creation – Read-Only Security User

A dedicated IAM user (cloud-security-user) was created with restricted access. 
Credentials were generated and delivered securely, establishing a separate 
non-root identity for least-privilege access to the AWS environment.

![MFA Enabled](https://github.com/Amir-Fadelelsaid/AWS-IAM-least-privilege-mfa-lab/blob/8ae7befafca177f145e71acd62cbdb222440b9e8/AWS%20IAM%20MFA%20enabled%20final.png)
### MFA Enforcement Completed

Multi-Factor Authentication (MFA) was successfully assigned to the IAM user, 
ensuring strong authentication and protecting the account from unauthorized access. 
Console access now requires MFA, completing the least-privilege security hardening process.

## Framework Alignment
- NIST 800-53 (AC-2, IA-2)
- CIS AWS Foundations Benchmark
- AWS IAM Best Practices

---

## Skills Demonstrated
- AWS IAM user and group management
- Identity security hardening
- Access control enforcement
- MFA implementation
- Cloud security best practices
