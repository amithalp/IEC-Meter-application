IEC Okta Authentication
A cloud integration to IEC (Israel Electric Corporation)

Overview
IEC Okta Authentication is a Hubitat Elevation app that allows users to authenticate with the Israel Electric Corporation (IEC) using Okta. It manages the entire authentication flow, including user ID submission, OTP (One-Time Password) verification, session authorization, and access token retrieval. The application also schedules a refresh process to keep your authentication valid. During the setup process, the application will create a device to capture all data available in your IEC account.

Prerequisites
Before you begin, ensure you have:

A Hubitat Elevation hub.
Access to IEC account details - this is usually your ID you use when you log in to your account on the IEC website.
Installation
Clone the Repository
sh
Copy code
git clone https://github.com/amithalp/IEC/IEC-Okta-Authentication.git
Deploy the Code
Navigate to your Hubitat Elevation hub's web interface.
Go to Apps Code and click on New App.
Copy and paste the content of IEC_Okta_Authentication1.groovy into the editor.
Click Save.
Install the App
Go to Apps.
Click on Add User App.
Select IEC Okta Authentication from the list.
Follow the on-screen instructions to configure the app.
Usage
To test the authentication process, perform the following steps:
Note: It is highly recommended that you keep the logs page open throughout the process to ensure no error logs are showing.

Enter User ID
After installing the app, enter your IEC user ID in the provided field.
Click Initiate Authentication to begin the process. You should receive an OTP via SMS or email according to your preferences on the IEC website.
Verify OTP
Enter the received OTP in the designated field.
Click Verify OTP Code. Upon successful verification, you will proceed to the next step.
Authorize Session
Once the OTP is verified, click Authorize Session to authorize your session and complete the login process.
Get Access Token
After session authorization, click Get Access Token.
The app will retrieve an access token which will be used for subsequent API calls.
Debugging
If you encounter issues during the authentication process, check the logs in the Logs section of your Hubitat interface for detailed error messages and debugging information.

Contributing
Contributions to enhance the app or fix issues are welcome. Please feel free to fork the repository and submit pull requests.

Support
If you need assistance or have any questions, please raise an issue in the GitHub repository, and the maintainers will address it as soon as possible.

License
This project is licensed under the MIT License - see the LICENSE file for details.
