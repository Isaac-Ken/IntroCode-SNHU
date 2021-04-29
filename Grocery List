#Creating Dictionary
grocery_item = {} 

#Creating list
grocery_history = [] 
#exit value
stop =False
#While loop
while not stop:

    #Collect user Data
    name=input("Item name:"+"\n")
    
    quantity= input("Quantity purchased:"+" \n")
    
    cost=input("Price per item:"+" \n")

   #adding items to list
    grocery_item={"name":name,"quantity":int(quantity),"cost":float(cost)}
    #remove data from list and add to dictionary 
    grocery_history.append(grocery_item)

    #Enter Next Items
    response=input("Would you like to enter another item?\nType 'c' for continue or 'q' to quit:\n")
   #Exit While loop
    if response=="q":
     stop=True
    #continue While loop 
    else:
      stop=False

  
#End Variable  
grand_total=0
 
#for object in dictionary
for item in grocery_history:
  
#acess values from dictionary
  item_total=item["quantity"]*item["cost"]
#Calculate total
  grand_total+=item_total 
#Format Output
  print('%d %s @ $%.2f ea $%.2f' %(item["quantity"],item["name"],item["cost"],item_total))
  
  #set to 0
  item_total=0
#Format Total
print("Grand total: $%.2f" % grand_total)
