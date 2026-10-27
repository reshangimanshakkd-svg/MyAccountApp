# MyAccountApp - Mobile Application Development (Practical 04)

A React Native mobile application built using **Expo Router** to demonstrate form handling, validation, and parameter passing between screens.

## 🚀 Key Features

### 1. Registration Screen (`app/index.js`)

- Captures user details: **Username**, **Email**, **Phone Number**, **Password**, **Confirm Password**, and **Year of Birth**.
- **Form Validation**:
  - Ensures no fields are left blank.
  - Verifies that `Password` and `Confirm Password` match.
  - Validates **Year of Birth** input (ensures it is a valid numeric year).

### 2. Review Screen (`app/review.js`)

- Retrieves parameters passed from the Registration screen using `useLocalSearchParams`.
- Displays user details along with the **calculated Age**.
- **Conditional Navigation (18+ Check)**:
  - If the calculated age is under 18, shows an Alert warning that the user must be at least 18 years old to proceed.
- Provides an **Edit Info** button (`router.back()`) to edit details and a **Confirm & Submit** button to proceed.

### 3. Success Screen (`app/success.js`)

- Displays a personalized completion message welcoming the user by name.

## 🛠️ Setup & Execution

1. Install dependencies:
   ```bash
   npm install
   ```
