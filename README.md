# Title
Food Truck Ordering system

# Description
As part of our Bootcamp Challenge, we will be designing an interactive ordering system from a food truck menu using the skills we've learned in Python coding. 
This code provides a simple way to order a variety of food from the Food Truck Menu. When you run the code, you will see a welcome message: 'Welcome to Rebecca's Food Truck.' You will then be asked to choose a menu category to order from. The available categories are Snacks, Meals, Drinks, and Desserts, each with a corresponding number for selection.

After selecting a category (for example, No. 1 for Snacks), you will be prompted to choose a specific item within that category. Once you make your selection, you will be asked how many of that item you would like to order. After entering the quantity, you will be asked if you would like to continue ordering.

If you type yes 'Y' the process will start over, allowing you to select from the main menu categories again. If you type no, 'N' a receipt will be printed, listing all the items you ordered, their quantities, and the total price.

# Instructions

**Order System**

1. Create an empty list. This list will later store a customer's order in dictionary format, as follows:
   
   ![image](https://github.com/ReccaS/python-challenge-1/assets/168928543/ab3bd079-98c5-4bf4-982b-77b70b51d3bb)
2. After the sub-menu is printed, prompt the customer to enter their selection from the menu, saving it as a variable menu_selection.
3. Use input validation to check if the customer input menu_selection is a number. If it isn't, print an error message. If it is a number, convert the input to an integer and use it to check if it is in the keys of menu_items.
4. If the user input is not in the menu_items keys, print an error. Otherwise, perform the following actions:

     * Get the item name from the menu_items dictionary and store it as a variable.
     * Ask the customer for the quantity of the menu item, using the item name variable in the question, and let them know that the quantity will default to 1 if their input is invalid. Save their answer as a variable called quantity.
     * Check that the customer input is a number. If it isn't, set the quantity to the value 1. If it is a number, convert the variable to an integer.
     * Append the customer's order to the order list in dictionary format with the following keys: "Item name", "Price", and "Quantity. You will need this information to print the receipt at the end of the order. The price should be found in the menu_items dictionary.

 5. Inside the continuous while loop that prompts the customer if they would like to keep ordering, write a match:case statement that checks for y or n (upper or lowercase), and includes a default option if neither letter is entered by the customer. The following actions should be performed for each case:

     * y: Set the place_order variable to True and break from the continuous while loop.
     * n: Set the place_order variable to False, print "Thank you for your order", and break from the continuous while loop.
     * Default: Tell the customer to try again because they didn't type a valid input.

**Order Receipt**

6. Create a for loop to loop through the order list.
7. Inside the loop, save the value of each key as their own variable: item_name, price, and quantity.
8. Calculate the number of empty spaces that should be added to the display so that the receipt uses the following format:

    ![image](https://github.com/ReccaS/python-challenge-1/assets/168928543/d1cc1ace-1a4c-4e92-9968-7092269becd0)
   
10. Create the space strings as their own variables using string multiplication.
11. Print the line for the receipt using the format in Step 8.
12. Upon exiting the for loop, use list comprehension and sum() to calculate the total price of the order and display it to the customer. Make sure you multiply the price by the quantity in your list comprehension.
    
## Contact Information

Created by [ReccaS](https://github.com/ReccaS) - feel free to contact me! 

## References
Python code file from edX Boot Camps LLC, and is intended for educational purposes only.



