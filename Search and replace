import re

#Paragraph provided for search and replace

lorem_ipsum = '''Lorem ipsum dolor sit-amet, consectetur adipiscing elit. Phasellus iaculis velit ac nunc interdum tempor. 
Ut volutpat elit metus, vel auctor enim commodo at. Nunc quis quam non ligula ultricies luctus porta id justo. 
Quisque dapibus est ut sagittis bibendum. Mauris ullamcorper pellentesque porttitor. Ut sit:amet ex nec dolor gravida 
porttitor. Proin at justo finibus justo vestibulum congue. Suspendisse et ipsum et ipsum eleifend dapibus a fermentum 
lacus. Vivamus porta nunc eu nisl sagittis, quis vulputate metus dignissim. Integer non fermentum nisl, id vestibulum 
elit. Sed euismod vestibulum purus ut porttitor. Integer sit-amet mollis neque. Donec sed lacinia diam, ac finibus 
lectus. Mauris tempor ipsum nisl, vitae posuere est lacinia nec. Nam eget euismod odio.'''

#literal charchters
regex="[^a-zA-Z\d]"
#find all literalcharcters in lorem_ipsum
result=re.findall(regex,lorem_ipsum)
#print results

total_char=(len(result))
print("Total charcters: ",int (total_char))
#creates variable for all instances of 'sit-amet'
#special charcter search 

regex="sit[-]amet"
#Assign the outcome to a variable named 'occurrance_sit_amet'
occurrance_sit_amet=re.findall(regex,lorem_ipsum)
#print number of times dashes  apppear between sit and amet 
total_oc=(len(occurrance_sit_amet))
print("Number of occurrances: ",int (total_oc))


# replace "sit-amet" with "sit amet"
replace_results=re.sub(regex,"sit amet",lorem_ipsum)




#print new results
print("\nEdited text: \n"+replace_results)
