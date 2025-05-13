# hotel_menu
it's a mini project about hotel/restaurant menu for costumer
# define the menu of restro
menu = {
    "pizza": 40,
    "pasta": 50,
    "burger": 60,
    "salad": 70,
    "coffe": 80,
}
# greet
print("welcome to PRIYANSHU's restaurant")
print("pizza: Rs40\npasta: Rs50\nburger: Rs60\nsalad: Rs70\ncoffe: Rs80")

order_total = 0

item_1 = input("enter your order= ")
if item_1 in menu:
    order_total += menu[item_1]
    print(f"your item {item_1} has been added to order")
else:
    print("this item is not available")

another_order = input("Do you want to oder something else? (yes/no) = ")
if another_order == "yes":
    item_2 = input("enter your second order= ")
    if item_2 in menu:
        order_total += menu[item_2]
        print(f"your item {item_2} has been added to order")
    else:
        print(f"your item {item_2} is not available")
        
print(f"the  total amount of order to pay is {[order_total]}RUPEES")
print("thank you\n\tcome again")
