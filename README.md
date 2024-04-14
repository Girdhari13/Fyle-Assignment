# Tax-Calculator
This is a simple tax calculator implemented in JavaScript. It calculates the overall income after considering gross income, extra income, age group and deductions. Additionally, it provides validation for input fields.

## References & Requirements
- The tax calculation works based on this formula -
    - Overall income (after deductions) under 8 (≤) Lakhs is not taxed.
        - Ex - if Gross Annual Income + Extra Income - Deductions =  6 Lakhs, no tax
        - if Gross Annual Income + Extra Income - Deductions =  9 Lakhs, tax
    - Income over 8 (>) Lakhs, the amount over 8 Lakhs is taxed at
        - 30% for people with age < 40
        - 40% for people with age ≥ 40 but < 60
        - 10% for people with age ≥ 60
        - Example
            - Age = 34, Income = 40 Lakhs, no deductions, tax = .3 * (40 - 8) = .3 * 32 = 9.6 Lakhs
- Do not restrict the user from entering incorrect values like characters in the number fields
    - Highlight an error icon to the right of the input field (shown as an example in the above image as a circle with `!`). Hovering over it should show the error in a tooltip
    - If no errors are present, don't show the error icon
    - This should be present in all the number fields
- The age dropdown field should have 3 values -
    - <40
    - ≥ 40 & < 60
    - ≥ 60
    - If the user has not entered this value and clicks on submit, show an error icon hovering over which should show that the input field is mandatory
- Error icons should not be visible in the form by default.
- Clicking on submit should show a modal which would show the final values based on the above calculations.

## Assumptions
- **Input Validation:**
  - Input values are validated on focus, change, and when the submit button is clicked.
  - Errors are displayed to the user under the following conditions:
    - Typing a number less than zero results in an error message "Please type non-negative numbers".
    - Clicking on an input field and not typing anything or leaving any field empty and clicking the submit button results in an error message "This input field is mandatory".
    - Typing anything other than a number results in an error message "Please type numbers only".
- **Overall Income Calculation:**
  - If the sum of gross income, extra income, and deductions is less than or equal to 8 lakhs, the overall income is displayed as the sum of gross income and extra income.

## Run Locally
To run your application locally, follow these steps:
1. **Download the Code**: Download the HTML, CSS, and JavaScript files to your local machine.
2. **Open HTML File**: Open the HTML file in your preferred web browser. You can do this by double-clicking the HTML file or right-clicking and selecting "Open with" and choosing your web browser.
3. **Ensure Internet Connection**: Since your application uses Bootstrap icons via CDN links, ensure that you have an internet connection while running the application locally. If you don't have an internet connection, the icons may not be visible.
4. **Interact with the Application**: Once the HTML file is opened in your web browser, you can interact with the tax calculator just like you would on a live website. Input values, click the submit button, and verify that the calculations and error messages work as expected.

## Usage
To use the tax calculator:
- Input the gross income, extra income, age group, and total deductions.
- Click the submit button to calculate the overall income and display the result.
- If any input is invalid, error messages will be shown to guide the user on how to correct the inputs.

## Test Cases:

#Case No:1
<img width="353" alt="Screenshot 2024-04-14 165550" src="https://github.com/Girdhari13/Fyle-assignment/assets/156057543/a35fb369-a8a4-4c78-aecc-6ca9357c8dd3">
#Case No:2
<img width="314" alt="Screenshot 2024-04-14 165521" src="https://github.com/Girdhari13/Fyle-assignment/assets/156057543/49128259-dab1-4aef-b35f-48de20f39746">
#Case No:3
<img width="343" alt="Screenshot 2024-04-14 165452" src="https://github.com/Girdhari13/Fyle-assignment/assets/156057543/83373083-74bd-41d6-81eb-aec2a3c98384">
#Case No:4
<img width="323" alt="Screenshot 2024-04-14 165413" src="https://github.com/Girdhari13/Fyle-assignment/assets/156057543/7dbaf11a-0d58-4561-bad6-417c3e571e5c">
#Case No:5
<img width="266" alt="Screenshot 2024-04-14 165341" src="https://github.com/Girdhari13/Fyle-assignment/assets/156057543/502a4c34-654a-4ce9-a354-842c77c00a2c">
#Case no:6
<img width="312" alt="Screenshot 2024-04-14 165257" src="https://github.com/Girdhari13/Fyle-assignment/assets/156057543/0ad6294c-ce9b-4996-9a86-2ac95f186f28">
#Case No:7
<img width="272" alt="Screenshot 2024-04-14 163635" src="https://github.com/Girdhari13/Fyle-assignment/assets/156057543/0e792d25-c0c1-457a-b625-b3be7ba3865c">
