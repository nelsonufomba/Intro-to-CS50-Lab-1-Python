# Intro-to-CS50-Lab-1-Python
Population Growth
#Input 
List= []
startsize = input("Enter the population startsize: ")
startsize = int(startsize)
if startsize < 9:
    print("Invalid Input")
    startsize = input("Enter the population startsize above 9:")
endsize = input("Enter the population endsize: ")
endsize = int(endsize)
if endsize <= startsize:
    print("Invalid Input")
    endsize = input("Enter the population endsize greater than startsize:")

#Main code
n = startsize
while (n < endsize):
    n = n + (n/3) - (n/4)
    List.append(n) #adds the population size to the array
    if( n > endsize):
        break
years= len(List) 

#Output
print("The number of years is : ",years)
    
