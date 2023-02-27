# Automated-Coffeeshop
Automated coffee shop Python code on GitHub - experience the future of coffee ordering and delivery.

print("Hello! Welcome to Our shop!!!!!!")
name = input("What is your name?\n ")
if name == "Mark" or name == "Ashik" or name == "Loki" :
  evilstatus = input("Are you that " + name + ", who haven't paid the bill off his last coffee?\n ")
  if evilstatus == "Yes":
    good_deeds = int(input("Now pay your debt first. It was BDT120. \n "))
  if evilstatus == "Yes" and good_deeds < 120:
    print("You are not allowed here " + name + ". Get out!!!")
    exit()
  else:
    print("Ok " + name + ", Thank you so much for coming. Please have a seat!\n ")
else:
  print("Hello " + name + ", Thank you so much for coming our shop")
Menu = "Espresso, Latte, Black Coffee, Cappuccino, Iced Coffee, Americano"
print(name + ", What would you like to order from our menu?\nOur todays menu is " + Menu )
order = input ("\n ")
if order == "Latte" :
  price = 120
elif order == "Black Coffee" :
  price = 60
elif order =="Espresso" :
  price = 80
elif order == "Cappuccino" :
  price = 100
elif order == "Iced Coffee" :
  price = 110
elif order == "Americano" :
 price = 150
else :
  print("Sorry we don't have that!!") 
  exit()
quantity = input("How many cups of " + order + " would you like?\n ")
cream = input("Sounds good " + name + ". You have choose " + quantity + " cup of " + order + ". Do you want to add extra whipped cream for BDT30 per coffee?\n ")
if cream == "Yes" :
  total = (price * int(quantity)) + (30 * int(quantity))
  print("Ok, " + name + ". Your total bill is BDT" + str(total) + ". We will have your coffee in a moment")
if cream == "No" :
    total = price * int(quantity)
    print("Ok, " + name + ". Your total bill is BDT" + str(total) + ". We will have your coffee in a moment")
print("(Coffee is making.........)\n.\n.\n.\n ")
wait = input("(after 2 minutes)\nWe are extremely sorry " + name + ". Can you please wait 5 minutes more?\n ")
if wait != "No" :
  print("Thank you so much for understanding the circumstances.\n ")
print("(After a few minutes)\nHere is your coffee, " + name + ". Enjoy!\n")
input("Submit your review.\n ")
print("Thanks for your kind review.")
exit()
