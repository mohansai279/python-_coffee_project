# python-_coffee_project
The Coffee Machine project is a simulation of a software-driven coffee machine that manages inventory, processes payments, and serves various coffee drinks. The program is interactive and runs in a continuous loop, responding to user commands while also providing administrative functionalities.
# Coffee Machine

```bash
python 9.coffe_machine_Project.py
```

Follow the prompts to select your coffee and make payments. Enjoy your coffee!

## Detailed Logic Breakdown

### Step 1: Defining the Machine's "Brain": The Data Structures

- **Menu (The Recipe Book)**:
  - A nested dictionary containing coffee types as keys and their ingredients and costs as values.

- **Resources (The Inventory)**:
  - A dictionary representing the current stock of ingredients.

- **Profit (The Cash Box)**:
  - A numeric variable initialized to 0, tracking total profit.

### Step 2: The Machine's Capabilities: The Core Functions

- **show_menu()**: Displays available coffees and their costs.
  
- **check_resources(order_ingredients)**: Checks if enough ingredients are available for the selected coffee.

- **process_coins(coffee_cost)**: Handles user coin input and calculates total money received.

- **is_payment_successful(money_received, coffee_cost)**: Verifies payment and updates profit.

- **make_coffee(coffee_name, coffee_ingredients)**: Deducts ingredients from inventory and confirms coffee preparation.

### Step 3: The Machine's Main Operation: The while Loop

- The main loop is controlled by a boolean flag (`is_on`), running continuously until set to False.

- Each iteration calls `show_menu()` and prompts the user for their choice.

- The command router directs the flow based on user input, handling commands for turning off the machine, reporting status, processing drink orders, or managing invalid inputs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
