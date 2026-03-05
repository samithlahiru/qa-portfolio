# Test Cases – Authentication (Sign-Up & Login)

## 1. Sign-Up Test Cases

| TC ID | Test Case Description | Precondition | Steps | Expected Result | Priority |
|-------|---------------------|--------------|-------|----------------|----------|
| TC_001 | Verify that the Sign-Up button is clickable and renders the Sign-Up page successfully | System is up; User is on homepage | Click **Sign-Up** button | Sign-Up page loads correctly | P2 |
| TC_002 | Verify that all required form fields are rendered | System is up; User is on Sign-Up page | Check page fields | All required fields displayed (First Name, Last Name, Username, Email, Phone Number, Password, Terms Checkbox) | P2 |
| TC_003 | Verify that the user can type in the First Name field | On Sign-Up page | Enter text in First Name | Text is entered successfully | P2 |
| TC_004 | Verify that the user can type in the Last Name field | On Sign-Up page | Enter text in Last Name | Text is entered successfully | P2 |
| TC_005 | Verify that the user can type in the Username field | On Sign-Up page | Enter text in Username | Text is entered successfully | P2 |
| TC_006 | Verify that the user can type in the Email field | On Sign-Up page | Enter text in Email | Text is entered successfully | P2 |
| TC_007 | Verify that the user can type in the Phone Number field (optional) | On Sign-Up page | Enter number in Phone Number | Text is entered successfully; field is optional | P2 |
| TC_008 | Verify that the user can type in the Password field | On Sign-Up page | Enter text in Password | Text is entered successfully | P2 |
| TC_009 | Verify required field validation for First Name | Leave First Name empty | Submit form | Error: "Please fill out this field." | P2 |
| TC_010 | Verify required field validation for Last Name | Leave Last Name empty | Submit form | Error: "Please fill out this field." | P2 |
| TC_011 | Verify required field validation for Username | Leave Username empty | Submit form | Error: "Please fill in this field." | P2 |
| TC_012 | Verify required field validation for Email | Leave Email empty | Submit form | Error: "Please fill out this field." | P2 |
| TC_013 | Verify optional Phone Number field behavior | Leave Phone Number empty | Submit form | No error; user can continue | P2 |
| TC_014 | Verify required field validation for Password | Leave Password empty | Submit form | Error: "Please fill out this field." | P2 |
| TC_015 | Verify Terms and Conditions checkbox validation | Do not check checkbox | Submit form | Error: "Please check this box if you want to proceed." | P2 |
| TC_016 | Verify successful sign-up with valid data | Fill all fields correctly | Submit form | Account created; success message or redirect | P2 |
| TC_017 | Verify sign-up blocked with already registered email | Use existing email | Submit form | Error: "Email is already taken." | P2 |
| TC_018 | Verify sign-up blocked with already registered username | Use existing username | Submit form | Error: "Username is already taken." | P2 |
| TC_019 | Verify optional Phone Number duplicate behavior | Use existing phone number | Submit form | No error (optional) | P2 |
| TC_020 | Verify invalid email format | Enter invalid email | Submit form | Error: "Please match the requested format." | P2 |
| TC_021 | Verify invalid phone number (optional) | Enter invalid phone number | Submit form | Error: "Enter a valid phone number." | P2 |
| TC_022 | Verify password minimum length validation | Enter short password | Submit form | Error: "Your password must contain 8 or more characters." | P2 |
| TC_023 | Verify password breach check | Enter breached password | Submit form | Error: "This password has been found in a breach; please try another." | P2 |
| TC_024 | Verify Terms and Privacy agreement | Do not check checkbox | Submit form | User cannot sign up; validation error appears | P2 |
| TC_025 | Verify page responsiveness | Open Sign-Up on different devices | Inspect page | Page is responsive on all screen sizes | P2 |
| TC_026 | Verify labels and UI alignment | Inspect Sign-Up page visually | - | All fields, buttons, labels aligned and legible | P2 |

---

## 2. Login Test Cases

| TC ID | Test Case Description | Precondition | Steps | Expected Result | Priority |
|-------|---------------------|--------------|-------|----------------|----------|
| TC_001 | Verify navigation to Login page | System is up | Open login URL | Login page loads successfully | P1 |
| TC_002 | Verify page loads completely | System is up | Open login page | Page loads with no errors | P1 |
| TC_003 | Verify login page header text | On login page | Check page header | Header shows "Sign in" text | P1 |
| TC_004 | Verify "Continue with Google" button exists | On login page | Check page | Button is visible | P1 |
| TC_005 | Verify input field for email/username exists | On login page | Check input fields | Input field visible | P1 |
| TC_006 | Verify "Continue" button exists | On login page | Check button | Button visible and clickable | P1 |
| TC_007 | Verify links "Forgot Password?" and "Sign Up" exist | On login page | Check links | Links are visible at bottom | P1 |
| TC_008 | Verify security message display | On login page | Check message | "Secured by" message displayed | P2 |
| TC_009 | Verify development mode message (if applicable) | On dev environment | Inspect page | "Development mode" message visible | P1 |
| TC_010 | Verify "Continue with Google" is clickable | On login page | Click button | Opens Google auth window | P1 |
| TC_011 | Verify Google account login | User has Google account | Use Google login | Successful login; redirected to dashboard/home | P1 |
| TC_012 | Verify login with valid email/username | User registered | Enter credentials | Successful login | P1 |
| TC_013 | Verify error on invalid email format | Enter invalid email | Submit form | Error: "Please match the requested format." | P1 |
| TC_014 | Verify error on invalid password | Enter wrong password | Submit form | Error: "Invalid email or username" | P1 |
| TC_015 | Verify empty input submission blocked | Submit empty fields | Submit form | Error: "Please fill out this field." | P1 |
| TC_016 | Verify password reset page opens | Click "Forgot Password?" | Open page | Page allows password reset | P1 |
| TC_017 | Verify password reset email received | Enter registered email | Send reset code | Email received successfully | P1 |
| TC_018 | Verify form responsiveness | Open login page on different devices | Inspect page | Form responsive and properly aligned | P1 |
| TC_019 | Verify login form works on all screen sizes | Open login page on devices | Inspect page | Smooth UX across all devices | P3 |
| TC_020 | Verify security message on login page | Open login page | Check message | "Secured by" message displayed | P2 |
