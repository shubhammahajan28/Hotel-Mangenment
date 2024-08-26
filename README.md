# Hotel-Managenment
Menu ={
    "Chicken Thali":150,
    "Butter Nan":20,
    "Paneer Masala":90,
    "Paneer Aaganra":120,
    "Roti":10,
    "Chicken special thali":150,

}
print("''''Welcome to Hotel Bhau''''\n** Menu Card **")

print("Chicken Thali : 150 Rs\nButter Nan: 20 RS \nPaneer Masala :90 Rs \nPaneer Aaganra:120 Rs\nRoti:10 RS\nChicken Special Thali:150 Rs")

Total = 0

item_1 = input("Enter the name of item you want to order=")
if item_1 in Menu:
    Total += Menu[item_1]
    print(f"Your item{item_1}has been added to your order")
else:
    print(f"Oredered item{item_1} is not available yet")

another_order = input("Do you want another item? (Yes/No)")
if another_order == "Yes":
    item_2 = input("Enter the name of Second item =")
    if item_2 in Menu:
        Total += Menu[item_2]
        print(f"Item{item_2}has added to order")
    else:
        print(f"Oredered item{item_2} is not available yet")

print(f"The total amount of item to pays is {Total}")
