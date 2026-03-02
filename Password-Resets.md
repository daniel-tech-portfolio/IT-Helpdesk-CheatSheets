# Password Reset Troubleshooting Guide

## Purpose
Provide a standard process for securely resetting user passwords in a help desk environment.

---

## Step 1: Verify User Identity

Always confirm the user’s identity before resetting passwords:

• Employee ID
• Security questions
• Manager verification
• Company badge

---

## Step 2: Determine Account Type

Check if the account is:

• Active Directory domain account
• Local workstation account
• Microsoft 365 account
• VPN or application-specific account

---

## Step 3: Reset Password in Active Directory

1. Open Active Directory Users and Computers
2. Locate the user account
3. Right-click → Reset Password
4. Check:
   - User must change password at next logon

---

## Step 4: Unlock Account (If Needed)

If locked out:

• Right-click account → Properties → Account tab
• Clear "Account is locked out"

---

## Step 5: Provide Secure Instructions

Never send passwords via email.

Best practices:

• Provide temporary password verbally
• Require immediate change
• Recommend strong password creation

---

## Common Issues

User still cannot log in:

• Caps Lock enabled
• Wrong domain selected
• Account expired
• Network connectivity issues

---

## Security Best Practices

• Always verify identity
• Follow least privilege principles
• Document all password resets in ticket system
