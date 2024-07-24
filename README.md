# Expence---Tracker

## Aim:
TO create a python code for calculating the expences(i.e  an expence tracker).

## Apparatus:
1. python compiler (or) python 3.7 installation
2. window 10 or above


## Algorithm:

1. Define the Expense Class.
2. Create a List to Store Expenses.
3. User Interface (Optional).
4. Input and Adding Expenses.
5. Viewing Expenses Provide options to view all expenses, expenses by category, or expenses within a date range.
6. Editing and Deleting Expenses includes allowing the user to modify or delete existing expenses.
7. Calculating Totals and Averages .Calculate the total expenses, average expenses, and expenses by category.
8. Display the overall expence by category.
9. End the progran.

## Program:

```
class Expense:
    def __init__(self, date, description, amount, category):
        self.date = date
        self.description = description
        self.amount = amount
        self.category = category

expenses = []

def add_expense():
    date = input("Enter the date (YYYY-MM-DD): ")
    description = input("Enter the description: ")
    amount = float(input("Enter the amount: "))
    category = input("Enter the category: ")
    expense = Expense(date, description, amount, category)
    expenses.append(expense)
    print("Expense added successfully!")

def view_expenses():
    print("Date\tDescription\tAmount\tCategory")
    for expense in expenses:
        print(f"{expense.date}\t{expense.description}\t{expense.amount}\t{expense.category}")

def calculate_total_expenses():
    total = sum(expense.amount for expense in expenses)
    print("Total Expenses:", total)

while True:
    print("\nExpense Tracker")
    print("1. Add Expense")
    print("2. View Expenses")
    print("3. Calculate Total Expenses")
    print("4. Exit")
    choice = input("Enter your choice: ")

    if choice == "1":
        add_expense()
    elif choice == "2":
        view_expenses()
    elif choice == "3":
        calculate_total_expenses()
    elif choice == "4":
        break
    else:
        print("Invalid choice. Please try again.")
```


## Output:

# Add expence:

![add expence](https://github.com/user-attachments/assets/9937e85e-be7f-4997-a562-b94bf3740ab2)


# View expence:

![view expence](https://github.com/user-attachments/assets/1136d15d-099a-43fc-92ea-2d768872c380)


# Total expence:

![total](https://github.com/user-attachments/assets/633e25de-cc98-461d-807d-642822158be7)


# Exit from the progran:

![exit](https://github.com/user-attachments/assets/78bccf98-1bb1-443f-b25a-1a4d6ff1ac39)


## Result:
Thus the program for creating an expence tracker is excuted successfully.

