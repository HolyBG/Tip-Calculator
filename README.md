# Tip Calculator

## Objective

Create a simple python script that will calculate the bill that would be paid with multiple people paying AND with the tip!

### Skills Learned

- Strings, Integers, & Floating Point Datatypes
- Data Manipulation
- Mathematical Operations
- f-Strings
- Formatting Outputs

### Tools Used

- Python 3.12

## Steps
```
#Welcome Message
print("Welcome to the tip calculator!")

#input for total bill
total_bill = input("What was the total bill? $")

#input for tip percentage
tip_percentage = input("How much would you like to leave as a tip? 10, 12, or 15? ")

#input for the number of people splitting the bill
number_of_people = input("How many people are splitting the bill? ")

#converting the inputs to floats
total_bill_float = float(total_bill)
tip_percentage_float = float(tip_percentage)
number_of_people_float = float(number_of_people)

#calculating the tip amount
tip_amount = total_bill_float * (tip_percentage_float / 100)

#calculating the total bill with tip
total_bill_with_tip = total_bill_float + tip_amount

#calculating the amount each person should pay
amount_per_person = total_bill_with_tip / number_of_people_float

#formatting the amount each person should pay to 2 decimal places
final_amount = "{:.2f}".format(amount_per_person)

#printing the amount each person should pay
print(f"Each person should pay: ${final_amount}")
```
