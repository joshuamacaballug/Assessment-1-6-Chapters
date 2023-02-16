# Assessment-1-6-Chapters

Chapter 1 

Exercise 1:

print ("Python uses interpreter to convert source code into machine code.")
print ("Interpreter 'translates' program one statement at a time.")
#print displays the sentence within the quotations.

Exercise 2: 

print("Please enter the radius of the circle: ")
rad = float(input()) #Float is used for decimal integers
pi = 3.14 
circle = 2 * pi * rad #Code used to solve the equation
print("\nThe circumference is: ", circle)

Exercise 3a:

i1 = input("Please Enter Your Name: ")
i2 = int(input("Please Enter Your Age: "))
i3 = input("Please Enter Your Location: ")

print("Thank you, these are your informations: ")

print("Your name is: ",i1)
print("Your age is: ",i2)
print("Your Location is: ",i3)

Exercise 3b: 

name = input("What is your name?: \n")
print("Your name is: ", name)
age = input("What is your age?: ")
print(age)
name2 = name.title() #use title() code to capitalize the first letter in the word
print("It is good to meet you, ", name2)

print("The length of your name is: ", len(name2)) # len()is used to calculate how much letters are there in a word
        
print("You will be " + str(int(age)+1) + " in a year.") #the (age)+1 adds 1 more digit to the age


Exercise 4: 

print("Please enter three(3) numbers: ")
digits = list(map(int, input().split()))
digits.sort()
print("These are your numbers in ascending format:")
print(digits)
digits.sort()
digits.reverse()
print("These are your numbers in descending format: ")
print(digits)

Exercise 5:

print("Please enter two(2) numbers.")
a=int(input("First number: "))
b=int(input("Second number: "))

print("The Sum of these two numbers is: ",a+b)
print("The Difference of these two numbers is: ",a-b)
print("The Product of these two numbers is: ",a*b)
print("The Quotient of these two numbers is: ",a/b)
print("The Remainder of these two numbers is: ",a%b)


Exercise 6: 

print("Please enter the length of the three sides of the triangle: ") #Input for the 3 corner of a triangle

s1 = int(input("1st Side: "))
s2 = int(input("2nd Side: "))
s3 = int(input("3rd Side: "))


if s1 == s2 == s3:
	    print("That is an equilateral triangle!")
elif s1==s2 or s2==s3 or s3==s2: #Checking if the sides are isoceles or not.
	    print("That is an isosceles triangle!")
else:
	    print("That is a scalene triangle!")
      
Exercise 7:

num = int(input("Please enter a number: "))
if num % 2 == 0:
    int_type = 'even'
else:
    int_type = 'odd'

print(f"The number you entered is an {int_type} number.")

Exercise 8:

print("Please enter three numbers\n")
n1 = int(input("1st number: "))
n2 = int(input("2nd number: "))
n3 = int(input("3rd number: "))
if (n1 >= n2) and (n1 >= n3):
   ans = n1
elif (n2 >= n1) and (n2 >= n3):
   ans = n2
else:
   ans = n3

print(ans, "is the largest number you've entered.")


Exercise 9:

coaster = True

while coaster:

    print("Welcome to the roller coaster! This ride requires you to be at least at the age of 10 and a height of 1.35")

    age = int(input("Please enter your age: "))

    if age <= 9:
        print ("Sorry, You are too young to ride the Coaster.")
        break

    elif age > 10:
        print ("You age is eligible to ride the Roller Coaster")
     
    height = float(input("What is your height?(Enter in meter. Ex: 1.55): "))
    
    if height <= 1.3:
        print ("Sorry, You are too short to ride the Coaster.")
        break

    elif height > 1.35:
        print ("You are eligible to ride the Roller Coaster!")

    again = input("Would you like to try this again?: ").lower() 
    while True:
        if again == 'yes': 
            coaster = True
            break
        elif again == 'no': 
            coaster = False
            break
        else:
            again = input('Invalid input. Type "YES" to try again or "NO" to leave": ').lower()
            
            
 Exercise 10: 
 
 for Num in range(1, 101):
    #The numbers ranging from 1 to 100.

    if Num % 3 == 0 and Num % 5 == 0:
        print("FizzBuzz!: "+str(Num))
        #If any numbers are divisible with 3 and 5 it says FizzBuzz

    elif Num % 3 == 0:
        print("Fizz!:" +str(Num))
        #If 3 is divisible with one of the numbers in 1 to 100 

    elif Num % 5 == 0:
        print("Buzz!:" +str(Num))
        #If 5 is divisible with one of the numbers in 1 to 100 

    else:

        print(Num)
        
        
  Exercise 14: 
  
  Rows = 5
for i in range(0, Rows):
          #The nested loop for each columns.
    for I in range(0, i + 1):
        print("*", end=' ') #Here the asteris prints.
    print("\r") #A new line after each row.
    
    
  Chapter 2
  
  Exercise 1: 
  #Asking the user to enter 5 numbers in
num1 = (input("Enter 1st number: "))
num2 = (input("Enter 2nd number: "))
num3 = (input("Enter 3rd number: "))
num4 = (input("Enter 4th number: "))
num5 = (input("Enter 5th number "))


list = [num1, num2, num3, num4, num5]
#This the list where the inputted numbers from the user goes to.


print("These are the five digits you have entered: ", list)
#Displays the message and list

Exercise 2: 
  

diglist = [15, 27, 67, 36, 26, 97, 69, 41, 18, 55]
for x in diglist:
    print(x)


maxval = max(diglist)
minval = min(diglist)
print(minval, maxval)

diglist.sort()

print(diglist)


diglist.sort(reverse = True)
print(diglist) 


diglist2 = [17, 42]
diglist.append(diglist2)

print(diglist)

Exercise 3:

Dict = {"Movie Title:": "Back to the Future", "Director:": "Robert Zemeckis", "Release date:": "July 3, 1985", "Box office:": "388.8 Million USD"}

for k, v in Dict.items():
    print(k, v)
    
Exercise 4: 

year = (2017,2003,2011,2005,1987,2009,2020,2018,2009)


print(year[1])


year1 = (2009, 2018, 2020, 2009, 1987, 2005, 2011, 2003, 2017)
rev = reversed(year1)
print(tuple(rev))
print(year1)


amount = year.count(2009)


print(amount)


print(year.index(2018))


print(len(year))

Chapter 3:

Exercise 1:

def name (firstname, lastname):
    firstname= firstname
    lastname=lastname
    print(f'Full Name: {firstname.title()} {lastname.title()}')

firstname=str(input("Input first name: "))
lastname = str(input("Last Name: "))

name(firstname,lastname)

Exercise 2:

def name (num1, num2):
    num1=num1
    num2=num2
    result=num1+num2
    print(f'Result: {result}')

num1 =int(input("Enter first number: "))
num2 = int(input(" Enter second number: "))

Exercise 3: 








