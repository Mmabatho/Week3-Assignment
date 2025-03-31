def calculate_discount(price,discount_percentage): #Lets us define the function and its parameters
    if discount_percentage >= 20: #Here we check the condition of the discount pecentage
        discount_amount = (price * discount_percentage)/100 #Allows to calculate the discounted price
        new_price = price - discount_amount #checking the new price without the discounted price
        return new_price #showing the new price
    else:
        return price #showing the default price
normal_price = float(input('Enter Price: ')) #For capturing the product price
percent = float(input('Enter a percentage: ')) #For capturing the price percentage discount
price = calculate_discount(normal_price, percent ) #Calls the price 
print(price)
