        #   TITLE: Grocery Budget Planner 

1.Problem Definition
Many people struggle to keep their monthly grocery spending in check. It’s easy to buy more than you need or lose track of how much everything costs, which often leads to overspending. A Grocery Budget Planner is a tool designed to fix this by helping people easily:
✦︎ Plan their shopping trips in advance.
✦︎ Record what they buy and how much it costs.
✦ Monitor their total spending to stay within their budget.

2.Objectives
𖦹 to design a tool that helps users create a grocery list with item names, price and quantity.
𖦹 to calculate the total cost dynamically.
𖦹 to provide a comparison between planned budget and improve money management habits.

3.Requirements Analysis
❀ The system should allow the user to:
•	Add grocery items with name, price, and quantity
•	Automatically calculate cost of each item
•	Display all stored items and total expense
•	Accept a monthly grocery budget from the user
•	Check whether the total cost is within the budget or exceeding it
•	Exit safely from the program
     
     ✿ Inputs Required:
•	Item name
•	Price
•	Quantity
•	Budget amount
     ✿ Outputs:
•	List of items
•	Total cost
•	Budget status (within or exceeded)

3.Top – Down Design / Modularization
‪‪❤︎ 1. ‬ Menu Display Shows user choices.‬‬‬‬‬‬
‪‪❤︎‬ 2. Item Entry Records item details (name, price, quantity), calculates cost, and updates the list.‬‬‬‬‬‬
‪‪❤︎ 3. ‬Display Prints all recorded items and the total spending.‬‬‬‬‬‬
‪‪❤︎ 4. ‬Budget Checking Accepts a user-defined budget and compares it against the total spending.‬‬‬‬‬‬
‪‪❤︎‬ 5. Exit Module Terminates the program loop. ‬‬‬‬‬‬


4.Algorithm Development
Algorithm for Grocery Budget Planner
1.	Start
2.	Create an empty list grocery and set total = 0
3.	Repeat the following using a loop:
a. Display menu
b. Take user choice
c. If choice = 1:
o	Read item name, price, qty
o	Compute cost = price × qty
o	Add item to list
o	Update total
           d. If choice = 2:
o	Display the stored grocery list
o	Display total cost
           e. If choice = 3:
o	Read user budget
o	Compare budget with total
o	Display appropriate message 
           f. If choice = 4:
o	Exit loop
g. Else display “Invalid choice”
4.	End

5.	Implementation (Code)
           Short, simple, handwritten code:
grocery = []
total = 0

while True:
    print ("1. Add Item")
    print ("2. View List")
    print ("3. Check Budget")
    print ("4. Exit")

    choice = int (input ("Enter Choice: "))

    if choice == 1:
        name = input ("Item name: ")
        price = float (input ("Price: "))
        qty = int (input ("Qty: "))
        cost = price * qty

        Grocery. append([name, price, qty, cost])
        total = total + cost
        print ("Item Added\n")

    Elif choice == 2:
        print ("\n Grocery List:")
        for g in grocery:
            print (g [0], "| Price:", g [1], "| Qty:", g [2], "| Total:", g [3])
        print ("Total =", total, "\n"
Elif choice == 3:
        b = float (input ("Enter Budget: "))
        if total > b:
            print ("You Crossed Budget by", total - b, "\n")
        else:
            print ("Within Budget. Balance =", b - total, "\n")

    Elif choice == 4:
        break

    else:
        print ("Invalid Choice\n")

6.	Testing And Refinement
Test Case 1

Input:
Add item → Rice, price = 40, qty = 2

Expected output:
Cost = 80 added
Total = 80


Test Case 2
Input:
Budget = 100

Expected Output:
Within budget → Balance = 20
________________________________________
Test Case 3
Input:
Budget = 50

Expected Output:
Exceeded budget by 30


Testing Summary
★ Items add correctly
★ Total cost updates properly
★ Budget comparison works
★ Program handles invalid choices





7.	Screenshots 
All screenshots are available in the /screenshots folder.
Examples Includes:
. Input Screenshot
. Output Screenshot

8.Screen Recording
. A short recording demonstrating code execution is available in the /recordings folder.



8.	Conclusion
This project helped me create a simple Grocery Budget Planner that allows users to add items, check total cost, and compare it with their monthly budget. It is easy to use and helps in managing daily grocery expenses. By using basic Python concepts like loops, lists, and conditions, the program works smoothly and solves a real-life problem in a simple way.

              
                                 THANK YOU

