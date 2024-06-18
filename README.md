# restaurent_menu
Structure Definitions
items: This structure holds information about individual items, including the item name, price, and quantity.
orders: This structure contains details about an order, including the customer name, date, number of items, and an array of items structures.
Functions
generateBillHeader: This function prints the header of the bill, displaying the restaurant name, date, and customer name.
generateBillBody: This function prints each item's details, including the name, quantity, and total price for that item.
generateBillFooter: This function prints the bill's footer, showing the subtotal, discount, net total, and applicable taxes, culminating in the grand total.
Main Function Workflow
Dashboard: The program starts by displaying a menu with options to:

Generate a new invoice.
Show all invoices.
Search for a specific invoice by customer name.
Exit the program.
Option 1: Generate Invoice:

Prompts the user for customer name and date.
Asks for the number of items and details for each item (name, quantity, and unit price).
Generates and prints the invoice using the generateBillHeader, generateBillBody, and generateBillFooter functions.
Optionally saves the invoice to a file named "RestaurantBill.dat".
Option 2: Show All Invoices:

Reads and displays all saved invoices from the "RestaurantBill.dat" file, showing each invoice's details using the bill generation functions.
Option 3: Search Invoice:

Prompts the user for a customer name and searches for matching invoices in the "RestaurantBill.dat" file.
If found, displays the invoice details; otherwise, informs the user that no such invoice exists.
Option 4: Exit:

Exits the program.
Additional Details
The program uses fgets for input to handle strings with spaces.
The invoice details are stored in a binary file "RestaurantBill.dat".
Discounts and taxes are applied in the footer calculation.
Sample Usage
Generating an Invoice:

Enter customer details and items.
View the generated invoice on the screen.
Save the invoice if desired.
Viewing All Invoices:

Select the option to display all past invoices saved in the file.
Searching for an Invoice:

Enter a customer name to search for and display their invoice if it exists.
This program efficiently handles basic restaurant billing tasks, making it easy to generate, view, and search invoices.
