# cis129_lab03_coffeeShop.py
# Define prices
coffee_price = 5.00
muffin_price = 4.00
tax_rate = 0.06

# Welcome message
print("***************************************")
print("My Coffee and Muffin Shop")

# Get user input
num_coffees = int(input("Number of coffees bought? "))
num_muffins = int(input("Number of muffins bought? "))

# Calculate costs
subtotal_coffees = num_coffees * coffee_price
subtotal_muffins = num_muffins * muffin_price
subtotal = subtotal_coffees + subtotal_muffins
tax = subtotal * tax_rate
total = subtotal + tax

# Display receipt
print("***************************************")
print("My Coffee and Muffin Shop Receipt")
print(f"{num_coffees} Coffee at ${coffee_price:.2f} each: $ {subtotal_coffees:.2f}")
print(f"{num_muffins} Muffins at ${muffin_price:.2f} each: $ {subtotal_muffins:.2f}")
print(f"6% tax: $ {tax:.2f}")
print("---------")
print(f"Total: $ {total:.2f}")
print("***************************************")
