
# Food Truck Order System

## Introduction

Welcome to the Variety Food Truck! Our food truck offers a diverse selection of delicious snacks, meals, drinks, and desserts. Whether you're in the mood for a quick snack, a hearty meal, a refreshing drink, or a sweet treat, we've got something for everyone. Our convenient order system allows you to browse the menu, make your selections, and receive a receipt detailing your order and total cost.

## Project Overview

This project is a Python-based order system for the Variety Food Truck. The system enables customers to interactively choose items from the menu, specify quantities, and generate a formatted receipt. The program emphasizes input validation, data handling, and formatted output, ensuring a smooth and user-friendly experience.

## Features

- **Menu Display**: Categorized menu showing Snacks, Meals, Drinks, and Desserts.
- **Interactive Ordering**: Customers can select items, specify quantities, and add them to their order.
- **Input Validation**: Ensures all inputs (menu selection, item selection, quantity) are valid.
- **Formatted Receipt**: Generates and displays a receipt with itemized costs and a total.

## Usage

1. **Running the Program**: 
   - Execute the Python script to start the program. The program greets the customer and displays the available menu categories.
   
2. **Selecting Items**:
   - The customer selects a menu category by entering its number. They can then choose an item within that category.
   - The program prompts for the quantity of the selected item. If the input is invalid, it defaults to 1.

3. **Finalizing the Order**:
   - After selecting items, the customer can choose to continue ordering or finalize the order.
   - Upon finalizing, the program generates a formatted receipt with all items, their prices, quantities, and the total cost.

## Project Requirements

### Order System

- **Order List Initialization**: An order list is initialized to store the customer's order in dictionary format.
- **Menu Selection Prompt**: The user is prompted to select a menu item, stored in the `menu_selection` variable.
- **Input Validation**: The `menu_selection` input is checked as a number, and an error is printed if it is not.
- **Integer Conversion**: `menu_selection` is converted to an integer after validation.
- **Selection Verification**: An if-else statement checks if `menu_selection` is in the `menu_items` keys, and an error is printed if it isn't.
- **Item Name Extraction**: The item name is extracted from the `menu_items` dictionary and stored as a variable.
- **Quantity Prompt and Validation**: The customer is prompted for a quantity, which defaults to 1 if the input is invalid.
- **Order List Update**: The selected item, price, and quantity are appended to the order list in dictionary format.
- **Match-Case Statement**: A `match-case` statement handles whether the customer continues ordering or finishes.
- **Case Conversion**: The match-case statement converts user input to lowercase before checking the case.

### Order Receipt

- **Order Loop**: A `for` loop is used to loop through the order list and process each item.
- **Key Extraction**: The value of each key in the order dictionary (item name, price, quantity) is saved as a variable.
- **Formatting Calculations**: The number of formatting spaces is correctly calculated to ensure proper alignment.
- **Space Strings**: Space strings are created using string multiplication to align the receipt output.
- **Receipt Printing**: The order is printed with item name, price, and quantity aligned correctly.
- **Total Cost Calculation**: List comprehension is used to calculate the total price of the order.
- **Total Cost Output**: The total price is printed at the end of the receipt.

## Example Usage

### Example Order Process

```python
Welcome to the variety food truck.
From which menu would you like to order? 
1: Snacks
2: Meals
3: Drinks
4: Dessert
Type menu number: 1
You selected Snacks
What Snacks item would you like to order?
Item # | Item name                | Price
-------|--------------------------|-------
1      | Cookie                   | $0.99
2      | Banana                   | $0.69
3      | Apple                    | $0.49
4      | Granola bar              | $1.99
Please input the number corresponding to your menu choice: 1
How many Cookie would you like to order? 2
Would you like to keep ordering? (Y)es or (N)o n
Thank you for your order.

This is what we are preparing for you.

Item name                 | Price  | Quantity
--------------------------|--------|----------
Cookie                    | $0.99  | 2        

Total cost: $1.98
```

### Example Output

After placing an order and completing the process, the customer receives a receipt like the following:

```
This is what we are preparing for you.

Item name                 | Price  | Quantity
--------------------------|--------|----------
Cookie                    | $0.99  | 2        

Total cost: $1.98
```

## License

This project is under the GNU General Public License (GPL)
