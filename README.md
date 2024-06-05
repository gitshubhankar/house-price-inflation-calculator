# House Price Inflation Calculator

This Python script calculates the adjusted price of a house after a certain number of years, taking inflation into account.

## Usage

1. Clone or download the repository.
2. Make sure you have Python installed on your system.
3. Execute by filling input values after running the following code:

```bash
 def calculate_adjusted_price(initial_price, inflation_rate, years):
    adjusted_price = initial_price * (1 + inflation_rate) ** years
    return adjusted_price

def main():
    initial_price = float(input("Enter the initial price of the house: ₹   "))
    inflation_rate = float(input("Enter the annual inflation rate (in decimal): "))
    years = int(input("Enter the number of years: "))
    
    adjusted_price = calculate_adjusted_price(initial_price, inflation_rate, years)
    
    print("The adjusted price of the house after {} years is: ₹{:,.2f}".format(years, adjusted_price))

if __name__ == "__main__":
    main()
