#Prompt user to input a rental option
rentalCode =input("(B)udget, (D)aily, or (W)eekly rental?\n")
#Prompt user based on rental option  
if rentalCode =="B" or rentalCode =="D":
	rentalPeriod=int(input("Number of Days Rented:\n"))
if rentalCode=="W":
	 rentalPeriod=int(input("Number of Weeks Rented:\n"))
#If inccorect input try a correct input 
### this function never worked right so its chopped for now	
#Prompt for Odometer stats
odoStart=int(input("Starting Odometer Reading:\n"))
odoEnd=int(input("Ending Odometer Reading:\n"))
#calculate total miles from odometer inputs
totalMiles=int(odoEnd)-int(odoStart)
##Prices for Input
budget_charge = 40.00
daily_charge = 60.00
weekly_charge = 190.00
#Based on price and rental code calculate a base charge
if rentalCode == 'B':
  baseCharge = rentalPeriod * budget_charge
elif rentalCode=='D':
  baseCharge=rentalPeriod* daily_charge
elif rentalCode=='W':
	 baseCharge=rentalPeriod* weekly_charge
    
if rentalCode == 'B':
#Cost for miles driven
  mileCharge=0.25*totalMiles
#Average miles driven in a day   
averageDayMiles=totalMiles/rentalPeriod
if rentalCode == "D":
#If the average is under 100 miles no mile charge
    averageDayMiles = int(totalMiles) / int(rentalPeriod)
if averageDayMiles <= 100:
  extraMiles = 0
#If the average is over 100 add an extra mile charge 
elif averageDayMiles > 100:
  extraMiles = averageDayMiles - 100
mileCharge = 0.25 * extraMiles 

if rentalCode =="W" and averageDayMiles > 900:
#If the average is over 900 a day add  additioncal charge 
  milecCharge = rentalPeriod * 100
elif rentalCode =="W" and averageDayMiles<= 900:
#If the average is under 900 a day no additioncal charge 
  milecCharge=0
#Calculate total amunt due 
ammountDue=float(baseCharge)+float(mileCharge)
#Print stats 
print("Rental Summary")
print("Rental Code:        "+str(rentalCode))
print("Rental Period:      "+str(rentalPeriod))
print("Starting Odometer:  "+str(odoStart))
print("Ending Odometer:    "+str(odoEnd))
print("Miles Driven:       "+str(totalMiles))
#                  special formating for decimal
print("Amount Due:       "+ "${:,.2f}" .format(ammountDue))
