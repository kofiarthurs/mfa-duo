<h1>Multiple-Factor Authentication (MFA) with DUO</h1>
<h2>Description</h2>
Today we are going to be setting up multi-factor authentication (MFA) with DUO. DOU by Cisco is a web application that allows companies to setup MFA for their business applications through various means, such as hardware tokens, mobile, desktop authentication and so on. 

<h2>Applications</h2>
<img src="https://imgur.com/qYZvvlc.png" height="80%" width="80%"/>

They have a variety of applications that companies can choose to setup, allowing for seamless integration.

<h2>User Setup</h2>
<img src="https://imgur.com/F6rzVKf.png" height="80%" width="80%"/>
There are multiple ways to set up users. The options are External Directories, Import Users and Add User.
External Directories have 3 ways we can connect directories, Microsoft Entra ID, Active Directory and OpenLDAP.
Import Users allows us to bulk import multiple users from a csv file.
Add User is for manually adding a single user at a time.

<h2>User Enrollment</h2>
<img src="https://imgur.com/0CdPUHJ.png" height="80%" width="80%"/>

To enroll users, you can use the Bulk Enroll Users option or the Send Enrollment Email option under Add User. In order to enroll users they need an email. Once they get the link they can go through the setup process on their devices.
<img src="https://imgur.com/eNGKIm9.png" height="80%" width="80%"/>

The user would first download the DUO application before clicking on the setup link so that the link connects to the app automatically. Once on the app, they can put in their details and complete the set up.

<h2>User Profile</h2>
<img src="https://imgur.com/u0rpfom.png" height="80%" width="80%"/>

Under the users profile you can view their details and edit configurations. Status allows us to require MFA for the user, bypass it or disable access entirely. Bypass might be used when a user needs access but MFA isnt working. Disabled denys access to the user even when MFA is used.
<img src="https://imgur.com/wsPmT7F.png" height="80%" width="80%"/>

Authentication Experience’s option, Automatic Selection of Authentication Methods can be enabled or disabled. When its enabled the last-used method or most secure method, as defined by Duo, will be selected for the user.

Groups can be created to simplify the management of users. Under groups you get the same Status options, Active, Bypass and Disabled. This allows us to manage a large groups of users statuses simultaneously.
<img src="https://imgur.com/fGDEEgK.png" height="80%" width="80%"/>

We can view the user’s recent authentications, which was a browser in this case, phone details and endpoints. We can reactivate the mobile app when MFA isn’t registering. Endpoints lists the devices connected to the users accounts, for example, phones and tablets.
<img src="https://imgur.com/kbXZEcX.png" height="80%" width="80%"/>

Hardware tokens are physical devices that create MFA codes.
Bypass Codes can be sent to the user, these bypass MFA. DUO keeps a log of who creates the codes for security purposes.

WebAuthn allows us to connect biometric and passkey authentication methods. These can be built into the device or be a separate device. A passkey is a credential that allows a user to login without a password, you can use a finger print, face id, pin or pattern

Desktop Authenticators is the DUO desktop app.

<h2>Phones</h2>
<img src="https://imgur.com/vGkTByW.png" height="80%" width="80%"/>

Once a user has connected their phone, we are given information such as the make and model of the device. Under Device Security we are given info about the devices security features, such as Disk Encryption, Passcode Set and Biometrics. Tampered refers to the device being jailbroken or rooted which may be more susceptible to malware and unauthorised access.

Lastly, we have other features that allow us to create access policies for specific device brands, view reports for authentication auditing and identity monitoring.

