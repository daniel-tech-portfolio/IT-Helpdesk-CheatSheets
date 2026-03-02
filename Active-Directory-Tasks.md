# Active Directory Support Tasks Guide

## Purpose
Provide a reference workflow for common Active Directory (AD) support tasks performed by help desk technicians in a Windows enterprise environment.

---

## Common Help Desk AD Responsibilities

Typical Tier 1 tasks include:

• Resetting user passwords  
• Unlocking accounts  
• Creating user accounts  
• Disabling or enabling accounts  
• Updating user information  
• Adding users to security groups  

---

## Step 1: Access Active Directory

Open:

Active Directory Users and Computers (ADUC)

Path:

Start → Administrative Tools → ADUC

---

## Step 2: Reset a User Password

1. Locate the user in ADUC
2. Right-click the account
3. Select **Reset Password**
4. Enter temporary password
5. Check:
   - User must change password at next logon

---

## Step 3: Unlock a Locked Account

If user is locked out:

1. Right-click user account → Properties
2. Go to **Account** tab
3. Clear **Account is locked out**
4. Click Apply

---

## Step 4: Create a New User Account

1. Right-click appropriate OU
2. Select **New → User**
3. Enter user details:
   - Name
   - Username
   - Email
4. Assign initial password
5. Set password policies

---

## Step 5: Disable or Enable Accounts

Disable account when:

• Employee leaves organization  
• Security risk suspected  

Steps:

Right-click user → Disable Account

---

## Step 6: Add User to Security Groups

Used to assign permissions.

Steps:

1. Open user properties
2. Select **Member Of** tab
3. Click **Add**
4. Enter group name

Examples:

• Domain Users  
• VPN Access  
• File Share Groups  

---

## Step 7: Move Users Between Organizational Units (OUs)

Used for:

• Department changes  
• Policy application  

Steps:

Drag user account to correct OU.

---

## Common Issues and Fixes

| Issue | Cause | Solution |
|------|------|----------|
| User cannot log in | Locked account | Unlock account |
| Access denied to resources | Missing group membership | Add to proper group |
| Password reset not working | Replication delay | Wait or check DC sync |
| Cannot find user | Wrong OU | Search entire directory |

---

## Security Best Practices

• Verify user identity before changes  
• Follow least privilege principles  
• Document all AD modifications  
• Avoid granting unnecessary permissions  

---

## Escalation Criteria

Escalate to Tier 2 if:

• Domain controller issues occur  
• Replication failures suspected  
• Group Policy conflicts present  
• Permission inheritance problems exist  

---

## Key AD Concepts for Help Desk

• Domain = Centralized authentication environment  
• OU = Organizational structure for users and computers  
• Security Groups = Permission management tools  
• Group Policy = Enforces system configurations  

---

*This guide reflects real-world Active Directory support procedures used by IT help desk technicians.*
