# Intro-to-CS50-Lab-1 and problem set mario-Python
Population Growth
#Input 
#Input 
List= []
startsize = int(input("Enter the population startsize: "))
while (startsize<9) :
    print("Invalid Input")
    startsize = int(input("Enter the population startsize:"))
    if (startsize >= 9):
        break
endsize = int(input("Enter the population endsize: "))
while (endsize<startsize) :
    print("Invalid Input")
    endsize = int(input("Enter the population endsize:"))
    if (endsize > startsize):
        break
#Main code
n = startsize
while (n < endsize):
    List.append(n) #adds the population size to the array
    n = n + (n//3) - (n//4)
    if( n > endsize):
        break
years= len(List) 

#Output
print("The number of years is : ",years)

#Mario blocks
height = int(input("Enter the height of pyramid: "))
for i in range(0, height):
    for j in range(0, height-i):
        print (".", end = " ")
    for k in range(0, i+1):
        print("#", end = " ")
    print("  ", end = " ")
    for l in range(0, i+1):
        print("#", end = " ")
    print()

