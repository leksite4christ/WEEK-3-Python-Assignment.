# WEEK-3-Python-Assignment.
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount = price * (discount_percent / 100)
        return price - discount
    else:
        return price

# Prompt the user to enter the original price
price = float(input("Enter the original price: "))

# Prompt the user to enter the discount percentage
discount_percent = float(input("Enter the discount percentage: "))

# Calculate the final price after applying the discount
final_price = calculate_discount(price, discount_percent)

# Print the final price
if final_price == price:
    print(f"No discount applied. The original price is: ${price:.2f}")
else:
    print(f"The final price after applying the discount is: ${final_price:.2f}")

