# Loan Qualification Checker

This project is a simple JavaScript application that determines loan eligibility based on an applicant's annual income and credit score. The application evaluates eligibility for three types of loans:

1. **Duplex Loan**
2. **Condo Loan**
3. **Car Loan**

## Features

- Checks eligibility criteria for duplex, condo, and car loans.
- Uses predefined minimum income and credit score thresholds.
- Returns a message indicating which loans the applicant qualifies for.
- Provides a default message if the applicant doesn't meet any loan criteria.

## Code Explanation

### Constants

- `minIncomeForDuplex` and `minCreditScoreForDuplex` define the minimum income and credit score needed for a duplex loan.
- `minIncomeForCondo` and `minCreditScoreForCondo` define the requirements for a condo loan.
- `minIncomeForCar` and `minCreditScoreForCar` define the requirements for a car loan.

### Function: `getLoanMessage`

This function takes two parameters:

- `annualIncome`: The applicant's annual income.
- `creditScore`: The applicant's credit score.

The function evaluates the input values against the loan requirements and returns one of the following messages:

1. "You qualify for a duplex, condo, and car loan."
2. "You qualify for a condo and car loan."
3. "You qualify for a car loan."
4. "You don't qualify for any loans."

### Example Usage

```javascript
const duplexLoanMsg = getLoanMessage(85000, 850);
const condoLoanMsg = getLoanMessage(65000, 690);
const carLoanMsg = getLoanMessage(45000, 660);
const noLoanMsg = getLoanMessage(25000, 550);

console.log(duplexLoanMsg); // Output: "You qualify for a duplex, condo, and car loan."
console.log(condoLoanMsg); // Output: "You qualify for a condo and car loan."
console.log(carLoanMsg);   // Output: "You qualify for a car loan."
console.log(noLoanMsg);    // Output: "You don't qualify for any loans."
```

## Requirements

- **Programming Language**: JavaScript
- **Runtime Environment**: Any environment that supports JavaScript execution (e.g., Node.js, browser console).

## How to Use

1. Define the `annualIncome` and `creditScore` for the applicant.
2. Call the `getLoanMessage` function with these values.
3. Display or use the returned message as needed.

## Customization

You can customize the minimum income and credit score thresholds by modifying the constants at the beginning of the code.

For example, to change the minimum income for a car loan:

```javascript
const minIncomeForCar = 35000; // Updated value
```

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute the code.
