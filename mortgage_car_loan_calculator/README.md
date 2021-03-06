# Problem: Mortgage / Car Loan Calculator

> You'll need three pieces of information
* The loan amount
* The annual Percentage Rate (APR)
* The loan duration 


> From the above, you'll need to calculate the following two things:
* Monthly interest rate
* Loan duration in months


### You can use the following formula:

```rb
m = p * (j / (1 - (1 + j)**(-n)))
```
> m = monthly payment
> p = loan amount
> j = monthly interest rate
> n = loan duration in months


# Solution: Mortgage / Car Loan Calculator (PEDAC)

### Problem
Problem statement is clear and explicit on the problem, which is to collect three inputs (amount, annual_percent, duration), then calculate and provide the monthly interest rate, and loan duration in months.
*The problem statement does not explicitly say that I cannot simply ask for user for loan duration in months - from the beginning - so I will.

### Examples / test cases
calculate_monthly_interest_rate()


### Data-structures
#### Input
* String

#### Processing
* Integer for number of months.   
* Float for annual percentage rate.  
* Float for loan amount.  

#### Output
* String monthly for interest rate.  
* String for loan duration in months.

### Algorithm

START of program.  
PRINT the welcome statement.   
UNTIL user has supplied all three valid inputs.  
GET and VALIDATE(must be Float) loan_amount.  
GET and VALIDATE(must be Float) annual_percentate_rate.  
GET and VALIDATE(must be Integer) loan_duration_in_months.  
CALC monthly interest - ref formula below.  
PRINT The loan duration.  
PRINT monthly interest rate.  

```ruby
  def calculate_monthly_interest_rate(rate)
    rate_to_decimal = rate / 100
    monthly_rate = rate_to_decimal / 12
  end
```
END UNTIL.  
END of program.  

### Code
>lib/calculator.  
>spec/calculator_spec (* comment out run_program in main before running specs). 
