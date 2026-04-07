---
id: macbook-pro-setup
title: Macbook Pro Setup
---

## Prior to Start Date

- Accounts (complete before your start date)
  - Ensure you have completed [Create Accounts](./create-accounts)
- Install **Okta Verify** and **Microsoft Teams** on your mobile phone  
  - Okta URL: https://ecfmg.okta.com

---

# Prerequisites (On Start Date)

> ⚠️ WARNING: DO NOT PERFORM STEPS OUT OF ORDER  
> We perform these steps as a team. Do not do them independently.  
> Wait until you are on a Teams call with the Connected Apps team.

- Message **Seven Thomas** (or Patrick Gidich if unavailable) on Teams when ready

---

## General Notes

- **Patience**
  - Some parts will be boring or frustrating, but consistency across the team matters
- You will receive your username and temporary password on your start date

> 💡 If you have issues, contact Seven Thomas or Patrick Gidich first  
> They may direct you to the Intealth Help Desk:  
> 📞 215-823-2163  
> 📧 servicedesk@intealth.org

---

## Register Password Reset

- [Register to Reset Password](https://support.microsoft.com/en-us/account-billing/register-the-password-reset-verification-method-for-a-work-or-school-account-47a55d4a-05b0-4f67-9a63-f39a43dbe20a)
  - Use personal device or incognito browser
  - Suggestion: add phone as secondary method
  - Username = full email (e.g., jdoe@intealth.org)

- Reset portal (later if needed):
  - https://passwordreset.microsoftonline.com/

---

## Password Requirements

- Must be changed every 6 months
- Cannot be changed multiple times in one day
- Minimum 12 characters
- Must include letters and numbers
- Cannot:
  - contain `*`
  - start with a number
- Must be unique from previous passwords
- No repeated or sequential patterns
- No personal/company-related words
- No common or compromised passwords

---

# 1 - Start Up and Sign In

1. Plug in MacBook
2. Start setup:
   - Language: English
   - Region: United States
   - Transfer: Setup as new
   - Accessibility: Not Now
   - WiFi: connect
   - Data & Privacy: Continue

3. Create computer account:
   - Full Name: first + last name
   - Account Name: first name
   - Password: generate from 1Password

4. Sign in with Apple ID (use personal)
   - Accept terms
   - Verify

5. Optional settings:
   - iCloud Keychain → setup later
   - FileVault → keep enabled
   - Touch ID → set up
   - Apple Pay → skip
   - Theme → your preference

---

## 1B - Install Updates

- Open System Settings → General → Software Update
- Click Update

---

## 1C - Add Apple ID (if skipped)

- System Settings → Sign in with Apple ID

---

# 2 - Partition Drive & Base Folder Structure:

1. **Launch Disk Utility**
    - Press `Command+Space`, type "Disk Utility", and select it.

2. **Add a New Volume** (this is where your code will go)
    - Click the plus (+) button in the header.
    - Name: **files**
    - Format: **APFS**

3. **Create Base Folder Structure**
    1. Launch Finder (`Command+Space`, type "Finder", and select it).
    2. Go to `/Volumes/files`:
        - Press `Command+Shift+G`, type `/Volumes/files`, and press Return.
    3. Create the following folders (`Command+Shift+N` for new folder):
        - **applications** — where you'll install MuleSoft
        - **cloud-files** — where you'll mount OneDrive
        - **src** — where your code goes
            - *Drag **src** to Favorites in the sidebar*
        - **vm-images** — where your Parallels VMs will go

4. **Show Hard Disks in Finder Sidebar**
    - In the top menu, go to Finder → Settings → Sidebar.
    - Under "Locations", ensure "Hard Disks" is checked.

---

# 3 - Install Chrome / Office / OneDrive / Git

## Chrome
- https://www.google.com/chrome/

## Password Manager (1Password)
- Desktop: https://1password.com/downloads/mac/
- Browser: https://1password.com/downloads/browser-extension

## Microsoft Office
- https://portal.office.com/account
- Install for all users
- Mount OneDrive to:

/volumes/files/cloud-files


### Outlook Setup
- Disable Focused Inbox
- Set working hours
- Optional: set compact density

## Microsoft Teams
- https://www.microsoft.com/en-us/microsoft-teams/download-app

---

# 4 - Install Git / Node / Runtime / Java

## Install Git (Command Line Tools)

```bash
xcode-select --install
```

Check Updates 

 ```bash
softwareupdate --list
softwareupdate --install --all