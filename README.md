# Entra Conditional Access MFA Policy

Implementation of Multi-Factor Authentication enforcement using Microsoft Entra ID Conditional Access. This lab demonstrates the modern approach to MFA enforcement, contrasts it with legacy per-user MFA, and validates policy application using sign-in log analysis.

## Conditional Access Policy: MFA Enforcement

## Overview

This lab demonstrates how to enforce Multi Factor Authentication (MFA) using Microsoft Entra ID Conditional Access, the modern and recommended approach to identity security. It also contrasts Conditional Access-based MFA with legacy per-user MFA.

The lab includes validation of policy enforcement using Microsoft Entra ID sign-in logs.

## Goals

* Understand the difference between **legacy per user MFA** and **Conditional Access based MFA**
* Configure Conditional Access in **Report only mode** before enforcement
* Enforce MFA using Conditional Access
* Test MFA enforcement using a standard user account
* Verify policy application using **Microsoft Entra ID sign in logs**

## Environment

* Microsoft Entra ID (trial tenant)
* Microsoft Entra admin portal
* Test users
* Security groups

## Configuration Summary

### 1. Users and Groups

* Created test users (for example: standard user and HR user)
* Created a department based security group
* Assigned users to the group to test **group based policy inheritance**

### 2. Conditional Access Policy

* Created a Conditional Access policy requiring **MFA**
* Initially set the policy to **Report only** for safe testing
* Switched the policy to **On** to enforce MFA

### 3. MFA Enforcement Method

* Disabled **legacy per user MFA**
* Enforced MFA exclusively through **Conditional Access** (recommended approach)

### 4. Testing and Validation

* Signed in as a test user using a private browser session
* Confirmed the MFA challenge was triggered
* Verified policy enforcement using **Microsoft Entra ID sign in logs**
* Confirmed Conditional Access policy status showed as **Applied**

## Security Best Practices Demonstrated

* Use **Conditional Access policies** instead of legacy per user MFA
* Test security policies using **Report only mode** before enforcement
* Validate policy behaviour using **sign in logs**
* Apply authentication controls through **centralised identity policies**
* Implement MFA as part of a **modern identity security architecture**

## Key Learning Outcomes

* Per user MFA is a **legacy feature** and should not be used for new deployments
* Conditional Access is the **modern and recommended way to enforce MFA**
* Report only mode is critical for safely testing security policies
* Sign in logs provide **definitive validation** of Conditional Access enforcement

## Next Steps

* Implement location based Conditional Access
* Add device compliance requirements
* Configure and exclude break glass accounts
* Expand testing to additional users and scenarios
