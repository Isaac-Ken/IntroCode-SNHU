#account balance 
account_balance = float(00.00)
mybalance = float(00.00)

#exit value
stop =False
#While loop
while not stop:
	

	
	
	#deposit function
	def deposit():
	#collect customer input
	  deposit_ammount=float(input("How much would you like to deposit today?\n"))
	  #Calculate New Balnce
	  mybalance=account_balance+ deposit_ammount
	  print("Deposit was $%.2f, current balance is $%.2f"%(deposit_ammount,mybalance))
	  
	  #printbalance function
	def printbalance():
	  print("Your current balance:\n%.2f"%(mybalance))
	  
	#withdraw function
	def withdraw(mybalance):
	#collect cutomer input
	  withdraw_amount=float(input("How much would you like to withdraw today?\n"))
	#OverDraw Results
	  if withdraw_amount >mybalance:
	    print("$%.2f is greater than your account balance of $%.2f"%(withdraw_amount,mybalance))
	#Sucesfull Withdraw Results,calculate new balnce
	  else:
	    account_balance=mybalance-withdraw_amount
	    print("Withdrawal amount was $%.2f, current balance is $%.2f"%(withdraw_amount,account_balance))
	#prompt user for Input option
	userchoice = input("What would you like to do? (press Q to quit)\n(B)alance,(D)eposit,(W)ithdraw\n")
	#options to call for function 
	if (userchoice == 'D'):
	  deposit ()
	elif (userchoice=="B"):
	  printbalance()
	elif (userchoice=="W"):
	  withdraw(mybalance)
	#exit 
	elif userchoice=="Q":
	   print("Thank you for banking with us.")
	   
	

    
    
 #Enter Next Items
response=input("Would you like to enter another item?\nType 'c' for continue or 'q' to quit:\n")
#Exit While loop
if response=="q":
	stop=True
#continue While loop 
else:
	stop=False
