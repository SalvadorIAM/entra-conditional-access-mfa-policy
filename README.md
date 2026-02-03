# sc300-entra-conditional-access-mfa-lab
Hands-on lab documenting MFA enforcement using Microsoft Entra Conditional Access
# Microsoft Entra ID – Conditional Access MFA Lab (SC-300)

## Overview
This lab demonstrates how to enforce Multi-Factor Authentication (MFA) using Microsoft Entra ID Conditional Access (modern approach) and contrasts it with legacy per-user MFA. The lab also shows how to validate enforcement using Entra ID sign-in logs.

## Goals
- Understand the difference between legacy per-user MFA and Conditional Access
- Configure Conditional Access in Report-only mode and then enforce it
- Test MFA enforcement using a standard user account
- Verify policy application using sign-in logs

## Environment
- Microsoft Entra ID (trial tenant)
- Microsoft Entra admin portal
- Test users and security groups

## What was configured

### 1. Users and Groups
- Created test users (example: standard user and HR user)
- Created a department-based security group
- Assigned users to the group to test group-based policy inheritance

### 2. Conditional Access Policy
- Created a Conditional Access policy requiring MFA
- Initially set the policy to Report-only for safe testing
- Switched the policy to On to enforce MFA

### 3. MFA Enforcement Method
- Disabled legacy per-user MFA
- Enforced MFA exclusively through Conditional Access (recommended approach)

### 4. Testing and Validation
- Signed in as a test user using a private browser session
- Confirmed MFA challenge was triggered
- Verified policy enforcement using Microsoft Entra ID sign-in logs
- Confirmed Conditional Access policy status showed as Applied

## Key Learning Outcomes
- Per-user MFA is a legacy feature and should not be used for new deployments
- Conditional Access is the modern and recommended way to enforce MFA
- Report-only mode is critical for testing policies safely
- Sign-in logs provide definitive proof of Conditional Access enforcement

## Next Steps
- Implement location-based Conditional Access
- Add device compliance requirements
- Configure and exclude break-glass accounts
- Expand testing to additional users and scenarios
