# Login Functionality Test Cases
This repository contains test cases for the Login Functionality of an application. The purpose of these test cases is to validate that users can securely log in to the system and handle all edge cases to ensure functionality, usability, and security.

Test Cases List
1. Positive Test Cases
Verify login with valid credentials.

Description: Ensure that the user is able to log in successfully with a valid username and password.
Expected Result: The user should be redirected to the dashboard.
Verify password masking.

Description: Ensure the password field masks input characters.
Expected Result: The password field should display * or • for each character typed.
Verify the "Remember Me" functionality.

Description: Check that selecting the "Remember Me" option retains login information.
Expected Result: On the next visit, the username is pre-filled, and the session persists if not logged out manually.
Verify redirection after successful login.

Description: Ensure that the user is redirected to the correct dashboard or landing page upon successful login.
Expected Result: User lands on their designated dashboard.
2. Negative Test Cases
Verify login with invalid credentials.

Description: Attempt login with an incorrect username or password.
Expected Result: The system should display an error message: "Invalid username or password."
Verify login with an empty username field.

Description: Attempt login while leaving the username field blank.
Expected Result: The system should display an error message: "Username is required."
Verify login with an empty password field.

Description: Attempt login while leaving the password field blank.
Expected Result: The system should display an error message: "Password is required."
Verify login with special characters in the username.

Description: Attempt login using special characters in the username.
Expected Result: The system should display an error message: "Invalid username format."
Verify login when account is locked.

Description: Attempt login when the account is locked due to multiple failed attempts.
Expected Result: The system should display an error message: "Your account is locked. Please reset your password or contact support."
3. Security Test Cases
Verify SQL injection prevention.

Description: Attempt login using malicious SQL queries in the username or password field.
Expected Result: The system should block the request and prevent database tampering.
Verify session timeout.

Description: Log in and remain idle for the defined session timeout period.
Expected Result: The session should automatically log out the user after the timeout period.
Verify multi-factor authentication (if applicable).

Description: Check that multi-factor authentication is triggered after valid credentials are entered.
Expected Result: User receives an OTP or verification code to proceed with login.
Verify brute-force attack prevention.

Description: Attempt multiple login attempts with incorrect credentials.
Expected Result: The system should lock the account after a defined number of failed attempts.
