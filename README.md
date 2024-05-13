### Get User  Information
Get user information(groups,alias etc)

`gam info user useraccount
`
### **Suspend a User Account
**To temporarily disable a user account, preventing the user from accessing their account until reactivation:

`gam suspend user useraccount
`
### **Unsuspend a User Account
**To reactivate a previously suspended user account, ensuring the user can access their account again:

`gam unsuspend user useraccount
`

### Remove Recovery Email
To delete the recovery email address for a specific user, enhancing account security or in preparation for account changes:

`gam update user useraccount recoveryemail ''recoverymail''
`
### Update User Password
To change the password for a user account, which is essential for account security, especially after a breach or as routine maintenance:

`gam update user useraccount password PasswordHere
`
### Show Out of Office (OOO) 
gam user useraccount show vacation

### Set Out of Office (OOO) Auto-Reply
To configure an automatic out-of-office reply for a user who is no longer available, ensuring that senders receive a prompt response with redirection instructions:


`gam user useraccount vacation on subject "Out of Office" message "OOO Message" start 2024-03-17 end 2024-07-20
`
### Delete Email Signature
To remove the current email signature for a user, which might be necessary during updates or rebranding phases:

`gam user useraccount sig "Signature"
`
### Email Delegation
To grant one user (delegate) the ability to access and manage another user's email account, facilitating teamwork or ensuring continuity during absences:


`gam user delegateduser add delegate useraccount
`
